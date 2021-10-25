---
title: 타사 목록
description: 타사 목록 설정을 업데이트하여 상거래 카탈로그가 기존 Amazon Seller Central 목록에서 제품을 가져오는지 결정합니다.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 타사 목록

타사 목록 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 [!DNL Commerce] 카탈로그는 기존 제품에서 제품을 가져옵니다 [!DNL Amazon Seller Central] 목록. 모든 목록이 일치하는지 확인하기 위해 Amazon에서 목록을 가져오는 것이 가장 좋습니다 [!DNL Commerce] 제품. 목록에 포함된 경우 [!DNL Commerce] 카탈로그 역할을 통해 단일 카탈로그에서 모든 제품을 관리하고 Amazon 판매 채널 기능을 사용할 수 있습니다. 이러한 기능에는 Amazon을 통한 주문 처리 및 주문 관리, 지능형 가격 조정 및 수량 관리가 포함됩니다.

Amazon 목록을 가져오도록 구성되면 Amazon 판매 채널에서 Amazon 목록을 으로 가져옵니다 [!DNL Commerce] 카탈로그, 기존 제품에 일치시키려고 합니다. 일치하는 항목이 자동으로 없으면 Amazon 목록을 새 항목으로 가져올 수 있습니다 [!DNL Commerce] 제품을 선택하거나 목록을 제품에 수동으로 일치시킵니다.

Amazon 목록을 가져오도록 선택한 경우 [!DNL Commerce] Amazon 판매자 SKU 및 Amazon ASIN에 대한 값이 있는 속성. 없는 경우 [!DNL Commerce] [제품 속성](./ob-creating-magento-attributes.md)를 만들고 할당하는 것이 좋습니다. 이러한 속성을 매핑하면 가져온 Amazon 목록을 과 올바르게 일치시킬 수 있습니다 [!DNL Commerce] 제품.

초기 목록 가져오기는 다음과 같이 시작됩니다. [스토어 통합](./store-integration.md) 가 완료되었습니다. 나중에, 크론 설정을 기준으로 [!DNL Commerce] 새로 추가된 Amazon 목록(Amazon Sales Channel에서 만들어지지 않음)을 지속적으로 확인하고 [!DNL Commerce] 타사 목록 설정에 따라 카탈로그입니다.

## 타사 목록 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 저장 대시보드에서

1. 를 확장합니다. _[!UICONTROL Third Party Listings]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Import Third Party Listings]** (필수) 옵션을 선택합니다.

   - `Import Listing` - (기본값) Amazon 목록의 제품 정보를 사용자의 [!DNL Commerce] 제품 카탈로그 이 옵션은 기본값이며 권장됩니다.

   - `Do Not Import Listing` - 수동으로 선택할 시기 [새 제품 만들기 및 할당](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}()을 [!DNL Commerce] Amazon 목록에 대한 카탈로그
   >[!NOTE]
   >다음 옵션 필드는 `Import Listing`.

1. 대상 **[!UICONTROL Attribute That Contains Amazon Seller SKU]**&#x200B;을(를) 선택하고 을(를) 선택합니다. [!DNL Commerce] Amazon 판매자 SKU 값과 일치하는 특성입니다.

1. 대상 **[!UICONTROL Attribute That Contains Amazon ASIN]**&#x200B;을(를) 선택하고 을(를) 선택합니다. [!DNL Commerce] 생성한 속성을 확인하고 Amazon ASIN과 일치시킵니다.

   >[!NOTE]
   >이러한 필드를 만들지 않은 경우 [!DNL Commerce] Amazon 목록에 대한 속성은 [Amazon 일치용 속성 만들기](./ob-creating-magento-attributes.md).

1. 완료되면 를 클릭합니다. **[!UICONTROL Save listing settings]**.

![타사 목록](assets/amazon-third-party-listings.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Import Third Party Listings] | 필수 여부. 옵션:<ul><li>**[!UICONTROL Import Listing]** - (기본값) Amazon 목록의 제품 정보를 사용자의 [!DNL Commerce] 제품 카탈로그 </li><li>**[!UICONTROL Do Not Import Listing]** - 수동으로 선택할 시기 [새 제품 만들기 및 할당](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}()을 [!DNL Commerce] Amazon 목록에 대한 카탈로그</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | 로 설정된 경우에만 활성 `Import Listing`.<br>을(를) 선택합니다 [!DNL Commerce] 속성을 Amazon 판매자 SKU에 대한 Amazon 속성과 일치하는 것으로 사용합니다. 이 속성이 없는 경우 다음을 참조하십시오 [Amazon Matching을 위한 Amazon 제품 속성 만들기](./ob-creating-magento-attributes.md). 필요한 경우 [!DNL Commerce] [속성](./managing-attributes.md) 이 Amazon 데이터와 일치하는 속성을 만들거나 편집합니다. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | 로 설정된 경우에만 활성 `Import Listing`.<br>을(를) 선택합니다 [!DNL Commerce] Amazon ASIN에 대한 Amazon 속성과 일치하는 속성입니다. 이 속성이 없는 경우 다음을 참조하십시오 [Amazon Matching을 위한 Amazon 제품 속성 만들기](./ob-creating-magento-attributes.md). 필요한 경우 [!DNL Commerce] [속성](./managing-attributes.md) 이 Amazon 데이터와 일치하는 속성을 만들거나 편집합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
