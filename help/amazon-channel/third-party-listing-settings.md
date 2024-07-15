---
title: Amazon Sales Channel - [!UICONTROL Third-party Listings]
description: 서드파티 목록 설정 업데이트에서는 Commerce 카탈로그가 기존 Amazon Seller Central 목록에서 제품을 가져오는지 여부를 결정합니다.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

타사 목록 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

이 설정은 [!DNL Commerce] 카탈로그가 기존 [!DNL Amazon Seller Central] 목록에서 제품을 가져오는지 여부를 결정합니다. Amazon에서 목록을 가져와서 모든 목록에 일치하는 [!DNL Commerce] 제품이 있는지 확인하는 것이 좋습니다. 목록이 [!DNL Commerce] 카탈로그에 포함된 경우 단일 카탈로그에서 모든 제품을 관리하고 Amazon 판매 채널 기능을 사용할 수 있습니다. 이러한 기능에는 Amazon을 통한 이행 및 주문 관리, 지능형 가격 조정 및 수량 관리 등이 포함됩니다.

Amazon 목록을 가져오도록 구성된 경우 Amazon 판매 채널은 Amazon 목록을 [!DNL Commerce] 카탈로그로 가져와서 기존 제품에 일치시키려고 합니다. 일치하는 항목이 자동으로 없으면 Amazon 목록을 새 [!DNL Commerce] 제품으로 가져오거나 목록을 제품에 수동으로 일치시킬 수 있습니다.

Amazon 목록을 가져오려면 Amazon 판매자 SKU 및 Amazon ASIN 값이 있는 [!DNL Commerce] 특성을 선택하십시오. [!DNL Commerce] [제품 특성](./ob-creating-magento-attributes.md)이 없는 경우 만들어 할당하는 것이 좋습니다. 이러한 특성을 매핑하면 가져온 Amazon 목록을 [!DNL Commerce] 제품에 올바르게 연결할 수 있습니다.

[스토어 통합](./store-integration.md)이 완료되면 초기 목록 가져오기가 시작됩니다. 그 후 크론 설정을 기반으로 [!DNL Commerce]에서 새로 추가된 Amazon 목록(Amazon Sales Channel에서 만들어지지 않음)을 계속 확인하고 타사 목록 설정에 따라 [!DNL Commerce] 카탈로그를 업데이트합니다.

## 서드파티 목록 설정 구성

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Third Party Listings]_섹션을 확장합니다.

1. **[!UICONTROL Import Third Party Listings]**(필수)에 대해 다음 옵션을 선택하십시오.

   - `Import Listing` - (기본값) Amazon 목록의 제품 정보를 [!DNL Commerce] 제품 카탈로그로 가져오려면 선택합니다. 이 옵션은 기본값이며 권장됩니다.

   - `Do Not Import Listing` - Amazon 목록의 [!DNL Commerce] 카탈로그에 수동으로 [새 제품을 만들고 할당](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html)하려는 경우 선택합니다.

   >[!NOTE]
   >다음 옵션 필드는 `Import Listing`(으)로 설정된 경우에만 활성화됩니다.

1. **[!UICONTROL Attribute That Contains Amazon Seller SKU]**&#x200B;의 경우 Amazon 판매자 SKU 값과 일치하는 [!DNL Commerce] 특성을 선택하십시오.

1. **[!UICONTROL Attribute That Contains Amazon ASIN]**&#x200B;의 경우 만든 [!DNL Commerce] 특성을 선택하고 이를 Amazon ASIN과 일치시키십시오.

   >[!NOTE]
   >Amazon 목록에 대해 이러한 [!DNL Commerce] 특성을 만들지 않은 경우 [Amazon 일치에 대한 특성 만들기](./ob-creating-magento-attributes.md)를 참조하십시오.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![타사 목록](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | 필수. 옵션:<ul><li>**[!UICONTROL Import Listing]** - (기본값) Amazon 목록의 제품 정보를 [!DNL Commerce] 제품 카탈로그로 가져오려면 선택합니다. </li><li>**[!UICONTROL Do Not Import Listing]** - Amazon 목록의 [!DNL Commerce] 카탈로그에 수동으로 [새 제품을 만들고 할당](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html)하려는 경우 선택합니다.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | `Import Listing`(으)로 설정된 경우에만 활성화됩니다.<br>Amazon 판매자 SKU에 대한 Amazon 특성과 일치하는 [!DNL Commerce] 특성을 선택합니다. 이 특성이 없으면 [Amazon 일치를 위한 Amazon 제품 특성 만들기](./ob-creating-magento-attributes.md)를 참조하십시오. 필요한 경우 [!DNL Commerce] [특성](./managing-attributes.md)을(를) 검토하고 이 Amazon 데이터와 일치하는 특성을 만들거나 편집하십시오. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | `Import Listing`(으)로 설정된 경우에만 활성화됩니다.<br>Amazon ASIN에 대한 Amazon 특성과 일치하는 [!DNL Commerce] 특성을 선택합니다. 이 특성이 없으면 [Amazon 일치를 위한 Amazon 제품 특성 만들기](./ob-creating-magento-attributes.md)를 참조하십시오. 필요한 경우 [!DNL Commerce] [특성](./managing-attributes.md)을(를) 검토하고 이 Amazon 데이터와 일치하는 특성을 만들거나 편집하십시오. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
