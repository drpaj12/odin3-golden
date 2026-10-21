# Odin III QoR — k6_frac_N10_frac_chain_mem32K_40nm — M2

VTR 3c9a4d23b27d · odin3 a3182864d5a7 (build 1b5403d92742) · ABC script 0d0d27670d8c · legs P 6baf6f3cfaf9, O' 4396fe838a76
· host 13th Gen Intel(R) Core(TM) i7-13700, 23.5 GiB · 2026-10-21T02:22:58Z

## Netlist

| design | leg | luts | ffs | adders | mults | ram_slices | depth | abc_depth | exchange |
|---|---|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | 97 | 82 | 0 | 0 | 8 | 3 | 3 |  |
| ch_intrinsics | O' | 96 | 82 | 0 | 0 | 8 | 3 | 3 |  |
| stereovision3 | P | 124 | 117 | 28 | 0 | 0 | 2 | 4 |  |
| stereovision3 | O' | 124 | 117 | 31 | 0 | 0 | 2 | 4 |  |
| diffeq2 | P | 198 | 96 | 132 | 5 | 0 | 4 | 4 |  |
| diffeq2 | O' | 196 | 96 | 136 | 5 | 0 | 4 | 4 |  |
| diffeq1 | P | 294 | 193 | 132 | 5 | 0 | 5 | 5 |  |
| diffeq1 | O' | 294 | 193 | 136 | 5 | 0 | 5 | 5 |  |
| mkPktMerge | P | 176 | 18 | 42 | 0 | 459 | 2 | 2 |  |
| mkPktMerge | O' | 176 | 18 | 51 | 0 | 459 | 2 | 2 |  |
| raygentop | P | 1046 | 946 | 413 | 15 | 21 | 3 | 4 |  |
| raygentop | O' | 1073 | 946 | 453 | 15 | 21 | 3 | 3 |  |
| sha | P | 1212 | 893 | 309 | 0 | 0 | 4 | 4 |  |
| sha | O' | 1210 | 893 | 320 | 0 | 0 | 3 | 3 |  |
| boundtop | P | 540 | 383 | 151 | 0 | 32 | 3 | 3 |  |
| boundtop | O' | 537 | 383 | 166 | 0 | 32 | 3 | 3 |  |
| mkSMAdapter4B | P | 1073 | 639 | 344 | 0 | 153 | 5 | 5 |  |
| mkSMAdapter4B | O' | 1096 | 639 | 370 | 0 | 153 | 5 | 5 |  |
| or1200 | P | 2430 | 672 | 496 | 1 | 64 | 8 | 8 |  |
| or1200 | O' | 2466 | 672 | 563 | 1 | 64 | 8 | 8 |  |
| stereovision0 | P | 6861 | 11433 | 2659 | 0 | 0 | 5 | 5 |  |
| stereovision0 | O' | 6826 | 11458 | 2741 | 0 | 0 | 5 | 5 |  |
| stereovision1 | P | 6355 | 10315 | 2294 | 152 | 0 | 3 | 3 |  |
| stereovision1 | O' | 6355 | 10315 | 2482 | 152 | 0 | 3 | 3 |  |
| mkDelayWorker32B | P | 436 | 34 | 768 | 0 | 1336 | 5 | 5 |  |
| mkDelayWorker32B | O' | 436 | 34 | 833 | 0 | 1336 | 5 | 5 |  |
| stereovision2 | P | 8415 | 15585 | 12081 | 468 | 0 | 3 | 3 |  |
| stereovision2 | O' | 8413 | 15573 | 12175 | 468 | 0 | 3 | 3 |  |
| blob_merge | P | 3381 | 575 | 3516 | 0 | 0 | 5 | 5 |  |
| blob_merge | O' | 6009 | 575 | 3815 | 0 | 0 | 5 | 5 |  |
| spree | P | 690 | 200 | 62 | 1 | 128 | 16 | 16 |  |
| arm_core | P | 9407 | 2727 | 384 | 0 | 1192 | 20 | 20 |  |


