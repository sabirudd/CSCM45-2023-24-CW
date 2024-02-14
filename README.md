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


## Results (from the report):
| Model                          | Label Type | Parameters           | Precision | Recall | F1-Score | Time/s | Efficiency (F1%/Time) |
| ------------------------------ | ---------- | -------------------- | --------- | ------ | -------- | ------ | ---------------------- |
| **K-Means**                    | Coarse     | n_clusters=20        | 0.05      | 0.05   | 0.05     | 20     | 0.250                 |
|                                |            | n_clusters=10        | 0.03      | 0.05   | 0.03     | 10     | 0.300                 |
|                                | Fine       | n_clusters=100       | 0.01      | 0.01   | 0.01     | 49     | 0.020                 |
| **Linear Discriminative Analysis** | Coarse | n_components=2      | 0.27      | 0.28   | 0.27     | 3      | 9.000                 |
|                                |            | n_components=9       | 0.27      | 0.28   | 0.27     | 3      | 9.000                 |
|                                |            | n_components=19      | 0.27      | 0.28   | 0.27     | 3      | 9.000                 |
|                                | Fine       | n_components=2       | 0.19      | 0.21   | 0.19     | 3      | 6.333                 |
|                                |            | n_components=49      | 0.19      | 0.21   | 0.19     | 3      | 6.333                 |
|                                |            | n_components=99      | 0.19      | 0.21   | 0.19     | 3      | 6.333                 |
| **Support Vector Machine**     | Coarse     | C=1.0               | 0.40      | 0.40   | 0.40     | 597    | 0.067                 |
|                                |            | C=5.0               | 0.42      | 0.42   | 0.42     | 710    | 0.059                 |
|                                |            | C=10.0              | 0.41      | 0.41   | 0.41     | 712    | 0.058                 |
|                                | Fine       | C=1.0               | 0.29      | 0.29   | 0.28     | 569    | 0.051                 |
|                                |            | C=5.0               | 0.30      | 0.31   | 0.30     | 662    | 0.045                 |
|                                |            | C=10.0              | 0.30      | 0.31   | 0.30     | 664    | 0.045                 |
| **Neural Network**             | Coarse     | 5 N-Layers          | 0.36      | 0.36   | 0.36     | 361    | 0.100                 |
|                                | Fine       | 5 N-Layers          | 0.25      | 0.25   | 0.25     | 291    | 0.100                 |
| **Convolutional Neural**       | Coarse     | 2 C, 5 N-Layers      | 0.51      | 0.50   | 0.50     | 539    | 0.093                 |
|                                | Fine       | 2 C, 5 N-Layers      | 0.38      | 0.37   | 0.37     | 533    | 0.069                 |


