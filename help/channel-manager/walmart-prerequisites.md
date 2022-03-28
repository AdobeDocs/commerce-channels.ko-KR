---
title: 월마트 사전 요구 사항
description: Channel Manager와 통합하기 위해 필요한 Walmart Marketplace 정보 및 리소스가 있는지 확인합니다.
exl-id: c4f247e8-280a-4595-a6c8-cf8b732d7aab
source-git-commit: 1f493dd40e23d459645704e5a52f9cc5edf4629f
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 월마트의 사전 요구 사항

채널 관리자를 사용하려면 Walmart Marketplace에 대한 상거래 판매 채널을 구성하려면 다음 리소스 및 정보가 필요합니다.

* 등록된 Marketplace 판매자 계정에 로그인할 수 있는 자격 증명과 Walmart에서 판매할 승인

* Adobe Commerce 또는 Magento Open Source을 Walmart Marketplace에 연결하기 위한 API 키

   Walmart Marketplace API 키를 사용하면 Adobe Commerce 또는 Magento Open Source용 채널 관리자와 Walmart Marketplace를 통합할 수 있습니다. Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

## Marketplace 판매자 계정 설정

1. [Walmart Seller 응용 프로그램 제출](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
1. 월마트의 승인을 받은 후에 [Walmart Seller 계정 설정](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

## Walmart Marketplace API 키 생성

1. Walmart Marketplace로 이동하여 [Adobe용 솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

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

## Walmart Marketplace 스토어 상태

Walmart Marketplace에 제품을 게시할 때 사용 가능 여부는 Walmart Marketplace 저장소의 상태에 따라 다릅니다.

* 라이브 스토어의 경우, 제품 오퍼가 나열되며 일치 작업이 완료되면 판매 가능합니다.

* 라이브 상태가 아닌 저장소의 경우 제품 오퍼가 스테이징되어 고객에게 표시되지 않습니다. 스토어가 라이브로 전환되면 준비된 목록이 라이브 스토어에 자동으로 푸시됩니다.

![[!DNL Walmart Seller Central] 준비된 제품](assets/walmart-seller-central-staged.png)
