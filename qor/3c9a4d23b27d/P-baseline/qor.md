# Odin III QoR — k6_frac_N10_frac_chain_mem32K_40nm — P-baseline

VTR 3c9a4d23b27d · legs P 6baf6f3cfaf9
· host 13th Gen Intel(R) Core(TM) i7-13700, 23.5 GiB · 2026-10-12T08:03:48Z

## Netlist

| design | leg | luts | ffs | adders | mults | ram_slices | depth | abc_depth | exchange |
|---|---|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | 97 | 82 | 0 | 0 | 8 | 3 | 3 |  |
| stereovision3 | P | 124 | 117 | 28 | 0 | 0 | 2 | 4 |  |
| diffeq2 | P | 198 | 96 | 132 | 5 | 0 | 4 | 4 |  |
| diffeq1 | P | 294 | 193 | 132 | 5 | 0 | 5 | 5 |  |
| mkPktMerge | P | 176 | 18 | 42 | 0 | 459 | 2 | 2 |  |
| raygentop | P | 1046 | 946 | 413 | 15 | 21 | 3 | 4 |  |
| sha | P | 1212 | 893 | 309 | 0 | 0 | 4 | 4 |  |
| boundtop | P | 540 | 383 | 151 | 0 | 32 | 3 | 3 |  |
| mkSMAdapter4B | P | 1073 | 639 | 344 | 0 | 153 | 5 | 5 |  |
| or1200 | P | 2430 | 672 | 496 | 1 | 64 | 8 | 8 |  |
| stereovision0 | P | 6861 | 11433 | 2659 | 0 | 0 | 5 | 5 |  |
| stereovision1 | P | 6355 | 10315 | 2294 | 152 | 0 | 3 | 3 |  |
| mkDelayWorker32B | P | 436 | 34 | 768 | 0 | 1336 | 5 | 5 |  |
| stereovision2 | P | 8415 | 15585 | 12081 | 468 | 0 | 3 | 3 |  |
| blob_merge | P | 3381 | 575 | 3516 | 0 | 0 | 5 | 5 |  |
| LU8PEEng | P | 19591 | 6224 | 4560 | 8 | 1409 | 97 | 97 |  |
| bgm | P | 25807 | 5105 | 2270 | 11 | 0 | 14 | 14 |  |
| mcml | P | 81215 | 51529 | 25137 | 27 | 348 | 26 | 26 |  |
| LU32PEEng | P | 69095 | 19668 | 13470 | 32 | 5251 | 98 | 98 |  |
| spree | P | 690 | 200 | 62 | 1 | 128 | 16 | 16 |  |
| arm_core | P | 9407 | 2727 | 384 | 0 | 1192 | 20 | 20 |  |

## Packed

| design | leg | CLB | memories | mults | W×H | hard blocks |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 68 | 1 | 0 | 12×12 |  |
| stereovision3 | P | 15 | 0 | 0 | 7×7 |  |
| diffeq2 | P | 23 | 0 | 5 | 16×16 |  |
| diffeq1 | P | 35 | 0 | 5 | 16×16 |  |
| mkPktMerge | P | 34 | 15 | 0 | 28×28 |  |
| raygentop | P | 141 | 1 | 6 | 19×19 |  |
| sha | P | 131 | 0 | 0 | 16×16 |  |
| boundtop | P | 52 | 1 | 0 | 15×15 |  |
| mkSMAdapter4B | P | 176 | 5 | 0 | 20×20 |  |
| or1200 | P | 265 | 2 | 1 | 26×26 |  |
| stereovision0 | P | 706 | 0 | 0 | 33×33 |  |
| stereovision1 | P | 806 | 0 | 43 | 40×40 |  |
| mkDelayWorker32B | P | 481 | 43 | 0 | 50×50 |  |
| stereovision2 | P | 1940 | 0 | 192 | 82×82 |  |
| blob_merge | P | 502 | 0 | 0 | 29×29 |  |
| LU8PEEng | P | 2144 | 45 | 8 | 56×56 |  |
| bgm | P | 2777 | 0 | 11 | 63×63 |  |
| mcml | P | 6773 | 159 | 27 | 98×98 |  |
| LU32PEEng | P | 7483 | 168 | 32 | 102×102 |  |
| spree | P | 63 | 3 | 1 | 14×14 |  |
| arm_core | P | 853 | 24 | 0 | 37×37 |  |

## Routed

