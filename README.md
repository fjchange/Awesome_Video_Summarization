# Awesome Video Summarization

## 1. Task Definition

Video summarization aims to generate a short synopsis that summarize the video content by selecting its most informative and important parts.

According different definition of "part", e.g., frame or segment, video summarization have two types of sub-tasks.

- Video storyboard.
- Video skim.

<img src="https://i.loli.net/2021/07/06/wBPu4S9VObDY2oi.png" alt="image-20210706111113950" style="zoom:67%;" />

### Three setting

In Video Summarization with Long Short-term Memory (ECCV 2016), it proposed three types of setting for video summarization.

> - **Canonical**  This is the standard supervised learning setting where the <u>training, validation, and testing sets are from the same dataset, though they are disjoint</u>
> - **Augmented** In this setting, for a given dataset, we randomly leave 20% of it for testing, and <u>augment the remaining 80% with the other three datasets to form an augmented training and validation dataset</u>. Our hypothesis is that, despite being heterogeneous in styles and contents, the augmented dataset can be beneficial in improving the performance of our models because of the increased amount of annotations.
> - **Transfer** In this setting, for a given dataset, we <u>use the other three datasets for training and validation and test the learned models on the dataset</u>. We are interested in investigating if existing datasets can effectively transfer summarization models to new unannotated datasets. If the transfer can be successful, <u>then it would be possible to summarize a large number of videos in the wild where there is virtually no closely corresponding annotation.</u>

## 2. Datasets

Usually，video summary adopt four datasets below, but usually test on the former two datasets. While some works also conduct on VTW directly.

- SumMe
- TVSum
- YouTube
- OVP

#### Detailed comparisions

![image-20210705164729185](https://i.loli.net/2021/07/05/AZkY2SMVBefcKwD.png)

Recently, ICCV 2019 CoView proposed another dataset with near 20 annotators.  **It consists of about _1500_ videos and the distribution among training and testing is _1200_ and _300_ of the total videos, **respectively. 

## 3. Survey

1. Video Summarization Using Deep Neural Networks: A Survey. [paper]()

## 4. Supervised Papers

#### 2021

- DSNet: A Flexible Detect-to-Summarize Network for Video Summarization, TIP 2021 [paper](), [Code]()

- Reconstructive Sequence-Graph Network for Video Summarization, TPAMI 2021.
- 

#### 2019 

- Stacked Memory Network for Video Summarization, ACM MM 2019
- Rethinking the evaluation of video summaries, CVPR 2019 [codes](https://github.com/mayu-ot/rethinking-evs)

#### 2018

-  Deep Reinforcement Learning for Unsupervised Video Summarization with Diversity-Representativeness Reward, AAAI 2018 [paper](https://arxiv.org/abs/1801.00054)

- Query-Conditioned Three-Player Adversarial Network for Video Summarization, BMVC 2018

- Video Summarization using fully convolutional sequence networks, ECCV 2018，[unofficial codes](https://github.com/weirme/Video_Summary_using_FCSN) 
- HSA-RNN: Hierarchical Structure-Adaptive RNN for Video Summarization, CVPR 2018. [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Zhao_HSA-RNN_Hierarchical_Structure-Adaptive_CVPR_2018_paper.pdf)
- Retrospective Encoders for Video Summarization, ECCV 2018
- Video Summarization with Attention, [ACCV 2018](http://accv2018.net/program/) [AIU2018 workshop](http://www.sys.info.hiroshima-cu.ac.jp/aiu2018/).
- Video Summarization via Semantic Attended Networks, AAAI 2018

#### 2016

- Video Summarization with Long Short-term Memory, ECCV 2016 [codes](https://github.com/kezhang-cs/Video-Summarization-with-LSTM)
- Title Generation for User Generated Videos， ECCV 2016

#### 2015

- Video Co-summarization: Video Summarization by Visual Co-occurrence, CVPR 2015
- TVSum: Summarizing Web Videos Using Titles, CVPR 2015

#### 2014

- Category-specific video summarization, ECCV 2014.



## 5. Unsupervised Papers

#### 2020 

- Global-and-Local Relative Position Embedding for Unsupervised Video Summarization, ECCV 2020 [paper]()

#### 2019

- Discriminative feature learning for unsupervised video summarization, AAAI 2019.
- Video Summarization by Learning from Unpaired Data, CVPR 2019

#### 2017

- Unsupervised Video Summarization with Adversarial LSTM Networks， CVPR 2017, [codes](https://github.com/j-min/Adversarial_Video_Summary)
- 







## 6. Weakly Supervised Papers



## 7. Multimodal Approaches



## 8. Performance


|              |           | SumMe |      |      | TVSum |      |      |
| ------------ | --------- | ----- | ---- | ---- | ----- | ---- | ---- |
| Method       | Pub-Year  | C     | A    | T    | C     | A    | T    |
| Gygli et al. | ECCV 2014 | 39.7  |      |      |       |      |      |
| dppLSTM      | ECCV 2016 | 38.6  |      |      | 54.7  |      |      |
| SASUM        | AAAI 2018 | 45.3  |      |      | 58.2  |      |      |
| FCSN         | ECCV 2018 | 47.5  | 51.1 | 44.1 | 56.8  | 59.2 | 58.2 |
|              |           |       |      |      |       |      |      |
| DSNet        | TIP 2021  | 50.2  | 50.7 | 46.5 | 62.1  | 63.9 | 59.4 |
| RSGN         | PAMI 2021 | 45.0  | 45.7 | 44.0 | 60.1  | 61.1 | 60.0 |





