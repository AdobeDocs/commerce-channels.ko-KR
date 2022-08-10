---
title: Amazon 및 상거래 카탈로그 정보
description: Amazon 판매 채널은 Amazon 목록을 상거래 백엔드로 가져와서 제품 및 매출과 계속 동기화합니다.
exl-id: 659c9830-0a1d-4a0d-bb9c-afb609c0fbba
source-git-commit: 5d30a5282ede2db0d9619eb2263b733328d26426
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Amazon 및 [!DNL Commerce] 카탈로그

Adobe Commerce 또는 Magento Open Source 백엔드는 모든 제품 및 관련 설정 및 정보(이미지, 옵션, 가격 등)와 주문 및 배송 구성이 있는 카탈로그를 포함합니다. 사용자 [!DNL Amazon Seller Central] 또한 계정에는 카탈로그 및 주문 구성이 있으며, 이를 통해 매출을 엄격히 추적합니다 [!DNL Amazon Marketplace].

한 위치를 통해 제품 카탈로그와 매출을 보다 효과적으로 관리 및 검토하기 위해 Amazon 판매 채널은 Amazon 목록을 [!DNL Commerce] 백엔드, 제품 및 판매, 보고서 문제 및 트렌드를 지속적으로 동기화합니다. 여러 버전과의 통합을 지원합니다 [!DNL Amazon Seller Central] 계정, 여러 저장소에 대한 단일 인터페이스를 통해 모든 데이터를 추적합니다.

## 제품 속성

Adobe Commerce 및 Magento Open Source 관리 카탈로그는 제품 사용과 동기화됩니다 [속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;} 를 사용하여 제품 설정과 데이터를 정의합니다. Amazon은 온보딩을 통해 매핑되는 특성도 사용합니다. 다음 기간 동안 [사전 설정 작업](./amazon-pre-setup-tasks.md) Amazon 판매 채널용의 경우 Amazon 목록을 사용자의 사이트로 가져올 때 올바른 제품 매핑을 보장하기 위해 추가 Amazon 속성(필요한 경우)을 정의합니다 [!DNL Commerce] 카탈로그 이러한 속성에는 UPC, EAN, ISBN 및 ASIN([!DNL Amazon Standard Identification Number]). 온보딩을 통해 Amazon과 제품 간 동기화 [!DNL Commerce] 카탈로그를 구성합니다. 적절한 매핑 [!DNL Commerce] 및 Amazon 제품을 사용하면 제품 정보, 주문 및 인벤토리를 지속적으로 동기화할 수 있습니다.

카탈로그에 대해 작성되거나 구성되지 않은 경우 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html)온보딩 전에 {target=&quot;_blank&quot;} 및 제품에 대한 값. Amazon 속성을 가져올 때 검색, 탐색, 가격 규칙 등에 사용할 수 있습니다. 자세한 내용은 [ASIN, UPC, EAN, ISBN, SKU 및 기타 바코드는 무엇을 의미합니까?](https://sellerskills.com/multi-channel-operations/what-asin-upc-ean-isbn-sku-and-other-barcodes-mean/#what-is-isbn-number){target=&quot;_blank&quot;}

온보딩 후에는 언제든지 제품 속성 및 Amazon 매핑을 관리하고 업데이트할 수 있습니다.

## 제품 목록

Amazon 목록은 을 통해 판매하는 모든 제품에 대한 제품 페이지입니다 [!DNL Amazon Marketplace], 속성을 통해 매핑된 제품 설명, 가격, 이미지 등을 표시합니다. 온보딩 중에 [!DNL Commerce] 제품은 Amazon 목록에 자동으로 게시될 수 있습니다. 기존 Amazon 목록을 [!DNL Commerce] 제품.

목록을 만든 경우 [!DNL Commerce] 제품을 사용하면 승인을 위해 Amazon에 제출됩니다. 가장 성공적인 목록은 몇 시간 이내에 승인됩니다. 목록이 승인되면 [!DNL Amazon Marketplace] 을 참조하십시오. 다음 [!DNL Amazon Sales Channel] 확장은 Amazon 목록을 검토할 수 있는 탭 세트를 제공합니다. 문제 또는 필요한 데이터에 따라 [!DNL Amazon Seller Central] 이러한 목록에 대한 구체적인 세부 사항이 필요하면 계정을 사용하십시오.

- [활성](./active-listings.md): 마켓플레이스를 통해 사용할 수 있는 승인된 제품 목록을 나열합니다.

- [목록 준비](./ready-to-list.md): 규칙 요구 사항을 나열하고 Amazon에 게시할 준비가 된 제품을 나열합니다.

- [비활성](./inactive-listings.md): 특정 이유(예: 브랜딩 문제 등), 닫힘 및 재지정 필요 등으로 인해 마켓플레이스에서 사용할 수 없는 제품을 나열합니다.

- [부적격](./ineligible-listings.md): 목록 규칙으로 인해 에는 마켓플레이스에 적극적으로 나열할 수 없는 제품(예: `0` 수량 또는 판매 일자).

- [완료되지 않음](./incomplete-listings.md): 필수 정보가 없는 제품을 나열합니다. 다른 검토를 위해 제품 데이터를 업데이트합니다.

- [종료됨](./ended-listings.md): 목록에 사용할 수 있지만 Amazon에서 수동으로 제거된 제품 목록을 표시합니다. 이 제품을 다시 목록을 만들 수 있습니다.

## 데이터 동기화

Adobe Commerce과 Magento Open Source은 제품 및 주문 데이터를 [!DNL Amazon Seller Central] 계정 및 [!DNL Commerce] 백엔드. 지속적인 업데이트는 다음을 통해 단일 소스를 제공합니다. [!DNL Commerce] 재고 관리 및 유지 관리, 주문 이행, 판매 추적, 간접비 및 작업 중복 감소 보고 기능은 트렌드를 추적하고 두 시스템 간에 발생한 통신 문제를 해결하기 위한 최신 데이터를 캡처합니다.

모든 동기화는 [cron 작업](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}, 5분마다 업데이트하도록 설정 [사전 설정 작업](./amazon-pre-setup-tasks.md).