WARNING hardblocks_lost (model:count of hard blocks with no reader in the pre-VPR BLIF that the BLIF the flow started from had read; VPR sweeps them):

- mkPktMerge O': adder:19
- boundtop O': adder:90
- mkSMAdapter4B O': adder:35
- stereovision1 O': adder:120
- mkDelayWorker32B O': adder:706

## Packed

| design | leg | CLB | memories | mults | W×H | hard blocks |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 68 | 1 | 0 | 12×12 |  |
| ch_intrinsics | O' | 68 | 1 | 0 | 12×12 | = P |
| stereovision3 | P | 15 | 0 | 0 | 7×7 |  |
| stereovision3 | O' | 16 | 0 | 0 | 7×7 | = P |
| diffeq2 | P | 23 | 0 | 5 | 16×16 |  |
| diffeq2 | O' | 22 | 0 | 5 | 16×16 | = P |
| diffeq1 | P | 35 | 0 | 5 | 16×16 |  |
| diffeq1 | O' | 33 | 0 | 5 | 16×16 | = P |
| mkPktMerge | P | 34 | 15 | 0 | 28×28 |  |
| mkPktMerge | O' | 33 | 15 | 0 | 28×28 | = P |
| raygentop | P | 141 | 1 | 6 | 19×19 |  |
| raygentop | O' | 141 | 1 | 6 | 19×19 | = P |
| sha | P | 131 | 0 | 0 | 16×16 |  |
| sha | O' | 137 | 0 | 0 | 16×16 | = P |
| boundtop | P | 52 | 1 | 0 | 15×15 |  |
| boundtop | O' | 56 | 1 | 0 | 15×15 | = P |
| mkSMAdapter4B | P | 176 | 5 | 0 | 20×20 |  |
| mkSMAdapter4B | O' | 181 | 5 | 0 | 20×20 | = P |
| or1200 | P | 265 | 2 | 1 | 26×26 |  |
| or1200 | O' | 275 | 2 | 1 | 27×27 | = P |
| stereovision0 | P | 706 | 0 | 0 | 33×33 |  |
| stereovision0 | O' | 712 | 0 | 0 | 33×33 | = P |
| stereovision1 | P | 806 | 0 | 43 | 40×40 |  |
| stereovision1 | O' | 834 | 0 | 44 | 40×40 | ≠ P |
| mkDelayWorker32B | P | 481 | 43 | 0 | 50×50 |  |
| mkDelayWorker32B | O' | 485 | 43 | 0 | 50×50 | = P |
| stereovision2 | P | 1940 | 0 | 192 | 82×82 |  |
| stereovision2 | O' | 1899 | 0 | 194 | 82×82 | ≠ P |
| blob_merge | P | 502 | 0 | 0 | 29×29 |  |
| blob_merge | O' | 521 | 0 | 0 | 29×29 | = P |
| spree | P | 63 | 3 | 1 | 14×14 |  |
| arm_core | P | 853 | 24 | 0 | 37×37 |  |

## Routed

