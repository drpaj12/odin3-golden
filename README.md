# odin3-golden

Archived reference netlists ("goldens") for [Odin III](https://github.com/drpaj12/odin3).
Each golden is a BLIF produced by an upstream oracle — Yosys+Parmys (via the VTR flow) or Odin II —
and is what Odin III's output is compared against with `tools/netlist-compare` and `tools/equiv-check`.

## Layout

Written by `odin3/tools/run-oracle.sh`; never hand-edit a file here.

```
<arch>/<name>/
  <leaf>.parmys.blif       # Yosys+Parmys output (VTR stage "parmys")
  <leaf>.parmys.prov       # provenance for that run
  <leaf>.odin.blif         # Odin II output (VTR stage "odin")
  <leaf>.odin.prov
  <leaf>.<tool>.log        # only when that tool failed: flow-log tail + error lines
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
status=<ok|failed>
blif_sha256=<sha256 of the BLIF; only when status=ok>
date=<UTC ISO-8601>
```

A BLIF without a matching `.prov` is invalid. A failed run is recorded too (`status=failed` plus
its `.log`), so the set of designs an oracle cannot handle is part of the archive. The versions
behind each `vtr_commit` are listed in `odin3/docs/ORACLES.md`.

`*.blif` is stored with Git LFS.
