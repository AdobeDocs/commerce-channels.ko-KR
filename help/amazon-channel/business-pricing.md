---
title: (B2B) 비즈니스 가격
description: ' [!DNL Commerce] store products on the Amazon Business (B2B) site by enabling business in your Amazon [!DNL Seller Central] 계정을 나열할 수 있습니다.'
redirect_from: /sales-channels/asc/ob-business-pricing.html: 
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 539
ht-degree: 0%

---

# (B2B) 비즈니스 가격

(B2B) 비즈니스 가격 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스합니다.

[!DNL Amazon Business] 는 Amazon 등록 비즈니스 계정에만 사용할 수 있는 시장이며, 미국, 프랑스, 독일 및 영국에서만 사용할 수 있습니다. 마켓플레이스에서 B2B 비즈니스 가격을 허용하는 경우 목록 설정 내에서 편집할 수 있습니다.

[!DNL B2B Business Pricing] 에서는 Amazon 쇼핑 경험의 예상 성과를 사용하여 비즈니스 계정이 있는 판매자가 서로 구매할 수 있습니다. B2B 비즈니스 가격을 통해 기업은 구매 수량에 따라 계층형 가격을 제공할 수 있습니다.

제품이 [!DNL Amazon Business (B2B)] 사이트에 나열되도록 하려면 먼저 [!DNL Amazon Seller Central] 계정에서 비즈니스를 활성화해야 합니다. B2B 기능에 대한 자세한 내용은 [Amazon 를 참조하십시오. B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target=&quot;_blank&quot;}(판매자 중앙 로그인 필요).

## (B2B) 비즈니스 가격 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. _[!UICONTROL (B2B) Business Price]_섹션을 확장합니다.

1. **[!UICONTROL Enable Business Pricing]**&#x200B;에 대해 옵션을 선택합니다.

   - `Disabled` - (기본값) B2B(Business-to-Business) 판매를 활성화하지 않을 시기를 선택합니다. 이 섹션의 다른 모든 필드는 선택한 경우 비활성화됩니다.

   - `Enabled` - Business-to-Business 판매 활성화 시점을 선택합니다. 사용 가능으로 설정하면 모든 가격책정 규칙이 적용된 후 업무 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 1달러 이상이어야 합니다.

1. **[!UICONTROL Enable Tiered Pricing]**&#x200B;에 대해 옵션을 선택합니다.

   - `Disabled` - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 시점을 선택합니다. 선택한 경우 이 섹션의 모든 _[!UICONTROL Pricing Level]_필드가 비활성화됩니다.

   - `Enabled` - 주문 수량에 따라 가격책정 조정을 사용할 시기를 선택합니다. 선택한 경우 _[!UICONTROL Pricing Level]_필드가 활성화됩니다.

1. **[!UICONTROL Pricing Level]** 설정을 완료합니다.

   비즈니스 목록에 대한 계층 가격을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어, 첫 번째 행의 첫 번째 필드에 `5` 를 입력하고 두 번째 필드에 `5`을 입력하면 다른 비즈니스가 5개 이상의 수량을 구매할 때 가격이 5% 할인을 적용합니다.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![Amazon 비즈니스 가격(B2B)](assets/amazon-business-pricing.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Enable Business Pricing] | 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) 비즈니스 영업에 비즈니스를 사용으로 설정하지 않을 시기를 선택합니다. 선택한 경우 이 섹션의 다른 모든 필드는 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - 비즈니스 판매 활성화 시점을 선택합니다. 선택한 경우, 모든 가격책정 규칙이 적용된 후 업무 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 1달러 이상이어야 합니다.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (필수) 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 시점을 선택합니다. 선택한 경우 이 섹션의 모든 _[!UICONTROL Pricing Level]_필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - 주문 수량에 따라 조정되는 가격을 사용하도록 설정할 시기를 선택합니다. 선택한 경우 _[!UICONTROL Pricing Level]_필드가 활성화됩니다.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | 계층화된 가격책정이 사용되면 비즈니스 목록의 계층 가격을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어, 첫 번째 행의 첫 번째 필드에 `5` 를 입력하고 두 번째 필드에 `5`을 입력하면 다른 비즈니스가 5개 이상의 수량을 구매할 때 가격이 5% 할인을 적용합니다. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
