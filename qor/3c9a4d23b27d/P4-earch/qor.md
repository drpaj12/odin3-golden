# Odin III QoR — EArch — P4-earch

VTR 3c9a4d23b27d · odin3 1cc53b820a37 (build 3e8f917db615) · ABC script 0d0d27670d8c · legs O' c6b0b87fe3a6
· host 13th Gen Intel(R) Core(TM) i7-13700, 23.5 GiB · 2026-10-21T15:28:49Z

## Netlist

| design | leg | luts | ffs | adders | mults | ram_slices | depth | abc_depth | exchange |
|---|---|---|---|---|---|---|---|---|---|
| ch_intrinsics | O' | 96 | 82 | 0 | 0 | 8 | 3 | 3 |  |
| stereovision3 | O' | 124 | 117 | 31 | 0 | 0 | 2 | 4 |  |
| diffeq2 | O' | 196 | 96 | 136 | 5 | 0 | 4 | 4 |  |
| diffeq1 | O' | 294 | 193 | 136 | 5 | 0 | 5 | 5 |  |
| mkPktMerge | O' | 176 | 18 | 51 | 0 | 459 | 2 | 2 |  |
| raygentop | O' | 1073 | 946 | 453 | 15 | 21 | 3 | 3 |  |
| sha | O' | 1210 | 893 | 320 | 0 | 0 | 3 | 3 |  |
| boundtop | O' | 537 | 383 | 166 | 0 | 32 | 3 | 3 |  |
| mkSMAdapter4B | O' | 1096 | 639 | 370 | 0 | 153 | 5 | 5 |  |
| or1200 | O' | 2466 | 672 | 563 | 1 | 64 | 8 | 8 |  |
| stereovision0 | O' | 6826 | 11458 | 2741 | 0 | 0 | 5 | 5 |  |
| stereovision1 | O' | 6355 | 10315 | 2482 | 152 | 0 | 3 | 3 |  |
| mkDelayWorker32B | O' | 436 | 34 | 833 | 0 | 1336 | 5 | 5 |  |
| stereovision2 | O' | 8413 | 15573 | 12175 | 468 | 0 | 3 | 3 |  |
| blob_merge | O' | 6009 | 575 | 3815 | 0 | 0 | 5 | 5 |  |


WARNING hardblocks_lost (model:count of hard blocks with no reader in the pre-VPR BLIF that the BLIF the flow started from had read; VPR sweeps them):

- mkPktMerge O': adder:19
- boundtop O': adder:90
- mkSMAdapter4B O': adder:35
- stereovision1 O': adder:120
- mkDelayWorker32B O': adder:706

## Packed

| design | leg | CLB | memories | mults | W×H | hard blocks |
|---|---|---|---|---|---|---|
| ch_intrinsics | O' | 65 | 1 | 0 | 12×12 |  |
| stereovision3 | O' | 14 | 0 | 0 | 7×7 |  |
| diffeq2 | O' | 22 | 0 | 5 | 16×16 |  |
| diffeq1 | O' | 28 | 0 | 5 | 16×16 |  |
| mkPktMerge | O' | 33 | 15 | 0 | 28×28 |  |
| raygentop | O' | 133 | 1 | 6 | 19×19 |  |
| sha | O' | 119 | 0 | 0 | 15×15 |  |
| boundtop | O' | 49 | 1 | 0 | 15×15 |  |
| mkSMAdapter4B | O' | 157 | 5 | 0 | 20×20 |  |
| or1200 | O' | 222 | 2 | 1 | 27×27 |  |
| stereovision0 | O' | 688 | 0 | 0 | 33×33 |  |
| stereovision1 | O' | 778 | 0 | 44 | 40×40 |  |
| mkDelayWorker32B | O' | 470 | 43 | 0 | 50×50 |  |
| stereovision2 | O' | 1870 | 0 | 192 | 82×82 |  |
| blob_merge | O' | 486 | 0 | 0 | 28×28 |  |

## Routed

| design | leg | status | vpr_status | min W | CPD (ns) | Fmax (MHz) | WL |
|---|---|---|---|---|---|---|---|
| ch_intrinsics | O' | ok | success | 38 | 2.172 | 460.4 | 1143 |
| stereovision3 | O' | ok | success | 26 | 2.514 | 397.7 | 541 |
| diffeq2 | O' | ok | success | 56 | 13.279 | 75.3 | 7866 |
| diffeq1 | O' | ok | success | 60 | 17.659 | 56.6 | 9540 |
| mkPktMerge | O' | ok | success | 36 | 4.319 | 231.6 | 13548 |
| raygentop | O' | ok | success | 86 | 4.841 | 206.6 | 21717 |
| sha | O' | ok | success | 78 | 9.816 | 101.9 | 14219 |
| boundtop | O' | ok | success | 38 | 3.209 | 311.6 | 5813 |
| mkSMAdapter4B | O' | ok | success | 74 | 5.613 | 178.1 | 17706 |
| or1200 | O' | ok | success | 88 | 8.989 | 111.2 | 48074 |
| stereovision0 | O' | ok | success | 66 | 4.053 | 246.7 | 60586 |
| stereovision1 | O' | ok | success | 80 | 5.341 | 187.2 | 116024 |
| mkDelayWorker32B | O' | ok | success | 38 | 8.935 | 111.9 | 18736 |
| stereovision2 | O' | ok | success | 82 | 13.338 | 75.0 | 373176 |
| blob_merge | O' | ok | success | 86 | 14.022 | 71.3 | 72524 |

## Cost

| design | leg | front-end wall (s) | front-end peak (MiB) | VPR time (s) | VPR mem (MiB) | slice |
|---|---|---|---|---|---|---|
| ch_intrinsics | O' | 0.1 | 36 | 1.4 | 70 |  |
| stereovision3 | O' | 0.2 | 36 | 0.7 | 67 |  |
| diffeq2 | O' | 0.1 | 36 | 5.8 | 76 |  |
| diffeq1 | O' | 0.1 | 38 | 4.6 | 77 |  |
| mkPktMerge | O' | 0.2 | 37 | 6.9 | 95 |  |
| raygentop | O' | 0.8 | 40 | 12.1 | 102 |  |
| sha | O' | 1.2 | 41 | 6.4 | 95 |  |
| boundtop | O' | 1.1 | 39 | 2.9 | 79 |  |
| mkSMAdapter4B | O' | 1.4 | 42 | 12.1 | 111 |  |
| or1200 | O' | 3.0 | 44 | 38.7 | 148 |  |
| stereovision0 | O' | 5.1 | 68 | 27.1 | 279 |  |
| stereovision1 | O' | 7.7 | 76 | 72.2 | 374 |  |
| mkDelayWorker32B | O' | 4.6 | 54 | 36.8 | 377 |  |
| stereovision2 | O' | 5.6 | 150 | 211.1 | 1350 |  |
| blob_merge | O' | 3.6 | 60 | 44.1 | 222 |  |

`*`: a stage log had no `time -v` figures (job.json `cost_warnings`), so the front-end cost is incomplete. `xl`: the job ran in the 9 GiB `odin3-heavyxl.slice` (plan point (d)). Comparability (spec §18 item 2): P's front end is two VTR stages, Parmys and ABC, timed by VTR's own `time -v`, and VTR's ABC stage also pays a BLIF write and read per clock domain; an Odin III leg's front end is one `odin3` process timed by the harness (plus VTR's ABC stage for O' and R). Both are wall time and peak RSS, but not measured the same way.
