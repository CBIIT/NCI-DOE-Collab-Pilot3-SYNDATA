# Synthetic Data Generation with Machine Learning (SYNDATA)

SYNDATA software includes a suite of statistical/machine learning models to generate discrete/categorical synthetic data. To train each model, the user must provide the input data from which the model parameters will be infered. Once the models are trained, they can be used to generate entirely synthetic data. Finally, in addition to the actual models, SYNDATA includes code to process data, evaluate results (based on cross validation), and create a PDF report.

For more details of the methods implemented and the metrics used to evaluate synthetic data generation models, we refer to our paper: [Generation and evaluation of synthetic patient data](https://bmcmedresmethodol.biomedcentral.com/track/pdf/10.1186/s12874-020-00977-1.pdf).


## Installation

This software suite runs on specific versions of Python and its libraries. We recommend creating a Python environment and install all dependencies from `requirements.txt` file. To create an environment and install the correct version of the packages, do:

`python3 -m venv datagen_env`

then activate the environment:

`source datagen_env/bin/activate`

finally, install all dependencies:

`python -m pip install -r requirements.txt`

Done. You can now start running your experiments.


## Quick Start

A demo file is available in the `experiments/` folder. It runs an experiment with [UCI's Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer) data. One can build up on this file to create new experiments.

`python demo.py`

A folder with logs and a PDF report will be created in `outputs/` folder. Check that out after running your experiment. The `demo.py` script may take a few minutes to complete. We recomend using a GPU-powered computer for a faster execution.


## Authors:

- Andre Goncalves (LLNL)
- Rui Meng (LLNL)
- Braden Soper (LLNL)
- Priyadip Ray (LLNL)
- Ana Paula Sales (LLNL)


## Code Release

LLNL-CODE-831774
