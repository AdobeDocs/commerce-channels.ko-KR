---
title: 다음 기간 동안 이행
description: Amazon 목록의 주문이 이행되는(배송된) 방식을 결정하려면 이행 기준 설정을 사용하십시오.
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# 다음 기간 동안 이행

_[!UICONTROL Fulfilled By]_설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 주문 충족을 수행하는(또는 출하) 당사자를 정의합니다. 하나의 방법을 사용하여 모든 주문이 이행되는 경우 머천트(사용자) 또는 Amazon 중에서 선택합니다. 위치를 통해 주문을 이행하고 Amazon을 사용할 계획이라면, 세 번째 옵션을 사용하고 [!DNL Commerce] 제품 속성입니다.

- **[!UICONTROL Fulfilled by Merchant]** - 상인이 모든 주문을 이행한다면 선택합니다. 주문이 제출되면, 재고가 주문에서 제외됩니다 [!DNL Commerce] 카탈로그

- **[!UICONTROL Fulfilled by Amazon]** - Amazon이 모든 주문을 충족하는지 선택합니다. 이 옵션을 사용하면 제품 인벤토리가 [!DNL Commerce] 주문 시 카탈로그 Amazon 이행 주문에 대한 재고 재고가 저장되고 창고에서 제외됩니다. 이 옵션을 할당하기 전에 [!DNL Amazon Seller Central] 제품이 _Amazon의 기능_ (FBA) 이행. FBA 인벤토리는 [!DNL Amazon Seller Central] 계정. 이 이행 방법을 사용하면 Amazon 판매 채널은 두 채널 간에 수량 업데이트를 공유하지 않습니다 [!DNL Commerce] 및 Amazon. 따라서 Amazon 판매 채널에서 수량 설정에 설명된 모든 마케팅 도구를 사용할 수는 없습니다.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 귀하 및 Amazon이 귀하의 제품을 만족시킬 수 있는 경우, [!DNL Commerce] 머천트별 이행 및 Amazon에 의한 이행값 제품 속성. 제품당 이 값을 설정하면 주문이 이행되는 사람이 표시됩니다.

이행 방법은 지역 속성이며 **[!UICONTROL Amazon Marketplace Country]** 정의된 시간 설정 [스토어 통합](./store-integration.md). 변경이 수행되면 변경 사항은 해당 페이지를 공유하는 모든 Amazon 목록에 영향을 줍니다 [!DNL Amazon Seller SKU] Amazon에서 동일한 지역(에 정의된 대로)에 판매됩니다 _[!UICONTROL Amazon Marketplace Country]_기간 [스토어 통합](./store-integration.md)). 공유로 변경 [!DNL Amazon Seller SKU] 미국은 다른 지역(스토어 통합 중에 정의됨)에 대해 설정된 Amazon 스토어에 영향을 주지 않습니다.

>[!NOTE]
>
>Amazon(FBA)에 의해 주문이 이행되고 순서를 가져오는 경우 주문 세부 사항에 일부 필드에 대한 더미 데이터를 볼 수 있습니다. 자세한 내용은 [Amazon 주문 세부 사항](./amazon-order-details.md).

## 구성 [!UICONTROL Fulfilled By] 설정 {#configure-fulfilled-by-settings}

1. 클릭 **[!UICONTROL Listing Settings]** 저장 대시보드에서

1. 를 확장합니다. _[!UICONTROL Fulfilled By]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Product Fulfilled By]**&#x200B;를 선택하고 다음 명령을 이행하는 사용자를 선택합니다.

   - `Fulfilled by Merchant` - 상인은 주문 완료

   - `Fulfilled by Amazon` - Amazon 웨어하우스 주문 이행

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] 속성은 제품당 주문을 이행하는 사용자를 나타냅니다.

      선택한 경우 [!DNL Commerce] 매핑할 속성입니다. **[!UICONTROL Fulfilled by Attribute]**.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save listing settings]**.

![설정별](assets/amazon-fulfilled-by.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 옵션:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) 주문을 이행하는지 선택합니다. 주문이 제출되면, 재고가 주문에서 제외됩니다 [!DNL Commerce] 카탈로그 신규 제품이 생성되면 Merchant Actured의 이행 방법이 지정됩니다.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Amazon이 주문을 이행하는지 선택합니다. 이 이행 방법을 사용할 경우 제품 재고가 사용자 제품에서 제외됩니다 [!DNL Commerce] 주문 시 카탈로그 제품이 만들어지면 _[!UICONTROL Fulfilled by Amazon (FBA)]_를 이행 유형으로 사용합니다. 귀하의 제품이 귀하의 내에서 FBA 이행 자격이 있는지 확인하십시오 [!DNL Amazon Seller Central] 계정이 필요합니다. FBA 인벤토리는 또한 [!DNL Amazon Seller Central] 계정이 필요합니다. 이 이행 방법을 사용하면 수량 업데이트가 사용자의 [!DNL Commerce] 카탈로그이므로, [재고/수량 설정](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 기존 항목이 있는지 선택 [!DNL Commerce] 상인에 의해 이행되는지 또는 Amazon에 의해 이행되는지를 결정하는 속성입니다. 선택한 경우, **[!UICONTROL Fulfilled by Attribute]** 사용할 수 있습니다.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 을(를) 선택합니다 [!DNL Commerce] 이행 방법을 결정하는 데 사용되는 속성입니다.<br><br>예를 들어 속성이 _다음 기간 동안 이행_ 속성 값을 _[!UICONTROL Fulfilled By Merchant]_또는_[!UICONTROL Fulfilled By Amazon (FBA)]_&#x200B;를 지정하는 경우, 시스템은 해당 값을 새 제품의 이행 유형으로 사용합니다. 판매업체는 귀하의 제품이 [!DNL Amazon Seller Central] 계정이 필요합니다. FBA 재고는 Amazon 판매자 계정을 통해 직접 관리됩니다.<br><br>옵션은 Amazon 제품에 대해 설정한 속성에 따라 다릅니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
