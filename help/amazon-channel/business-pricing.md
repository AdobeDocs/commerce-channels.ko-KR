---
title: (B2B) 영업가격
description: 다음을 나열할 수 있습니다. [!DNL Commerce] Amazon에서 비즈니스를 활성화하여 Amazon 비즈니스(B2B) 사이트에 제품을 저장합니다 [!DNL Seller Central] 계정입니다.
redirect_from: /sales-channels/asc/ob-business-pricing.html
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# (B2B) 영업가격

(B2B) 비즈니스 가격 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

[!DNL Amazon Business] 은(는) Amazon 등록 비즈니스 계정에만 해당하는 마켓플레이스이며 미국, 프랑스, 독일 및 영국에서만 사용할 수 있습니다. 마켓플레이스에서 B2B 비즈니스 가격을 허용하는 경우 목록 설정 내에서 편집할 수 있습니다.

[!DNL B2B Business Pricing] 비즈니스 계정이 있는 상인이 Amazon 쇼핑 경험의 예상 성과로 서로 구매할 수 있습니다. B2B 비즈니스 가격을 통해 기업은 구매 수량에 따라 계층화된 가격을 제공할 수 있습니다.

에 제품을 나열하려면 [!DNL Amazon Business (B2B)] 사이트, 먼저 [!DNL Amazon Seller Central] 계정입니다. B2B 기능에 대한 자세한 내용은 [Amazon: B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"} (판매자 중앙 로그인 필요).

## (B2B) 비즈니스 가격 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 _[!UICONTROL (B2B) Business Price]_섹션.

1. 대상 **[!UICONTROL Enable Business Pricing]**&#x200B;옵션을 선택합니다.

   - `Disabled` - (기본값) B2B 판매를 사용하지 않으려는 시기를 선택합니다. 선택하면 이 섹션의 다른 모든 필드가 비활성화됩니다.

   - `Enabled` - B2B(Business-to-Business) 판매를 활성화할 시기를 선택합니다. 활성화되면 모든 가격책정 규칙이 적용된 후 비즈니스 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 $1보다 작을 수 없습니다.

1. 대상 **[!UICONTROL Enable Tiered Pricing]**&#x200B;옵션을 선택합니다.

   - `Disabled` - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 경우 선택합니다. 선택 시 모두 _[!UICONTROL Pricing Level]_이 섹션의 필드는 비활성화되어 있습니다.

   - `Enabled` - 주문 수량을 기준으로 가격책정 조정을 사용가능으로 설정할 시기를 선택합니다. 이 옵션을 선택하면 _[!UICONTROL Pricing Level]_필드가 활성화되어 있습니다.

1. 다음을 완료합니다. **[!UICONTROL Pricing Level]** 설정.

   비즈니스 목록에 대해 계층 가격을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어, `5` 첫 번째 행의 첫 번째 필드에서 `5` 두 번째 필드에서는 다른 사업자가 5개 이상 물량을 구매할 경우 5% 할인이 적용된다.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![Amazon Business Pricing(B2B)](assets/amazon-business-pricing.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Enable Business Pricing] | 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) Business To Business Sales를 사용하지 않으려면 선택합니다. 이 옵션을 선택하면 이 섹션의 다른 모든 필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - Business to Business Sales를 활성화하고자 할 때 선택합니다. 이 옵션을 선택하면 모든 가격 책정 규칙이 적용된 후 비즈니스 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 $1보다 작을 수 없습니다.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (필수) 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 경우 선택합니다. 선택 시 모두 _[!UICONTROL Pricing Level]_이 섹션의 필드는 비활성화되어 있습니다.</li><li>**[!UICONTROL Enabled]** - 주문 수량에 따라 조정되는 가격책정을 사용할지 선택합니다. 이 옵션을 선택하면 _[!UICONTROL Pricing Level]_필드가 활성화되어 있습니다.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | 계층형 가격책정이 활성화되면 비즈니스 목록에 대한 계층 가격책정을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어, `5` 첫 번째 행의 첫 번째 필드에서 `5` 두 번째 필드에서는 다른 사업자가 5개 이상 물량을 구매할 경우 5% 할인이 적용된다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
