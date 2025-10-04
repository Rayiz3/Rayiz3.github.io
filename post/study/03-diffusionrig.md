---
layout: post
title: DiffusionRig
description: Lorem ipsum dolor est
image: assets/images/study/pic3.png
nav-menu: false
show_tile: false
---

본 연구는 **Facial expression & manipulation**이라는 키워드로 최근 연구를 조사하고, 그 중 하나를 선택해 학습 동작을 직접 확인해 보았습니다. 최종적으로 Diffusion model 기반의 학습모델인 **DiffusionRig**를 선택하게 되었고, 논문에서 소개한 모델의 방법론을 파악한뒤 제공되는 코드를 이용해 실제 학습 및 추론을 진행했습니다.

기존의 방법은 대부분 zero-shot learning을 사용합니다. 큰 데이터셋으로 학습한 후 **데이터셋에 없는 완전히 새로운 대상을 이용해 모델을 시험**하는 방식을 사용하는데, 이 방식은 시험 대상의 **정밀한 요소들(high frequency)**를 잘 반영하지 못한다는 문제점이 있었습니다. 이를 해결하기 위해 **DiffusionRig**는 두 단계로 이루어진 새로운 학습 pipline을 제시합니다. 1단계에서는 큰 데이터셋으로부터 **일반적인 얼굴의 특징을(generic facial prior)**를 학습하고, 2단계에서는 20장 내외의 작은 데이터셋으로부터 **개인화된 특징(personalized prior)**를 학습합니다.

<img src="{{ "assets/images/study/3_1.png" | absolute_url }}" alt="image1" class="post" />

<img src="{{ "assets/images/study/3_2.png" | absolute_url }}" alt="image2" class="post" />

본 연구는 Physical buffer 수정을 통한 DiffusionRig의 facial manipulation의 성능을 확인하고자 하였습니다. 우선 DiffusionRig 연구에서 제공하는 personalized dataset중 **Biden dataset**을 사용해 학습을 진행하였고, 그 다음 **즉석으로 촬영하여 생성한 dataset**에 대해 어느정도 학습하는지 확인해보았습니다.

자세한 연구 내용은 [여기][link] 보고서에서 확인할 수 있습니다.

[link]:  https://drive.google.com/file/d/1QuHPx0cbuk35KoIYv6s4j0EnuLhQkk3e/view?usp=sharing