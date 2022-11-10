---
title: '`[!DNL Walmart] 요구 사항'
description: '''필요한 항목이 있는지 확인합니다. [!DNL Walmart Marketplace]Channel Manager와 통합할 정보 및 리소스'
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: fd60c8917e4b4e155fb2897ade6e1d96aff2de9d
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# [!DNL Walmart] 요구 사항

[!DNL Channel Manager] 를 구성하려면 다음 리소스 및 정보가 필요합니다. [!DNL Commerce] 영업 채널 [!DNL Walmart Marketplace.]

* 판매 승인 [!DNL Walmart] 등록된 Marketplace 판매자 계정에 로그인할 자격 증명

* Adobe Commerce 또는 Magento Open Source을 연결할 API 키 [!DNL Walmart Marketplace]

   다음 [!DNL Walmart Marketplace] API 키를 사용하면 두 API 간에 통합할 수 있습니다 [!DNL Channel Manager] Adobe [!DNL Commerce] Magento Open Source과 월마트 마켓플레이스 중 어느 것을 선택하시겠습니까? Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

## 설정 [!DNL Walmart Seller] account

1. [Walmart Seller 응용 프로그램 제출](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
1. 승인을 받은 후 [!DNL Walmart], [Walmart Seller 계정 설정](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

## 생성 [!DNL Walmart Marketplace] 프로덕션 API 키

1. 이동 [!DNL Walmart Marketplace] 생성하다 [Adobe용 솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. 키 만들기 및 권한 구성:

   * 솔루션 공급자로 Adobe 를 선택합니다.

   * 다음 표에 표시된 대로 권한을 설정합니다. 자세한 내용은 [API 자격 증명](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 에서 _Walmart Marketplace 판매자 도움말_.

   **Walmart에 대한 Adobe API 키 구성**

   | **권한** | **설정** |
   |----------------|-------------|
   | 컨텐츠 | 전체 액세스 |
   | 피드 가져오기 | 보기 전용 |
   | 인벤토리 | 전체 액세스 |
   | 항목 | 전체 액세스 |
   | 지연 시간 | 전체 액세스 |
   | 주문 | 전체 액세스 |
   | 가격 | 전체 액세스 |
   | 보고서 | 보기 전용 |
   | 반환 | 전체 액세스 |
   | 규칙 | 전체 액세스 |
   | 배송 | 전체 액세스 |

## [!DNL Walmart Marketplace] 저장 상태

제품을 마켓플레이스에 연결할 때 사용 가능 여부는 사용자의 상태에 따라 다릅니다 [!DNL Walmart Marketplace] 저장소:

* 라이브 스토어의 경우, 제품 오퍼가 나열되며 일치 작업이 완료되면 판매 가능합니다.

* 라이브 상태가 아닌 저장소의 경우 제품 오퍼가 스테이징되어 고객에게 표시되지 않습니다. 이 [!DNL Walmart Marketplace] 스토어가 라이브로 전환되고 준비된 목록이 라이브 스토어에 자동으로 푸시됩니다.

![[!DNL Walmart Seller Central] 준비된 제품](assets/walmart-seller-central-staged.png)

>[!IMPORTANT]
>
>후 [!DNL Channel Manager] 설치 및 구성되면 모든 재고, 가격 및 주문 업데이트가 자동으로 동기화됩니다. 연결 안 함 [!DNL Channel Manager] 제품 및 주문 데이터를 업데이트하는 다른 통합을 비활성화해야 할 때까지 live Mart Marketplace에 연결할 수 있습니다. 다른 통합이 구성된 경우 의 품목 수량 및 가격을 확인하십시오. [!DNL Commerce] 의 수량 일치 [!DNL Walmart Marketplace] 라이브 스토어에 연결하기 전에

