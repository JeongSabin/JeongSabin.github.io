---
layout: post
title: Mini-batch, Feedforward Network, Sequence data, Recurrent Network
description: >
  2023.04.19 열세번째 게시글
tags: [hydejack]
---

# Mini-batch

### Mini-batch란 한번에 모델에 입력되는 일정 개수의 데이터 묶음을 의미한다.
### 이러한 묶음을 통해 모델이 데이터를 처리하고 학습하는데 있어서 효율성과 안정성을 높일 수 있다.
## Mini-batch size 는 일반적으로 32, 64, 128 등의 값으로 설정된다.


## Feedforward Network (FFNN)
### Feedforward 네트워크는 FFNN(FeedForward Neural Network) 이라고 불린다.
### 입력 데이터가 순서대로 처리되는 네트워크 구조를 의미한다.
### 즉, 입력 데이터가 한 방향으로만 흐르며,  출력 결과는 입력 데이터의 특성만으로 결정된다. 이러한 구조는 이미지 분류, 객체 검출 등에 활용된다.
_자세한 내용은 이후에 FFNN 에 대한 게시글로 다루겠다._

# Sequence data
### Sequence data 는 시계열 데이터와 같이 시간적인 변화가 중요한 데이터를 의미한다.


# Recurrent Network (RNN)
### Recurrent Network 는 입력 데이터가 순서대로 처리되는 feedforward 네트워크와는 달리, 이전에 처리된 입력 데이터와 현재 입력 데이터가 함께 고려되어 처리되는 네트워크 구조를 의미한다. 이러한 구조는 자연어 처리, 음성인식 등에서 활용된다.
