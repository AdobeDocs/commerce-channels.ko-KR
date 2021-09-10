---
title: 제품 목록 조건
description: 제품 목록 조건 설정을 사용하여 상거래 제품을 "새로 만들기" 또는 "새로 고침"과 같은 Amazon 제품 조건에 매핑합니다.
redirect_from: /sales-channels/asc/ob-product-listing-condition.html: 
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 526
ht-degree: 0%

---

# 제품 목록 조건

제품 목록 조건 설정은 저장소 목록 설정의 일부입니다. [대시보드](./amazon-store-dashboard.md)의 목록 설정에 액세스할 수 있습니다.

Amazon에는 정의된 조건이 있는 제품 목록이 필요합니다. 모든 제품이 동일한 조건인 경우 Amazon 조건 옵션 중 하나를 선택하여 모든 제품을 글로벌 조건 값으로 표시할 수 있습니다. 표준 Amazon 조건은 다음과 같습니다.

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>갱신된(재생된) 제품을 판매하는 경우 [!DNL Amazon Renewed Program]에 등록해야 합니다. [갱신된 제품](./renewed-products.md)을 참조하십시오.

그러나 카탈로그에 다른 조건(예: 새로 만들기, 사용 및 새로 고침)의 제품이 포함된 경우 **[!UICONTROL Assign Condition Using Product Attribute]**&#x200B;을 선택해야 합니다. 이 설정을 사용하면 [!DNL Commerce] 조건 속성 및 값을 Amazon 목록 조건에 매핑할 수 있습니다.

[사전 설정 작업](./amazon-pre-setup-tasks.md) 중에는 제품 조건에 대해 [!DNL Commerce] 제품 속성을 만드는 것이 좋습니다. 다양한 조건으로 제품을 제공하고 조건 속성을 만들지 않은 경우 [제품 속성 만들기 [!DNL Commerce]](./ob-creating-magento-attributes.md)를 참조하십시오. 조건 속성이 만들어지면 [!DNL Commerce] 카탈로그의 각 제품에 조건 값을 할당할 수 있습니다.

## 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. **[!UICONTROL Product Listing Condition]** 섹션을 확장합니다.

1. **[!UICONTROL Listing Product Condition]**&#x200B;에 대해 옵션을 선택합니다.

   모든 목록에 대한 글로벌 조건 값에 대한 표준 Amazon 조건 중 하나를 선택합니다. 기본 설정은 `New`입니다.

   조건이 다른 제품/목록이 있는 경우 `Assign Condition Using Product Attribute`을 선택하여 표시되는 추가 필드에서 제품 조건 설정을 정의합니다.

1. **조건 속성**&#x200B;에 대해 [!DNL Commerce] 속성을 선택하여 각 표준 Amazon 조건 속성에 대한 값을 매핑합니다.

   `Used` 또는 `Collectible` 조건에 제품이 있지만 더 이상 구별되지 않는 경우 단일 `Used` 또는 `Collectible` Amazon 조건에 매핑하고 나머지는 비워 둘 수 있습니다. 이 메서드는 모든 `Used` 또는 `Collectible` 조건을 단일 Amazon 사용 또는 수집 가능 조건에 매핑합니다.

   예를 들어 제품에 대해 단일 `Used` 조건이 있습니다. 매핑 시 Amazon 조건 `Used; Like New`, `Used; Very Good`, `Used; Good` 또는 `Used; Acceptable`에 매핑할지 여부를 선택합니다. 원하는 Amazon 조건에 대한 필드만 완료하고 다른 `Used` 옵션이 `--Select Option--`로 설정된 상태로 둡니다. 예제 이미지에서 `Used` 조건의 모든 [!DNL Commerce] 제품은 Amazon `Used; Very Good` 조건에 매핑됩니다.

   `New`을 제외하고 조건에 대한 설명 텍스트를 입력할 수도 있습니다.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![제품 목록 조건](assets/amazon-product-listing-condition.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Listing Product Condition] | 제품 목록 조건입니다. 옵션: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>단일 제품 조건을 판매하는 경우 표준 Amazon 조건 중 하나를 선택하십시오. `Collectible: Very Good` [!DNL Commerce] 카탈로그에 다양한 조건의 제품이 포함된 경우 `Assign Condition Using Product Attribute`을 선택합니다. |
| [!UICONTROL Condition Attribute] | 제품에 대한 조건을 정의하는 [!DNL Commerce] 속성입니다. Amazon 조건 속성에 매핑하기 위해 만든 Magento 속성을 선택합니다. [사전 설정 작업 예시](./ob-creating-magento-attributes.md)에서는 이름을 `Amazon Condition`로 지정할 것을 권장합니다. 선택한 경우 표준 Amazon 조건을 매핑하기 위한 추가 필드가 나타납니다. |
| [!UICONTROL Additional Condition fields] | 각 표준 Amazon 조건에 대해 해당 조건을 선택합니다. 옵션은 [Amazon 조건 속성을 만들 때 추가한 조건 레이블입니다](./ob-creating-magento-attributes.md).<br><br>또는 조건에 제품이  `Used` 있지만  `Collectible` 더 이상 구별하지 않는 경우 단일 또는  `Used`   `Collectible` Amazon 조건에 매핑하고 다른 조건을 비워 둘 수 있습니다. 이 메서드는 모든 `Used` 또는 `Collectible` 조건을 단일 Amazon 사용 또는 수집 가능 조건에 매핑합니다. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
