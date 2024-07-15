---
title: 카탈로그 속성 매핑
description: '''일치하는 [DNL!에 대한 속성 매핑'' Commerce] 제품을 기존 [!DNL Walmart Marketplace] 목록에 추가 및  [!DNL Channel Manager] 과(와) [!DNL Walmart] 간의 데이터 동기화'''
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 카탈로그 속성 매핑

[!DNL Commerce]의 목록을 [!DNL Walmart Marketplace]에 연결하기 전에 [!DNL Commerce] 카탈로그의 고유 식별자 중 하나 이상을 Walmart의 해당 식별자에 매핑해야 합니다.

이 단계는 [!DNL Commerce] 제품을 기존 [!DNL Walmart] 목록에 일치시키고 [!DNL Commerce]과(와) [!DNL Walmart] 간에 제품 데이터를 동기화하는 데 필요합니다. [!DNL Commerce] 제품에는 [!DNL Walmart]에 필요한 다음 제품 식별자(제품 ID) 중 하나와 일치하는 제품 특성이 하나 이상 있어야 합니다.

**필수 [!DNL Walmart] 제품 ID**

| **허용된 형식** | **이름** | **목적** | **허용되는 숫자** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 글로벌 무역 항목 | 범용성, 전 세계적으로 사용 | 14자리 |
| ISBN | 국제 표준 도서 번호 | 페이퍼백, 하드커버 및 전자책 | 10 또는 13자리 |
| ISSN | 국제 표준 일련 번호 | 모든 매체 인쇄 및 전자 인쇄에 게재되는 모든 종류의 잡지, 잡지, 신문 및 정기 간행물을 식별하기 위해 사용되는 8자리 일련 번호 | 숫자 8개 |
| UPC | 범용 제품 코드 | 표준 소매 추적 코드 | 12자리 |

카탈로그에 일치하는 특성이 없으면 [기존 카탈로그 특성을 추가하거나 변환](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)하십시오.

## 고유 식별자 매핑

1. 판매 채널 스토어의 **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** 페이지에서 **[!UICONTROL Channel Settings]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Channel Settings]**&#x200B;에서 **[!UICONTROL Map Attributes]**&#x200B;을(를) 선택합니다.

   - 매핑할 [!DNL Walmart Marketplace] 특성을 찾습니다.

   - [!DNL Commerce] 저장소 카탈로그에서 해당 특성을 선택합니다.

     다음 예제에서는 [!UICONTROL Walmart Marketplace UPC] 특성을 제품 카탈로그의 UPC 특성에 매핑합니다.

     ![제품 일치 조건에 대한 특성 매핑](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - **[!UICONTROL Save]**&#x200B;을(를) 선택합니다.
