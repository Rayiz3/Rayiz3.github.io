---
layout: post
title: Rosetta Stone
description: Lorem ipsum dolor est
image: assets/images/study/pic1.png
nav-menu: true
show_tile: false
---

<img src="https://img.shields.io/badge/c++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white">
<img src="https://img.shields.io/badge/c++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white">

**RosettaStone**은 C++기반의 하스스톤 강화학습 시뮬레이터와 그것을 개발하는 오픈소스 프로젝트입니다. **하스스톤**은 블리자드 엔터테인먼트가 개발한 온라인 수집용 전략형 카드 게임으로, 턴을 번갈아가며 여러가지 카드의 효과를 사용해 상대의 체력을 모두 소진시키면 승리하게 됩니다. **RosettaStone**은 이 게임의 규칙을 학습하여 일반 사용자를 상대로 능숙할 플레이를 할 수 있는 강화학습 모델을 만드는 것이 목표입니다.

하지만 문제가 하나 있었습니다. 스타크래프트와 같이 강화학습을 사용해 인공지능을 만든 게임들의 경우 해당 게임사에서 게임 개발에 사용한 소스코드나 API를 제공해 준 경우였습니다. 그러나 하스스톤의 경우 계속해서 업데이트를 하며 서비스하고 있기 때문에, **별도의 API를 제공해 주지 않는다는 것**이었습니다. 때문에 강화학습 모델을 설계하는 한 편 게임의 규칙, 즉 카드의 효과들을 전부 손수 구현해야 했습니다. 여기서 제가 맡게 된 역할 또한 **특정 확장팩에 해당하는 카드들의 효과를 구현**하는 것이었습니다.

<img src="{{ "assets/images/study/1_1.png" | absolute_url }}" alt="image1" class="post" />

저는 하스스톤의 확장팩중 '울둠의 구원자'에 속한 카드군을 구현하였고, 이 과정에서 기존에 적절하지 않게 구현되었던 공통 효과들도 수정하였습니다.

**RossettaStone**에 대한 자세한 정보는 [여기][link] github 저장소에서 확인할 수 있습니다.

[link]: https://github.com/utilForever/RosettaStone