# odin3-golden

Archived reference netlists ("goldens") for [Odin III](https://github.com/drpaj12/odin3).
Each golden is a BLIF produced by an upstream oracle — Yosys+Parmys (via the VTR flow) or Odin II —
and is what Odin III's output is compared against with `tools/netlist-compare` and `tools/equiv-check`.

## Layout

```
<arch>/<design>/
  <design>.parmys.blif     # Yosys+Parmys output
  <design>.odin.blif       # Odin II output
  PROVENANCE               # see below
```

`<arch>` is the architecture file's basename without `.xml` (e.g. `EArch`,
`k6_frac_N10_frac_chain_mem32K_40nm`).

## Provenance rule

**Every golden records the VTR commit hash and the architecture file that produced it.**
The `PROVENANCE` file next to each BLIF holds at least:

```
vtr_commit=<full sha of external/vtr-verilog-to-routing>
arch=<path of the arch .xml relative to $VTR_ROOT>
source=<path of the .v relative to $VTR_ROOT>
tool=<parmys|odin_ii>
date=<UTC ISO-8601>
```

A golden without a matching `PROVENANCE` entry is invalid. Regenerate goldens with
`odin3/tools/run-oracle.sh`; never hand-edit a BLIF here.

`*.blif` is stored with Git LFS.