| design | leg | status | vpr_status | min W | CPD (ns) | Fmax (MHz) | WL |
|---|---|---|---|---|---|---|---|
| ch_intrinsics | P | ok | success | 40 | 1.934 | 517.0 | 1093 |
| ch_intrinsics | O' | ok | success | 42 | 2.054 | 486.8 | 1348 |
| stereovision3 | P | ok | success | 26 | 2.440 | 409.8 | 382 |
| stereovision3 | O' | ok | success | 28 | 2.340 | 427.4 | 492 |
| diffeq2 | P | ok | success | 68 | 12.430 | 80.5 | 6368 |
| diffeq2 | O' | ok | success | 50 | 12.738 | 78.5 | 7132 |
| diffeq1 | P | ok | success | 50 | 17.196 | 58.2 | 9217 |
| diffeq1 | O' | ok | success | 50 | 17.073 | 58.6 | 9010 |
| mkPktMerge | P | ok | success | 40 | 4.063 | 246.1 | 13085 |
| mkPktMerge | O' | ok | success | 40 | 4.126 | 242.4 | 12870 |
| raygentop | P | ok | success | 58 | 5.190 | 192.7 | 20146 |
| raygentop | O' | ok | success | 66 | 4.989 | 200.4 | 20038 |
| sha | P | ok | success | 66 | 9.305 | 107.5 | 11230 |
| sha | O' | ok | success | 66 | 9.735 | 102.7 | 11790 |
| boundtop | P | ok | success | 38 | 2.735 | 365.7 | 5353 |
| boundtop | O' | ok | success | 34 | 2.722 | 367.3 | 5278 |
| mkSMAdapter4B | P | ok | success | 46 | 5.461 | 183.1 | 15859 |
| mkSMAdapter4B | O' | ok | success | 48 | 6.015 | 166.3 | 15554 |
| or1200 | P | ok | success | 78 | 9.497 | 105.3 | 38743 |
| or1200 | O' | ok | success | 78 | 9.162 | 109.1 | 40012 |
| stereovision0 | P | ok | success | 46 | 4.516 | 221.4 | 53023 |
| stereovision0 | O' | ok | success | 48 | 3.822 | 261.6 | 53065 |
| stereovision1 | P | ok | success | 74 | 5.438 | 183.9 | 110454 |
| stereovision1 | O' | ok | success | 74 | 5.450 | 183.5 | 112671 |
| mkDelayWorker32B | P | ok | success | 40 | 8.724 | 114.6 | 18222 |
| mkDelayWorker32B | O' | ok | success | 38 | 7.967 | 125.5 | 18261 |
| stereovision2 | P | ok | success | 86 | 13.476 | 74.2 | 379193 |
| stereovision2 | O' | ok | success | 86 | 12.792 | 78.2 | 358970 |
| blob_merge | P | ok | success | 64 | 14.667 | 68.2 | 57997 |
| blob_merge | O' | ok | success | 58 | 14.357 | 69.7 | 55178 |
| spree | P | ok | success | 58 | 10.945 | 91.4 | 10399 |
| arm_core | P | ok | success | 96 | 23.537 | 42.5 | 148706 |

## Cost

| design | leg | front-end wall (s) | front-end peak (MiB) | VPR time (s) | VPR mem (MiB) | slice |
|---|---|---|---|---|---|---|
| ch_intrinsics | P | 0.3 | 36 | 1.2 | 71 |  |
| ch_intrinsics | O' | 0.1 | 36 | 0.9 | 70 |  |
| stereovision3 | P | 0.3 | 36 | 0.5 | 67 |  |
| stereovision3 | O' | 0.1 | 36 | 0.4 | 67 |  |
| diffeq2 | P | 0.2 | 36 | 3.3 | 76 |  |
| diffeq2 | O' | 0.1 | 36 | 2.4 | 76 |  |
| diffeq1 | P | 0.2 | 38 | 2.5 | 77 |  |
| diffeq1 | O' | 0.1 | 37 | 2.4 | 77 |  |
| mkPktMerge | P | 0.4 | 38 | 3.7 | 94 |  |
| mkPktMerge | O' | 0.1 | 38 | 3.8 | 94 |  |
| raygentop | P | 2.2 | 48 | 5.5 | 101 |  |
| raygentop | O' | 0.5 | 40 | 5.5 | 101 |  |
| sha | P | 1.2 | 51 | 4.1 | 98 |  |
| sha | O' | 0.8 | 41 | 3.8 | 98 |  |
| boundtop | P | 3.5 | 49 | 1.7 | 79 |  |
| boundtop | O' | 0.7 | 39 | 1.8 | 81 |  |
| mkSMAdapter4B | P | 2.2 | 56 | 5.4 | 104 |  |
| mkSMAdapter4B | O' | 1.0 | 42 | 5.8 | 101 |  |
| or1200 | P | 3.0 | 63 | 14.0 | 135 |  |
| or1200 | O' | 2.0 | 44 | 12.8 | 139 |  |
| stereovision0 | P | 4.9 | 101 | 18.0 | 272 |  |
| stereovision0 | O' | 3.4 | 68 | 18.0 | 267 |  |
| stereovision1 | P | 6.0 | 123 | 33.3 | 345 |  |
| stereovision1 | O' | 4.2 | 76 | 30.3 | 347 |  |
| mkDelayWorker32B | P | 7.2 | 118 | 21.3 | 310 |  |
| mkDelayWorker32B | O' | 2.1 | 54 | 16.2 | 310 |  |
| stereovision2 | P | 6.3 | 196 | 136.7 | 1162 |  |
| stereovision2 | O' | 2.7 | 150 | 134.8 | 1148 |  |
| blob_merge | P | 5.4 | 209 | 21.7 | 185 |  |
| blob_merge | O' | 2.5 | 60 | 16.8 | 192 |  |
| spree | P | 1.0 | 40 | 2.9 | 82 |  |
| arm_core | P | 24.2 | 124 | 54.8 | 310 |  |

