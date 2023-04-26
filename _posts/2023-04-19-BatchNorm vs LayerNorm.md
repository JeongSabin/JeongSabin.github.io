---
layout: post
title: BatchNorm vs LayerNorm
description: >
  2023.04.19 열두번째 게시글
tags: [hydejack]
---

# BatchNorm vs LayerNorm

### Batch Normaliztion 과 Layer Normalization 은 모두 Deep Learning 모델에서 사용되는 normalization 기법 중에 두 가지이다.

### Batch Normalization 은 각 layer 의 입력값을 평균과 분산으로 normalize 하여 학습을 안정화 하는 기법이다. Batch Normalization 은 Mini-batch 를 이용하여 평균과 분산은 계산하므로, mini-batch size 가 작아질수록 normalization 의 효과가 떨어지며, 배치 사이즈가 크면 학습 시간이 늘어날 수 있다.

### 반면, Layer Normalization 은 큰 Batch Normalization 과 달라 mini-batch 의 특성에 영향을 받지 않는다. 대신, 각 샘플(데이터포인트) 의 feature 들에 대한 normalization 을 수행한다.
### 따라서, mini-batch size 가 작아져도 normalization 효과가 유지되며, RNN 과 같은 sequence 모델에 적용하기 용이하다.

### 따라서, Batch Normalization 은 큰 mini-batch size 에 적합하며, Layer Normalization 은 작은 mini-batch size 에 적합하다.
### 또한, Batch Normalization 은 각 층에서의 출력값들이 다른 층에서의 입력값으로 사용되는 feedforward 네트워크에 적합하며, Layer Normalization 은 sequence data 와 같은 RNN 모델에 적합하다.

_mini-batch, feedforward, sequence data, RNN 에 대해서는 다음에 설명하겠다._
