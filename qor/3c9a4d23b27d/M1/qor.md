# Odin III QoR — k6_frac_N10_frac_chain_mem32K_40nm — M1

VTR 3c9a4d23b27d · odin3 828c3f16a455 (build 425c4c3f2bbc) · ABC script 0d0d27670d8c · legs P 6baf6f3cfaf9, P' a7d7637a6a5c
· host 13th Gen Intel(R) Core(TM) i7-13700, 23.5 GiB · 2026-10-19T05:32:02Z

## Netlist

| design | leg | luts | ffs | adders | mults | ram_slices | depth | abc_depth | exchange |
|---|---|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | 97 | 82 | 0 | 0 | 8 | 3 | 3 |  |
| ch_intrinsics | P' | 97 | 82 | 0 | 0 | 8 | 3 | 3 | blif |
| stereovision3 | P | 124 | 117 | 28 | 0 | 0 | 2 | 4 |  |
| stereovision3 | P' | 165 | 120 | 28 | 0 | 0 | 4 | 4 | blif |
| diffeq2 | P | 198 | 96 | 132 | 5 | 0 | 4 | 4 |  |
| diffeq2 | P' | 195 | 96 | 132 | 5 | 0 | 5 | 5 | blif |
| diffeq1 | P | 294 | 193 | 132 | 5 | 0 | 5 | 5 |  |
| diffeq1 | P' | 295 | 193 | 132 | 5 | 0 | 5 | 5 | blif |
| mkPktMerge | P | 176 | 18 | 42 | 0 | 459 | 2 | 2 |  |
| mkPktMerge | P' | 176 | 18 | 42 | 0 | 459 | 2 | 2 | blif |
| raygentop | P | 1046 | 946 | 413 | 15 | 21 | 3 | 4 |  |
| raygentop | P' | 1062 | 946 | 413 | 15 | 21 | 3 | 3 | blif |
| sha | P | 1212 | 893 | 309 | 0 | 0 | 4 | 4 |  |
| sha | P' | 1209 | 893 | 309 | 0 | 0 | 4 | 4 | blif |
| boundtop | P | 540 | 383 | 151 | 0 | 32 | 3 | 3 |  |
| boundtop | P' | 539 | 383 | 151 | 0 | 32 | 3 | 3 | blif |
| mkSMAdapter4B | P | 1073 | 639 | 344 | 0 | 153 | 5 | 5 |  |
| mkSMAdapter4B | P' | 1155 | 639 | 344 | 0 | 153 | 5 | 5 | blif |
| or1200 | P | 2430 | 672 | 496 | 1 | 64 | 8 | 8 |  |
| or1200 | P' | 2420 | 672 | 496 | 1 | 64 | 8 | 8 | blif |
| stereovision0 | P | 6861 | 11433 | 2659 | 0 | 0 | 5 | 5 |  |
| stereovision0 | P' | 6860 | 11433 | 2659 | 0 | 0 | 5 | 5 | blif |
| stereovision1 | P | 6355 | 10315 | 2294 | 152 | 0 | 3 | 3 |  |
| stereovision1 | P' | 6358 | 10315 | 2294 | 152 | 0 | 3 | 3 | blif |
| mkDelayWorker32B | P | 436 | 34 | 768 | 0 | 1336 | 5 | 5 |  |
| mkDelayWorker32B | P' | 436 | 34 | 768 | 0 | 1336 | 5 | 5 | blif |
| stereovision2 | P | 8415 | 15585 | 12081 | 468 | 0 | 3 | 3 |  |
| stereovision2 | P' | 8413 | 15585 | 12081 | 468 | 0 | 3 | 3 | blif |
| blob_merge | P | 3381 | 575 | 3516 | 0 | 0 | 5 | 5 |  |
| blob_merge | P' | 3410 | 575 | 3516 | 0 | 0 | 5 | 5 | blif |
| LU8PEEng | P | 19591 | 6224 | 4560 | 8 | 1409 | 97 | 97 |  |
| LU8PEEng | P' | 19564 | 6224 | 4560 | 8 | 1409 | 97 | 97 | blif |
| bgm | P | 25807 | 5105 | 2270 | 11 | 0 | 14 | 14 |  |
| bgm | P' | 25663 | 5105 | 2270 | 11 | 0 | 14 | 14 | blif |
| mcml | P | 81215 | 51529 | 25137 | 27 | 348 | 26 | 26 |  |
| mcml | P' | 81396 | 51529 | 25137 | 27 | 348 | 26 | 26 | blif |
| LU32PEEng | P | 69095 | 19668 | 13470 | 32 | 5251 | 98 | 98 |  |
| LU32PEEng | P' | 69122 | 19668 | 13470 | 32 | 5251 | 97 | 97 | blif |
| spree | P | 690 | 200 | 62 | 1 | 128 | 16 | 16 |  |
| arm_core | P | 9407 | 2727 | 384 | 0 | 1192 | 20 | 20 |  |

