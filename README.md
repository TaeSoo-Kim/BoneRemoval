# BoneRemoval
BoneRemoval Project for Siemens HC Medical Imaging Team, summer 2016.


## Model Leaderboard

###Current models and performance on training set *with* padding data.

| Model | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy  | Test Set Accuracy | CPU Time(s)| GPU Time(s) |#Params
| ---|:---:|:---:|:---:| :---:|:---:|:---:|:---:|:---:|:---:|
|  Baseline              | 0.0717 | 0.9782 | 0.0809 | 0.9723 | 0.964 | 194.54 | **5.49** | 68920|
|  Baseline+(BN->ReLU)   | x | x | x | x | x | 204.06 | 6.40 | 68920|
| Decomp Net             | 0.1289 | 0.9711 | 0.0824 | **0.9725** | 0.963 | 64.70 | 6.94 | 7416 
| Decomp Net+(BN->ReLU)  | x | x | x | x | x | 88.21 | 13.09 | 7416
| Baseline filtergroup v1| 0.0884 | 0.9742 | 0.087 | 0.969 | 0.956 | 135.69 | 5.81 | 46968
| Baseline filtergroup v2| 0.1821 | 0.9374 | 0.1575 | 0.9436 | 0.928 | 66.80 | 6.32 | 21992
| Decomp filtergroup v1  | 0.1989 | 0.9377 | 0.1545 | 0.9448 | 0.937 | 37.80 | 13.83 | 4696
| Decomp filtergroup v2  | 0.2465 | 0.9150 | 0.1916 | 0.9284 | 0.923 | **32.72** | 18.00 | **2216**
| Decomp filtergroup v2, student | 0.2431 | 0.9320 | 0.1806 | 0.9460 | 0.941 | **32.72** | 18.00 | **2216**
| Decomp filtergroup v3 | x | x | x | x | x | 57.46 | 24.00 | **3560**
| Decomp filtergroup v3, student | x | x | x | x | x | 57.46 | 24.00 | **3560**
