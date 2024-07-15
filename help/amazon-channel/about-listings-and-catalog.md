---
title: Amazon 및 Commerce 카탈로그
description: Amazon 판매 채널은 Amazon 목록을 Commerce 백엔드로 가져오고 제품 및 판매와 계속 동기화합니다.
role: Leader, Admin, User
feature: Sales Channels, Integration, Tools and External Services, Merchandising, Catalog Management
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Amazon 및 [!DNL Commerce] 카탈로그

Adobe Commerce 또는 Magento Open Source 백엔드에는 모든 제품 및 관련 설정 및 정보(이미지, 옵션, 가격 등)와 주문 및 배송 구성이 포함된 카탈로그가 포함되어 있습니다. [!DNL Amazon Seller Central] 계정에도 카탈로그 및 주문 구성이 있으며 [!DNL Amazon Marketplace]을(를) 통해 판매를 엄격하게 추적합니다.

한 곳에서 제품 카탈로그 및 판매를 보다 효율적으로 관리하고 검토하기 위해 Amazon 판매 채널은 Amazon 목록을 [!DNL Commerce] 백엔드로 가져오고 지속적으로 제품 및 판매와 동기화하며 문제 및 트렌드를 보고합니다. 여러 [!DNL Amazon Seller Central] 계정과의 통합을 지원하므로 여러 저장소에 대한 단일 인터페이스를 통해 모든 데이터를 추적할 수 있습니다.

## 제품 속성

Adobe Commerce 및 Magento Open Source은 제품 설정 및 데이터를 정의하기 위해 제품 [특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을(를) 사용하는 것과 카탈로그 관리를 동기화합니다. Amazon은 온보딩을 통해 매핑될 속성을 사용하기도 합니다. Amazon 판매 채널에 대한 [사전 설정 작업](./amazon-pre-setup-tasks.md)을 수행하는 동안 필요한 경우 추가 Amazon 특성을 정의하여 Amazon 목록을 [!DNL Commerce] 카탈로그로 가져올 때 올바른 제품 매핑을 보장합니다. 이러한 특성에는 UPC, EAN, ISBN 및 ASIN([!DNL Amazon Standard Identification Number])이 포함됩니다. 온보딩을 통해 제품이 특성을 사용하여 Amazon과 [!DNL Commerce] 카탈로그 간에 동기화됩니다. [!DNL Commerce]과(와) Amazon 제품의 적절한 매핑을 통해 제품 정보, 주문 및 인벤토리를 지속적으로 동기화할 수 있습니다.

카탈로그에 대해 이러한 특성을 만들거나 구성하지 않은 경우 온보딩 전에 [!DNL Commerce] [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) 및 값을 제품에 추가해야 합니다. Amazon 속성을 가져오면 검색, 탐색, 가격 규칙 등에 사용할 수 있습니다. [ASIN, UPC, EAN, ISBN, SKU 및 기타 바코드는 무엇을 의미합니까?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

온보딩 후 언제든지 제품 속성 및 Amazon 매핑을 관리하고 업데이트할 수 있습니다.

## 제품 목록

Amazon 목록은 [!DNL Amazon Marketplace]을(를) 통해 판매하는 모든 제품에 대한 제품 페이지로, 특성을 통해 제품 설명, 가격, 이미지 등을 표시합니다. 온보딩 중에 [!DNL Commerce] 제품을 Amazon 목록에 자동으로 게시하도록 구성할 수 있습니다. 기존 Amazon 목록을 [!DNL Commerce] 제품에 매핑하여 가져올 수도 있습니다.

목록 [!DNL Commerce]개 제품을 만들면 승인을 위해 Amazon에 제출됩니다. 대부분의 성공적인 목록은 몇 시간 이내에 승인됩니다. 목록이 승인되면 [!DNL Amazon Marketplace]에 고객의 즉시 주문에 대한 목록이 나타납니다. [!DNL Amazon Sales Channel] 확장은 Amazon 목록을 검토할 수 있는 탭 집합을 제공합니다. 문제 또는 필수 데이터에 따라 [!DNL Amazon Seller Central] 계정에서 이러한 목록에 대한 특정 세부 정보를 검토해야 합니다.

- [활성](./active-listings.md): 마켓플레이스를 통해 사용할 수 있는 승인된 제품 목록을 나열합니다.

- [목록 준비](./ready-to-list.md): 목록 규칙 요구 사항을 충족하고 Amazon에 게시할 준비가 된 제품을 나열합니다.

- [비활성](./inactive-listings.md): 특정 이유(예: 브랜딩 문제)로 인해 차단되고 닫혀 있고 다시 게시해야 하는 등의 이유로 마켓플레이스에서 사용할 수 없는 제품을 나열합니다.

- [부적격](./ineligible-listings.md): 목록 규칙으로 인해 마켓플레이스에 활발하게 나열할 수 없는 제품을 나열합니다(예: `0` 수량 또는 판매 날짜).

- [완료 안 됨](./incomplete-listings.md): 필수 정보가 누락된 제품을 나열합니다. 다른 검토를 위해 제품 데이터를 업데이트합니다.

- [종료](./ended-listings.md): 목록에 사용할 수 있는 제품 목록을 나열하지만 Amazon에서 수동으로 제거되었습니다. 이러한 제품을 다시 나열할 수 있습니다.

## 데이터 동기화 중

Adobe Commerce과 Magento Open Source은 [!DNL Amazon Seller Central] 계정과 [!DNL Commerce] 백 엔드 간에 제품 및 주문 데이터를 전달합니다. 지속적인 업데이트는 [!DNL Commerce]을(를) 통해 단일 소스로 제공하여 인벤토리를 관리하고 유지 관리하며 주문을 이행하고 매출을 추적하고 오버헤드와 작업 중복을 줄입니다. 보고는 최신 데이터를 캡처하여 트렌드를 추적하고 두 시스템 간에 포착된 통신 문제를 해결합니다.

모든 동기화는 [cron 작업](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)에 의해 관리되며, [사전 설정 작업](./amazon-pre-setup-tasks.md)에서 5분마다 업데이트되도록 설정됩니다.