## Packed

| design | leg | CLB | memories | mults | W×H | hard blocks |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 68 | 1 | 0 | 12×12 |  |
| ch_intrinsics | P' | 69 | 1 | 0 | 12×12 | = P |
| stereovision3 | P | 15 | 0 | 0 | 7×7 |  |
| stereovision3 | P' | 16 | 0 | 0 | 7×7 | = P |
| diffeq2 | P | 23 | 0 | 5 | 16×16 |  |
| diffeq2 | P' | 23 | 0 | 5 | 16×16 | = P |
| diffeq1 | P | 35 | 0 | 5 | 16×16 |  |
| diffeq1 | P' | 31 | 0 | 5 | 16×16 | = P |
| mkPktMerge | P | 34 | 15 | 0 | 28×28 |  |
| mkPktMerge | P' | 21 | 15 | 0 | 28×28 | = P |
| raygentop | P | 141 | 1 | 6 | 19×19 |  |
| raygentop | P' | 140 | 1 | 6 | 19×19 | = P |
| sha | P | 131 | 0 | 0 | 16×16 |  |
| sha | P' | 137 | 0 | 0 | 16×16 | = P |
| boundtop | P | 52 | 1 | 0 | 15×15 |  |
| boundtop | P' | 59 | 1 | 0 | 15×15 | = P |
| mkSMAdapter4B | P | 176 | 5 | 0 | 20×20 |  |
| mkSMAdapter4B | P' | 190 | 5 | 0 | 20×20 | = P |
| or1200 | P | 265 | 2 | 1 | 26×26 |  |
| or1200 | P' | 274 | 2 | 1 | 27×27 | = P |
| stereovision0 | P | 706 | 0 | 0 | 33×33 |  |
| stereovision0 | P' | 708 | 0 | 0 | 33×33 | = P |
| stereovision1 | P | 806 | 0 | 43 | 40×40 |  |
| stereovision1 | P' | 807 | 0 | 44 | 40×40 | ≠ P |
| mkDelayWorker32B | P | 481 | 43 | 0 | 50×50 |  |
| mkDelayWorker32B | P' | 380 | 43 | 0 | 50×50 | = P |
| stereovision2 | P | 1940 | 0 | 192 | 82×82 |  |
| stereovision2 | P' | 1949 | 0 | 186 | 80×80 | ≠ P |
| blob_merge | P | 502 | 0 | 0 | 29×29 |  |
| blob_merge | P' | 509 | 0 | 0 | 29×29 | = P |
| LU8PEEng | P | 2144 | 45 | 8 | 56×56 |  |
| LU8PEEng | P' | 2150 | 45 | 8 | 56×56 | = P |
| bgm | P | 2777 | 0 | 11 | 63×63 |  |
| bgm | P' | 2754 | 0 | 11 | 63×63 | = P |
| mcml | P | 6773 | 159 | 27 | 98×98 |  |
| mcml | P' | 6880 | 159 | 27 | 98×98 | = P |
| LU32PEEng | P | 7483 | 168 | 32 | 102×102 |  |
| LU32PEEng | P' | 7482 | 168 | 32 | 102×102 | = P |
| spree | P | 63 | 3 | 1 | 14×14 |  |
| arm_core | P | 853 | 24 | 0 | 37×37 |  |

## Routed

