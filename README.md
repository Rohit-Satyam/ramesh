# ramesh
**Design formula**: The design formula specifies the column(s) in the metadata table and how they should be used in the analysis. For our dataset we only have one column we are interested in, which is `~category`. This column has two factor levels, which tells DESeq2 that for each gene we want to evaluate gene expression change with respect to these different levels.
