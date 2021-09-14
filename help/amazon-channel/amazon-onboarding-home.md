---
title: 온보드 Amazon Sales Channel
description: Adobe 상거래 및 Magento Open Source에서 사전 설정 작업, 온보딩 단계 및 Amazon이 Amazon Sales Channel과 작동하는 방식에 대해 알아봅니다.
redirect_from: /sales-channels/amazon/amazon-onboarding-home.html
exl-id: 99b64083-36e6-442e-9d20-4676e78ec3ae
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 온보드 Amazon 영업 채널

이 섹션에서는 사전 설정 작업, 온보딩 단계 및 Adobe Commerce 및 Magento Open Source에서 Amazon이 Amazon 판매 채널과 작동하는 방식에 대한 일부 주요 개념을 설명합니다.

[!DNL Amazon Sales Channel] 확장은 여러 Amazon 스토어를 지원합니다. Amazon 미국/캐나다/멕시코 지역에서 작동하는 단일 [!DNL Amazon Seller Central] 계정에 대해 세 개의 Amazon 스토어를 만듭니다(미국 판매, 멕시코 판매 및 캐나다 판매에 각각 하나씩). 3개의 상점마다 시장국가를 설립한다. 둘 이상의 [!DNL Amazon Seller Central] 계정이 있는 경우 각 [!DNL Amazon Seller Central] 계정에 대해 최대 3개의 Amazon 스토어를 보유할 수 있습니다. 영국에서 판매하시면 네 번째 Amazon이 있습니다

>[!TIP]
>
>북미 또는 유럽(UK) 지역의 [!DNL Amazon Seller Central]에 있는 [전문 판매자 계정](https://sell.amazon.com/){target=&quot;_blank&quot;}이 필요합니다. Amazon은 매월 구독료를 받고 판매료를 받습니다. [Amazon을 참조하십시오. 판매 계획 선택](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}.<br><br>
>온보딩은 간단합니다. 스토어를 만든 다음 [!DNL Amazon Seller Central] 계정에 연결합니다.
>스토어가 연결되면 Amazon 채널은 [특성 매핑](./attributes-view.md).<br><br>에 따라 Amazon 목록을 가져와서 카탈로그에 일치시키려고 합니다
>Amazon 판매 채널 설정은 Amazon 목록에 영향을 줍니다. 초기 목록, 가격 및 제품 설정이 기본적으로 사용됩니다. 저장소가 [!DNL Amazon Seller Central] 계정에 연결된 후 [스토어 설정](./ob-store-review.md)(목록, 가격, 주문 및 보고)을 수정할 수 있습니다.

| 단계 | 수행 |
|--- |--- |
| [사전 설정 작업](./amazon-pre-setup-tasks.md) | 온보딩하기 전에 활성 및 승인된 [!DNL Amazon Seller Central] 계정이 있는지 확인해야 합니다. 온보딩 전에 완료해야 하는 일부 [!DNL Commerce] 요구 사항과 권장 사항도 있습니다. |
| [Amazon API 키 확인](./amazon-verify-api-key.md) | Amazon 판매 채널에 액세스할 때 [!DNL Commerce]은(는) 저장소 구성에 추가한 Amazon API 키를 자동으로 확인하고 확인합니다. API 키가 추가되지 않았거나 잘못된 경우 [Amazon API 키](./amazon-verify-api-key.md)를 추가 또는 업데이트하라는 메시지가 표시됩니다. |
| [스토어 통합](./store-integration.md) | 이 단계에는 Amazon 판매 채널 저장소를 만든 다음 [!DNL Amazon Seller Central] 계정에 연결하는 작업이 포함됩니다. 이 단계를 위해 [!DNL Amazon Seller Central] 계정(판매자 계정을 만드는 데 사용되는 이메일 또는 전화)에 대한 기본 로그인 자격 증명이 필요합니다. |
| [목록 규칙 만들기](./ob-create-listing-rule.md) | Amazon 판매 채널 저장소를 접속하면 목록 규칙을 만들라는 메시지가 표시됩니다. 이 단계는 권장되지만 이 단계를 건너뛰고 가져오기 프로세스를 시작할 수도 있습니다. 또한 [스토어에 있는 [대시보드](./amazon-store-dashboard.md)설정을 저장하고 나열할 수도 있습니다.](./ob-store-review.md) |