`*`: a stage log had no `time -v` figures (job.json `cost_warnings`), so the front-end cost is incomplete. `xl`: the job ran in the 9 GiB `odin3-heavyxl.slice` (plan point (d)). Comparability (spec §18 item 2): P's front end is two VTR stages, Parmys and ABC, timed by VTR's own `time -v`, and VTR's ABC stage also pays a BLIF write and read per clock domain; an Odin III leg's front end is one `odin3` process timed by the harness (plus VTR's ABC stage for O' and R). Both are wall time and peak RSS, but not measured the same way.

## Attribution

Geomeans over the 15 gate designs.

| metric | O'/P (front end) |
|---|---|
| num_clb | 1.012 |
| min_chan_width | 0.985 |
| critical_path_delay_ns | 0.986 |
| crit_path_routed_wirelength | 1.034 |

## Functional check and determinism

| design | fcheck P |
|---|---|
| ch_intrinsics | untested (baseline: x-state) |
| stereovision3 | pass |
| diffeq2 | pass |
| diffeq1 | pass |
| mkPktMerge | pass |
| raygentop | fail (baseline: dropped-latches) |
| sha | fail (baseline: D2b) |
| boundtop | fail (baseline: dropped-latches) |
| mkSMAdapter4B | pass |
| or1200 | fail (baseline: D2b) |
| stereovision0 | fail (baseline: x-state) |
| stereovision1 | fail (baseline: lost-sign-bits) |
| mkDelayWorker32B | pass |
| stereovision2 | fail (baseline: lost-sign-bits) |
| blob_merge | fail (baseline: D2b) |
| spree | pass |
| arm_core | fail |

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
| **geomean (15)** |  |  | 1.000 |  |  | 0.996 |  |  | 0.999 |  |  | 1.000 |  |

Non-gating rows (spree, arm_core):

| design | CLB P | CLB golden | P/golden | W P | W golden | P/golden | CPD P | CPD golden | P/golden | WL P | WL golden | P/golden | outside |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| spree | 63 | 63 | 1.000 | 58 | 58 | 1.000 | 10.945 | 10.945 | 1.000 | 10399 | 10399 | 1.000 |  |
| arm_core | 853 | 853 | 1.000 | 96 | 96 | 1.000 | 23.537 | 23.537 | 1.000 | 148706 | 148706 | 1.000 |  |
| **geomean (2)** |  |  | 1.000 |  |  | 1.000 |  |  | 1.000 |  |  | 1.000 |  |
