---
title: 온보드 Amazon Sales Channel
description: 사전 설정 작업, 온보딩 단계 및 Amazon이 Adobe Commerce 및 Magento Open Source에서 Amazon Sales Channel과 작동하는 방식에 대해 알아봅니다.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 온보드 Amazon Sales Channel

이 섹션에서는 사전 설정 작업, 온보딩을 위한 단계 및 Amazon이 Adobe Commerce 및 Magento Open Source에서 Amazon 판매 채널과 작동하는 방식에 대한 몇 가지 주요 개념에 대해 설명합니다.

다음 [!DNL Amazon Sales Channel] 확장은 여러 Amazon 스토어를 지원합니다. 단일 [!DNL Amazon Seller Central] Amazon 미국/캐나다/멕시코 지역에서 운영하는 계정은 3개의 Amazon 매장을 만듭니다(미국 판매, 멕시코 판매 및 캐나다 판매에 대해 각각 하나씩). 3개의 상점은 각각 시장 국가를 생성 중에 정의합니다. 두 개 이상 있으면 [!DNL Amazon Seller Central] 계정에서 각 스토어에 대해 최대 3개의 Amazon 스토어를 보유할 수 있습니다. [!DNL Amazon Seller Central] 계정. 영국에서도 판매한다면 네 번째 Amazon 매장이 생길 것이다.

>[!TIP]
>
>A [전문 판매자 계정](https://sell.amazon.com/){target="_blank"} on [!DNL Amazon Seller Central] in the North America or European (UK) region is required. Amazon charges a monthly subscription and fees for selling. See [Amazon: Choose your selling plan](https://sell.amazon.com/pricing.html){target="_blank"}.<br><br>
>온보딩은 간단합니다. 스토어를 만든 다음 [!DNL Amazon Seller Central] 계정입니다.
>스토어가 연결되면 Amazon 채널은 다음에 따라 Amazon 목록을 가져와서 카탈로그에 일치시키려고 합니다. [속성 매핑](./attributes-view.md).<br><br>
>Amazon 판매 채널 설정은 Amazon 목록에 영향을 줍니다. 초기 목록, 가격 및 제품 설정이 기본값으로 설정됩니다. 다음을 수정할 수 있습니다. [스토어 설정](./ob-store-review.md) (목록, 가격 책정, 주문 및 보고) 스토어가 [!DNL Amazon Seller Central] 계정입니다.

| 단계 | 수행 항목 |
|--- |--- |
| [사전 설정 작업](./amazon-pre-setup-tasks.md) | 온보딩하기 전에 활성 상태의 가 승인되었는지 확인해야 합니다 [!DNL Amazon Seller Central] 계정입니다. 또한 몇 가지 [!DNL Commerce] 온보딩 전에 완료해야 하는 요구 사항 및 권장 사항. |
| [Amazon API 키 확인](./amazon-verify-api-key.md) | Amazon 판매 채널에 액세스할 때 [!DNL Commerce] 스토어 구성에 추가한 Amazon API 키를 자동으로 확인하고 확인합니다. API 키가 추가되지 않았거나 유효하지 않은 경우 [Amazon API 키 추가 또는 업데이트](./amazon-verify-api-key.md). |
| [스토어 통합](./store-integration.md) | 이 단계에는 Amazon 판매 채널 스토어를 만든 다음 사이트에 연결하는 작업이 포함되어 있습니다. [!DNL Amazon Seller Central] 계정입니다. 에 대한 기본 로그인 자격 증명이 필요합니다. [!DNL Amazon Seller Central] 이 단계의 계정(판매자 계정을 만드는 데 사용되는 이메일 또는 전화)입니다. |
| [목록 규칙 만들기](./ob-create-listing-rule.md) | Amazon 판매 채널 스토어에 연결하면 목록 규칙을 만들라는 메시지가 표시됩니다. 이 단계는 권장되지만 건너뛰고 목록 가져오기 프로세스를 시작할 수도 있습니다. 에 액세스할 수도 있습니다. [저장 및 목록 설정](./ob-store-review.md) 스토어에서 [대시보드](./amazon-store-dashboard.md). |
