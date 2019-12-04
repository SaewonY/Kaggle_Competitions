# iMet Collection 2019 - FGVC6

![image](https://user-images.githubusercontent.com/40786348/64306284-3a9b1c80-cfcd-11e9-9180-a5228370262d.png)

<br>

**Bronze medal (67th place, private lb 0.624)**

<br>

## Competition Solution

- Ensembled Total 10 models (5fold, tta 2)
  - resnet50 - Image size 296
  - se_resnext101_32x4d - Image size 380
- Stratified 5 KFold
- BCE Loss + Focal Loss 
- Earlystopping based on F2 score 
- Augmentations: horizontal_flip, random_rotate, random_crop, color_jitter

- Various Techniques Implemented
  - label_smoothing: eps [0, 1] - [link](https://arxiv.org/pdf/1812.01187.pdf)
  - mixup data & mixup loss : [True, False] (alpha 0.4) - [link](https://arxiv.org/abs/1710.09412)
  - Fbeta Loss etc...

<br>
<br>

## Usage

* Encode and Decode to upload on kaggle script
* argument example is on **script_template.py**
```
1. python build.py => build/script.py produced
2. copy and paste on kaggle script kernel and commit
3. Run example: --train_augments "random_crop, horizontal_flip, random_rotate", --test_augments "random_crop"
```

<br>
<br>

## Pretrained Weights

- resnet50 - [link](https://www.kaggle.com/pytorch/resnet50)
- se_resnext101_32x4d - [link](https://www.kaggle.com/seefun/se-resnext-pytorch-pretrained)

<br>
<br>

## Competition Top Place Solutions 
* 1st place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/94687#latest-570986) 
* 4th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/94817#latest-550074)
* 6th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/95282#latest-550969) with code [here](https://github.com/YU1ut/imet-6th-soltuion)
* 10th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/95311#latest-568748)