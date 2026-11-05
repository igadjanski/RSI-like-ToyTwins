# RSI formula (Eschrich et al. 2009)

## Source
Eschrich SA, et al. A gene expression model of intrinsic tumor radiosensitivity:
prediction of response and prognosis after chemoradiation.
Int J Radiat Oncol Biol Phys 2009;75(2):489-496. doi:10.1016/j.ijrobp.2009.06.014
Equation: page 6 of the author manuscript (PMC3038688), Results section.

## Equation
RSI = sum over the 10 genes of (coefficient x rank of the gene's expression)
Ranks: the 10 genes are rank-ordered within a sample, lowest expression = rank 1.
No intercept term appears in the printed equation.

## Coefficients (as printed, in order)
| Gene | Coefficient | HU6800 probe set |
|---|---|---|
| AR | -0.0098009 | M23263_at |
| cJun | +0.0128283| J04111_at |
| STAT1 | +0.0254552| AFFX-HUMISGF3A/M97935_MA_at |
| PKC | -0.0017589 | X06318_at |
| RelA |-0.0038171 | U33838_at |
| cABL | +0.1070213| X16416_at |
| SUMO1 | -0.0002509| U83117_at |
| CDK1 | -0.0092431| U24153_at |
| HDAC | -0.0204469| D50405_at |
| IRF1 | -0.0441683| L05072_s_at |

## Training data
48 NCI-60 cancer cell lines; outcome SF2; Affymetrix HU6800, MAS 5.0.
High RSI = radioresistance.

## Open questions
- Are ranks 1-10 used as is, or rescaled? 
- Update: rescaling is probably not applied, and tie handling is still unknown.

