---
title: 제품 목록 조건
description: 제품 목록 조건 설정을 사용하여 상거래 제품을 "신규" 또는 "재생"과 같은 Amazon 제품 조건에 매핑합니다.
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 제품 목록 조건

제품 목록 조건 설정은 스토어 목록 설정의 일부입니다. 다음에서 목록 설정에 액세스할 수 있습니다. [대시보드 저장](./amazon-store-dashboard.md).

Amazon의 경우 정의된 조건을 가지려면 제품 목록이 필요합니다. 모든 제품이 동일한 조건인 경우 Amazon 조건 옵션 중 하나를 선택하여 모든 제품을 글로벌 조건 값으로 나타낼 수 있습니다. 표준 Amazon 조건은 다음과 같습니다.

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
>리뉴얼된(재생) 제품을 판매하는 경우 [!DNL Amazon Renewed Program]. 다음을 참조하십시오 [갱신한 제품](./renewed-products.md).

그러나 카탈로그에 다른 조건(예: 신규, 사용 및 재생)의 제품이 포함되어 있는 경우 다음을 선택해야 합니다 **[!UICONTROL Assign Condition Using Product Attribute]**. 이 설정을 사용하면 [!DNL Commerce] 조건 속성 및 값을 Amazon 목록의 조건에 추가합니다.

다음 기간 동안 [사전 설정 작업](./amazon-pre-setup-tasks.md), 다음을 만드는 것이 좋습니다. [!DNL Commerce] 제품 조건에 대한 제품 속성. 다양한 조건의 제품을 제공하고 조건 속성을 만들지 않은 경우 다음을 참조하십시오. [에서 제품 속성 만들기 [!DNL Commerce]](./ob-creating-magento-attributes.md). condition 속성이 만들어지면 의 각 제품에 조건 값을 할당할 수 있습니다. [!DNL Commerce] 카탈로그.

## 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 **[!UICONTROL Product Listing Condition]** 섹션.

1. 대상 **[!UICONTROL Listing Product Condition]**&#x200B;옵션을 선택합니다.

   모든 목록의 글로벌 조건 값에 대한 표준 Amazon 조건 중 하나를 선택합니다. 기본 설정: `New`.

   조건이 다른 제품/목록이 있는 경우 `Assign Condition Using Product Attribute` 표시되는 추가 필드에 제품 조건 설정을 정의합니다.

1. 대상 **조건 속성**, 을(를) 선택합니다. [!DNL Commerce] 속성을 사용하여 각 표준 Amazon 조건 속성에 대한 값을 매핑할 수 있습니다.

   에 제품이 있는 경우 `Used` 또는 `Collectible` 조건은 구분하지만 더 이상 구분하지 않습니다. 매핑할 수 있습니다. `Used` 또는 `Collectible` Amazon 조건 및 다른 조건은 비워 둡니다. 이 메서드는 `Used` 또는 `Collectible` 단일 Amazon 사용 또는 수집 가능 조건에 대한 조건.

   예를 들어, 단일 `Used` 제품에 대한 조건입니다. 매핑 시 Amazon 조건에 매핑할지 여부를 선택합니다 `Used; Like New`, `Used; Very Good`, `Used; Good`, 또는 `Used; Acceptable`. 원하는 Amazon 조건에 대한 필드만 완료하고 다른 필드는 남겨둡니다. `Used` 옵션으로 설정됨 `--Select Option--`. 예제 이미지에서 모두 [!DNL Commerce] 의 제품 `Used` 조건이 Amazon에 매핑됨 `Used; Very Good` 조건.

   조건에 대한 설명 텍스트를 입력할 수도 있습니다. 단, `New`.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![제품 목록 조건](assets/amazon-product-listing-condition.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Listing Product Condition] | 제품 목록의 상태. 옵션: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>단일 제품 조건을 판매하는 경우 표준 Amazon 조건 중 하나를 선택하십시오. 다음의 경우 [!DNL Commerce] 카탈로그에 다양한 조건의 제품이 포함되어 있습니다. `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | 다음 [!DNL Commerce] 제품에 대한 조건을 정의하는 속성입니다. Amazon 조건 속성에 매핑하기 위해 만든 Magneto 속성을 선택합니다. 다음에서 [사전 설정 작업 예](./ob-creating-magento-attributes.md) 이름을 로 지정할 것을 권장합니다. `Amazon Condition`. 선택하면 표준 Amazon 조건을 매핑하기 위한 추가 필드가 표시됩니다. |
| [!UICONTROL Additional Condition fields] | 각 표준 Amazon 조건에 대해 해당 조건을 선택합니다. 옵션은 다음을 수행할 때 추가한 조건 레이블입니다. [이(가) Amazon 조건 속성을 만들었습니다.](./ob-creating-magento-attributes.md).<br><br>에 제품이 있는 경우 `Used` 또는 `Collectible` 조건은 구분하지만 더 이상 구분하지 않습니다. 매핑할 수 있습니다. `Used` 또는 `Collectible` Amazon 조건 및 다른 조건은 비워 둡니다. 이 메서드는 모두 매핑합니다. `Used` 또는 `Collectible` 단일 Amazon 사용 또는 수집 가능 조건에 대한 조건. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
