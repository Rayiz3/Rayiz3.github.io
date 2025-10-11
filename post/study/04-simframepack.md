---
layout: post
title: SimFramepack
description: Lorem ipsum dolor est
image: assets/images/study/pic4.gif
nav-menu: false
show_tile: false
---

SimFrampack의 T2V 모델인 **Frampack을 기반으로 한 물리 시뮬레이션 모델**로, KCVL 연구실에서 연구중이었던 주제였습니다. 여름 개별연구 동안 연구활동을 보조하여 코드 구조를 학습하고, 하이퍼파라미터를 조절하며, 여러가지 입력값에 대한 모델의 정성적 성능을 분석해보았습니다.

<img src="{{ "assets/images/study/4_1.png" | absolute_url }}" alt="image1" class="post" />

현재는 충분히 다양한 종류의 T2V 기반 물리 시뮬레이션 모델이 개발되어왔습니다. 하지만 기존 모델(e.g. Go-with-the-Flow)의 경우 **물체가 가지고 있는 물성 외의 out-of-distribution 결과**를 잘 구현하지 못한다는 단점이 있었습니다. 이를 해결하기 위해 SimFramepack에서는 기존에 전달하던 입력값을 바꾸어 이미지가 프롬프트에서 지시한 동작과 물성을 구현할 수 있도록 하였습니다.

<img src="{{ "assets/images/study/4_2.png" | absolute_url }}" alt="image1" class="post" />

실험 결과 rescaling factor, shift, inversion step 등 하이퍼파라미터에 따라 결과값에 미치게 되는 영향에 대해 정리하였습니다. 또한 주어진 src video의 motion condition이 명시되어 text prompt를 따르는 극단적인 변화는 보이지 않음을 확인하였습니다.

연구활동에 대한 내용은 [여기][link] 슬라이드 링크에서 확인할 수 있습니다.

[link]: https://docs.google.com/presentation/d/1j4SWEPGlHlNGgFT3w0mpdSJFBbaw0EZcAk6s0j9aJDM/edit?usp=sharing