| design | leg | status | vpr_status | min W | CPD (ns) | Fmax (MHz) | WL |
|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | ok | success | 40 | 1.934 | 517.0 | 1093 |
| stereovision3 | P | ok | success | 26 | 2.440 | 409.8 | 382 |
| diffeq2 | P | ok | success | 68 | 12.430 | 80.5 | 6368 |
| diffeq1 | P | ok | success | 50 | 17.196 | 58.2 | 9217 |
| mkPktMerge | P | ok | success | 40 | 4.063 | 246.1 | 13085 |
| raygentop | P | ok | success | 58 | 5.190 | 192.7 | 20146 |
| sha | P | ok | success | 66 | 9.305 | 107.5 | 11230 |
| boundtop | P | ok | success | 38 | 2.735 | 365.7 | 5353 |
| mkSMAdapter4B | P | ok | success | 46 | 5.461 | 183.1 | 15859 |
| or1200 | P | ok | success | 78 | 9.497 | 105.3 | 38743 |
| stereovision0 | P | ok | success | 46 | 4.516 | 221.4 | 53023 |
| stereovision1 | P | ok | success | 74 | 5.438 | 183.9 | 110454 |
| mkDelayWorker32B | P | ok | success | 40 | 8.724 | 114.6 | 18222 |
| stereovision2 | P | ok | success | 86 | 13.476 | 74.2 | 379193 |
| blob_merge | P | ok | success | 64 | 14.667 | 68.2 | 57997 |
| LU8PEEng | P | ok | success | 84 | 74.178 | 13.5 | 292889 |
| bgm | P | ok | success | 84 | 22.125 | 45.2 | 360800 |
| mcml | P | ok | success | 120 | 48.154 | 20.8 | 852861 |
| LU32PEEng | P | ok | success | 100 | 73.157 | 13.7 | 1125747 |
| spree | P | ok | success | 58 | 10.945 | 91.4 | 10399 |
| arm_core | P | ok | success | 96 | 23.537 | 42.5 | 148706 |

## Cost

| design | leg | front-end wall (s) | front-end peak (MiB) | VPR time (s) | VPR mem (MiB) | slice |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 0.3 | 36 | 1.2 | 71 |  |
| stereovision3 | P | 0.3 | 36 | 0.5 | 67 |  |
| diffeq2 | P | 0.2 | 36 | 3.3 | 76 |  |
| diffeq1 | P | 0.2 | 38 | 2.5 | 77 |  |
| mkPktMerge | P | 0.4 | 38 | 3.7 | 94 |  |
| raygentop | P | 2.2 | 48 | 5.5 | 101 |  |
| sha | P | 1.2 | 51 | 4.1 | 98 |  |
| boundtop | P | 3.5 | 49 | 1.7 | 79 |  |
| mkSMAdapter4B | P | 2.2 | 56 | 5.4 | 104 |  |
| or1200 | P | 3.0 | 63 | 14.0 | 135 |  |
| stereovision0 | P | 4.9 | 101 | 18.0 | 272 |  |
| stereovision1 | P | 6.0 | 123 | 33.3 | 345 |  |
| mkDelayWorker32B | P | 7.2 | 118 | 21.3 | 310 |  |
| stereovision2 | P | 6.3 | 196 | 136.7 | 1162 |  |
| blob_merge | P | 5.4 | 209 | 21.7 | 185 |  |
| LU8PEEng | P | 47.5 | 373 | 124.6 | 758 |  |
| bgm | P | 45.2 | 500 | 156.8 | 947 |  |
| mcml | P | 1568.2 | 973 | 505.0 | 2224 |  |
| LU32PEEng | P | 446.4 | 1186 | 880.5 | 2264 |  |
| spree | P | 1.0 | 40 | 2.9 | 82 |  |
| arm_core | P | 24.2 | 124 | 54.8 | 310 |  |

`*`: a stage log had no `time -v` figures (job.json `cost_warnings`), so the front-end cost is incomplete. `xl`: the job ran in the 9 GiB `odin3-heavyxl.slice` (plan point (d)). Comparability (spec §18 item 2): P's front end is two VTR stages, Parmys and ABC, timed by VTR's own `time -v`, and VTR's ABC stage also pays a BLIF write and read per clock domain; an Odin III leg's front end is one `odin3` process timed by the harness (plus VTR's ABC stage for O' and R). Both are wall time and peak RSS, but not measured the same way.

## Functional check and determinism

| design | fcheck P |
|---|---|
| ch_intrinsics | skipped |
| stereovision3 | skipped |
| diffeq2 | skipped |
| diffeq1 | skipped |
| mkPktMerge | skipped |
| raygentop | skipped |
| sha | skipped |
| boundtop | skipped |
| mkSMAdapter4B | skipped |
| or1200 | skipped |
| stereovision0 | skipped |
| stereovision1 | skipped |
| mkDelayWorker32B | skipped |
| stereovision2 | skipped |
| blob_merge | skipped |
| LU8PEEng | skipped |
| bgm | skipped |
| mcml | skipped |
| LU32PEEng | skipped |
| spree | skipped |
| arm_core | skipped |

## Cross-check against VTR's golden

