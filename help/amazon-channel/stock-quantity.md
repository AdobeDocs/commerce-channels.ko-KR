---
title: 재고/수량
description: Commerce 스토어의 제품 수량 세부 정보의 동기화를 제어하려면 [!DNL Amazon Seller Central] 계정, 재고/수량 설정을 갱신합니다.
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# 재고/수량

*[!UICONTROL Stock/Quantity]* 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이 설정은 의 제품 수량 세부 정보를 동기화하는 데 사용됩니다. [!DNL Commerce] 상점에서 고객의 수량을 검색합니다 [!DNL Amazon Seller Central] 계정입니다. 이 도구는 강력하고 인벤토리를 정리하는 동안 구매자에게 긴급도를 표시하여 추가 광고에 사용할 수 있습니다. 예를 들어, 일부 판매자는 창고에 특정 SKU의 150개 품목이 재고에 있을 수 있으며 Amazon 구매자가 모든 재고를 구매할 수 있도록 하고자 할 수 있습니다. 다른 판매자는 최종 사용자에게 희소성을 생성하기 위해 한 번에 하나의 품목만 나열하기를 원할 수 있다. 이 경우 다음을 설정합니다. *[!UICONTROL Maximum Listed Quantity]* 끝 `1`.

수량은 지역 속성이며 **[!UICONTROL Amazon Marketplace Country]** 다음 기간 동안 정의 설정 [스토어 통합](./store-integration.md). 제품의 수량이 변경되면 해당 수량을 공유하는 모든 Amazon 목록에 변경 사항이 적용됩니다 [!DNL Amazon Seller SKU] 동일한 국가에서 판매되는 Amazon 스토어에서. 공유에 대한 변경 [!DNL Amazon Seller SKU] 미국에서는 다른 국가에 설정된 Amazon 스토어에 영향을 주지 않습니다. 가장 오래된 생성 날짜를 사용하여 통합된 첫 번째 Amazon 저장소가 수량 설정에서 우선순위를 제어합니다.

>[!NOTE]
>
>Adobe Commerce 및 Magento Open Source 2.3.x 사용자의 경우 Amazon 판매 채널은 추가 설정 없이 Inventory management 확장 사용을 지원합니다. 다음을 참조하십시오 [재고 관리](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}.

## 재고/수량 설정 구성 {#configure-stock--quantity-settings}

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 **[!UICONTROL Stock / Quantity]** 섹션.

1. 대상 **[!UICONTROL Out-of-Stock Threshold]** (필수) Amazon 목록에 적합한 제품을 유지하기 위해 제품의 가장 낮은 수량에 대한 숫자 값을 입력합니다.

   기본값은 입니다 `0`. 다음의 경우 [!DNL Commerce] 제품 재고가 이 숫자보다 낮으면 해당 Amazon 목록은 Amazon을 통한 판매에 부적합합니다.

1. 대상 **[!UICONTROL Maximum Listed Quantity]** (필수) Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.

   이 설정은 입력한 값으로 적격한 모든 Amazon 목록을 나열합니다. 품목이 판매될 때 Amazon 목록 수량은 변경되지 않습니다. 실제 제품 수량이 더 많거나 더 적은 경우에도 사용 가능한 목록 수량은 항상 이 값을 사용합니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다. 예를 들어, 에 수량이 80인 제품이 있을 수 있습니다 [!DNL Commerce] 카탈로그. 을 로 설정 `10`, Amazon 목록에는 항상 사용 가능한 수량이 표시됩니다. `10` 제품에 대한 판매가 이루어질 때 및 는 변경되지 않습니다.

1. 대상 **[!UICONTROL "Do Not Manage Stock" Quantity]** (필수) Amazon 목록에 표시할 수량 값을 입력합니다.

   Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 대상 [!DNL Commerce] 재고를 관리하지 않도록 설정되었지만 Amazon에 나열하려는 제품은 여기에 입력된 사용 가능한 수량과 함께 목록이 게시됩니다.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![재고/수량 설정](assets/amazon-stock-quantity.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Amazon 목록에 적합한 제품을 유지하기 위해 제품의 최저 수량에 대한 숫자 값을 입력합니다(기본값: `0`).<br><br>다음의 경우 [!DNL Commerce] 제품 재고가 이 숫자보다 낮으면 해당 Amazon 목록은 Amazon을 통한 판매에 부적합합니다. |
| [!UICONTROL Maximum Listed Quantity] | Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.<br><br>품목이 판매되면 Amazon 목록은 여기에 입력한 수량과 함께 다시 게시됩니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다.<br><br>예를 들어, 최대 목록 수량 값을 다음과 같이 입력합니다. `10`. 제품에 대한 실제 수량은 다음과 같습니다. `80`. 이 값을 로 설정했기 때문입니다. `10`, Amazon 목록에는 항상 사용 가능한 수량이 표시됩니다. `10`. 재고 수량이 적은 경우에도 사용 가능한 수량은 항상 정의된 값으로 표시됩니다. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Amazon 목록의 표시 수량 값을 입력합니다.<br><br>Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 대상 [!DNL Commerce] 재고를 관리하지 않도록 설정되어 있지만 Amazon에 나열하려는 제품은 여기에 입력한 값의 사용 가능한 수량과 함께 목록이 게시됩니다. |

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

예를 들어, *[!UICONTROL Maximum Listed Quantity]* 다음으로: `12`, 제품에 가 있더라도 Amazon 목록에는 수량이 12로 표시됩니다. [!DNL Commerce] 수량 80:

![최대 목록 수량 예 1](assets/amazon-max-listed-quantity.png)

다음을 설정하는 경우 *[!UICONTROL Maximum Listed Quantity]* 다음으로: `1`, 모든 적격 제품이 수량으로 나열됩니다. `1`. 품목이 판매되면 시스템은 [!DNL Commerce] 제품 및 추가 재고가 있는 경우 수량이 인 Amazon에 품목을 재판매합니다. `1`.

이 옵션은 일반적으로 1개 수량으로 주문하는 제품에 유용할 수 있습니다. 또한 Amazon 목록을 볼 때 쇼핑객의 긴급도가 증가합니다.

![최대 목록 수량 예 2](assets/amazon-max-listed-quantity-1.png)
