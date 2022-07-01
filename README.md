# NCI-DOE-Collab-Pilot3-SYNDATA

## Description
SYNDATA is a suite of statistical and machine learning methods to generate discrete/categorical synthetic data. SYNDATA is useful for data scientists and statisticians that need data to train their models but have limited access to real patient data due to HIPAA constraints.

SYNDATA includes the following methods to generate synthetic data:
 * Mixture of Product of Multinomials (MPoM) 
 * Independent Marginals
 * Categorical Latent Gaussian process (CLGP)
 * Multivariate Imputation by Chained Equations (MICE)

For more details of the methods implemented and the metrics used to evaluate synthetic data generation methods, please refer to this paper: [Generation and evaluation of synthetic patient data](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## User Community
Data scientists and statisticians interested in producing real-like synthetic clinical data.

## Usability	
Users must provide their own input data of discrete/categorical variables only. SYNDATA includes scripts to prepare an example dataset. 

To utilize SYNDATA, users must be experienced with Python and be familiar with the methods listed above to set the parameters appropriately. 
 
We recommend using a GPU-powered computer for faster execution of SYNDATA.

## Uniqueness	
SYNDATA gives the user four methods to use for generating synthetic clinical data containing discrete/categorical variables only. In addition, SYNDATA provides the user with a list of performance metrics for assessing each method individually and/or comparing multiple methods at once. 

The performance metrics include:
 * data utility metrics - gauge to what extent the statistical properties of the real (private) data are captured and transferred to the synthetic dataset (i.e. support coverage, cross-classification)
 * disclosure metrics - measure how much of the real data may be revealed (directly or indirectly) by the synthetic data (i.e. membership disclosure, attribute disclosure)

## Components	

* Script:
  * [demo.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/blob/main/experiments/demo.py): demo script to train different methods on an example dataset, generate synthetic data, and produce performance metric reports
* Data:
  * [UCIBreast.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/blob/main/datasets/UCIBreast.py): code to prepare an example dataset from [UCI Machine Learning Repository Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/breast+cancer) 

## Technical Details
Refer to this [README](./Technical_README.md).

## Reference
For more details, refer to this [publication](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## Authors:

- Andre Goncalves (LLNL)
- Rui Meng (LLNL)
- Braden Soper (LLNL)
- Priyadip Ray (LLNL)
- Ana Paula Sales (LLNL)

LLNL - Lawrence Livermore National Laboratory

## Code Release

LLNL-CODE-831774
