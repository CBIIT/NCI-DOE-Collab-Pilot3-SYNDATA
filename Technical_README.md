## Setup

To set up the Python environment needed to run SYNDATA:
1. Install [conda](https://docs.conda.io/en/latest/) package manager. 
2. Clone this repository. 
3. Create the environment as shown below.

```bash
   conda env create -f environment.yml -n syndata
   conda activate syndata
```


## Quick Start

A demo file is available in the `experiments/` folder. It runs an experiment with [UCI's Breast Cancer](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer) data. One can build up on this file to create new experiments.

`python demo.py`

A folder with logs and a PDF report will be created in `outputs/` folder. Check that out after running your experiment. 