| design | leg | status | vpr_status | min W | CPD (ns) | Fmax (MHz) | WL |
|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | ok | success | 40 | 1.934 | 517.0 | 1093 |
| ch_intrinsics | P' | ok | success | 36 | 1.933 | 517.3 | 1096 |
| stereovision3 | P | ok | success | 26 | 2.440 | 409.8 | 382 |
| stereovision3 | P' | ok | success | 32 | 2.595 | 385.3 | 1078 |
| diffeq2 | P | ok | success | 68 | 12.430 | 80.5 | 6368 |
| diffeq2 | P' | ok | success | 50 | 12.974 | 77.1 | 7251 |
| diffeq1 | P | ok | success | 50 | 17.196 | 58.2 | 9217 |
| diffeq1 | P' | ok | success | 48 | 17.404 | 57.5 | 8915 |
| mkPktMerge | P | ok | success | 40 | 4.063 | 246.1 | 13085 |
| mkPktMerge | P' | ok | success | 36 | 3.701 | 270.2 | 13017 |
| raygentop | P | ok | success | 58 | 5.190 | 192.7 | 20146 |
| raygentop | P' | ok | success | 64 | 5.159 | 193.8 | 19728 |
| sha | P | ok | success | 66 | 9.305 | 107.5 | 11230 |
| sha | P' | ok | success | 58 | 10.215 | 97.9 | 12055 |
| boundtop | P | ok | success | 38 | 2.735 | 365.7 | 5353 |
| boundtop | P' | ok | success | 46 | 2.496 | 400.7 | 4749 |
| mkSMAdapter4B | P | ok | success | 46 | 5.461 | 183.1 | 15859 |
| mkSMAdapter4B | P' | ok | success | 56 | 5.861 | 170.6 | 16143 |
| or1200 | P | ok | success | 78 | 9.497 | 105.3 | 38743 |
| or1200 | P' | ok | success | 84 | 9.413 | 106.2 | 39507 |
| stereovision0 | P | ok | success | 46 | 4.516 | 221.4 | 53023 |
| stereovision0 | P' | ok | success | 46 | 3.698 | 270.4 | 52762 |
| stereovision1 | P | ok | success | 74 | 5.438 | 183.9 | 110454 |
| stereovision1 | P' | ok | success | 78 | 5.400 | 185.2 | 111935 |
| mkDelayWorker32B | P | ok | success | 40 | 8.724 | 114.6 | 18222 |
| mkDelayWorker32B | P' | ok | success | 38 | 7.357 | 135.9 | 18789 |
| stereovision2 | P | ok | success | 86 | 13.476 | 74.2 | 379193 |
| stereovision2 | P' | ok | success | 80 | 13.483 | 74.2 | 377884 |
| blob_merge | P | ok | success | 64 | 14.667 | 68.2 | 57997 |
| blob_merge | P' | ok | success | 64 | 15.054 | 66.4 | 57996 |
| LU8PEEng | P | ok | success | 84 | 74.178 | 13.5 | 292889 |
| LU8PEEng | P' | ok | success | 84 | 74.094 | 13.5 | 298564 |
| bgm | P | ok | success | 84 | 22.125 | 45.2 | 360800 |
| bgm | P' | ok | success | 82 | 21.900 | 45.7 | 352158 |
| mcml | P | ok | success | 120 | 48.154 | 20.8 | 852861 |
| mcml | P' | ok | success | 126 | 45.829 | 21.8 | 883625 |
| LU32PEEng | P | ok | success | 100 | 73.157 | 13.7 | 1125747 |
| LU32PEEng | P' | ok | success | 102 | 72.883 | 13.7 | 1129315 |
| spree | P | ok | success | 58 | 10.945 | 91.4 | 10399 |
| arm_core | P | ok | success | 96 | 23.537 | 42.5 | 148706 |

## Cost

