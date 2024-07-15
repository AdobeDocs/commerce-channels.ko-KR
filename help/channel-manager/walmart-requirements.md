---
title: '[!DNL Walmart] 요구 사항'
description: 'Channel Manager와 통합하는 데 필요한 [!DNL Walmart Marketplace]정보 및 리소스가 있는지 확인하십시오.'
role: Leader, Admin, Developer
feature: Sales Channels, Install, User Account, Tools and External Services
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# [!DNL Walmart] 요구 사항

[!DNL Walmart Marketplace.]에 대해 [!DNL Commerce] 판매 채널을 구성하려면 [!DNL Channel Manager]에 다음 리소스와 정보가 필요합니다.

* [!DNL Walmart] 판매자 계정

* Adobe Commerce 또는 Magento Open Source을 [!DNL Walmart Marketplace]에 연결하기 위한 API 키

  [!DNL Walmart Marketplace] API 키를 사용하면 Adobe [!DNL Commerce] 또는 Magento Open Source의 [!DNL Channel Manager]과(와) Walmart Marketplace 간의 통합이 가능합니다. Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

## [!DNL Walmart Seller] 계정 설정

[!DNL Walmart Seller Center](으)로 이동하여 [Walmart 판매자 계정](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp)을 설정합니다.

## [!DNL Walmart Marketplace] 프로덕션 API 키 생성

1. [!DNL Walmart Marketplace](으)로 이동하여 Adobe에 대한 [솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey)를 생성합니다.

1. 키를 만들고 권한을 구성합니다.

   * Adobe 를 솔루션 공급자로 선택합니다.

   * 다음 표에 표시된 대로 권한을 설정합니다. 자세한 내용은 _Walmart Marketplace 판매자 도움말_&#x200B;에서 [API 자격 증명](https://sellerhelp.walmart.com/seller/s/guide?article=000006422)을 참조하십시오.

   Walmart에 대한 **Adobe API 키 구성**

   | **권한** | **설정** |
   |----------------|-------------|
   | 콘텐츠 | 전체 액세스 권한 |
   | 피드 가져오기 | 보기 전용 |
   | 인벤토리 | 전체 액세스 권한 |
   | 항목 | 전체 액세스 권한 |
   | 지연 시간 | 전체 액세스 권한 |
   | 주문 | 전체 액세스 권한 |
   | 가격 | 전체 액세스 권한 |
   | 보고서 | 보기 전용 |
   | 반환 | 전체 액세스 권한 |
   | 규칙 | 전체 액세스 권한 |
   | 배송 | 전체 액세스 권한 |

## [!DNL Walmart Marketplace] 저장소 상태

제품을 마켓플레이스에 연결할 때 사용 가능한 목록은 [!DNL Walmart Marketplace] 저장소의 상태에 따라 다릅니다.

* 라이브 스토어의 경우, 일치 작업이 완료되면 제품 오퍼가 나열되어 판매될 수 있습니다.

* 라이브가 아닌 스토어의 경우 제품 오퍼가 스테이징되어 고객에게 표시되지 않습니다. [!DNL Walmart Marketplace] 스토어가 라이브로 전환되면 준비된 목록이 자동으로 라이브 스토어로 푸시됩니다.

스테이징된 제품 ![[!DNL Walmart Seller Central]개](assets/walmart-seller-central-staged.png){width="600" zoomable="yes"}

>[!IMPORTANT]
>
>[!DNL Channel Manager]을(를) 설치하고 구성한 후에는 모든 재고, 가격 및 주문 업데이트가 자동으로 동기화됩니다. 제품 및 주문 데이터를 업데이트하는 다른 통합을 사용하지 않도록 설정할 때까지 [!DNL Channel Manager]을(를) 실시간 Walmart Marketplace 저장소에 연결하지 마십시오. 다른 통합을 구성한 경우 라이브 스토어에 연결하기 전에 [!DNL Commerce]의 항목 수량과 가격이 [!DNL Walmart Marketplace]의 수량과 일치하는지 확인하십시오.

