---
title: "[!DNL (B2B) Business Price](Amazon 목록)"
description: Amazon [!DNL Seller Central] 계정에서 비즈니스를 활성화하여 Amazon 비즈니스(B2B) 사이트에  [!DNL Commerce] 스토어 제품을 나열할 수 있습니다.
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Amazon 목록 [!DNL (B2B) Business Price]

(B2B) 비즈니스 가격 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [Amazon 스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

[!DNL Amazon Business]은(는) Amazon 등록 비즈니스 계정만 사용할 수 있는 마켓플레이스이며 미국, 프랑스, 독일 및 영국에서만 사용할 수 있습니다. 마켓플레이스에서 B2B 비즈니스 가격을 허용하는 경우 목록 설정 내에서 편집할 수 있습니다.

[!DNL B2B Business Pricing]을(를) 사용하면 비즈니스 계정이 있는 판매자가 Amazon 쇼핑 환경의 예상 성능으로 서로 구매할 수 있습니다. B2B 비즈니스 가격을 통해 기업은 구매 수량에 따라 계층화된 가격을 제공할 수 있습니다.

제품을 [!DNL Amazon Business (B2B)] 사이트에 나열하려면 먼저 [!DNL Amazon Seller Central] 계정에서 비즈니스를 사용하도록 설정해야 합니다. B2B 기능에 대한 자세한 내용은 [Amazon: B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"}을 참조하십시오(Seller Central 로그인 필요).

## [!DNL (B2B) Business Price] 설정 구성

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL (B2B) Business Price]_섹션을 확장합니다.

1. **[!UICONTROL Enable Business Pricing]**&#x200B;에 대해 옵션을 선택하십시오.

   - `Disabled` - (기본값) Business-to-Business Sales를 사용하지 않으려면 선택합니다. 선택하면 이 섹션의 다른 모든 필드가 비활성화됩니다.

   - `Enabled` - B2B 판매를 사용하도록 설정할 시기를 선택합니다. 활성화되면 모든 가격책정 규칙이 적용된 후 비즈니스 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 $1보다 작을 수 없습니다.

1. **[!UICONTROL Enable Tiered Pricing]**&#x200B;에 대해 옵션을 선택하십시오.

   - `Disabled` - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 경우 선택합니다. 선택하면 이 섹션의 모든 _[!UICONTROL Pricing Level]_필드가 비활성화됩니다.

   - `Enabled` - 주문 수량에 따라 가격 조정을 사용하도록 설정할 시기를 선택합니다. 선택하면 _[!UICONTROL Pricing Level]_필드가 활성화됩니다.

1. **[!UICONTROL Pricing Level]** 설정을 완료합니다.

   비즈니스 목록에 대해 계층 가격을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어 첫 번째 행의 첫 번째 필드에 `5`을(를) 입력하고 두 번째 필드에 `5`을(를) 입력하면 다른 사업체가 5개 이상의 수량을 구매할 때 가격은 5% 할인을 적용합니다.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![Amazon Business Pricing(B2B)](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| 필드 | 설명 |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) Business to Business Sales를 사용하지 않으려면 선택합니다. 이 옵션을 선택하면 이 섹션의 다른 모든 필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - 비즈니스에서 비즈니스 판매로 전환할 시기를 선택하십시오. 이 옵션을 선택하면 모든 가격 책정 규칙이 적용된 후 비즈니스 가격이 장부 가격과 동일하게 설정됩니다. 활성화된 경우 비즈니스 가격은 웹 사이트 가격 범위를 따릅니다. 비즈니스 가격은 $1보다 작을 수 없습니다.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (필수) 옵션: <ul><li>**[!UICONTROL Disabled]** - (기본값) 모든 주문 수량에 대해 동일한 목록 가격을 원하는 경우 선택합니다. 선택하면 이 섹션의 모든 _[!UICONTROL Pricing Level]_필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - 주문 수량에 따라 조정된 가격을 사용하도록 설정하려면 선택합니다. 선택하면 _[!UICONTROL Pricing Level]_필드가 활성화됩니다.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | 계층형 가격책정이 활성화되면 비즈니스 목록에 대한 계층 가격책정을 설정하는 최대 5개의 수량/할인 설정을 정의할 수 있습니다. 각 행에 적용할 수량 임계값 및 할인 퍼센트를 입력합니다. 예를 들어 첫 번째 행의 첫 번째 필드에 `5`을(를) 입력하고 두 번째 필드에 `5`을(를) 입력하면 다른 사업체가 5개 이상의 수량을 구매할 때 가격은 5% 할인을 적용합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
