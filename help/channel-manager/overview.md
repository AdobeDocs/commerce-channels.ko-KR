---
title: 정보 [!DNL Channel Manager]
description: 설치 및 사용 방법 알아보기 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source 스토어를 타사 마켓플레이스와 통합하고 판매 채널을 만들어 마켓플레이스 목록, 가격, 인벤토리 및 판매를 상거래 관리자와 원활하게 관리할 수 있습니다.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: ef4c1362424285d4969fe173a0790809fccff80b
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---


# 정보 [!DNL Channel Manager]

[!DNL Channel Manager] 은 Adobe Commerce 또는 Magento Open Source 제품 카탈로그를 와 통합하여 매출을 늘리고 새 고객에게 도달하도록 도와줍니다. [!DNL Walmart US Marketplace].

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-home.png)

채널 관리자는 Walmart Marketplace에서 판매하려는 Adobe Commerce 또는 Magento Open Source 판매자를 지원합니다.

설치 및 구성 후 [!DNL Channel Manager], [!DNL Commerce] 관리자가 확장되어 관리할 수 있습니다 [!DNL Walmart Marketplace] 상거래 환경에서 원활하게 영업 운영 수행

* **목록 관리**-전자 상거래 카탈로그의 제품을 기존 Walmart Marketplace 목록에 일치시켜 제품 목록을 쉽게 게시합니다.

* **Inventory management**-머천트의 마켓플레이스 판매자 계정의 항목은 정확한 재고 수준을 보장하기 위해 상거래에서 자동으로 동기화되고 업데이트됩니다.

* **가격 업데이트**-자동 가격 동기화를 통해 시장 목록을 위한 정확한 가격 책정 유지 Adobe Commerce에서 가격이 변경되면 10분 이내에 변경 사항이 마켓플레이스에 반영됩니다.

* **주문 관리**-마켓플레이스에서 새로운 주문이 생성되면 Channel Manager는 주문을 Adobe Commerce과 동기화하고 주문 확인을 마켓플레이스에 보내 각 주문에 대해 재고가 예약되도록 합니다.

* **배송 관리**-Adobe Commerce에서 주문이 출하된 것으로 표시되면, 출하 갱신은 [!DNL Walmart Marketplace]. 이 알림은 판매자가 이행 SLA 요구 사항을 충족하고 고객이 현재 주문에 대한 배송 업데이트 알림을 받을 수 있도록 해줍니다.

* **취소**-Adobe Commerce에서 주문이 취소되면 Channel Manager는 업데이트된 주문 정보를 마켓플레이스에 전송하여 해당 마켓플레이스 주문에 대한 작업을 복제합니다.

## 채널 관리자 작업의 예상 지연

데이터 동기화 프로세스 간 [!DNL Channel Manager] 연결된 [!DNL Walmart Marketplace] 스토어를 완료하려면 시간이 필요합니다. 에 대한 예상 처리 시간 검토 [!DNL Channel Manager] 영업 채널 작업 계획을 지원하는 작업입니다.

**채널 관리자 작업의 예상 지연**

| **작업** | **설명** | **예상 지연** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 채널 관리자에 제품 추가 | 상거래 제품 카탈로그에서 제품을 선택하고 채널 관리자로 가져옵니다. | **최대 5분**-전체 제품 카탈로그와 같이 제품을 많이 선택하면 가져오기 프로세스가 길어집니다. |
| Walmart Marketplace에서 제품 일치 | 채널 관리자에서 제품 목록을 선택하고 매칭하려면 Walmart로 보내십시오. | **최대 30분**-여러 제품을 선택하면 선택한 수량에 따라 대응 프로세스가 더 길어집니다. |
| 인벤토리 업데이트 | 상거래에 재고 수량이 변경되면 [!DNL Channel Manager] Walmart에 업데이트를 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변경되면 Channel Manager 는 업데이트를 Walmart로 동기화합니다. | **최대 5분** |
| Walmart에서 Commerce로 주문 동기화 | 고객은 Walmart Marketplace에서 상거래 제품을 주문합니다. Walmart가 채널 관리자에게 주문을 보냅니다. 순서는 주문 대시보드에 표시됩니다. | **최대 30분** |
| Commerce Order Management에서 만든 순서 | 채널 관리자는 Mart 주문에서 상거래 주문을 만들고 상거래 주문 번호를 포함하도록 주문 대시보드를 업데이트합니다. | **최대 5분** |

## 월마트의 사전 요구 사항

Commerce를 Walmart Marketplace와 통합하려면 Walmart에서 다음 정보가 필요합니다.

* 등록된 Marketplace 판매자 계정에 로그인할 수 있는 자격 증명과 Walmart에서 판매할 승인

* Adobe Commerce 또는 Magento Open Source을 Walmart Marketplace에 연결하기 위한 API 키

   Walmart Marketplace API 키를 사용하면 Adobe Commerce 또는 Magento Open Source용 채널 관리자와 Walmart Marketplace를 통합할 수 있습니다. Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

### Marketplace 판매자 계정 설정

1. [Walmart Seller 응용 프로그램 제출](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI).
2. 월마트의 승인을 받은 후에 [Walmart Seller 계정 설정](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Walmart Marketplace API 키 생성

1. Walmart Marketplace로 이동하여 [Adobe용 솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. 키 만들기 및 권한 구성:

   * 솔루션 공급자로 Adobe 를 선택합니다.

   * 다음 표에 표시된 대로 권한을 설정합니다. 자세한 내용은 [API 자격 증명](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 에서 *[!DNL Walmart Marketplace]판매자 도움말*.

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
