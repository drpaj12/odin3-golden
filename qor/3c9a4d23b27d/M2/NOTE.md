# M2 and Phase 3 close (2026-10-20)

M2: the O' leg (Odin III front end, linked ABC, VTR from `-start vpr`) routes all 15 designs of the
local gate on k6_frac_N10_frac_chain_mem32K_40nm (main 69f92d1c). Geomeans O'/P: CLB 0.976, channel
width 0.967, critical-path delay 0.974, wirelength 0.811. Outliers not investigated (PHASE3 decision
58): blob_merge LUTs 1.87x, raygentop 1.42x.

Phase 3 closed on this table and the M3 `exit-run exit-20261020` (main 69f92d1c) without a final M3
table (decision 58): run 66 of 68 ok, arm_core routes after PR D (#179, 148 s on O and O');
fcheck O 12 pass, raygentop/boundtop/stereovision0 untested (decision 57); rerun check 15 of 15
byte-identical. The four big designs (mcml, LU32PEEng, bgm, LU8PEEng) are shipped out (decision 54).
