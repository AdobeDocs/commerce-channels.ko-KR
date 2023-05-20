---
title: '''[!DNL Walmart] 요구 사항'
description: '필요한 항목이 있는지 확인합니다. [!DNL Walmart Marketplace]Channel Manager와 통합할 정보 및 리소스'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# [!DNL Walmart] 요구 사항

[!DNL Channel Manager] 를 구성하려면 다음 리소스 및 정보가 필요합니다. [!DNL Commerce] 에 대한 판매 채널 [!DNL Walmart Marketplace.]

* A [!DNL Walmart] 판매자 계정

* Adobe Commerce 또는 Magento Open Source을 연결할 API 키 [!DNL Walmart Marketplace]

   다음 [!DNL Walmart Marketplace] API 키를 통해 [!DNL Channel Manager] Adobe [!DNL Commerce] 아니면 Magento Open Source과 월마트 마켓을 Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

## 설정 [!DNL Walmart Seller] account

로 이동 [!DNL Walmart Seller Center] 을(를) 설정하려면 [Walmart Seller 계정](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## 생성 [!DNL Walmart Marketplace] 프로덕션 API 키

1. 다음으로 이동 [!DNL Walmart Marketplace] 생성 방법 [Adobe을 위한 솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. 키를 만들고 권한을 구성합니다.

   * Adobe 를 솔루션 공급자로 선택합니다.

   * 다음 표에 표시된 대로 권한을 설정합니다. 자세한 내용은 [API 자격 증명](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 다음에서 _Walmart Marketplace 판매자 도움말_.

   **Walmart에 대한 Adobe API 키 구성**

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

제품을 마켓플레이스에 연결할 때 목록 가용성은 의 상태에 따라 다릅니다. [!DNL Walmart Marketplace] 스토어:

* 라이브 스토어의 경우, 일치 작업이 완료되면 제품 오퍼가 나열되어 판매될 수 있습니다.

* 라이브가 아닌 스토어의 경우 제품 오퍼가 스테이징되어 고객에게 표시되지 않습니다. 다음의 경우 [!DNL Walmart Marketplace] 스토어가 라이브로 전환되면 스테이징된 목록이 자동으로 라이브 스토어에 푸시됩니다.

![[!DNL Walmart Seller Central] 스테이징된 제품](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>다음 이후 [!DNL Channel Manager] 가 설치되고 구성되면 모든 재고, 가격 및 주문 업데이트가 자동으로 동기화됩니다. 연결 안 함 [!DNL Channel Manager] 제품 및 주문 데이터를 업데이트하는 다른 통합을 비활성화하기 전까지 라이브 Walmart Marketplace 스토어에 액세스할 수 있습니다. 다른 통합이 구성된 경우 품목 수량 및 가격이 [!DNL Commerce] 수량 일치 [!DNL Walmart Marketplace] 라이브 스토어에 연결하기 전에.

