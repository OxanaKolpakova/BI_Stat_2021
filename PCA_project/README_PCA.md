We need to predict the critical temperature of the superconductor (column critical_temp) from various characteristics of the substance and its composition (all other columns).

As a result of the analysis, we got:
1) built a multiple linear regression model
 lm  <- (critical_temp ~., datа),  adj. R ^ 2 = 0.74.
2) To improve the model, we performed PCA, identified the most significant PCs.
3) built a new multiple linear regression model 
postPCA_model <- lm (critical_temp ~., datа) using the predicted PCs, - adj. R ^ 2 = 0.59.
The new linear model turned out to be worse than the previous one ((.
4) To improve the model, we decided to run a kernel PCA.
We ran out of memory for analysis.
5) Download file of kernel PCs courtesy by Danil Linvinov and take recommended 5PCs and transform test data.
 
(( But I did not complete the analysis because
I could not convert the PCs_kernel% *% #testSet_forPCA matrix.
The provided X_kpca.npy file and my testSet_forPCA 
have different number of observations. I could not quickly solve this problem ((

I wrote code for further linear modeling with transformed data analysis.
