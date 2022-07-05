# NCI-DOE-Collab-Pilot3-SYNDATA

## Description
SYNDATA is a suite of statistical and machine learning methods to generate discrete/categorical synthetic data. SYNDATA is useful for data scientists and statisticians that need data to train their models but have limited access to real patient data due to HIPAA constraints.

SYNDATA includes the following methods to generate synthetic data:
 * Mixture of Product of Multinomials (MPoM) 
 * Independent Marginals
 * Categorical Latent Gaussian process (CLGP)
 * Multivariate Imputation by Chained Equations (MICE)

For more details on the methods implemented and the metrics used to evaluate synthetic data generation methods, refer to this paper: [Generation and evaluation of synthetic patient data](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## User Community
Data scientists and statisticians interested in producing realistic synthetic clinical data.

## Usability	
Users must provide their own input data of discrete/categorical variables only. SYNDATA includes scripts to prepare an example dataset. 

To utilize SYNDATA, users must have experience with Python and be familiar with the methods listed above to set the parameters appropriately. 
 
A GPU-powered computer would allow faster execution of SYNDATA.

## Uniqueness	
SYNDATA gives the user four methods to use for generating synthetic clinical data containing discrete/categorical variables only. 

In addition, SYNDATA provides performance metrics for assessing each method individually and/or comparing multiple methods at once. Some of these performance metrics are as follows:
 * Data utility metrics gauge to what extent the method captures and transfers the statistical properties of the real (private) data to the synthetic dataset (that is, support coverage, cross-classification).
 * Disclosure metrics measure how much of the real data may be revealed (directly or indirectly) by the synthetic data (that is, membership disclosure, attribute disclosure).

## Components	

* Script: The [demo.py](./experiments/demo.py) file contains a demo script to train different methods on an example dataset, generate synthetic data, and produce performance metric reports.
* Data: The [UCIBreast.py](./datasets/UCIBreast.py) file contains code to prepare an example dataset from [UCI Machine Learning Repository Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/breast+cancer).

## Technical Details
Refer to this [README](./Technical_README.md).

## Reference
For more details, refer to this [publication](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## Authors

- Andre Goncalves (LLNL)
- Rui Meng (LLNL)
- Braden Soper (LLNL)
- Priyadip Ray (LLNL)
- Ana Paula Sales (LLNL)

LLNL - Lawrence Livermore National Laboratory

## Code Release

LLNL-CODE-831774
