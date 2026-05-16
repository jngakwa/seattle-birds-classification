# Seattle Birds Classification

## Overview
This project uses neural networks to classify 12 bird species common to the Seattle 
area based on their calls. Audio recordings from the Xeno-Canto archive were 
preprocessed into mel spectrograms and used to train and compare multiple neural 
network architectures including feedforward networks, convolutional neural networks 
(CNNs), and recurrent neural networks (RNNs).

## Repository Structure
Deep Learning/
├── Code/
│   └── Bird_Identification_NN.ipynb
├── Data/
│   ├── bird_spectrograms.hdf5  (not included - exceeds GitHub file size limit)
│   ├── test1.mp3               (not included)
│   ├── test2.mp3               (not included)
│   └── test3.mp3               (not included)
└── Report/
    └── Seattle_Birds_Classification_Report.docx

## Species Classified
| Code | Species |
|------|---------|
| amecro | American Crow |
| amerob | American Robin |
| bewwre | Bewick's Wren |
| bkcchi | Black-capped Chickadee |
| daejun | Dark-eyed Junco |
| houfin | House Finch |
| houspa | House Sparrow |
| norfli | Northern Flicker |
| rewbla | Red-winged Blackbird |
| sonspa | Song Sparrow |
| spotow | Spotted Towhee |
| whcspa | White-crowned Sparrow |

## Models
- Binary CNN and RNN classifying daejun vs houfin
- Multiclass feedforward NN, CNN, and RNN classifying all 12 species
- CNN architecture comparison on balanced dataset

## Results
| Model | Dataset | Accuracy |
|-------|---------|----------|
| Binary CNN | Original | 90.48% |
| Multiclass CNN | Original | 50.88% |
| Multiclass CNN A | Balanced | 38.54% |

## Data
The spectrogram data is not included in this repository due to file size limits. 
The original data comes from the Xeno-Canto bird sounds archive and was preprocessed 
into mel spectrograms with dimensions of 128 x 517 per sample.

## Dependencies
- h5py
- numpy
- matplotlib
- librosa
- scikit-learn
- keras
- tensorflow

## Author
Njenga Gakwa  
DATA 5322 Statistical Machine Learning II  
Seattle University, 2026
