---
layout: post
title: Video LDMs
description: Lorem ipsum dolor est
image: assets/images/study/pic2.png
nav-menu: false
show_tile: false
---

<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white">
<img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">

이미지 생성 분야는 유의미할 정도로 많은 연구가 진행되었고, 이를 기반으로 한 서비스와 모델 공유 생태계가 활성화될 만큼 안정적으로 자리잡았습니다. 하지만 **영상 생성**의 경우, 2023년 여름 당시에는 막 연구가 시작되었기 때문에 큰 진전을 보이고 있지 않았습니다. 이러한 맥락에서 2023 CVPR에서 발표된 NVIDIA사의 **VideoLDMs**는 적은 계산량으로도 비교적 길고 해상도가 높은 영상을 생성하는 획기적인 모델이었습니다.

하지만 **VideoLDMs** 학습 및 추론 코드가 공개되어 있지 않았기 때문에, NCSOFT의 Vision AI Generation 팀에서는 영상 생성 기반 기술을 내재화하기 위해 논문을 기반으로 해당 모델의 코드를 직접 구현하기로 하였습니다.

**Video LDMs**의 기본 구조는 기존에 학습되어 있던 Image LDMs T2I(Text-to-Image) 모델에 temporal layer를 추가하여 spatial consistency에 대한 학습 없이 temporal consistency에 대한 학습만 할 수 있도록 한 것입니다. **AnimateDiff**는 이와 유사한 원리를 가진 T2V 모델로, 추론 코드가 공개되어 있기에 해당 코드를 참고하여 Video LDMs의 학습 및 추론 코드를 구현하였습니다.

<img src="{{ "assets/images/study/2_1.gif" | absolute_url }}" alt="image1" class="post" />

총 3주 동안 관련 연구에 대해 조사하였고, 이를 바탕으로 나머지 3주 동안 VideoLDMs의 코드를 구현하였으며, 구현원리가 올바르게 작동하는지 확인하기 위해 1주동안 시험 학습을 진행하였습니다. 짧은 인턴십 기간으로 인해 아쉽게도 그 결과를 확인하지는 못했으나, 어느정도 유의미한 학습단계를 밝고 있음을 확인하였습니다.

학습과정에서 생성한 일부 샘플 영상들을 [여기][link]에서 확인할 수 있습니다.

[link]: https://github.com/Rayiz3/T2V-model-sample