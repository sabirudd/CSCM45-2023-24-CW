`05/12/2023 - 13/12/2023`

# CSCM45 - Big Data & Machine Learning (2023/24) Coursework
Implementation and comparison of several classical machine learning methods. <br />
Comparison (detailed in report) generated using confusion matrices, F1-score and accuracy curves. <br />
All data was normalised and then trained using a portion of the main dataset (trn) and then tested using a different portion of the dataset (tst). <br />

## ML methods implemented:
```
> K-Means Clustering
> Linear Discriminative Analysis
> Support Vector Machine
> Neural Networks
> Convolutional Neural Networks
```


## Modules used:
```
> numpy
> matplotlib
> skimage
> sklearn
> tensorflow
```


## Dataset:
CIFAR-100 (fine and coarse)


## File Structure:
```
.
├── files
│   ├── classes
│       ├── coarse_labels.csv
│       └── fine_labels.csv
│   ├── datasets
│       ├── trnImage.npy
│       ├── trnLabel_coarse.npy
│       ├── trnLabel_fine.npy
│       ├── tstImage.npy
│       ├── tstLabel_coarse.npy
│       └── tstLabel_fine.npy
└── CSCM45_CW.ipynb
```
