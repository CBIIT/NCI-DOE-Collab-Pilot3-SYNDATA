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

1) Downloads the [UCI's Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer), label encodes each categorical variable in the dataset, and prepares the input data for training.
2) Defines the methods, parameters, and performance metrics to use.
3) Trains each method with the input data.
4) Generates multiple samples of synthetic data and saves them and the performance results to a pickle file.
5) Produces a PDF report comparing the performance of the methods. 
To run SYNDATA, an example of how to set up exdemo.py Within `experiments/` folder is a. It runs an experiment with [UCI's Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer) data. One can build up on this file to create new experiments.

```
python demo.py
```

Examples of the output files with the logs, results, and PDF report from running `demo.py` can be found here [`outputs/demo/` folder] (https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/tree/main/outputs/demo).
