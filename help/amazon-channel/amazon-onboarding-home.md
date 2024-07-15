---
title: "온보드 [!DNL Amazon Sales Channel]"
description: 사전 설정 작업, 온보딩 단계 및 Amazon이 Adobe Commerce 및 Magento Open Source에서 Amazon Sales Channel과 작동하는 방식에 대해 알아봅니다.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 6321f17c0e6f9e86bb3f5755dc7710fa68d68b0d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 온보드

이 섹션에서는 사전 설정 작업, 온보딩을 위한 단계 및 Amazon이 Adobe Commerce 및 Magento Open Source에서 Amazon 판매 채널과 작동하는 방식에 대한 몇 가지 주요 개념에 대해 설명합니다.

[!DNL Amazon Sales Channel] 확장은 여러 Amazon 스토어를 지원합니다. Amazon 미국/캐나다/멕시코 지역에서 운영하는 단일 [!DNL Amazon Seller Central] 계정의 경우 세 개의 Amazon 매장을 만듭니다(미국 판매, 멕시코 판매 및 캐나다 판매에 대해 각각 하나씩). 3개의 상점은 각각 시장 국가를 생성 중에 정의합니다. [!DNL Amazon Seller Central] 계정이 두 개 이상인 경우 각 [!DNL Amazon Seller Central] 계정에 대해 최대 세 개의 Amazon 스토어를 보유할 수 있습니다. 영국에서도 판매한다면 네 번째 Amazon 매장이 생길 것이다.

>[!TIP]
>
>북미 또는 유럽(영국) 지역의 [!DNL Amazon Seller Central]에 대한 [전문 판매자 계정](https://sell.amazon.com/){target="_blank"}이(가) 필요합니다. Amazon은 월 구독료와 판매 수수료를 부과합니다. [Amazon: 판매 계획 선택](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>을 참조하세요.
>온보딩은 간단합니다. 스토어를 만든 다음 [!DNL Amazon Seller Central] 계정에 연결하세요.
>스토어가 연결되면 Amazon 채널은 [특성 매핑](./attributes-view.md)을(를) 기반으로 Amazon 목록을 가져와서 카탈로그에 일치시키려고 합니다.<br><br>
>Amazon 판매 채널 설정은 Amazon 목록에 영향을 줍니다. 초기 목록, 가격 및 제품 설정이 기본값으로 설정됩니다. 스토어가 [!DNL Amazon Seller Central] 계정에 연결되면 [스토어 설정](./ob-store-review.md)(목록, 가격, 주문 및 보고)을 수정할 수 있습니다.

| 단계 | 수행 항목 |
|---------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [사전 설정 작업](./amazon-pre-setup-tasks.md) | 온보딩하기 전에 활성 상태의 승인된 [!DNL Amazon Seller Central] 계정이 있는지 확인해야 합니다. 또한 온보딩 전에 완료해야 하는 [!DNL Commerce] 요구 사항 및 권장 사항도 있습니다. |
| [Amazon API 키 확인](./amazon-verify-api-key.md) | Amazon 판매 채널에 액세스할 때 [!DNL Commerce]은(는) 스토어 구성에 추가한 Amazon API 키를 자동으로 확인하고 유효성을 검사합니다. API 키가 추가되지 않았거나 유효하지 않은 경우 [Amazon API 키를 추가 또는 업데이트](./amazon-verify-api-key.md)하라는 메시지가 표시됩니다. |
| [스토어 통합](./store-integration.md) | 이 단계에는 Amazon 판매 채널 스토어를 만든 다음 [!DNL Amazon Seller Central] 계정에 연결하는 작업이 포함됩니다. 이 단계를 수행하려면 [!DNL Amazon Seller Central] 계정(판매자 계정을 만드는 데 사용되는 전자 메일 또는 전화)에 대한 기본 로그인 자격 증명이 필요합니다. |
| [목록 규칙 만들기](./ob-create-listing-rule.md) | Amazon 판매 채널 스토어에 연결하면 목록 규칙을 만들라는 메시지가 표시됩니다. 이 단계는 권장되지만 건너뛰고 목록 가져오기 프로세스를 시작할 수도 있습니다. [대시보드](./amazon-store-dashboard.md) 스토어에서 [스토어 및 목록 설정](./ob-store-review.md)에 액세스할 수도 있습니다. |
