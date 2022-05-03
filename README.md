# NCI-DOE-Collab-Pilot3-SYNDATA
Suite of statistical/machine learning models to generate discrete/categorical synthetic data

## Description
Given a sample corpus of biomedical text (such as pathology reports), this resource builds a long short-term memory (LSTM) model, a type of recurrent neural network (RNN), to automatically generate synthetic biomedical text of desired clinical context. This resource addresses the challenge of collecting labeled data, specifically clinical data, needed to create robust machine learning and deep learning models.

## User Community
Data scientists interested in generating more examples of unstructured text with a specific label from a given corpus for training machine learning or deep learning models on clinical text.

## Usability	
Data scientists can train the provided untrained model on their own data or with preprocessed data of clinical pathology reports included with this resource. These reports came from the [Surveillance, Epidemiology, and End Results](https://seer.cancer.gov/) (SEER) Program.

To use this resource, users must be familiar with natural language processing (NLP) and training neural networks, specifically RNNs.

## Uniqueness	
Generative models of text is a known problem in the natural language processing community. The model architecture provided in this resource was tested on unstructured clinical data from SEER. Data scientists can further optimize this architecture using the [CANcer Distributed Learning Environment](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/candle) (CANDLE). 

## Components	
* Script to train a LSTM-based model: [p3b2_baseline_keras2.py](https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-RNN-LSTM-based-Clinical-Text-Generator/blob/master/Pilot3/P3B2/p3b2_baseline_keras2.py)
* Data: The preprocessed training and test data of SEER clinical pathology reports are in the [LSTM-based Clinical Text Generator](https://modac.cancer.gov/searchTab?dme_data_id=NCI-DME-MS01-18031472) asset in the Model and Data Clearinghouse (MoDaC).


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
