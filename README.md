# BoneRemoval
BoneRemoval Project for Siemens HC Medical Imaging Team, summer 2016.


## Model Leaderboard
Current models and performance.

| Model                  | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy  | Test Set Accuracy | CPU Time(s)| GPU Time(s) | Training Data
| ---|:---:|:---:|:---:| :---:|:---:|:---:|:---:|:---:|:---:|
| Mingqing Baseline      | 0.0901 | 0.9712 | 0.0864 | 0.9695 | 0.972 |96.057|**5.33**|No Padding Set
| Mingqing Baseline + BN | 0.0550 | 0.9664 | 0.0866 | 0.9760 | 0.976 | x | x |No Padding Set
| Decomp Net             | 0.0901 | 0.9768 | 0.0699 | 0.9780 | 0.980 | **34.74** | 9.297 |No Padding Set
| Decomp Net+(ReLU->BN)  | 0.0635 | 0.9857 | 0.0619 | 0.9812 | x | x | x |No Padding Set
| Decomp Net+(BN->ReLU)  | 0.0612 | 0.9860 | 0.0565 |**0.982**|**0.986**| x | x |No Padding Set
| Resnet_decomp          | 0.0928 | 0.9760 | 0.0734| 0.976 | x | 78.73 | 60.90 (?) |No Padding Set
