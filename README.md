# DATA620004-FinalPJ-Task3
**Pengwei Song & Yifan Qi**

The pre-trained transformer based model can be downloaded from [Github](https://github.com/yitu-opensource/T2T-ViT/releases/download/main/81.5_T2T_ViT_14.pth.tar).

Use the T2T-VIT model:
```
CUDA_VISIBLE_DEVICES=1,2 python transfer_learning.py --lr 0.05 --b 32 —num-classes 100 --img-size 224 --dataset cifar100  --model t2t_vit_14 --transfer-learning True --transfer-model T2T_ViT_14.pth
```