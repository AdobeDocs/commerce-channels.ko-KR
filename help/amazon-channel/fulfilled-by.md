---
title: Amazon 목록에 대한 이행자 설정
description: 이행자 설정을 사용하여 Amazon 목록의 주문이 이행(출하)되는 방법을 결정합니다.
feature: Sales Channels, Products
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Amazon 목록에 대한 이행자 설정

_[!UICONTROL Fulfilled By]_설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

이러한 설정은 주문을 이행(또는 배송)하는 당사자를 정의합니다. 모든 주문이 한 가지 방법으로 이행된 경우 판매자(사용자) 또는 Amazon 중에서 선택합니다. 사용자의 위치에서 주문을 이행하고 Amazon을 사용할 계획이라면 세 번째 옵션을 사용하고 [!DNL Commerce] 제품 특성을 구성하는 것이 좋습니다.

- **[!UICONTROL Fulfilled by Merchant]** - 판매자인 귀하가 모든 주문을 충족하는지 여부를 선택합니다. 주문을 하면 [!DNL Commerce] 카탈로그에서 인벤토리가 공제됩니다.

- **[!UICONTROL Fulfilled by Amazon]** - Amazon이 모든 주문을 충족하는지 여부를 선택합니다. 이 옵션을 사용하면 주문을 했을 때 제품 인벤토리가 [!DNL Commerce] 카탈로그에서 공제되지 않습니다. Amazon 이행 주문의 재고 재고는 해당 창고에서 저장되고 공제됩니다. 이 옵션을 할당하기 전에 [!DNL Amazon Seller Central] 계정에서 제품이 _Amazon에서 이행함_(FBA) 이행에 적합한지 확인해야 합니다. FBA 인벤토리는 [!DNL Amazon Seller Central] 계정을 통해 직접 관리됩니다. 이 이행 방법을 사용하면 Amazon 판매 채널은 [!DNL Commerce]과(와) Amazon 간에 수량 업데이트를 공유하지 않습니다. 따라서 Amazon 판매 채널에서 수량 설정에 설명된 모든 마케팅 도구를 사용할 수 있는 것은 아닙니다.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 귀하와 Amazon이 제품을 이행한 경우 판매자가 이행한 값 및 Amazon이 이행한 값이 있는 [!DNL Commerce] 제품 속성을 만들 수 있습니다. 제품당 이 값을 설정하면 누가 주문을 이행하는지 나타냅니다.

이행 메서드는 지역 특성이며, [스토어 통합](./store-integration.md) 중에 정의된 **[!UICONTROL Amazon Marketplace Country]** 설정을 기반으로 합니다. 변경 사항이 적용되면 변경 사항은 동일한 지역에서 판매되는 Amazon 스토어의 [!DNL Amazon Seller SKU]을(를) 공유하는 모든 Amazon 목록에 영향을 줍니다([스토어 통합](./store-integration.md) 동안 _[!UICONTROL Amazon Marketplace Country]_에 정의됨). 미국에서 공유 [!DNL Amazon Seller SKU]을(를) 변경해도 저장소 통합 중에 정의된 다른 지역에 설정된 Amazon 저장소에는 영향을 주지 않습니다.

>[!NOTE]
>
>FBA(Amazon)에서 주문을 이행하고 주문을 가져오면 주문 세부 정보에서 일부 필드에 대한 더미 데이터를 볼 수 있습니다. [Amazon 주문 세부 사항](./amazon-order-details.md)을 참조하세요.

## [!UICONTROL Fulfilled By] 설정 구성 {#configure-fulfilled-by-settings}

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Fulfilled By]_섹션을 확장합니다.

1. **[!UICONTROL Product Fulfilled By]**&#x200B;의 경우 다음 주문을 이행할(배송할) 사용자를 선택하십시오.

   - `Fulfilled by Merchant` - 판매자가 주문을 충족합니다.

   - `Fulfilled by Amazon` - Amazon 웨어하우스가 순서를 충족합니다.

   - `Assign Fulfilled By Using Magento Product Attribute` - [!DNL Commerce] 특성은 제품당 주문을 이행하는 사용자를 나타냅니다.

     선택한 경우 **[!UICONTROL Fulfilled by Attribute]**&#x200B;에 매핑할 [!DNL Commerce] 특성을 선택합니다.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![설정에 의해 이행됨](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| 필드 | 설명 |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | 옵션:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) 주문을 이행할 경우 선택합니다. 주문을 하면 [!DNL Commerce] 카탈로그에서 인벤토리가 공제됩니다. 새 제품이 생성되면 이행된 머천트의 이행 방법이 지정됩니다.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Amazon이 주문을 충족하는지 여부를 선택합니다. 이 이행 방법을 사용하면 주문을 했을 때 제품 인벤토리가 [!DNL Commerce] 카탈로그에서 공제되지 않습니다. 제품이 만들어지면 이행 유형으로 _[!UICONTROL Fulfilled by Amazon (FBA)]_을(를) 사용하여 만들어집니다. 제품이 [!DNL Amazon Seller Central] 계정 내에서 FBA 이행에 적합한지 확인하십시오. FBA 인벤토리는 [!DNL Amazon Seller Central] 계정을 통해서도 직접 관리됩니다. 이 이행 방법을 사용하면 수량 업데이트가 [!DNL Commerce] 카탈로그에 대해 푸시되지 않으므로 [재고/수량 설정](./stock-quantity.md)에 설명된 일부 마케팅 도구를 사용할 수 없습니다.</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 기존의 [!DNL Commerce] 특성이 있는지 선택하여 해당 특성이 판매자에 의해 이행되는지 또는 Amazon에 의해 이행되는지 확인합니다. 선택하면 **[!UICONTROL Fulfilled by Attribute]**&#x200B;이(가) 활성화됩니다.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 이행 방법을 결정하는 데 사용되는 [!DNL Commerce] 특성을 선택합니다.<br><br>예를 들어 특성이 _이행자_&#x200B;이고 특성 값을 `Fulfilled By Merchant` 또는 `Fulfilled By Amazon (FBA)`(으)로 선택한 경우, 시스템은 해당 값을 새 제품에 대한 이행 유형으로 사용합니다. 판매자의 경우 [!DNL Amazon Seller Central] 계정 내에서 제품이 FBA 이행에 적합한지 확인해야 합니다. 또한 FBA 재고는 Amazon 판매자 계정을 통해 직접 관리됩니다.<br><br>옵션은 Amazon 제품에 대해 설정한 특성에 따라 다릅니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
