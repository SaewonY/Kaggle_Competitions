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
- pytorch template(https://github.com/victoresque/pytorch-template)

<br>

## Added datasets

- resnet50(https://www.kaggle.com/pytorch/resnet50)
- se-resnext(https://www.kaggle.com/seefun/se-resnext-pytorch-pretrained)

<br>

## Arguments

- model(default: resnet50): 아래의 모델의 종류 중에서 선택합니다.
    - resnet18
    - resnet34
    - resnet50
    - resnet101
    - resnet152
    - densenet121
    - densenet169
    - densenet201
    - densenet161
    - seresnext50
    - seresnext101


- train_augments(default: "random_crop, horizontal_flip): 아래에서 원하는 것을 넣거나 빼고 string으로 값을 줍니다.
- test_augments(default: "random_crop, horizontal_flip): 아래에서 원하는 것을 넣거나 빼고 string으로 값을 줍니다.
    - "random_crop, keep_aspect, horizontal_flip, vertical_flip, random_rotate, color_jitter"
    - ex: trainig 시 random crop과 horizontal flip만 원할 시 --train_augments "random_crop, horizontal_flip"
    - ex: test 시 random crop과 horizontal flip만 원할 시 --test_augments "random_crop, horizontal_flip"


- size(default: 288): 입력 영상의 크기를 설정합니다.
- augment_ratio(default: 0.5): augmentation이 적용되는 확률입니다.

- loss(default: "BCE"): loss를 선택합니다.
    - "BCE": binary cross entropy를 사용합니다.
    - "FOCAL": focal loss를 사용합니다.
    - "FBET": Fbet loss를 사용합니다.
    - "COMBINE": focal과 fbet을 함께 사용합니다.
    - ex: --loss COMBINE
 - label_smoothing : eps [0, 1]
    - 참고 논문 : Bag of Tricks for Image Classification with Convolutional Neural Networks
    - 설명 문단 : 5.2
    - https://arxiv.org/pdf/1812.01187.pdf
 - mixup data & mixup loss : [True, False] (alpha 0.4)
    - 참고 논문 : mixup: Beyond Empirical Risk Minimization
    - https://arxiv.org/abs/1710.09412