| design | leg | front-end wall (s) | front-end peak (MiB) | VPR time (s) | VPR mem (MiB) | slice |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 0.3 | 36 | 1.2 | 71 |  |
| ch_intrinsics | P' | 0.1 + 0.2 Parmys | 40 | 1.0 | 70 |  |
| stereovision3 | P | 0.3 | 36 | 0.5 | 67 |  |
| stereovision3 | P' | 0.1 + 0.2 Parmys | 40 | 0.8 | 69 |  |
| diffeq2 | P | 0.2 | 36 | 3.3 | 76 |  |
| diffeq2 | P' | 0.1 + 0.1 Parmys | 40 | 2.9 | 74 |  |
| diffeq1 | P | 0.2 | 38 | 2.5 | 77 |  |
| diffeq1 | P' | 0.1 + 0.1 Parmys | 41 | 3.3 | 77 |  |
| mkPktMerge | P | 0.4 | 38 | 3.7 | 94 |  |
| mkPktMerge | P' | 0.1 + 0.3 Parmys | 41 | 4.4 | 92 |  |
| raygentop | P | 2.2 | 48 | 5.5 | 101 |  |
| raygentop | P' | 0.3 + 1.8 Parmys | 46 | 7.2 | 100 |  |
| sha | P | 1.2 | 51 | 4.1 | 98 |  |
| sha | P' | 0.7 + 0.5 Parmys | 49 | 5.1 | 96 |  |
| boundtop | P | 3.5 | 49 | 1.7 | 79 |  |
| boundtop | P' | 0.3 + 3.1 Parmys | 45 | 2.3 | 80 |  |
| mkSMAdapter4B | P | 2.2 | 56 | 5.4 | 104 |  |
| mkSMAdapter4B | P' | 1.0 + 1.3 Parmys | 50 | 6.9 | 102 |  |
| or1200 | P | 3.0 | 63 | 14.0 | 135 |  |
| or1200 | P' | 2.6 + 1.2 Parmys | 54 | 20.1 | 138 |  |
| stereovision0 | P | 4.9 | 101 | 18.0 | 272 |  |
| stereovision0 | P' | 2.7 + 2.4 Parmys | 85 | 22.3 | 271 |  |
| stereovision1 | P | 6.0 | 123 | 33.3 | 345 |  |
| stereovision1 | P' | 3.8 + 2.1 Parmys | 90 | 47.1 | 343 |  |
| mkDelayWorker32B | P | 7.2 | 118 | 21.3 | 310 |  |
| mkDelayWorker32B | P' | 2.0 + 4.8 Parmys | 70 | 21.1 | 308 |  |
| stereovision2 | P | 6.3 | 196 | 136.7 | 1162 |  |
| stereovision2 | P' | 1.6 + 3.5 Parmys | 123 | 145.6 | 1016 |  |
| blob_merge | P | 5.4 | 209 | 21.7 | 185 |  |
| blob_merge | P' | 1.8 + 3.1 Parmys | 71 | 24.4 | 181 |  |
| LU8PEEng | P | 47.5 | 373 | 124.6 | 758 |  |
| LU8PEEng | P' | 30.7 + 14.3 Parmys | 174 | 146.2 | 737 |  |
| bgm | P | 45.2 | 500 | 156.8 | 947 |  |
| bgm | P' | 33.6 + 11.8 Parmys | 226 | 135.9 | 931 |  |
| mcml | P | 1568.2 | 973 | 505.0 | 2224 |  |
| mcml | P' | 1249.6 + 64.3 Parmys | 489 | 555.5 | 2173 |  |
| LU32PEEng | P | 446.4 | 1186 | 880.5 | 2264 |  |
| LU32PEEng | P' | 325.8 + 49.3 Parmys | 573 | 580.0 | 2242 |  |
| spree | P | 1.0 | 40 | 2.9 | 82 |  |
| arm_core | P | 24.2 | 124 | 54.8 | 310 |  |

`*`: a stage log had no `time -v` figures (job.json `cost_warnings`), so the front-end cost is incomplete. `xl`: the job ran in the 9 GiB `odin3-heavyxl.slice` (plan point (d)). Comparability (spec §18 item 2): P's front end is two VTR stages, Parmys and ABC, timed by VTR's own `time -v`, and VTR's ABC stage also pays a BLIF write and read per clock domain; an Odin III leg's front end is one `odin3` process timed by the harness (plus VTR's ABC stage for O' and R). Both are wall time and peak RSS, but not measured the same way.

## Attribution

Geomeans over the 19 gate designs.

| metric | P'/P (ABC) |
|---|---|
| num_clb | 0.976 |
| min_chan_width | 1.003 |
| critical_path_delay_ns | 0.983 |
| crit_path_routed_wirelength | 1.063 |

ABC exchange (3D I8; runs per exchange): P' blif 19

## Functional check and determinism

| design | fcheck P |
|---|---|
| ch_intrinsics | fail |
| stereovision3 | pass |
| diffeq2 | pass |
| diffeq1 | pass |
| mkPktMerge | pass |
| raygentop | fail |
| sha | fail |
| boundtop | fail |
| mkSMAdapter4B | pass |
| or1200 | fail |
| stereovision0 | fail |
| stereovision1 | fail |
| mkDelayWorker32B | pass |
| stereovision2 | fail |
| blob_merge | fail |
| LU8PEEng | pass |
| bgm | fail |
| mcml | pass |
| LU32PEEng | pass |
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
