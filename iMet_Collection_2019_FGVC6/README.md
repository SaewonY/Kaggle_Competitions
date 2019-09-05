# iMet Collection 2019 - FGVC6

![image](https://user-images.githubusercontent.com/40786348/64306284-3a9b1c80-cfcd-11e9-9180-a5228370262d.png)

<br>

* first kaggle project done within Sillim Kaggle study
* won **bronze medal (67th place, private lb 0.624)**

<br>

## Competition solutions 
* 1st place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/94687#latest-570986) 
* 4th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/94817#latest-550074)
* 6th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/95282#latest-550969) with code [here](https://github.com/YU1ut/imet-6th-soltuion)
* 10th place solution [here](https://www.kaggle.com/c/imet-2019-fgvc6/discussion/95311#latest-568748)
  
<br>

## References

- build script(https://github.com/lopuhin/kaggle-script-template)

<br>

## Added datasets in kaggle (pretrained weights)

- resnet50(https://www.kaggle.com/pytorch/resnet50)
- se-resnext(https://www.kaggle.com/seefun/se-resnext-pytorch-pretrained)

<br>

## Usage

* Encode and Decode to upload on kaggle script
* argument example is on **script_template.py**
```
1. python build.py => build/script.py produced
2. copy and paste on kaggle script kernel and commit
```

- choose one of the loss functions as follows
  - "BCE": binary cross entropy
  - "FOCAL": focal loss
  - "FBET": Fbet loss
  - "COMBINE": focal combined with fbet
  - ex: --loss COMBINE 

- availabel augmentations
  - random_crop
  - keep_aspect
  - horizontal_flip
  - vertical_flip
  - random_rotate
  - color_jitter
  - ex: --train_augments "random_crop, horizontal_flip, random_rotate", --test_augments "random_crop"
  
- etc..
  - label_smoothing: eps [0, 1], reference: https://arxiv.org/pdf/1812.01187.pdf
  - mixup data & mixup loss : [True, False] (alpha 0.4), reference: https://arxiv.org/abs/1710.09412
