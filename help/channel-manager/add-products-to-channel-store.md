---
title: Channel Manager에 제품 추가
description: '카탈로그의 제품을 채널 관리자에 구성된 판매 채널에 추가하여  [!DNL Walmart Marketplace] 판매에 대한 제품 분류를 만듭니다.'
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# [!DNL Channel Manager]에 제품 추가

[!DNL Walmart Marketplace] 판매 채널에 제품을 추가하려면 [!DNL Commerce] 제품 카탈로그에서 제품을 선택하고 [!DNL Channel Manager](으)로 가져오십시오.
선택한 제품 수에 따라 가져오기 프로세스가 최대 30분 이상 걸릴 수 있습니다.

## 전제 조건

**[카탈로그 특성 매핑](map-catalog-attributes.md)** - [!DNL Channel Settings] 구성에서 [!DNL Commerce] 제품 카탈로그의 하나 이상의 특성을 필요한 Walmart 제품 식별자—-GTIN, ISBN, ISSN, UPC, EAN 중 하나에 매핑합니다.

## 목록 요구 사항

[!DNL Commerce] 제품 목록에 다음과 같은 필수 특성 구성이 있어야 합니다.

- **[!UICONTROL Connect to Channel Manager]** 특성이 활성화되었습니다.

- 필요한 Walmart 속성에 유효한 값을 제공합니다.

   - 필수 [!DNL Walmart Marketplace] 제품 식별자-GTIN, ISBN, ISSN, UPC, EAN 중 하나와 일치하는 제품 특성 하나 이상.

   - 제품 가격이 최대 소수 둘째 자리까지 지정되었습니다. 예: `9.99`

   - 제품 무게가 최대 소수 두 자리까지 지정되었습니다(예: `1.25`).

>[!TIP]
>
>판매 채널 목록 최적화에 대한 자세한 내용은 [Walmart Marketplace 목록 품질 최적화 안내서](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf)를 참조하십시오.

## 제품 추가

1. 연결된 판매 채널 스토어에서 **제품 추가**&#x200B;를 선택하여 제품 카탈로그를 엽니다.

   ![판매 채널 스토어에 제품 추가](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   카탈로그가 새 탭에서 열립니다.

1. 카탈로그 제품 표에서 [!DNL Walmart Marketplace]에 판매할 제품을 선택합니다.

   ![판매 채널 스토어로 제품 보내기](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. 선택한 항목에 대해 **[!UICONTROL Connect to Channel Manager]** 특성을 사용하도록 설정합니다.

   - **[!UICONTROL Actions]**&#x200B;에서 **[!UICONTROL Update attributes]**&#x200B;을(를) 선택합니다.

   - **[!UICONTROL Connect to Channel Manager]** 특성으로 스크롤하여 활성화합니다.

   - 제품 특성에 필요한 [!DNL Walmart Product IDs] 중 하나 이상이 포함되어 있는지 확인하십시오.

   - **[!UICONTROL Save]**&#x200B;을(를) 선택합니다.

     확인 메시지가 표시됩니다.

     ![카탈로그에서 판매 채널 확인 메시지로 제품 가져오기](assets/product-import-from-catalog-confirmation.png){width="400"}

     업데이트가 예약되어 있다는 메시지가 나타나면 [`queue:consumers:start`](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] 명령을 사용하여 업데이트를 즉시 처리하십시오.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. 가져오기 작업이 완료되면 [!DNL Channel Manager](으)로 돌아가서 **[!UICONTROL Listings]**&#x200B;을(를) 선택하여 추가한 제품을 확인합니다.

   처음에는 제품이 *초안* 상태입니다. 테이블을 업데이트하려면 **[!UICONTROL Refresh products]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Draft]** 상태 카드를 선택하여 채널 관리자에 추가된 새 제품을 표시하도록 보기를 업데이트합니다.

   ![연결된 판매 채널로 제품 가져옴](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


