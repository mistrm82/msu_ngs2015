# DE analysis module for Week3


For RNA-seq data, the strategy taken is to count the number of reads that fall into annotated genes and to perform statistical analysis on the table of counts to discover quantitative changes in expression levels between experimental groups. Easy, right? Not, exactly.

1. We have integer counts and not continous measurements. Data is not normally distributed, so statistical methods we applied to microarray data don't work here. 

2. Replication levels in designed RNA-Seq experiments tend to be modest, often not much more than two or three. As a result, there is a need for statistical methods that perform well in small-sample situations. The low levels of replication rule out, for all practical purposes, distribution-free rank or permutation-based methods.  

3. The Poisson model doesn't work either -- it is a single parameter model with mean == variance and real data has more variance than Poisson can explain (which we will look at in our dataset). **using Poisson means underestimating variance and overstating the differences; only suitable for variability observed when sampling the same DNA population**

**Solution:** 


> ## Learning Objectives 
>
> * 
> * 
> * 
