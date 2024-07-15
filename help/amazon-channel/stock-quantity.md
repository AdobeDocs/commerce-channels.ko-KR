---
title: Amazon Sales Channel - [!UICONTROL Stock/Quantity]
description: Commerce 스토어에서  [!DNL Amazon Seller Central]  계정으로의 제품 수량 세부 정보의 동기화를 제어하려면 재고/수량 설정을 업데이트하십시오.
feature: Sales Channels, Inventory
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# [!UICONTROL Stock/Quantity]

*[!UICONTROL Stock/Quantity]* 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

이러한 설정은 [!DNL Commerce] 상점 앞에서의 제품 수량 세부 정보를 [!DNL Amazon Seller Central] 계정의 수량과 동기화하는 데 사용됩니다. 이 도구는 강력하고 인벤토리를 정리하는 동안 구매자에게 긴급도를 표시하여 추가 광고에 사용할 수 있습니다. 예를 들어, 일부 판매자는 창고에 특정 SKU의 150개 품목이 재고에 있을 수 있으며 Amazon 구매자가 모든 재고를 구매할 수 있도록 하고자 할 수 있습니다. 다른 판매자는 최종 사용자에게 희소성을 생성하기 위해 한 번에 하나의 품목만 나열하기를 원할 수 있다. 이 경우 *[!UICONTROL Maximum Listed Quantity]*&#x200B;을(를) `1`(으)로 설정합니다.

수량은 지역 특성이며 [스토어 통합](./store-integration.md) 중에 정의된 **[!UICONTROL Amazon Marketplace Country]** 설정을 기반으로 합니다. 제품의 수량이 변경되면 변경 사항은 같은 국가에서 판매하는 Amazon 스토어에서 해당 [!DNL Amazon Seller SKU]을(를) 공유하는 모든 Amazon 목록에 영향을 줍니다. 미국에서 공유된 [!DNL Amazon Seller SKU]을(를) 변경해도 다른 국가에 대해 설정된 Amazon 스토어에 영향을 주지 않습니다. 가장 오래된 생성 날짜를 사용하여 통합된 첫 번째 Amazon 저장소가 수량 설정에서 우선순위를 제어합니다.

>[!NOTE]
>
>Adobe Commerce 및 Magento Open Source 2.3.x 사용자의 경우 Amazon 판매 채널은 추가 설정 없이 Inventory management 확장 사용을 지원합니다. [인벤토리 관리](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}를 참조하세요.

## 재고/수량 설정 구성 {#configure-stock--quantity-settings}

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Stock / Quantity]** 섹션을 확장합니다.

1. **[!UICONTROL Out-of-Stock Threshold]**(필수)의 경우 Amazon 목록에 적합한 제품을 유지하기 위해 제품의 가장 낮은 수량에 대한 숫자 값을 입력합니다.

   기본값은 `0`입니다. [!DNL Commerce] 제품 재고가 이 숫자보다 낮은 경우 해당 Amazon 목록은 Amazon을 통한 판매에 부적합합니다.

1. **[!UICONTROL Maximum Listed Quantity]**(필수)의 경우 Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.

   이 설정은 입력한 값으로 적격한 모든 Amazon 목록을 나열합니다. 품목이 판매될 때 Amazon 목록 수량은 변경되지 않습니다. 실제 제품 수량이 더 많거나 더 적은 경우에도 사용 가능한 목록 수량은 항상 이 값을 사용합니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다. 예를 들어, [!DNL Commerce] 카탈로그에 수량이 80인 제품이 있을 수 있습니다. `10`(으)로 설정된 Amazon 목록에는 항상 `10` 사용 가능한 수량이 표시되며 제품에 대한 판매가 이루어질 때 변경되지 않습니다.

1. **[!UICONTROL "Do Not Manage Stock" Quantity]**(필수)에 Amazon 목록에 표시할 수량 값을 입력하십시오.

   Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 재고를 관리하지 않도록 설정되었지만 Amazon에 나열하려는 [!DNL Commerce] 제품의 경우 여기에 입력된 사용 가능한 수량으로 목록이 게시됩니다.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![재고/수량 설정](assets/amazon-stock-quantity.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Out-of-Stock Threshold] | Amazon 목록에 적합한 제품을 유지하기 위해 제품의 가장 낮은 수량에 대한 숫자 값을 입력하십시오(기본값: `0`).<br><br>제품 재고 [!DNL Commerce]이(가) 이 숫자보다 낮은 경우 해당 Amazon 목록은 Amazon을 통한 판매에 적합하지 않습니다. |
| [!UICONTROL Maximum Listed Quantity] | Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.<br><br>항목을 판매하면 Amazon 목록이 여기에 입력한 수량으로 다시 게시됩니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다.<br><br>예를 들어 최대 목록 수량 값을 `10`(으)로 입력합니다. 제품에 대한 실제 수량은 `80`입니다. 이 값을 `10`로 설정했으므로 Amazon 목록에는 항상 `10`의 사용 가능한 수량이 표시됩니다. 재고 수량이 적은 경우에도 사용 가능한 수량은 항상 정의된 값으로 표시됩니다. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Amazon 목록의 표시 수량 값을 입력합니다.<br><br>Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 재고를 관리하지 않도록 설정되었지만 Amazon에 나열하려는 [!DNL Commerce] 제품의 경우 여기에 입력한 값의 사용 가능한 수량으로 목록이 게시됩니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## 예: 최대 목록 수량

품목이 판매되면 Amazon 목록은 이 수량으로 재판매합니다.

예를 들어 *[!UICONTROL Maximum Listed Quantity]*&#x200B;을(를) `12`(으)로 설정하면 제품의 [!DNL Commerce] 수량이 80인데도 Amazon 목록에 12개의 수량이 표시됩니다.

![최대 목록 수량 예 1](assets/amazon-max-listed-quantity.png){width="300"}

*[!UICONTROL Maximum Listed Quantity]*&#x200B;을(를) `1`(으)로 설정하면 모든 적격 제품이 `1` 수량으로 나열됩니다. 항목이 판매되면 시스템은 사용자의 [!DNL Commerce] 제품을 확인하고, 재고가 더 있는 경우 수량을 `1`로 하여 Amazon에서 항목을 재설정합니다.

이 옵션은 일반적으로 1개 수량으로 주문하는 제품에 유용할 수 있습니다. 또한 Amazon 목록을 볼 때 쇼핑객의 긴급도가 증가합니다.

![최대 목록 수량 예 2](assets/amazon-max-listed-quantity-1.png){width="300"}
