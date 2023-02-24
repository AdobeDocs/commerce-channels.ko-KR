---
title: 카탈로그 속성 매핑
description: '일치하는 [DNL! 기존 제품에 대한 상거래 [!DNL Walmart Marketplace] 목록 및 데이터 동기화 [!DNL Channel Manager] 및 [!DNL Walmart]'
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 카탈로그 속성 매핑

목록을 연결하기 전에 [!DNL Commerce] to [!DNL Walmart Marketplace]를 설정하는 경우, [!DNL Commerce] 카탈로그에서 Walmart의 해당 식별자로 가져옵니다.

이 단계는 일치해야 합니다 [!DNL Commerce] 기존 [!DNL Walmart] 목록 및 제품 데이터 동기화 [!DNL Commerce] 및 [!DNL Walmart]. 다음 [!DNL Commerce] 제품에는 에 필요한 다음 제품 식별자(제품 ID) 중 하나와 일치하는 제품 속성이 하나 이상 있어야 합니다. [!DNL Walmart].

**필수 여부 [!DNL Walmart] 제품 ID**

| **수락된 유형** | **이름** | **목적** | **허용 가능한 자릿수** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 글로벌 무역 항목 | 전 세계적으로 사용되는 범용 | 14자리 |
| ISBN | 국제 표준 장부 번호 | 페이퍼백, 하드커버 및 전자책 | 10 또는 13자리 |
| ISN | 국제 표준 일련 번호 | 모든 미디어 인쇄물과 전자 매체에 게재된 모든 종류의 잡지, 저널, 신문 및 정기간행물을 식별하는 데 사용되는 8자리 일련 번호 | 8자리 |
| UPC | 범용 제품 코드 | 표준 소매 추적 코드 | 12자리 |

카탈로그에 일치하는 속성이 없으면 [기존 카탈로그 속성 추가 또는 변환](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## 고유 식별자 매핑

1. 에서 **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** 영업 채널 저장소 페이지에서 **[!UICONTROL Channel Settings]**.

1. 설정 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Map Attributes]**.

   - 를 찾습니다. [!DNL Walmart Marketplace] 매핑할 속성입니다.

   - 에서 해당 속성을 선택합니다 [!DNL Commerce] 카탈로그를 저장합니다.

      다음 예는 를 매핑합니다 [!UICONTROL Walmart Marketplace UPC] 속성을 제품 카탈로그의 UPC 속성에 추가합니다.

      ![제품 일치 기준에 대한 특성 매핑](assets/products-map-attributes-for-match.png)

   - 선택 **[!UICONTROL Save]**.
