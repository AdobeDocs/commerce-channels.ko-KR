---
title: Amazon 및 상거래 카탈로그
description: Amazon 판매 채널은 Amazon 목록을 Commerce 백엔드로 가져오고 제품 및 판매와 계속 동기화합니다.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Amazon 및 [!DNL Commerce] 카탈로그

Adobe Commerce 또는 Magento Open Source 백엔드에는 모든 제품 및 관련 설정 및 정보(이미지, 옵션, 가격 등)와 주문 및 배송 구성이 포함된 카탈로그가 포함되어 있습니다. 사용자 [!DNL Amazon Seller Central] 또한, 계정에는 카탈로그 및 주문 구성이 있어 다음을 통해 판매를 엄격하게 추적합니다. [!DNL Amazon Marketplace].

한 곳에서 제품 카탈로그 및 판매를 보다 효율적으로 관리하고 검토하기 위해 Amazon 판매 채널은 Amazon 목록을 로 가져옵니다. [!DNL Commerce] 제품 및 판매와 지속적으로 동기화하고 문제 및 트렌드를 보고합니다. 여러 과의 통합을 지원합니다. [!DNL Amazon Seller Central] 계정, 여러 스토어프론트에 대한 단일 인터페이스를 통해 모든 데이터를 추적합니다.

## 제품 속성

Adobe Commerce 및 Magento Open Source 카탈로그 관리제품 사용과 동기화 [속성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) 제품 설정 및 데이터를 정의합니다. Amazon은 온보딩을 통해 매핑될 속성을 사용하기도 합니다. 다음 기간 동안 [사전 설정 작업](./amazon-pre-setup-tasks.md) Amazon sales channel의 경우 Amazon 목록을 로 가져올 때 추가 Amazon 속성(필요한 경우)을 정의하여 올바른 제품 매핑을 보장합니다 [!DNL Commerce] 카탈로그. 이러한 속성에는 UPC, EAN, ISBN 및 ASIN([!DNL Amazon Standard Identification Number]). 온보딩을 통해 제품은 Amazon과 간에 동기화됩니다. [!DNL Commerce] 속성을 사용한 카탈로그. 의 적절한 매핑 [!DNL Commerce] 및 Amazon 제품은 제품 정보, 주문 및 재고를 지속적으로 동기화합니다.

카탈로그에 대해 이러한 속성을 만들거나 구성하지 않은 경우 [!DNL Commerce] [제품 속성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) 및 온보딩 전 제품에 대한 값. Amazon 속성을 가져오면 검색, 탐색, 가격 규칙 등에 사용할 수 있습니다. 다음을 참조하십시오 [ASIN, UPC, EAN, ISBN, SKU 및 기타 바코드는 무엇을 의미합니까?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target="_blank"}

온보딩 후 언제든지 제품 속성 및 Amazon 매핑을 관리하고 업데이트할 수 있습니다.

## 제품 목록

Amazon 목록은 을 통해 판매하는 모든 제품에 대한 제품 페이지입니다. [!DNL Amazon Marketplace], 제품 설명, 가격, 이미지 등을 속성을 통해 표시합니다. 온보딩 중에 다음을 구성할 수 있습니다. [!DNL Commerce] 제품은 Amazon 목록에 자동으로 게시될 수 있습니다. 기존 Amazon 목록을 다음에 매핑하여 가져올 수도 있습니다. [!DNL Commerce] 제품.

목록을 만든 경우 [!DNL Commerce] 제품은 승인을 위해 Amazon에 제출됩니다. 대부분의 성공적인 목록은 몇 시간 이내에 승인됩니다. 목록이 승인되면 [!DNL Amazon Marketplace] (고객이 즉시 주문). 다음 [!DNL Amazon Sales Channel] extension은 Amazon 목록을 검토하는 탭 집합을 제공합니다. 문제 또는 필수 데이터에 따라 다음을 검토해야 합니다. [!DNL Amazon Seller Central] 계정 을 참조하십시오.

- [활성](./active-listings.md): 마켓플레이스를 통해 사용할 수 있는 승인된 제품 목록을 나열합니다.

- [나열 준비 완료](./ready-to-list.md): 목록 규칙 요구 사항을 충족하고 Amazon에 게시할 준비가 된 제품을 나열합니다.

- [비활성](./inactive-listings.md): 특정 이유(예: 브랜딩 문제)로 차단되거나, 종료되었거나, 재판매해야 하는 등으로 인해 마켓플레이스에서 사용할 수 없는 제품을 나열합니다.

- [부적당해](./ineligible-listings.md): 목록 규칙으로 인해 은 마켓플레이스에서 적극적으로 나열할 수 없는 제품을 나열합니다(예: `0` 수량 또는 판매 일자).

- [미완료](./incomplete-listings.md): 필수 정보가 누락된 제품을 나열합니다. 다른 검토를 위해 제품 데이터를 업데이트합니다.

- [종료](./ended-listings.md): 목록에 사용할 수 있지만 Amazon에서 수동으로 제거된 제품 목록을 표시합니다. 이러한 제품을 다시 나열할 수 있습니다.

## 데이터 동기화 중

Adobe Commerce과 Magento Open Source은 제품 및 주문 데이터를 [!DNL Amazon Seller Central] 계정 및 [!DNL Commerce] 백엔드. 지속적인 업데이트는 다음을 통해 단일 소스를 제공합니다. [!DNL Commerce] 재고 관리 및 유지, 주문 이행, 판매 추적, 업무 부담 및 중복을 줄이기 위해 보고는 최신 데이터를 캡처하여 트렌드를 추적하고 두 시스템 간에 포착된 통신 문제를 해결합니다.

모든 동기화는 [cron job](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)에서 5분마다 업데이트하도록 설정 [사전 설정 작업](./amazon-pre-setup-tasks.md).