P against VTR's `golden_results.txt` for `vtr_reg_qor_chain` (another machine and VPR revision), with the bands of its pass requirements: num_clb 0.90–1.10, min_chan_width 0.25–1.30, critical_path_delay 0.50–1.40, crit_path_routed_wirelength 0.60–1.50. A metric outside its band is listed `outside` and fails nothing (PHASE3 exit item 5).

| design | CLB P | CLB golden | P/golden | W P | W golden | P/golden | CPD P | CPD golden | P/golden | WL P | WL golden | P/golden | outside |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| ch_intrinsics | 68 | 68 | 1.000 | 40 | 40 | 1.000 | 1.934 | 1.934 | 1.000 | 1093 | 1093 | 1.000 |  |
| stereovision3 | 15 | 15 | 1.000 | 26 | 26 | 1.000 | 2.440 | 2.440 | 1.000 | 382 | 382 | 1.000 |  |
| diffeq2 | 23 | 23 | 1.000 | 68 | 58 | 1.172 | 12.430 | 12.729 | 0.976 | 6368 | 6769 | 0.941 |  |
| diffeq1 | 35 | 35 | 1.000 | 50 | 62 | 0.806 | 17.196 | 16.973 | 1.013 | 9217 | 8657 | 1.065 |  |
| mkPktMerge | 34 | 34 | 1.000 | 40 | 40 | 1.000 | 4.063 | 4.063 | 1.000 | 13085 | 13085 | 1.000 |  |
| raygentop | 141 | 141 | 1.000 | 58 | 58 | 1.000 | 5.190 | 5.190 | 1.000 | 20146 | 20146 | 1.000 |  |
| sha | 131 | 131 | 1.000 | 66 | 66 | 1.000 | 9.305 | 9.305 | 1.000 | 11230 | 11230 | 1.000 |  |
| boundtop | 52 | 52 | 1.000 | 38 | 38 | 1.000 | 2.735 | 2.735 | 1.000 | 5353 | 5353 | 1.000 |  |
| mkSMAdapter4B | 176 | 176 | 1.000 | 46 | 46 | 1.000 | 5.461 | 5.461 | 1.000 | 15859 | 15859 | 1.000 |  |
| or1200 | 265 | 265 | 1.000 | 78 | 78 | 1.000 | 9.497 | 9.497 | 1.000 | 38743 | 38743 | 1.000 |  |
| stereovision0 | 706 | 706 | 1.000 | 46 | 46 | 1.000 | 4.516 | 4.516 | 1.000 | 53023 | 53023 | 1.000 |  |
| stereovision1 | 806 | 806 | 1.000 | 74 | 74 | 1.000 | 5.438 | 5.438 | 1.000 | 110454 | 110454 | 1.000 |  |
| mkDelayWorker32B | 481 | 481 | 1.000 | 40 | 40 | 1.000 | 8.724 | 8.724 | 1.000 | 18222 | 18222 | 1.000 |  |
| stereovision2 | 1940 | 1940 | 1.000 | 86 | 86 | 1.000 | 13.476 | 13.476 | 1.000 | 379193 | 379193 | 1.000 |  |
| blob_merge | 502 | 502 | 1.000 | 64 | 64 | 1.000 | 14.667 | 14.667 | 1.000 | 57997 | 57997 | 1.000 |  |
| LU8PEEng | 2144 | 2144 | 1.000 | 84 | 88 | 0.955 | 74.178 | 74.061 | 1.002 | 292889 | 290200 | 1.009 |  |
| bgm | 2777 | 2777 | 1.000 | 84 | 84 | 1.000 | 22.125 | 22.125 | 1.000 | 360800 | 360800 | 1.000 |  |
| mcml | 6773 | 6773 | 1.000 | 120 | 120 | 1.000 | 48.154 | 48.154 | 1.000 | 852861 | 852861 | 1.000 |  |
| LU32PEEng | 7483 | 7483 | 1.000 | 100 | 100 | 1.000 | 73.157 | 73.157 | 1.000 | 1125747 | 1125747 | 1.000 |  |
| **geomean (19)** |  |  | 1.000 |  |  | 0.995 |  |  | 1.000 |  |  | 1.001 |  |

Non-gating rows (spree, arm_core):

| design | CLB P | CLB golden | P/golden | W P | W golden | P/golden | CPD P | CPD golden | P/golden | WL P | WL golden | P/golden | outside |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| spree | 63 | 63 | 1.000 | 58 | 58 | 1.000 | 10.945 | 10.945 | 1.000 | 10399 | 10399 | 1.000 |  |
| arm_core | 853 | 853 | 1.000 | 96 | 96 | 1.000 | 23.537 | 23.537 | 1.000 | 148706 | 148706 | 1.000 |  |
| **geomean (2)** |  |  | 1.000 |  |  | 1.000 |  |  | 1.000 |  |  | 1.000 |  |
