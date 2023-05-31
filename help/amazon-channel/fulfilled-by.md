---
title: Amazon 목록에 대한 이행자 설정
description: 이행자 설정을 사용하여 Amazon 목록의 주문이 이행(출하)되는 방법을 결정합니다.
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Amazon 목록에 대한 이행자 설정

_[!UICONTROL Fulfilled By]_설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 주문을 이행(또는 배송)하는 당사자를 정의합니다. 모든 주문이 한 가지 방법으로 이행된 경우 판매자(사용자) 또는 Amazon 중에서 선택합니다. 위치에서 주문을 이행하고 Amazon을 사용할 계획이라면 세 번째 옵션을 사용하고 을 구성하는 것이 좋습니다. [!DNL Commerce] 제품 특성입니다.

- **[!UICONTROL Fulfilled by Merchant]** - 판매자인 귀하가 모든 주문을 이행할 경우 선택합니다. 주문이 이루어지면, 재고는 [!DNL Commerce] 카탈로그.

- **[!UICONTROL Fulfilled by Amazon]** - Amazon이 모든 주문을 충족하는지 여부를 선택합니다. 이 옵션을 사용하면 제품 재고가 [!DNL Commerce] 카탈로그(주문이 있을 경우). Amazon 이행 주문의 재고 재고는 해당 창고에서 저장되고 공제됩니다. 이 옵션을 할당하기 전에 [!DNL Amazon Seller Central] 제품이 적합한 계정 _Amazon에 의해 이행됨_ (FBA) 이행. FBA 인벤토리는 다음을 통해 직접 관리됩니다 [!DNL Amazon Seller Central] 계정. 이 이행 방법을 사용하면 Amazon 판매 채널은 다음 기간 동안 수량 업데이트를 공유하지 않습니다. [!DNL Commerce] 그리고 Amazon. 따라서 Amazon 판매 채널에서 수량 설정에 설명된 모든 마케팅 도구를 사용할 수 있는 것은 아닙니다.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 귀하와 Amazon이 제품을 이행할 수 있는 경우 다음을 만들 수 있습니다. [!DNL Commerce] 판매자가 이행하고 Amazon이 이행한 값이 있는 제품 속성. 제품당 이 값을 설정하면 누가 주문을 이행하는지 나타냅니다.

이행 방법은 지역 속성이며 다음을 기반으로 합니다. **[!UICONTROL Amazon Marketplace Country]** 설정 정의 기간 [스토어 통합](./store-integration.md). 변경 사항이 적용되면 해당 변경 사항은 해당 사항을 공유하는 모든 Amazon 목록에 영향을 줍니다 [!DNL Amazon Seller SKU] 에서 정의된대로 동일한 지역에서 판매되는 Amazon 스토어에서 _[!UICONTROL Amazon Marketplace Country]_다음 기간 동안 [스토어 통합](./store-integration.md)). 공유에 대한 변경 [!DNL Amazon Seller SKU] 미국에서는 다른 지역에 대해 설정된 Amazon 스토어에 영향을 주지 않습니다(스토어 통합 중에 정의됨).

>[!NOTE]
>
>FBA(Amazon)에서 주문을 이행하고 주문을 가져오면 주문 세부 정보에서 일부 필드에 대한 더미 데이터를 볼 수 있습니다. 다음을 참조하십시오 [Amazon 주문 세부 사항](./amazon-order-details.md).

## 구성 [!UICONTROL Fulfilled By] 설정 {#configure-fulfilled-by-settings}

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 _[!UICONTROL Fulfilled By]_섹션.

1. 대상 **[!UICONTROL Product Fulfilled By]**, 주문을 이행(배송)할 사용자 선택:

   - `Fulfilled by Merchant` - 상인이 질서를 지킨다.

   - `Fulfilled by Amazon` - Amazon 웨어하우스가 주문을 처리합니다.

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] 속성은 제품당 주문을 이행하는 사용자를 나타냅니다.

      선택한 경우 다음을 선택합니다. [!DNL Commerce] 매핑할 속성 **[!UICONTROL Fulfilled by Attribute]**.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![이행한 사람 설정](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 옵션:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) 주문을 이행할 경우 선택합니다. 주문이 이루어지면, 재고는 [!DNL Commerce] 카탈로그. 새 제품이 생성되면 이행된 머천트의 이행 방법이 지정됩니다.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Amazon이 주문을 이행하는지 여부를 선택합니다. 이 이행 방법을 사용하면 제품 재고가 [!DNL Commerce] 카탈로그(주문이 있을 경우). 제품이 만들어지면 _[!UICONTROL Fulfilled by Amazon (FBA)]_이행 유형으로 사용됩니다. 내 제품에서 FBA 이행 대상이 되는지 확인합니다. [!DNL Amazon Seller Central] 계정입니다. 또한 FBA 인벤토리는 다음을 통해 직접 관리됩니다. [!DNL Amazon Seller Central] 계정입니다. 이 이행 방법을 사용하면 수량 업데이트가 [!DNL Commerce] 카탈로그에는에 설명된 일부 마케팅 도구를 사용할 수 없습니다. [재고 / 수량 설정](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 기존 항목이 있는 경우 선택 [!DNL Commerce] 판매자가 이행했는지 또는 Amazon이 이행했는지를 결정하는 속성입니다. 선택하면, **[!UICONTROL Fulfilled by Attribute]** 을(를) 활성화합니다.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 다음을 선택합니다. [!DNL Commerce] 이행 방법을 결정하는 데 사용되는 속성입니다.<br><br>예를 들어 속성이 _이행한 사람_ 속성 값을 다음과 같이 선택합니다. `Fulfilled By Merchant` 또는 `Fulfilled By Amazon (FBA)`를 입력하면 시스템은 해당 값을 새 제품에 대한 이행 유형으로 사용합니다. 판매자로서, 귀하는 귀하의 제품이 귀하의 제품 내에서 FBA 이행에 적합한지 확인해야 합니다 [!DNL Amazon Seller Central] 계정입니다. 또한 FBA 재고는 Amazon 판매자 계정을 통해 직접 관리됩니다.<br><br>옵션은 Amazon 제품에 대해 설정한 속성에 따라 다릅니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
