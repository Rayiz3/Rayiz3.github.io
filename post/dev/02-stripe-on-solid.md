---
layout: post
title: Stripe on Solid
description: Lorem ipsum dolor est
image: assets/images/dev/pic2.png
nav-menu: false
show_tile: false
---

<img src="https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/solid-2C4F7C?style=for-the-badge&logo=solid&logoColor=white">
<img src="https://img.shields.io/badge/stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white">
<img src="https://img.shields.io/badge/flask-3BABC3?style=for-the-badge&logo=flask&logoColor=white">

**VoxFactory**는 주식회사 Audai의 주요 웹 서비스로, 생성형 AI를 통해 사용자가 원하는 발성 형태, 멜로디, 가사 등에 맞춰 노래를 부를 수 있는 가상 보컬들을 제공합니다. 당시 VoxFactory는 유료 상품이나 결제 행동과 관련된 부분이 아직 적용되지 않았는데, 2024년 여름 인턴십을 통해 **결제 페이지 개발을 위한 결제 모듈 구현**에 관련된 업무를 수행하게 되었습니다.

<img src="{{ "assets/images/dev/2_1.png" | absolute_url }}" alt="image1" class="post" />

결제 모듈 개발은 **Stripe** 사의 API를 사용하였습니다. Stripe는 전자 상거래 웹사이트를 위한 결제 처리 소프트웨어를 지원하는 다국적 금융 서비스 기업입니다. 큰 수고를 들이지 않고 빠르게 결제 페이지를 만들 수 있고, 실제로도 openAI나 Suno를 비롯한 많은 기업들이 사용하는 대표적인 API입니다. 그러나 문제가 있었는데, Stripe는 **VoxFactory의 프론트엔드 프레임워크인 SolidJS를 지원하지 않았다는 것**입니다. 이 때문에 먼저 SolidJS 기반에서 Stripe API가 작동할 수 있도록 손보는 작업을 수행해야 했습니다. 

<img src="{{ "assets/images/dev/2_3.png" | absolute_url }}" alt="image3" class="post" />

Stripe에서 제공하는 세 가지의 구현 방식(custom flow, checkout, link)을 조사한 뒤, 세 버전에 대한 demo 페이지를 모두 구현하여 어떤 방식이 VoxFactory의 사용자 경험과 제일 잘 맞을 것인지 비교해 보았습니다.
