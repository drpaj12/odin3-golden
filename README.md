# odin3-golden

Archived reference netlists ("goldens") for [Odin III](https://github.com/drpaj12/odin3).
Each golden is a BLIF produced by an upstream oracle — Yosys+Parmys (via the VTR flow) or Odin II —
and is what Odin III's output is compared against with `tools/netlist-compare` and `tools/equiv-check`.

**This repo holds the full verdict record but only a sample of the BLIFs.** Every run's `.prov`
(and `.log`, when it failed or was capped) is committed. The BLIFs are committed only for a small
representative sample, about 50 designs and 41 MB. The full BLIF set (2.7 GB+) is too large for
GitHub and is archived elsewhere:

- **Full set:** `golden-full-<vtr12>.tar.gz` plus `SHA256SUMS`, hosted at **TBD (Peter)**.
  Unpack it over a clone of this repo. Every BLIF's sha256 must match the `blif_sha256` in its
  `.prov`, and `SHA256SUMS` covers every file in the archive.
- **On the dev machine:** `~/odin3-ws/golden` holds the full set. Git ignores the non-sample BLIFs.

## Layout

Written by `odin3/tools/run-oracle.sh`; never hand-edit a file here.

```
<arch>/<name>/
  <leaf>.parmys.blif       # Yosys+Parmys output (VTR stage "parmys")
  <leaf>.parmys.prov       # provenance for that run
  <leaf>.odin.blif         # Odin II output (VTR stage "odin")
  <leaf>.odin.prov
  <leaf>.<tool>.log        # only when that tool failed or was capped: flow-log tail + error lines
```

`<arch>` is the architecture file's basename without `.xml` (e.g. `EArch`,
`k6_frac_N10_frac_chain_mem32K_40nm`). `<name>` is the design name, optionally grouped with `/`
(e.g. `micro/bm_and`); `<leaf>` is its last component.

## Provenance rule

**Every golden records the VTR commit hash and the architecture file that produced it.** Each
`<leaf>.<tool>.prov` holds:

```
vtr_commit=<full sha of external/vtr-verilog-to-routing>
vtr_dirty_files=<count of modified tracked files in that checkout; must be 0>
arch=<arch .xml path relative to $VTR_ROOT>
arch_sha256=<sha256 of the arch file>
source=<.v path relative to $VTR_ROOT>
source_sha256=<sha256 of the source>
tool=<parmys|odin>
mem_cap_mb=<memory cap the run had; absent in runs before the cap was recorded>
status=<ok|failed|capped>
blif_sha256=<sha256 of the BLIF; only when status=ok>
date=<UTC ISO-8601>
```

A BLIF without a matching `.prov` is invalid. A failed run is recorded too (`status=failed` plus
its `.log`), so the set of designs an oracle cannot handle is part of the archive. `status=capped`
means the run was killed at `mem_cap_mb` (cgroup memory cap). That is no verdict on the design;
rerun it with a larger `ODIN3_ORACLE_MEM_MB`. The versions
behind each `vtr_commit` are listed in `odin3/docs/ORACLES.md`.

## The sample

`odin3/tools/golden-sample --write` chooses the sample and regenerates the managed block in
`.gitignore` (`*.blif` is ignored, and each sampled BLIF is re-included). Run it after any golden
regeneration. The rule is deterministic:

- Designs are grouped by `regression/verilog/<category>` and `vtr`.
- A design is eligible when both tools are `ok` on both arches and every BLIF is at most 2 MB.
- Each group contributes up to 5 eligible designs at evenly spaced size ranks.
- `quickstart/blink` is always included.

Sampled `*.blif` files are stored with Git LFS.
