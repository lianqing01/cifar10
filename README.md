# CIFAR-10 homework

### Usage 

simply run the cmd for the training:

```bash
## 1 GPU for base model 

CUDA_VISIBLE_DEVICES=0 python -u train.py --work-path ./experiments/cifar10/densenet120bc

## 1 GPU for base model with cutout

CUDA_VISIBLE_DEVICES=0 python -u train.py --work-path ./experiments/cutout/densenet120bc

## 1 GPU for base model with mixup
CUDA_VISIBLE_DEVICES=0 python -u train.py --work-path ./experiments/mixup/densenet120bc

## 1 GPU for base model with cutout+mixup
CUDA_VISIBLE_DEVICES=0 python -u train.py --work-path ./experiments/cutout+mixup+cos/densenet120bc

## 2 GPU for large model

CUDA_VISIBLE_DEVICES=0,1 python -u train.py --work-path ./experiments/cutout+mixup+cos/densenet150bc
```




## Acknowledgement
This is code is heavily borrowed from [CIFAR-ZOO](https://github.com/BIGBALLON/CIFAR-ZOO)


