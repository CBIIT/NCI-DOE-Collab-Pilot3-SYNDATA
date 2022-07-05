## Setup

To set up the Python environment needed to run SYNDATA:
1. Install [conda](https://docs.conda.io/en/latest/) package manager. 
2. Clone this repository. 
3. Create the environment as shown below.

```bash
   conda env create -f environment.yml -n syndata
   conda activate syndata
```

## Training

The *experiments/* folder provides a starter script, [demo.py](./experiments/demo.py), to run SYNDATA. One can use this starter script to build additional scripts for running new experiments.

To run this script, execute the following command: 

```
python demo.py
```

The script performs the following steps: 

1) Downloads the [UCI's Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer), label encodes each categorical variable in the dataset, and prepares the input data for training.
2) Defines the methods, parameters, and performance metrics to use.
3) Trains each method with the input data.
4) Generates multiple samples of synthetic data and saves them and the performance results to a pickle file.
5) Produces a PDF report comparing the performance of the methods. 

Output files with the logs, results, and PDF report from running *demo.py* can be found in the [*outputs/demo/*](./outputs/demo) folder.

## Acknowledgments
   
This work has been supported in part by the Joint Design of Advanced Computing Solutions for Cancer (JDACS4C) program established by the U.S. Department of Energy (DOE) and the National Cancer Institute (NCI) of the National Institutes of Health.
