---
layout: post
title: Pokémon Deck Builder
description: Lorem ipsum dolor est
image: assets/images/dev/pic3.png
nav-menu: true
show_tile: false
---

<img src="https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/solid-2C4F7C?style=for-the-badge&logo=solid&logoColor=white">
<img src="https://img.shields.io/badge/d3force-F9A03C?style=for-the-badge&logo=d3&logoColor=white">

[*[바로가기]*][link]

전 세계적으로 유명한 IP인 포켓몬, 세계 대회까지 있다는 사실을 알고 있나요? 게임을 좋아하는 사람들에게는 포켓몬 배틀도 굉장히 인기있는 요소입니다. 포켓몬들마다 서로 다른 전략, 포켓몬들 사이의 시너지, 턴제 게임 특유의 수 싸움까지 여러 가지 볼 만한 요소가 가득한 것이 포켓몬 배틀의 묘미입니다.

<img src="{{ "assets/images/dev/3_1.png" | absolute_url }}" alt="image1" class="post" />

**Pokémon Deck Builder**는 사용자가 포켓몬 엔트리를 구상할 수 있도록 도와주는 대시보드 사이트입니다. 물론 인터넷에는 이미 너무 좋은 디자인의 포켓몬 엔트리 구성 사이트들이 많이 만들어져 있습니다. 하지만 한 가지 사소하지만 불편한 점이 있었는데, 바로 **포켓몬에 대한 어떠한 조언도 주지 않는다는 것**이었습니다. 포켓몬 자체 뿐 아니라 포켓몬의 **기술, 특성, 도구, (9세대 한정으로는)테라스탈 타입**까지 고려해야 하는 선택지가 너무 많은데, 도움이 될 만한 힌트가 없는 것이었죠. 당연할 수 있습니다. 왜냐하면 사이트를 찾아가며 포켓몬 엔트리를 구성하고자 하는 사람들은 대부분 이미 포켓몬들과 배틀에 대한 배경 지식을 어느정도 갖추고 있을테니까요. 하지만 저와 같이 **실전 배틀에 익숙하지 않은 사람**이 엔트리를 만드려고 한다면, 역시 어떻게 시작해야 할 지 막막할 수 밖에 없습니다.

<img src="{{ "assets/images/dev/3_2.png" | absolute_url }}" alt="image2" class="post" />

그래서 저는 데이터의 힘을 빌리기로 하였습니다. 실력 좋은 플레이어가 어떤 팀을 짰는지 엔트리를 만들면서 볼 수 있다면, 한 층 더 수월해지지 않겠어요? 그 실력 좋은 플레이어가 대회 랭커라면 더할 나위 없이 좋겠죠! 그래서 **2024년 포켓몬 월드 챔피언쉽의 랭킹 데이터**를 수집하게 되었습니다. 데이터는 선수마다 어떤 팀을 사용했는지, 포켓몬마다 어떤 도구나 특성 등을 사용했는지까지 제공합니다.

<img src="{{ "assets/images/dev/3_3.png" | absolute_url }}" alt="image3" class="post" />

엔트리 데이터는 무게가 있는 그래프로 나타내어집니다. 하나의 **점이 하나의 포켓몬을**, 점사 점사이를 잇는 **선은 두 포켓몬이 함께 채용되었음**을 의미합니다. 점이 클수록 그 포켓몬의 채용률이 높은 것이고, 선이 굵을 수록 두 포켓몬이 함께 사용된 횟수가 많은 것이죠. 점을 클릭하면 어떤 포켓몬이 사용되었는지 그 정보와 함께 표시됩니다.

<img src="{{ "assets/images/dev/3_4.png" | absolute_url }}" alt="image4" class="post" />

그래프에서 포켓몬을 찾거나, 직접 검색해서 원하는 포켓몬을 골라 엔트리에 추가할 수 있습니다. 추가한 포켓몬은 특성과 도구, 테라스탈 타입, 그리고 기술을 설정할 수 있게 됩니다. 

<img src="{{ "assets/images/dev/3_5.png" | absolute_url }}" alt="image5" class="post" />

만약 포켓몬의 설정을 어떻게 해야 할 지 막막해진다면, 다시 한 번 데이터의 힘을 빌릴 수 있습니다. Recommand 기능을 사용하면, 랭커들의 데이터를 기반으로 현재 엔트리의 포켓몬 조합에 따라 가장 많이 사용된 설정을 추천해줍니다.

<img src="{{ "assets/images/dev/3_6.png" | absolute_url }}" alt="image6" class="post" />

2024년 월드 챔피언십은 초전설 포켓몬을 최대 한 마리까지 사용 가능한 **레귤레이션 G** 룰에 따라 진행되었습니다. 현재는 환상의 포켓몬과 초전설 포켓몬을 최대 두 마리 까지 사용할 수 있는 **레귤레이션 J** 룰이 적용되고 있는데, 이에 맞추어 배틀 전략 또한 많이 바뀌었으므로 데이터를 새롭게 업데이트할 필요가 있어 보입니다.

[link]: https://pokedeckbuild.netlify.app/