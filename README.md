# BoneRemoval
BoneRemoval Project for Siemens HC Medical Imaging Team, summer 2016.


## Model Leaderboard
Current models and performance.

| Model                  | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy  | Test Set Accuracy | CPU Time | GPU Time|
| -----------------------|:-------------:| -----------------:|:---------------:| --------------------:|:--------:|:--------:|:-------:|
| Mingqing Baseline      | 0.0901        |  0.9712           |  0.0864         |                0.9695| 0.972 |x|x
| Mingqing Baseline + BN | 0.055      |   0.9664| 0.0866 | 0.976|x|x|x
| Decomp Net             | 0.0901     |    0.9768 |0.0699|0.978|0.980|x|x
| Decomp Net+(ReLU->BN)  | 0.0635     |    0.9857 |0.0619|0.981|x|x|x
| Decomp Net+(BN->ReLU)  | 0.0612     |    0.9860 |0.05649|0.982|x|x|x
| Resnet_decomp       | 0.0928     |    0.9760 |0.07340|0.976|x|x|x
