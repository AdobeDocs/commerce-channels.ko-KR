---
title: 타사 목록
description: 타사 목록 설정을 업데이트하여 상거래 카탈로그가 기존 Amazon Seller Central 목록에서 제품을 가져오는지 결정합니다.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 타사 목록

타사 목록 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스합니다.

이러한 설정은 [!DNL Commerce] 카탈로그가 기존 [!DNL Amazon Seller Central] 목록에서 제품을 가져오는지 여부를 결정합니다. 모든 목록에 [!DNL Commerce] 제품과 일치하는 항목이 있는지 확인하기 위해 Amazon에서 목록을 가져오는 것이 가장 좋습니다. 목록이 [!DNL Commerce] 카탈로그의 일부인 경우 단일 카탈로그에서 모든 제품을 관리하고 Amazon 판매 채널 기능을 사용할 수 있습니다. 이러한 기능에는 Amazon을 통한 주문 처리 및 주문 관리, 지능형 가격 조정 및 수량 관리가 포함됩니다.

Amazon 목록을 가져오도록 구성된 경우, Amazon 판매 채널은 Amazon 목록을 [!DNL Commerce] 카탈로그로 가져와 기존 제품에 일치시키려고 합니다. 일치하는 항목이 자동으로 없으면 Amazon 목록을 새 [!DNL Commerce] 제품으로 가져오거나 목록을 수동으로 제품에 일치시킬 수 있습니다.

Amazon 목록을 가져오도록 선택한 경우 Amazon Seller SKU 및 Amazon ASIN에 대한 값이 있는 [!DNL Commerce] 속성을 선택합니다. [!DNL Commerce] [제품 특성](./ob-creating-magento-attributes.md)이 없는 경우 만들고 할당해 보십시오. 이러한 속성을 매핑하면 가져온 Amazon 목록을 [!DNL Commerce] 제품에 올바르게 일치시킬 수 있습니다.

[스토어 통합](./store-integration.md)이 완료되면 초기 목록 가져오기가 시작됩니다. 이후 및 사용자의 기준 설정에 따라 [!DNL Commerce]은(는) 새로 추가된 Amazon 목록(Amazon Sales Channel에서 만들어지지 않음)을 계속 확인하고 타사 목록 설정에 따라 [!DNL Commerce] 카탈로그를 업데이트합니다.

## 타사 목록 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. _[!UICONTROL Third Party Listings]_섹션을 확장합니다.

1. **[!UICONTROL Import Third Party Listings]**(필수)에 대해 다음 옵션을 선택합니다.

   - `Import Listing` - (기본값) Amazon 목록의 제품 정보를  [!DNL Commerce] 제품 카탈로그로 가져올 시점을 선택합니다. 이 옵션은 기본값이며 권장됩니다.

   - `Do Not Import Listing` - Amazon 목록을 위한  [카탈로그에 새 제품을 수동으로 만들고 할당할 시기](https://docs.magento.com/user-guide/catalog/products.html)를  [!DNL Commerce] 선택합니다.
   >[!NOTE]
   >다음 옵션 필드는 `Import Listing`으로 설정된 경우에만 활성화됩니다.

1. **[!UICONTROL Attribute That Contains Amazon Seller SKU]**&#x200B;에 대해 Amazon 판매자 SKU 값에 일치하는 [!DNL Commerce] 속성을 선택합니다.

1. **[!UICONTROL Attribute That Contains Amazon ASIN]**&#x200B;에 대해 만든 [!DNL Commerce] 속성을 선택하여 Amazon ASIN에 일치시킵니다.

   >[!NOTE]
   >Amazon 목록에 대해 이러한 [!DNL Commerce] 속성을 만들지 않은 경우 [Amazon Matching](./ob-creating-magento-attributes.md)에 대한 속성 만들기를 참조하십시오.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![타사 목록](assets/amazon-third-party-listings.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Import Third Party Listings] | 필수 여부. 옵션:<ul><li>**[!UICONTROL Import Listing]** - (기본값) Amazon 목록의 제품 정보를  [!DNL Commerce] 제품 카탈로그로 가져올 시점을 선택합니다. </li><li>**[!UICONTROL Do Not Import Listing]** - Amazon 목록을 위한  [카탈로그에 새 제품을 수동으로 만들고 할당할 시기](https://docs.magento.com/user-guide/catalog/products.html)를  [!DNL Commerce] 선택합니다.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | `Import Listing`으로 설정된 경우에만 활성화됩니다.<br>Amazon  [!DNL Commerce] Seller SKU에 대한 Amazon 속성과 일치하도록 속성을 선택합니다. 이 특성이 없으면 [Amazon Matching](./ob-creating-magento-attributes.md)에 대한 Amazon 제품 속성 만들기를 참조하십시오. 필요한 경우 [!DNL Commerce] [attributes](./managing-attributes.md)를 검토하고 이 Amazon 데이터와 일치하는 속성을 만들거나 편집하십시오. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | `Import Listing`으로 설정된 경우에만 활성화됩니다.<br>Amazon  [!DNL Commerce] ASIN의 Amazon 속성과 일치하는 속성을 선택합니다. 이 특성이 없으면 [Amazon Matching](./ob-creating-magento-attributes.md)에 대한 Amazon 제품 속성 만들기를 참조하십시오. 필요한 경우 [!DNL Commerce] [attributes](./managing-attributes.md)를 검토하고 이 Amazon 데이터와 일치하는 속성을 만들거나 편집하십시오. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
