# M1 (Phase 3) QoR table: notes

- Run on odin3 828c3f16 (legs P and P'). Table regenerated 2026-10-19 05:32 UTC after the fcheck reruns on odin3 main 3831d10c.
- M1 is met: P' routes all 19 designs with VPR (spree and arm_core are skipped by the harness).
- **The "fcheck P" column is provisional.** It comes from the harness before the fcheck classification fix (odin3 branch `fix/fcheck-classify`).
  - Of the 10 P-leg fails, most are defects in the Parmys baseline netlist, not harness errors:
    - sha, blob_merge and or1200: the D2b subtract pad (`unconn` where `$sub` needs 1);
    - stereovision1 and stereovision2: lost sign bits;
    - raygentop and boundtop: dropped latches plus D2b.
  - ch_intrinsics and stereovision0 depend on the RTL's uninitialised state.
  - After that fix, such designs report `untested` (never a pass), and P-leg baseline defects are listed with a reason. The milestone gate judges only Odin III's legs.
  - This table will be replaced once the fix merges.
- The stereovision3 P' LUT gap (165 against 124, depth 4 against 2) is deferred to M3, by Peter's decision of 2026-10-19.
