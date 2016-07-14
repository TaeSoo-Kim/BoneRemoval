# BoneRemoval
BoneRemoval Project for Siemens HC Medical Imaging Team, summer 2016.


## Model Leaderboard
###Current models and performance on training set *without* padding data.

| Model | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy  | Test Set Accuracy | CPU Time(s)| GPU Time(s) |#Params
| ---|:---:|:---:|:---:| :---:|:---:|:---:|:---:|:---:|:---:|
|  Baseline              | 0.0901 | 0.9712 | 0.0864 | 0.9695 | 0.972 |96.057|**5.33**| 68920  
|  Baseline + BN         | 0.0550 | 0.9664 | 0.0866 | 0.9760 | 0.976 | x | x | 68920
| Decomp Net             | 0.0901 | 0.9768 | 0.0699 | 0.9780 | 0.980 | **34.74** | 9.297 | 7416
| Decomp Net+(ReLU->BN)  | 0.0635 | 0.9857 | 0.0619 | 0.9812 | x | x | x | 7416
| Decomp Net+(BN->ReLU)  | 0.0612 | 0.9860 | 0.0565 |**0.982**|**0.986**| x | x | 7416
| Resnet_decomp          | 0.0928 | 0.9760 | 0.0734| 0.976 | x | 78.73 | 60.90 (?) | 6248


###Current models and performance on training set *with* padding data.

| Model | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy  | Test Set Accuracy | CPU Time(s)| GPU Time(s) |#Params
| ---|:---:|:---:|:---:| :---:|:---:|:---:|:---:|:---:|:---:|
|  Baseline              | x | x | x | x | x | 109.5 | **5.33** | 68920|
|  Baseline+(BN->ReLU)   | x | x | x | x | x | x | x | 68920|
| Decomp Net             | 0.1045 | 0.9727 | 0.0797 | 0.9730 | x | **34.74** | 9.297 | 7416 
| Decomp Net+(BN->ReLU)  | 0.0822 | 0.9794 | 0.0689 |**0.980**| x | x | x | 7416
| Resnet_decomp          | x | x | x |x | x | x | x | 6248
| Baseline filtergroup v1| 0.0789 | 0.9727 | 0.0841 | 0.9730 | x | 76 | x | 46968
| Baseline filtergroup v2| 0.1053 | 0.9657 | 0.1072 | 0.9653 | x | 36.5 | x | 21992
| Decomp filtergroup v1  | 0.0924 | 0.9738 | 0.0792 | 0.9726 | x | 26.5 | x | 4696
| Decomp filtergroup v2  | x | x | x | x | x | **15.5** | x | **2216**
