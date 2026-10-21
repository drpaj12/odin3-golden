# M2 after the RAM-loss fix (2026-10-21)

O' leg on main after #196 (write_blif --vtr port buffer for box-driven outputs; Parmys's opt order with opt -full after flatten). 15 of 15 routed. Geomeans O'/P: LUTs 1.041, CLB 1.012, memories 1.000, channel width 0.985, delay 0.986, wirelength 1.034. mkPktMerge and boundtop now pack all their memories; raygentop LUTs 1.03 (was 1.42). Outlier left: blob_merge LUTs 1.78 (CLB 1.04).
