# ramesh
**Design formula**: The design formula specifies the column(s) in the metadata table and how they should be used in the analysis. For our dataset we only have one column we are interested in, which is `~category`. This column has two factor levels, which tells DESeq2 that for each gene we want to evaluate gene expression change with respect to these different levels. <br><br>
| Eif5a         | 112.8036 | 2.902334 | 0.507066 | 3.751648 | 0.000176 | 0.000685 | Eif5a         |
| ------------- | -------- | -------- | -------- | -------- | -------- | -------- | ------------- |
| Dmwd          | 14.14958 | 2.904271 | 0.760006 | 2.505599 | 0.012224 | 0.027943 | Dmwd          |
| 4932441J04Rik | 68.9476  | 2.904977 | 0.668137 | 2.851176 | 0.004356 | 0.011493 | 4932441J04Rik |
| Rps27l        | 15.55682 | 2.908503 | 0.705725 | 2.704316 | 0.006845 | 0.016982 | Rps27l        |
| Gm44280       | 72.1891  | 2.909245 | 0.627638 | 3.041953 | 0.00235  | 0.006724 | Gm44280       |
| Oasl1         | 17.63593 | 2.90998  | 0.803647 | 2.376641 | 0.017471 | 0.038122 | Oasl1         |
| H6pd          | 33.40748 | 2.9111   | 0.738076 | 2.5893   | 0.009617 | 0.022727 | H6pd          |


```r
library(DESeq2)
## Raw counts
dds <- estimateSizeFactors(dds.filtered)

## to view sizefactors
sizeFactors(dds)

```
