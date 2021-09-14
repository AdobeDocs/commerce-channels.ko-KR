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

_[!UICONTROL Fulfilled By]_설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스합니다.

이러한 설정은 주문 충족을 수행하는(또는 출하) 당사자를 정의합니다. 하나의 방법을 사용하여 모든 주문이 이행되는 경우 머천트(사용자) 또는 Amazon 중에서 선택합니다. 위치를 통해 주문을 이행하고 Amazon을 사용할 계획이라면, 세 번째 옵션을 사용하고 [!DNL Commerce] 제품 속성을 구성하는 것이 가장 좋습니다.

- **[!UICONTROL Fulfilled by Merchant]** - 상인이 모든 주문을 이행한다면 선택합니다. 주문이 제출되면 재고가 [!DNL Commerce] 카탈로그에서 제외됩니다.

- **[!UICONTROL Fulfilled by Amazon]** - Amazon이 모든 주문을 충족하는지 선택합니다. 이 옵션을 사용하면 주문이 이행될 때 [!DNL Commerce] 카탈로그에서 제품 인벤토리를 빼지 않습니다. Amazon 이행 주문에 대한 재고 재고가 저장되고 창고에서 제외됩니다. 이 옵션을 할당하기 전에 [!DNL Amazon Seller Central] 계정에서 제품이 _Amazon에 의해 처리됨_(FBA) 충족에 적합한지 확인해야 합니다. FBA 인벤토리는 [!DNL Amazon Seller Central] 계정을 통해 직접 관리됩니다. 이 이행 방법을 사용하면 Amazon 판매 채널은 [!DNL Commerce] 과 Amazon 간에 수량 업데이트를 공유하지 않습니다. 따라서 Amazon 판매 채널에서 수량 설정에 설명된 모든 마케팅 도구를 사용할 수는 없습니다.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 사용자 제품이 사용자 및 Amazon에 의해 이행될 수 있는 경우, 머천트별  [!DNL Commerce] 이행됨 및 Amazon에 의한 이행됨 값을 사용하여 제품 속성을 만들 수 있습니다. 제품당 이 값을 설정하면 주문이 이행되는 사람이 표시됩니다.

이행 방법은 지역 속성이며 [스토어 통합](./store-integration.md) 중에 정의된 **[!UICONTROL Amazon Marketplace Country]** 설정을 기반으로 합니다. 변경 사항이 적용되면, 변경 사항은 Amazon에서 [!DNL Amazon Seller SKU]을 공유하는 모든 Amazon 목록에 영향을 미칩니다. ([스토어 통합](./store-integration.md) 중에 _[!UICONTROL Amazon Marketplace Country]_에 정의된 대로) 동일한 지역에서 판매됩니다. 미국에서 공유 [!DNL Amazon Seller SKU]에 대한 변경 사항은 다른 지역(스토어 통합 중에 정의된 대로)에 설정된 Amazon 스토어에 영향을 주지 않습니다.

>[!NOTE]
>
>Amazon(FBA)에 의해 주문이 이행되고 순서를 가져오는 경우 주문 세부 사항에 일부 필드에 대한 더미 데이터를 볼 수 있습니다. [Amazon 주문 세부 사항](./amazon-order-details.md)을 참조하십시오.

## [!UICONTROL Fulfilled By] 설정 구성 {#configure-fulfilled-by-settings}

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. _[!UICONTROL Fulfilled By]_섹션을 확장합니다.

1. **[!UICONTROL Product Fulfilled By]**&#x200B;에 대해 명령을 이행하는 사람(출하)을 선택합니다.

   - `Fulfilled by Merchant` - 상인은 주문 완료

   - `Fulfilled by Amazon` - Amazon 웨어하우스 주문 이행

   - `Assign Fulfilled By Using Magento Product Attribute` -  [!DNL Commerce] 속성은 제품당 주문을 이행하는 사용자를 나타냅니다.

      선택한 경우 **[!UICONTROL Fulfilled by Attribute]**&#x200B;에 매핑할 [!DNL Commerce] 속성을 선택합니다.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![설정별](assets/amazon-fulfilled-by.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 옵션:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) 주문을 이행하는지 선택합니다. 주문이 제출되면 재고가 [!DNL Commerce] 카탈로그에서 제외됩니다. 신규 제품이 생성되면 Merchant Actured의 이행 방법이 지정됩니다.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Amazon이 주문을 이행하는지 선택합니다. 이 이행 방법을 사용하면 주문이 이행될 때 [!DNL Commerce] 카탈로그에서 제품 재고가 공제되지 않습니다. 제품을 만들 때 이행 유형으로 _[!UICONTROL Fulfilled by Amazon (FBA)]_을 사용하여 만들어집니다. 제품이 [!DNL Amazon Seller Central] 계정 내에서 FBA 이행을 받을 수 있는지 확인합니다. FBA 인벤토리는 [!DNL Amazon Seller Central] 계정을 통해 직접 관리됩니다. 이 이행 방법을 사용하면 수량 업데이트가 [!DNL Commerce] 카탈로그에 대해 푸시되지 않으므로 [재고/수량 설정](./stock-quantity.md)에 설명된 마케팅 도구 중 일부를 사용할 수 없습니다.</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - 상인에 의해  [!DNL Commerce] 이행되는지 또는 Amazon에 의해 이행되는지를 결정하는 기존 속성이 있는 경우 선택합니다. 이 옵션을 선택하면 **[!UICONTROL Fulfilled by Attribute]**&#x200B;이 활성화됩니다.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 이행 방법을 결정하는 데 사용되는 [!DNL Commerce] 속성을 선택합니다.<br><br>예를 들어 속성이  _이행_ 부산이고 속성 값을  _[!UICONTROL Fulfilled By Merchant]_또는_[!UICONTROL Fulfilled By Amazon (FBA)]_&#x200B;로 선택하는 경우, 시스템은 해당 값을 새 제품의 이행 유형으로 사용합니다. 머천트로서, 제품이 [!DNL Amazon Seller Central] 계정 내에서 FBA 이행을 받을 수 있는지 확인해야 합니다. FBA 재고는 Amazon 판매자 계정을 통해 직접 관리됩니다.<br><br>옵션은 Amazon 제품에 대해 설정한 속성에 따라 다릅니다. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
