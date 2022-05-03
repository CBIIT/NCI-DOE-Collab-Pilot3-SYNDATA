# NCI-DOE-Collab-Pilot3-SYNDATA

## Description
Suite of statistical/machine learning models to generate discrete/categorical synthetic data. Generate synthetic clinical data. It useful for data science researchers/statisticians that need the data to train their models but cannot have access to real data due to HIPPA constraints.

SYNDATA software includes a suite of statistical/machine learning models to generate discrete/categorical synthetic data. To train each model, the user must provide the input data from which the model parameters will be infered. Once the models are trained, they can be used to generate entirely synthetic data. Finally, in addition to the actual models, SYNDATA includes code to process data, evaluate results (based on cross validation), and create a PDF report.

For more details of the methods implemented and the metrics used to evaluate synthetic data generation models, we refer to our paper: [Generation and evaluation of synthetic patient data](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-020-00977-1).

## User Community
Data scientists and statisticians interested in generating more examples of unstructured text with a specific label from a given corpus for training machine learning or deep learning models on clinical text.

## Usability	
Data scientists can train the provided untrained model on their own data or with preprocessed data of clinical pathology reports included with this resource. These reports came from the [Surveillance, Epidemiology, and End Results](https://seer.cancer.gov/) (SEER) Program.

To use this resource, users must be familiar with natural language processing (NLP) and training neural networks, specifically RNNs.

## Uniqueness	
Generative models of text is a known problem in the natural language processing community. The model architecture provided in this resource was tested on unstructured clinical data from SEER. Data scientists can further optimize this architecture using the [CANcer Distributed Learning Environment](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/candle) (CANDLE). 
data-owners to generate and evaluate synthetic data based on real data in order to make it available to the broader research community.

## Components	

* Data:
  * [UCIBreast.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-SYNDATA/blob/main/datasets/UCIBreast.py)


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
