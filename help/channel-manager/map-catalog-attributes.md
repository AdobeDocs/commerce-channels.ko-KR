---
title: 카탈로그 속성 매핑
description: 일치하는 [DNL! 기존 제품에 대한 상거래 [!DNL Walmart Marketplace] 목록 및 데이터 동기화 [!DNL Channel Manager] 및 [!DNL Walmart].
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: fac4bbd3985e07b919f986c877b8584da797e6fe
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 카탈로그 속성 매핑

목록 게시 전 [!DNL Commerce] to [!DNL Walmart Marketplace]를 설정하는 경우, [!DNL Commerce] 카탈로그에서 Walmart의 해당 식별자로 가져옵니다.
이 단계는 일치해야 합니다 [!DNL Commerce] 기존 [!DNL Walmart] 목록 및 제품 데이터 동기화 [!DNL Commerce] 및 [!DNL Walmart].

제품 일치의 경우, Commerce 제품에는 다음에 필요한 다음 제품 식별자(제품 ID) 중 하나와 일치하는 제품 속성이 하나 이상 있어야 합니다. [!DNL Walmart].

**필수 Walmart 제품 ID**

| **수락된 유형** | **이름** | **목적** | **허용 가능한 자릿수** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 글로벌 무역 항목 | 전 세계적으로 사용되는 범용 | 14자리 |
| ISBN | 국제 표준 장부 번호 | 페이퍼백, 하드커버 및 전자책 | 10 또는 13자리 |
| ISN | 국제 표준 일련 번호 | 모든 미디어 인쇄물과 전자 매체에 게재된 모든 종류의 잡지, 저널, 신문 및 정기간행물을 식별하는 데 사용되는 8자리 일련 번호 | 8자리 |
| UPC | 범용 제품 코드 | 표준 소매 추적 코드 | 12자리 |

카탈로그에 일치하는 속성이 없으면 [기존 카탈로그 속성 추가 또는 변환](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## 고유 식별자 매핑

1. 설정 [!UICONTROL Listings] 영업 채널 저장소 페이지에서 **[!UICONTROL Settings]**.

   - 매핑할 Walmart Marketplace 속성을 찾습니다.

   - 에서 해당 속성을 선택합니다 [!DNL Commerce] 카탈로그를 저장합니다.

      다음 예에서는 Walmart Marketplace UPC 속성을 제품 카탈로그의 UPC 속성에 매핑합니다.
   ![제품 일치 기준에 대한 특성 매핑](assets/products-map-attributes-for-match.png)
   - 원할 경우 여러 속성을 매핑하여 일치 항목을 늘릴 수 있습니다. 두 개 이상의 속성을 매핑하는 경우 하나를 로 선택합니다 **기본 식별자**. 이

   - 선택 **[!UICONTROL Save]**.


## 매핑된 특성 구성 업데이트

매핑된 특성 설정을 업데이트하여 일치하는 제품에 대한 Commerce 제품 식별자를 변경합니다.

예를 들어 Commerce UPC 제품 속성 코드를 기반으로 하는 제품을 일치시키는 대신 SKU를 기반으로 일치시킬 수 있습니다. 또는 추가 속성을 매핑하여 일치를 개선합니다.

1. 에서 **[!UICONTROL Listings]**, 선택 **[!UICONTROL Settings]**.

1. 맵 속성 양식에서 필요에 따라 매핑된 속성 구성을 변경합니다.
