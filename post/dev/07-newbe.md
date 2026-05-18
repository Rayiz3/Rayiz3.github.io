---
layout: post
title: NewBe
description: Lorem ipsum dolor est
image: assets/images/dev/pic7.png
nav-menu: false
show_tile: false
---

<img src="https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
<img src="https://img.shields.io/badge/anthropic-191919?style=for-the-badge&logo=anthropic&logoColor=white">
<img src="https://img.shields.io/badge/langgraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white">
<img src="https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
<img src="https://img.shields.io/badge/expo-1C2024?style=for-the-badge&logo=expo&logoColor=white">
<img src="https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white">
<img src="https://img.shields.io/badge/postgresql-4169E1?style=for-the-badge&logo=postgresql&logoColor=white">
<img src="https://img.shields.io/badge/supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white">
<img src="https://img.shields.io/badge/fly.io-24175B?style=for-the-badge&logo=flydotio&logoColor=white">

<a class="button icon" href="https://drive.google.com/file/d/1G38iVP6fd30op1WCzdMyeuBA21iQX8mx/view?usp=sharing">
  <img src="{{ 'assets/images/dev/7_ico.png' | absolute_url }}" alt="icon" class="btn-icon">
  뉴비(NewBe) v1.0.1 다운로드
</a>

**NewBe**는 매일 마다 새로운 **뉴스 정보를 다양한 캐릭터가 요약**해주는 모바일 뉴스 요약 앱입니다. 매일 수집된 뉴스를 단순히 나열하는 대신, 요약된 이야기를 통해 핵심을 빠르게 이해할 수 있습니다.

<img src="{{ 'assets/images/dev/7_1.png' | absolute_url }}" alt="image6" class="post" />

**NewBe**에는 각 분야별로 여러분께 뉴스 소식을 알려줄 **'뉴비(New-Be)'**가 있습니다. 뉴비는 주제별 분류와 핵심 요약을 수행하는 LLM 기반 워크플로우로 구성된 에이전트(agent)로, 서로 다른 말투와 관점으로 뉴스 기사에 대한 이야기를 전달합니다. 내용을 요약하는 것 뿐 아니라 **어려울 수도 있는 용어를 쉽게 풀어 설명**해주기도 하기 때문에, 복잡한 기사 원문을 읽지 않고도 다양한 분야의 주요 이슈를 직관적으로 파악할 수 있습니다.

<img src="{{ 'assets/images/dev/7_2.png' | absolute_url }}" alt="image6" class="post" />

**Google 계정과의 연동을 제공**합니다. 이를 통해 사용자는 자신이 원하는 분야의 뉴비를 원하는 순서대로 배치하여 개인의 관심사에 맞게 소식을 받아 볼 수 있습니다.

<img src="{{ 'assets/images/dev/7_3.png' | absolute_url }}" alt="image6" class="post" />

외부 api를 통해 뉴스를 수집하고 요약하는 일련의 과정은 **LangGraph**를 사용하여 구현하였습니다. 현재는 간단한 선형 워크플로우를 가지고 있으나, 추후 시스템을 고도화하면서 동시 실행이나 피드백 등 복잡한 분기 제어를 수월하게 하기 위함입니다.

**NewBe**는 지속적으로 개발 중에 있습니다. 위 사진을 보다시피, 아직 모든 뉴비들에 대한 이미지 에셋이 완성되지 않았기 때문입니다. 따라서 현재는 플레이 스토어에 배포되어 있지않고, 데모 파일만 받아볼 수 있습니다. 코드 전문은 [여기][github] github 저장소를 살펴봐주세요!

### - 2026.05.16. -

**경제, IT, 연예, 스포츠, 국제** 분야에 대한 뉴비들의 이미지 에셋이 추가되었습니다!

<img src="{{ 'assets/images/dev/7_4.png' | absolute_url }}" alt="image6" class="post" />


[github]: https://github.com/Rayiz3/NewBe