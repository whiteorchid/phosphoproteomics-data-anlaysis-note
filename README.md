# phosphoproteomics-data-anlaysis-note
note the important steps in the phospho data analysis


The common issue in phospho proteomics data analysis is the missing values in the expression matrix. Various the tools have developed to address this issue.

**MissForest** and **KNNimpute** are among the nice tools to impute the missing values. 

1) MissForest: https://rpubs.com/lmorgan95/MissForest
   <br /> Just run the command ```imputed_X <- missForest(X)$ximp```, X is the expression matrix/data frame of phosphho proteomics data. This can takes near 10mins or longer to finish. 
   speedup is possible by using the parallel related packages in R. 
