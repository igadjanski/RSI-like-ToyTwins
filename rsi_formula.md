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
| AR | | M23263_at |
| cJun | | J04111_at |
| STAT1 | | AFFX-HUMISGF3A/M97935_MA_at |
| PKC | | X06318_at |
| RelA | | U33838_at |
| cABL | | X16416_at |
| SUMO1 | | U83117_at |
| CDK1 | | U24153_at |
| HDAC | | D50405_at |
| IRF1 | | L05072_s_at |

## Training data
48 NCI-60 cancer cell lines; outcome SF2; Affymetrix HU6800, MAS 5.0.
High RSI = radioresistance.

## Open questions
- Are ranks 1-10 used as is, or rescaled?
- Which direction does "rank-ordered" go for tied expression values?

