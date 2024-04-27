# Vim-F: Visual State Space Model Benefiting from Learning in the Frequency Domain

## Introduction

This project is based on Vim ([paper](https://arxiv.org/abs/2401.09417), [code](https://github.com/hustvl/Vim)) and we appreciate this excellent work. You only need to replace the original `models_mamba.py` with ours to reimplement our work.


## ImageNet classification

| Model       | Dataset   | Resolution | Top1 | Ckpt/Logs                                                    |
| ----------- | --------- | ---------- | ---- | ------------------------------------------------------------ |
| Vim-Ti-F(H) | ImgNet 1K | 224×224    | 75.2 | [ckpt](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.0/best_checkpoint.pth)/[log](https://github.com/yws-wxs/Vim-F/releases/download/v1.0.0.0/log.txt) |
| Vim-S-F(H)  | ImgNet 1K | 224×224    | 81.0 | retraining                                                   |

