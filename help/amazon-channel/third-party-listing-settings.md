---
title: AMAZON SALES CHANNEL - [!UICONTROL Third-party Listings]
description: 서드파티 목록 설정 업데이트에서는 상거래 카탈로그가 기존 Amazon Seller Central 목록에서 제품을 가져오는지 여부를 결정합니다.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

타사 목록 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이 설정에 따라 [!DNL Commerce] 카탈로그가 기존 제품에서 제품을 가져옵니다. [!DNL Amazon Seller Central] 목록. Amazon에서 목록을 가져와서 모든 목록에 일치하는 항목이 있는지 확인하는 것이 좋습니다 [!DNL Commerce] 제품. 목록이 사용자의 일부인 경우 [!DNL Commerce] 카탈로그에서는 단일 카탈로그에서 모든 제품을 관리하고 Amazon 판매 채널 기능을 사용할 수 있습니다. 이러한 기능에는 Amazon을 통한 이행 및 주문 관리, 지능형 가격 조정 및 수량 관리 등이 포함됩니다.

Amazon 목록을 가져오도록 구성된 경우 Amazon 판매 채널은 Amazon 목록을 로 가져옵니다. [!DNL Commerce] 카탈로그에서 기존 제품에 해당 항목을 일치시키고 있습니다. 일치하는 항목을 자동으로 찾을 수 없는 경우 Amazon 목록을 새 항목으로 가져올 수 있습니다 [!DNL Commerce] 제품 또는 수동으로 목록에 제품과 일치

Amazon 목록을 가져오려면 [!DNL Commerce] Amazon 판매자 SKU 및 Amazon ASIN에 대한 값이 있는 속성. 없는 경우 [!DNL Commerce] [제품 속성](./ob-creating-magento-attributes.md), 파일을 만들고 할당하는 것이 좋습니다. 이러한 속성을 매핑하면 가져온 Amazon 목록을 [!DNL Commerce] 제품.

다음과 같은 경우 초기 목록 가져오기가 시작됩니다. [스토어 통합](./store-integration.md) 이(가) 완료되었습니다. 나중에 그리고 크론 설정에 따라 [!DNL Commerce] 새로 추가된 Amazon 목록(Amazon Sales Channel에서 작성되지 않음)을 계속 확인하고 [!DNL Commerce] 타사 목록 설정에 따른 카탈로그.

## 서드파티 목록 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 _[!UICONTROL Third Party Listings]_섹션.

1. 대상 **[!UICONTROL Import Third Party Listings]** (필수) 다음 옵션을 선택합니다.

   - `Import Listing` - (기본값) Amazon 목록의 제품 정보를 로 가져올 시기를 선택합니다. [!DNL Commerce] 제품 카탈로그. 이 옵션은 기본값이며 권장됩니다.

   - `Do Not Import Listing` - 수동으로 수행하려는 경우 선택 [새 제품 만들기 및 할당](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) (으)로 [!DNL Commerce] Amazon 목록 카탈로그.

   >[!NOTE]
   >다음 옵션 필드는 로 설정된 경우에만 활성화됩니다. `Import Listing`.

1. 대상 **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, 을(를) 선택합니다. [!DNL Commerce] Amazon 판매자 SKU 값에 일치하는 속성입니다.

1. 대상 **[!UICONTROL Attribute That Contains Amazon ASIN]**, 을(를) 선택합니다. [!DNL Commerce] 속성을 생성한 다음 Amazon ASIN에 일치시킵니다.

   >[!NOTE]
   >생성하지 않은 경우 [!DNL Commerce] Amazon 목록에 대한 속성은 다음을 참조하십시오. [Amazon 일치에 대한 속성 만들기](./ob-creating-magento-attributes.md).

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![서드파티 목록](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | 필수. 옵션:<ul><li>**[!UICONTROL Import Listing]** - (기본값) Amazon 목록의 제품 정보를 로 가져올 시기를 선택합니다. [!DNL Commerce] 제품 카탈로그. </li><li>**[!UICONTROL Do Not Import Listing]** - 수동으로 수행하려는 경우 선택 [새 제품 만들기 및 할당](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) (으)로 [!DNL Commerce] Amazon 목록 카탈로그.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | 로 설정된 경우에만 활성화됨 `Import Listing`.<br>다음을 선택합니다. [!DNL Commerce] Amazon 판매자 SKU의 Amazon 속성과 일치하는 속성. 이 속성이 없는 경우 다음을 참조하십시오 [Amazon 일치를 위한 Amazon 제품 속성 만들기](./ob-creating-magento-attributes.md). 필요한 경우 다음을 검토합니다. [!DNL Commerce] [속성](./managing-attributes.md) 이 Amazon 데이터와 일치하는 속성을 만들거나 편집합니다. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | 로 설정된 경우에만 활성화됨 `Import Listing`.<br>다음을 선택합니다. [!DNL Commerce] Amazon ASIN의 Amazon 속성과 일치하는 속성. 이 속성이 없는 경우 다음을 참조하십시오 [Amazon 일치를 위한 Amazon 제품 속성 만들기](./ob-creating-magento-attributes.md). 필요한 경우 다음을 검토합니다. [!DNL Commerce] [속성](./managing-attributes.md) 이 Amazon 데이터와 일치하는 속성을 만들거나 편집합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
