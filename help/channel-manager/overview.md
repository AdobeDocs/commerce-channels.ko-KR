---
title: 정보 [!DNL Channel Manager]
description: 설치 및 사용 방법 알아보기 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source 스토어를 타사 마켓플레이스와 통합하고 판매 채널을 만들어 마켓플레이스 목록, 가격, 인벤토리 및 매출을 상거래 관리자와 원활하게 관리할 수 있습니다.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 7412a3d5b78e206521a048fb56edacd8f11ddb58
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 개요

Adobe Commerce 및 Magento Open Source용 채널 관리자는 Walmart, Amazon, eBay와 같은 타사 마켓플레이스에서 채널 판매를 관리할 수 있도록 관리자가 편리한 작업 공간을 제공합니다. 상거래 관리자로부터 영업 채널 운영을 원활하게 관리하면서 매출을 늘리고 신규 시장으로 확장할 수 있습니다.

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-admin-entry-page.png)

## 베타 릴리스 개요

Channel Manager 베타 릴리스는 Walmart Marketplace에서 제품을 제공하려는 Adobe Commerce 또는 Magento Open Source 판매자를 지원합니다.

이 릴리즈는 영업 채널 작업을 관리하는 다음과 같은 기능을 지원합니다.

* Adobe Commerce 또는 Magento Open Source과 Walmart Marketplace 간의 API 연결 설정

* 제품 일치 기능을 사용하여 Channel Manager의 제품을 Walmart에 게시합니다

* 예를 들어 채널 관리자에서 제품 목록 상태 보기 *초안*, *처리*, *일치함*, *오류*.

* Commerce에서 Walmart로 대응 제품에 대한 재고 수량 동기화

* Commerce에서 Walmart로 일치하는 제품에 대한 카탈로그 가격 동기화

* Walmart Marketplace에서 주문을 받고 [!DNL Commerce] 주문 대시보드

### 채널 관리자 작업의 예상 지연

데이터 동기화 프로세스 간 [!DNL Channel Manager] 연결된 [!DNL Walmart Marketplace] 스토어를 완료하려면 시간이 필요합니다. 에 대한 예상 처리 시간 검토 [!DNL Channel Manager] 영업 채널 작업 계획을 지원하는 작업입니다.

**채널 관리자 작업의 예상 지연**

| **작업** | **설명** | **예상 지연** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
| 채널 관리자에 제품 추가 | 상거래 제품 카탈로그에서 제품을 선택하고 채널 관리자로 가져옵니다. | **최대 5분**-전체 제품 카탈로그와 같이 제품을 많이 선택하면 가져오기 프로세스가 길어집니다. |
| Walmart Marketplace에서 제품 일치 | 채널 관리자에서 제품 목록을 선택하고 매칭하려면 Walmart로 보내십시오. | **최대 30분**-여러 제품을 선택하면 선택한 수량에 따라 대응 프로세스가 더 길어집니다. |
| 인벤토리 업데이트 | 상거래에 재고 수량이 변경되는 경우. 채널 관리자가 Walmart에 대한 업데이트를 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변경되면 Channel Manager 는 업데이트를 Walmart로 동기화합니다. | **최대 5분** |
| Walmart에서 Commerce로 주문 동기화 | 고객은 Walmart Marketplace에서 상거래 제품을 주문합니다. Walmart가 채널 관리자에게 주문을 보냅니다. 순서는 주문 대시보드에 표시됩니다. | **최대 30분** |
| Commerce Order Management에서 만든 순서 | 채널 관리자는 Mart 주문에서 상거래 주문을 만들고 상거래 주문 번호를 포함하도록 주문 대시보드를 업데이트합니다. | **최대 5분** |

## 월마트의 사전 요구 사항

Commerce를 Walmart Marketplace와 통합하려면 Walmart에서 다음 정보가 필요합니다.

* 등록된 Marketplace 판매자 계정에 로그인할 수 있는 자격 증명과 Walmart에서 판매할 승인

* Adobe Commerce 또는 Magento Open Source을 Walmart Marketplace에 연결하기 위한 API 키

   Walmart Marketplace API 키를 사용하면 Adobe Commerce 또는 Magento Open Source용 채널 관리자와 Walmart Marketplace를 통합할 수 있습니다. Channel Manager 온보딩 프로세스를 시작하기 전에 Seller Central에서 API 키를 설정합니다.

### Marketplace 판매자 계정 설정

1. [Walmart Seller 응용 프로그램 제출](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
2. 월마트의 승인을 받은 후에 [Walmart Seller 계정 설정](https://sellerhelp.walmart.com/seller/s/guide?article=000008219).

### Walmart Marketplace API 키 생성

1. Walmart Marketplace로 이동하여 [Adobe용 솔루션 공급자 프로덕션 API 키](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey).

1. 키 만들기 및 권한 구성:

   * 솔루션 공급자로 Adobe 를 선택합니다.

   * 다음 표에 표시된 대로 권한을 설정합니다. 자세한 내용은 [API 자격 증명](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 에서 *Walmart Marketplace 판매자 도움말*.

&#x200B;|    **Walmart에 대한 Adobe API 키 구성**
&#x200B;| **권한** | **설정** | |—|—| | 컨텐츠 | 전체 액세스 | | 피드 가져오기 | 보기 전용 | | 인벤토리 | 전체 액세스 | | 항목 | 전체 액세스 | | 지연 시간 | 전체 액세스 | | 순서 | 전체 액세스 | | 가격 | 전체 액세스 | | 보고서 | 보기 전용 | | 반환 | 전체 액세스 | | 규칙 | 전체 액세스 | | 배송 | 전체 액세스 |

## Walmart Marketplace 스토어 상태

Walmart Marketplace에 제품을 게시할 때 사용 가능 여부는 Walmart Marketplace 저장소의 상태에 따라 다릅니다.

* 라이브 스토어의 경우, 제품 오퍼가 나열되며 일치 작업이 완료되는 즉시 판매 가능합니다.

* 라이브 상태가 아닌 저장소의 경우 제품 오퍼가 스테이징되어 고객에게 표시되지 않습니다. 스토어가 작동하면 준비된 목록이 자동으로 라이브 스토어에 푸시됩니다.


![[!DNL Walmart Seller Central] 준비된 제품](assets/walmart-seller-central-staged.png)
