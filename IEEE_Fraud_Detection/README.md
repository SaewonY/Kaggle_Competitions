# IEEE-CIS Fraud Detection

![image](https://user-images.githubusercontent.com/40786348/66255296-f2823c00-e7bc-11e9-9170-ac782ccc8f5b.png)

<br>

시간이 없어서 제대로 참가 못해 아쉬움이 많이 남는 대회다. 뒤늦게나마 대회 전반적인 것들을 정리해보고자 한다. **upvote 수가 낮다고 해서 중요하지 않은 커널은 절대 아니다**. 최소한으로 봐야 하는 것들만 정리해봤다.

<br>

## Must Look Guideline
- **[400+ VOTES]** How all works together [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/107697)

<br>

## EDA Kernels
- **[700+ VOTES]** EDA and models [link](https://www.kaggle.com/artgor/eda-and-models)
- **[600+ VOTES]** Extensive EDA and Modeling XGB Hyperopt [link](https://www.kaggle.com/kabure/extensive-eda-and-modeling-xgb-hyperopt)
- **[300+ VOTES]** Tackling Class Imbalance [link](https://www.kaggle.com/shahules/tackling-class-imbalance) 
- **[200+ VOTES]** Fraud complete EDA [link](https://www.kaggle.com/jesucristo/fraud-complete-eda) 
- **[200+ VOTES]** IEEE Transaction columns Reference [link](https://www.kaggle.com/alijs1/ieee-transaction-columns-reference)
- **[40+ VOTES]** EDA for Columns V and ID [link](https://www.kaggle.com/cdeotte/eda-for-columns-v-and-id)

<br>

## Minifications (for faster data loading, less memory consume)
- **[100+ VOTES]** Reducing Memory size for IEEE [link](https://www.kaggle.com/mjbahmani/reducing-memory-size-for-ieee)
- **[50+ VOTES]** IEEE Data minification [link](https://www.kaggle.com/kyakovlev/ieee-data-minification)

<br>

## Data Cleansing
- **[60+ VOTES]** Cleaning P_emaildomain and R_emaildomain [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/100499#latest-616834)
- **[60+ VOTES]** All OS and Browser release date
 [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/106982)
- **[40+ VOTES]** Filling card NaNs [link](https://www.kaggle.com/grazder/filling-card-nans)

<br>

## Feature Engineering

- **[400+ VOTES]** Feature Engineering Techniques [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/108575#latest-642273)
- **[200+ VOTES]** IEEE - GB-2 (make Amount useful again) [link](https://www.kaggle.com/kyakovlev/ieee-gb-2-make-amount-useful-again)
- **[200+ VOTES]** IEEE - FE with some EDA [link](https://www.kaggle.com/kyakovlev/ieee-fe-with-some-eda)
- **[70+ VOTES]** IEEE - Basic FE - part 1 [link](https://www.kaggle.com/kyakovlev/ieee-basic-fe-part-1)

<br>

## Cross Validation 
- **[100+ VOTES]** IEEE - CV Options [link](https://www.kaggle.com/kyakovlev/ieee-cv-options)
- **[100+ VOTES]** Negative downsampling [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/108616#latest-634925)

<br>

## Must look kernels, discussions
- **[400+ VOTES]** Data Description (Details and Discussion) [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/101203)
- **[100+ VOTES]** Adversarial IEEE [link](https://www.kaggle.com/tunguz/adversarial-ieee)
- **[100+ VOTES]** Interesting finding about the V columns [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/105130#latest-631761)
- **[100+ VOTES]** Day and Time - powerful predictive feature? [link](https://www.kaggle.com/fchmiel/day-and-time-powerful-predictive-feature)
- **[100+ VOTES]** Find Unique clients [link](https://www.kaggle.com/alexanderzv/find-unique-clients)

- **[100+ VOTES]** Fraud Detection material/comps in Kaggle [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/99987)
- **[100+ VOTES]** Feature engineering: Time of day [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/100400)
- **[100+ VOTES]** Recursive feature elimination [link](https://www.kaggle.com/nroman/recursive-feature-elimination)
- **[100+ VOTES]** Public/Private LB test set split! [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/101040)
- **[90+ VOTES]** Extended TimeSeries Splitter [link](https://www.kaggle.com/mpearmain/extended-timeseriessplitter)
- **[80+ VOTES]** TransactionDT startdate [link](https://www.kaggle.com/kevinbonnes/transactiondt-starting-at-2017-12-01)
- **[80+ VOTES]** Reducing the gap between CV and LB [link](https://www.kaggle.com/c/elo-merchant-category-recommendation/discussion/77537)
- **[30+ VOTES]** Permutation importance function
 [link](https://www.kaggle.com/c/ieee-fraud-detection/discussion/107877#latest-635386) and explained [here](https://www.kaggle.com/dansbecker/permutation-importance)

<br>

## Winning Solutions
  
- 1st place solution short summary  [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111257#latest-641904) and part1 [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111284#latest-642018) part2 [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111308#latest-641998)

- 2nd place solution [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111321#latest-641942) and [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111554#latest-644838)

 - 5th place solution [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111735#latest-645520)

- 6th place solution [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111247#latest-644158)

- 11th place solution [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111235#latest-643771)

<br>

## some review about the competition 

- according to 1st place solution, the key to this competition is finding **Fraudulent Clients** (to predict unseen clients that are not in the train dataset) which means **time is not the most feature.**

- **steady EDA** and **finding some magic features** is most important in machine learning competition.

- how to find UIDs is explained [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111510), code provided [here](https://www.kaggle.com/kyakovlev/ieee-uid-detection-v6) and [here](https://www.kaggle.com/cdeotte/xgb-fraud-with-magic-0-9600)

- how the magic feature works is explained [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/111453)

- things you can learn from the IEEE competition [here](https://www.kaggle.com/c/ieee-fraud-detection/discussion/112047#latest-646439)
