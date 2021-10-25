---
title: 주식/수량
description: 전자 상거래 저장소에서 사용자 [!DNL Amazon Seller Central] 계정에서 재고/수량 설정을 업데이트합니다.
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 주식/수량

*[!UICONTROL Stock/Quantity]* 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 제품 수량 세부 사항을 [!DNL Commerce] 주문품의 수량에 대해 저장 [!DNL Amazon Seller Central] 계정이 필요합니다. 이 도구는 강력하며 인벤토리를 정리하는 동안 구매자에게 긴급성을 표시하여 추가 광고에 사용할 수 있습니다. 예를 들어, 일부 상인들은 창고에 있는 특정 SKU의 150개 항목을 가지고 있고 Amazon 구매자들이 모든 인벤토리를 구매할 수 있는지 확인하려고 할 수 있습니다. 다른 상인들은 한 번에 한 항목만 나열하여 최종 사용자에게 희소성을 줄 수 있습니다. 이 경우 *[!UICONTROL Maximum Listed Quantity]* to `1`.

수량은 지역 속성이며 **[!UICONTROL Amazon Marketplace Country]** 설정 [스토어 통합](./store-integration.md). 제품 수량이 변경되면 해당 제품 및 쿠키를 공유하는 모든 Amazon 목록에 영향을 줍니다 [!DNL Amazon Seller SKU] Amazon에서 동일한 국가에서 판매되는 매장에 해당 코드가 포함되어 있습니다. 공유로 변경 [!DNL Amazon Seller SKU] 미국에서는 다른 국가에 맞게 설정된 Amazon 스토어에 영향을 주지 않습니다. 통합된 첫 번째 Amazon 저장소는(가장 오래된 만들기 날짜와 함께) 수량 설정에서 우선순위를 제어합니다.

>[!NOTE]
>
>Adobe Commerce 및 Magento Open Source 2.3.x 사용자의 경우 Amazon 판매 채널은 추가 설정 없이 인벤토리 관리 확장 기능을 사용할 수 있습니다. 자세한 내용은 [인벤토리 관리](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target=&quot;_blank&quot;}.

## 재고/수량 설정 구성 {#configure-stock--quantity-settings}

1. 클릭 **[!UICONTROL Listing Settings]** 저장 대시보드에서

1. 를 확장합니다. **[!UICONTROL Stock / Quantity]** 섹션을 참조하십시오.

1. 대상 **[!UICONTROL Out-of-Stock Threshold]** (필수) 제품을 Amazon 목록에 사용할 수 있도록 하려면 제품의 최저 수량에 대한 숫자 값을 입력합니다.

   기본값은 입니다. `0`. 만약 [!DNL Commerce] 제품 재고가 이 수보다 낮으면 각 Amazon 목록은 Amazon을 통해 판매할 수 없습니다.

1. 대상 **[!UICONTROL Maximum Listed Quantity]** (필수) Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.

   이 설정은 입력한 값에 사용 가능한 모든 Amazon 목록을 표시합니다. 품목이 판매되면 Amazon 목록 수량이 변경되지 않습니다. 사용 가능한 목록 수량은 실제 제품 수량이 높거나 낮은 경우에도 항상 이 값을 사용합니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다. 예를 들어, 제품 내에 수량이 80인 제품이 있을 수 있습니다 [!DNL Commerce] 카탈로그 을 로 설정하고 `10`, Amazon 목록에는 항상 사용 가능한 수량이 표시됩니다. `10` 그리고 제품에 대한 판매가 있을 때는 변경되지 않습니다.

1. 대상 **[!UICONTROL "Do Not Manage Stock" Quantity]** (필수) Amazon 목록에 표시할 수량 값을 입력합니다.

   Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 대상 [!DNL Commerce] 재고 관리를 하도록 설정되어 있지 않지만 Amazon에 나열하려는 제품 목록에 여기에 입력한 사용 가능한 수량이 있는 제품이 게시됩니다.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save listing settings]**.

![주식/수량 설정](assets/amazon-stock-quantity.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | 제품을 Amazon 목록에 사용할 수 있도록 하려면 제품의 최저 수량에 대한 숫자 값을 입력합니다(기본값은 임) `0`).<br><br>만약 [!DNL Commerce] 제품 재고가 이 수보다 낮으면 각 Amazon 목록은 Amazon을 통해 판매할 수 없습니다. |
| [!UICONTROL Maximum Listed Quantity] | Amazon 목록에 표시할 수량에 대한 숫자 값을 입력합니다.<br><br>품목이 판매되면 Amazon 목록은 여기에 입력한 수량을 사용하여 다시 게시합니다. 이 설정은 일반적으로 제품 인벤토리를 관리하지 않을 때 사용됩니다.<br><br>예를 들어 다음과 같이 나열된 최대 수량 값을 입력합니다 `10`. 제품의 실제 수량은 다음과 같습니다 `80`. 이 값을 로 설정했으므로 `10`, Amazon 목록에는 항상 사용 가능한 수량이 표시됩니다. `10`. 재고 수량이 낮더라도 사용 가능한 수량은 항상 정의된 값과 함께 표시됩니다. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Amazon 목록의 표시 수량 값을 입력합니다.<br><br>Amazon을 사용하려면 사용 가능한 수량을 게시해야 합니다. 대상 [!DNL Commerce] 재고 관리를 하도록 설정되어 있지 않지만 Amazon에 나열하려는 제품 목록에 여기에 입력한 값의 사용 가능한 수량이 있는 제품이 게시됩니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## 예: 최대 나열된 수량

품목이 판매되면 Amazon이 이 수량으로 품목을 판매합니다.

예를 들어 *[!UICONTROL Maximum Listed Quantity]* 로서의 `12`로 지정하는 경우 Amazon 목록에는 제품에 가 있더라도 12개의 수량이 표시됩니다 [!DNL Commerce] 80 수량:

![최대 나열된 수량 예 1](assets/amazon-max-listed-quantity.png)

을 설정하는 경우 *[!UICONTROL Maximum Listed Quantity]* 로서의 `1`를 입력하면 가능한 모든 제품이 `1`. 제품이 판매되면 시스템이 [!DNL Commerce] 제품 및 추가 재고가 있는 경우 수량 `1`.

이 옵션은 일반적으로 수량이 1인 제품에 유용할 수 있습니다. 또한 Amazon 목록을 볼 때 구매자의 긴급성을 높입니다.

![최대 나열된 수량 예 2](assets/amazon-max-listed-quantity-1.png)
