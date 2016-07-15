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
| Baseline filtergroup v1| x | x | x | x | 0.956 | 135.69 | 5.81 | 46968
| Baseline filtergroup v2| x | x | x | x | x | 66.80 | 6.32 | 21992
| Decomp filtergroup v1  | x | x | x | x | x | 37.80 | 13.83 | 4696
| Decomp filtergroup v2  | x | x | x | x | x | **32.72** | 18.00 | **2216**
| Resnet_decomp          | x | x | x | x | x | x | x | 6248
