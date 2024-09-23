# Vim-F: Visual State Space Model Benefiting from Learning in the Frequency Domain

## Introduction

This project is based on  Vim ([paper](https://arxiv.org/abs/2401.09417), [code](https://github.com/hustvl/Vim)) and we appreciate this excellent work. You can simply replace main.py and models_mamba.py with our versions to reimplement our work. Among them, main.py has no substantial modifications, and only the code related to position embedding in the original file has been removed to fit our work.


## ImageNet classification
### Pre-training
#### V1
| Model       | Dataset   | Resolution | Top1 | Ckpt/Logs                                                    |
| :-----------: | :---------: | :----------: | :----: | :------------------------------------------------------------: |
| Vim-Ti-F(H) | ImgNet 1K | 224×224    | 76.0 | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.2/Ti_pre_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.2/Ti_pre_log.txt) |                
| Vim-S-F(H)  | ImgNet 1K | 224×224    | 80.5 | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.2/S_pre_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.2/S_pre_log.txt) |
#### V2
| Model       | Dataset   | Resolution | Top1 | Ckpt/Logs                                                    |
| :-----------: | :---------: | :----------: | :----: | :------------------------------------------------------------: |
| Vim-Ti-F| ImgNet 1K | 224×224    | 76.7      | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.3/v2-ti-f-ckp.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.3/v2-ti-f-log.txt) |
| Vim-S-F  | ImgNet 1K | 224×224    | 80.9| retraining                                             |

