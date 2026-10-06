# Data Dictionary (FORCE 2020, from LAS files)

Null value: -999.25. Units below marked [Likely] are not stated in the source and need confirming.

| Column | Meaning | Wells >50% filled | Plan |
|---|---|---|---|
| GR | Gamma ray | 118 | Feature |
| RDEP / RMED | Deep / medium resistivity | 116 / 114 | Feature (log10) |
| DTC | Compressional sonic | 102 | Feature |
| RHOB | Bulk density | 81 | Feature |
| NPHI | Neutron porosity | 52 | Feature, limits well count |
| PEF | Photoelectric factor | 51 | Test as feature |
| CALI / BS | Caliper / bit size | 82 / 73 | Quality flag (washouts) |
| DRHO | Density correction | 76 | Quality flag |
| SP, ROP, RSHA | Other curves | 69 / 64 / 43 | Test later |
| SGR, RMIC, RXO, DTS, DCAL, MUDWEIGHT, ROPA | Sparse curves | 2 to 37 | Excluded (too sparse) |
| DEPTH_MD, X_LOC, Y_LOC, Z_LOC | Depth and location | ~116 | Shortcut risk: test with and without |
| FORCE_2020_LITHOFACIES_LITHOLOGY | Target class code | 82 | Target (12 classes) |
| FORCE_2020_LITHOFACIES_CONFIDENCE | 1 high, 2 medium, 3 low | 82 | Test high-confidence only |

## Lithology codes (from starter notebook)
30000 Sandstone, 65030 Sandstone/Shale, 65000 Shale, 80000 Marl, 74000 Dolomite, 70000 Limestone, 70032 Chalk, 88000 Halite, 86000 Anhydrite, 99000 Tuff, 90000 Coal, 93000 Basement.
