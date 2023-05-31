---
title: 카탈로그 속성 매핑
description: '''일치하는 [DNL!에 대한 속성 매핑'' 기존 Commerce] 제품 [!DNL Walmart Marketplace] 다음 기간 동안 데이터 목록 및 동기화 [!DNL Channel Manager] 및 [!DNL Walmart].'''
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# 카탈로그 속성 매핑

목록을 연결하기 전에 [!DNL Commerce] 끝 [!DNL Walmart Marketplace]에서 하나 이상의 고유 식별자를 매핑해야 합니다. [!DNL Commerce] 카탈로그와 Walmart의 해당 식별자.

이 단계는 일치해야 합니다. [!DNL Commerce] 기존 제품 [!DNL Walmart] 목록 및 제품 데이터 동기화 [!DNL Commerce] 및 [!DNL Walmart]. 다음 [!DNL Commerce] 제품에는 필요한 다음 제품 식별자(제품 ID) 중 하나와 일치하는 제품 속성이 하나 이상 있어야 합니다. [!DNL Walmart].

**필수 [!DNL Walmart] 제품 ID**

| **수락된 유형** | **이름** | **목적** | **허용되는 숫자** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 글로벌 무역 항목 | 범용성, 전 세계적으로 사용 | 14자리 |
| ISBN | 국제 표준 도서 번호 | 페이퍼백, 하드커버 및 전자책 | 10 또는 13자리 |
| ISSN | 국제 표준 일련 번호 | 모든 매체 인쇄 및 전자 인쇄에 게재되는 모든 종류의 잡지, 잡지, 신문 및 정기 간행물을 식별하기 위해 사용되는 8자리 일련 번호 | 숫자 8개 |
| UPC | 범용 제품 코드 | 표준 소매 추적 코드 | 12자리 |

카탈로그에 일치하는 속성이 없으면 [기존 카탈로그 속성 추가 또는 변환](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

## 고유 식별자 매핑

1. 다음에서 **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** sales channel 스토어에 대한 페이지에서 **[!UICONTROL Channel Settings]**.

1. 날짜 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Map Attributes]**.

   - 다음 찾기 [!DNL Walmart Marketplace] 매핑할 속성입니다.

   - 에서 해당 속성을 선택합니다. [!DNL Commerce] 카탈로그 저장.

      다음 예제는 [!UICONTROL Walmart Marketplace UPC] 제품 카탈로그의 UPC 속성에 대한 속성입니다.

      ![제품 일치 기준에 대한 속성 매핑](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - 선택 **[!UICONTROL Save]**.
