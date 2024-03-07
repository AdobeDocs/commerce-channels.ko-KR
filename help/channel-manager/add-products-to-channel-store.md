---
title: Channel Manager에 제품 추가
description: '제품 분류 만들기 [!DNL Walmart Marketplace] 카탈로그의 제품을 Channel Manager에 구성된 판매 채널에 추가하여 판매'
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# 에 제품 추가 [!DNL Channel Manager]

에 제품을 추가하려면 [!DNL Walmart Marketplace] 판매 채널에서 다음을 선택합니다. [!DNL Commerce] 제품 카탈로그 및 가져오기 [!DNL Channel Manager].
선택한 제품 수에 따라 가져오기 프로세스가 최대 30분 이상 걸릴 수 있습니다.

## 전제 조건

**[카탈로그 속성 매핑](map-catalog-attributes.md)**- [!DNL Channel Settings] 구성, 의 하나 이상의 속성 매핑 [!DNL Commerce] 제품 카탈로그를 필수 Walmart 제품 식별자 중 하나로 변환 - GTIN, ISBN, ISSN, UPC, EAN.

## 목록 요구 사항

[!DNL Commerce] 제품 목록에는 다음과 같은 필수 속성 구성이 있어야 합니다.

- **[!UICONTROL Connect to Channel Manager]** 속성이 활성화되었습니다.

- 필요한 Walmart 속성에 유효한 값을 제공합니다.

   - 필요한 제품 속성 중 하나와 일치하는 제품 속성 하나 이상 [!DNL Walmart Marketplace] 제품 식별자-GTIN, ISBN, ISSN, UPC, EAN.

   - 제품 가격이 소수점 최대 두 자리까지 지정되는 경우 `9.99`

   - 제품 가중치를 최대 소수 두 자리로 지정(예: ) `1.25`

>[!TIP]
>
>판매 채널 목록 최적화에 대한 자세한 내용은 [Walmart Marketplace 목록 품질 최적화 안내서](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## 제품 추가

1. 연결된 판매 채널 스토어에서 **제품 추가** 제품 카탈로그를 엽니다.

   ![판매 채널 스토어에 제품 추가](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   카탈로그가 새 탭에서 열립니다.

1. 카탈로그 제품 그리드에서 판매할 제품을 선택합니다 [!DNL Walmart Marketplace].

   ![판매 채널 스토어로 제품 보내기](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. 활성화 **[!UICONTROL Connect to Channel Manager]** 선택한 항목에 대한 속성입니다.

   - 출처: **[!UICONTROL Actions]**, 선택 **[!UICONTROL Update attributes]**.

   - 다음으로 스크롤 **[!UICONTROL Connect to Channel Manager]** 속성을 지정하고 활성화합니다.

   - 제품 속성에 필요한 항목 중 하나 이상이 포함되어 있는지 확인합니다 [!DNL Walmart Product IDs].

   - 선택 **[!UICONTROL Save]**.

     확인 메시지가 표시됩니다.

     ![카탈로그에서 판매 채널로 제품 가져오기 확인 메시지](assets/product-import-from-catalog-confirmation.png){width="400"}

     업데이트가 예약되어 있다는 메시지가 나타나면 [`queue:consumers:start`](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] 즉시 업데이트를 처리하는 명령입니다.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. 가져오기 작업이 완료되면 로 돌아가 추가한 제품을 확인합니다. [!DNL Channel Manager] 및 선택 **[!UICONTROL Listings]**.

   처음에는 제품이 다음 위치에 있습니다 *초안* 상태. 선택 **[!UICONTROL Refresh products]** 테이블을 업데이트합니다.

1. 보기를 업데이트하여 Channel Manager에 추가된 새 제품을 표시합니다. **[!UICONTROL Draft]** 상태 카드입니다.

   ![연결된 판매 채널로 가져온 제품](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


