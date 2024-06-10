# Vim-F: Visual State Space Model Benefiting from Learning in the Frequency Domain

## Introduction

This project is based on  Vim ([paper](https://arxiv.org/abs/2401.09417), [code](https://github.com/hustvl/Vim)) and we appreciate this excellent work. You can simply replace main.py and models_mamba.py with our versions to reimplement our work. Among them, main.py has no substantial modifications, and only the code related to position embedding in the original file has been removed to fit our work.


## ImageNet classification
### Pre-training
| Model       | Dataset   | Resolution | Top1 | Ckpt/Logs                                                    |
| :-----------: | :---------: | :----------: | :----: | :------------------------------------------------------------: |
| Vim-Ti-F(H) | ImgNet 1K | 224×224    | 76.0 | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/Ti_pre_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/Ti_pre_log.txt) |                                                      |
| Vim-S-F(H)  | ImgNet 1K | 224×224    | 80.7 | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/S_pre_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/S_pre_log.txt) |


### Long sequence fine-tuning
| Model       | Dataset   | Resolution | Top1 | Ckpt/Logs                                                    |
| :-----------: | :---------: | :----------: | :----: | :------------------------------------------------------------: |
| Vim-Ti-F(H) | ImgNet 1K | 224×224    | 78.3       | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/Ti_ft_best_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.1/Ti_ft_log.txt) |
| Vim-S-F(H)  | ImgNet 1K | 224×224    | retraining | retraining                                             |
>Unlike the pre-training stage, Vim's source code did not automatically use the linear scaling rule to adjust the learning rate during the fine-tuning stage. We did not manually adjust the learning rate, so the performance declined.

