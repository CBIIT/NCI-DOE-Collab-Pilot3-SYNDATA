# NCI-DOE-Collab-Pilot3-SYNDATA

## Description
SYNDATA is a suite of statistical and machine learning models to generate discrete/categorical synthetic data. SYNDATA is useful for data scientists and statisticians that need data to train their models but have limited access to real patient data due to HIPPA constraints.

For more details of the methods implemented and the metrics used to evaluate synthetic data generation models, please refer to this paper: [Generation and evaluation of synthetic patient data](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## User Community
Data scientists and statisticians interested in producing real-like synthetic clinical data.

## Usability	
Users can train the provided untrained model on their own data or with preprocessed data of clinical pathology reports included with this resource. These reports came from the [Surveillance, Epidemiology, and End Results](https://seer.cancer.gov/) (SEER) Program.

To use this resource, users must be familiar with 
Data scientists can train the provided untrained model on their own data, or use the trained model to <fill in the details>. The provided scripts use data that have been downloaded from <location> and normalized.
 
Requires many software dependencies, even on well-supported high-performance computing systems such as NIH's Biowulf.
 
To use the software package in this repository, users must meet the following criteria:
 * Possess the basic skills to program and run Python scripts.
 * Able to process the input data into the data format accepted by the package.
 * Understand the input parameters of the <name> algorithm, so that they can set the parameters appropriately to execute the algorithm.

## Uniqueness	
SYNDATA includes 

## Components	

* Demo script to train models on input data from [UCI Machine Learning Repository Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/breast+cancer) and generate synthetic data:[demo.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/blob/main/experiments/demo.py)
* Data:
  * Code to prepare the dataset from [UCI Machine Learning Repository Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/breast+cancer): [UCIBreast.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/blob/main/datasets/UCIBreast.py)


## Technical Details
Refer to this [README](.Technical_README.md).

## Authors:

- Andre Goncalves (LLNL)
- Rui Meng (LLNL)
- Braden Soper (LLNL)
- Priyadip Ray (LLNL)
- Ana Paula Sales (LLNL)

LLNL - Lawrence Livermore National Laboratory

## Code Release

LLNL-CODE-831774
