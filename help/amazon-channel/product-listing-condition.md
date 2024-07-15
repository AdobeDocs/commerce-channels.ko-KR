---
title: Amazon 판매 채널 - 제품 목록 조건
description: 제품 목록 조건 설정을 사용하여 Commerce 제품을 "신규" 또는 "갱신"과 같은 Amazon 제품 조건에 매핑합니다.
feature: Sales Channels, Products, Merchandising
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 제품 목록 조건

제품 목록 조건 설정은 스토어 목록 설정의 일부입니다. [스토어 대시보드](./amazon-store-dashboard.md)에서 목록 설정에 액세스할 수 있습니다.

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
>갱신(재생)된 제품을 판매하는 경우 [!DNL Amazon Renewed Program]에 등록해야 합니다. [갱신된 제품](./renewed-products.md)을 참조하십시오.

그러나 카탈로그에 다른 조건(예: 새로 만들기, 사용됨 및 새로 고침)의 제품이 포함되어 있는 경우 **[!UICONTROL Assign Condition Using Product Attribute]**&#x200B;을(를) 선택해야 합니다. 이 설정을 사용하면 [!DNL Commerce] 조건 특성 및 값을 Amazon 목록의 조건에 매핑할 수 있습니다.

[사전 설정 작업](./amazon-pre-setup-tasks.md)을 수행하는 동안 제품 조건에 대한 [!DNL Commerce] 제품 특성을 만드는 것이 좋습니다. 다양한 조건의 제품을 제공하고 조건 특성을 만들지 않은 경우 [제품 특성 만들기 [!DNL Commerce]](./ob-creating-magento-attributes.md)를 참조하십시오. 조건 특성이 만들어지면 [!DNL Commerce] 카탈로그의 각 제품에 조건 값을 할당할 수 있습니다.

## 설정 구성

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Product Listing Condition]** 섹션을 확장합니다.

1. **[!UICONTROL Listing Product Condition]**&#x200B;에 대해 옵션을 선택하십시오.

   모든 목록의 글로벌 조건 값에 대한 표준 Amazon 조건 중 하나를 선택합니다. 기본 설정은 `New`입니다.

   조건이 다른 제품/목록이 있는 경우 `Assign Condition Using Product Attribute`을(를) 선택하여 표시되는 추가 필드에 제품 조건 설정을 정의합니다.

1. **Condition 특성**&#x200B;의 경우 [!DNL Commerce] 특성을 선택하여 각 표준 Amazon 조건 특성에 대한 값을 매핑합니다.

   `Used` 또는 `Collectible` 조건의 제품이 있지만 더 이상 구분하지 않는 경우 단일 `Used` 또는 `Collectible` Amazon 조건에 매핑하고 다른 조건은 비워 둘 수 있습니다. 이 메서드는 모든 `Used` 또는 `Collectible` 조건을 단일 Amazon 사용 또는 수집 가능 조건에 매핑합니다.

   예를 들어 제품에 대한 단일 `Used` 조건이 있습니다. 매핑할 때 Amazon 조건 `Used; Like New`, `Used; Very Good`, `Used; Good` 또는 `Used; Acceptable`에 매핑할지 여부를 선택합니다. 다른 `Used` 옵션을 `--Select Option--`(으)로 설정한 상태로 두고 원하는 Amazon 조건에 대한 필드만 완료하십시오. 예제 이미지에서 `Used` 조건의 모든 [!DNL Commerce] 제품이 Amazon `Used; Very Good` 조건에 매핑됩니다.

   `New`을(를) 제외한 조건에 대한 설명 텍스트를 입력할 수도 있습니다.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![제품 목록 조건](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Listing Product Condition] | 제품 목록의 상태. 옵션: `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>단일 제품 조건을 판매하는 경우 표준 Amazon 조건 중 하나를 선택하십시오. [!DNL Commerce] 카탈로그에 다양한 조건의 제품이 포함되어 있는 경우 `Assign Condition Using Product Attribute`을(를) 선택하십시오. |
| [!UICONTROL Condition Attribute] | 제품에 대한 조건을 정의하는 [!DNL Commerce] 특성입니다. Amazon 조건 속성에 매핑하기 위해 만든 Magneto 속성을 선택합니다. [사전 설정 작업 예제](./ob-creating-magento-attributes.md)에서는 이름을 `Amazon Condition`(으)로 지정할 것을 권장합니다. 선택하면 표준 Amazon 조건을 매핑하기 위한 추가 필드가 표시됩니다. |
| [!UICONTROL Additional Condition fields] | 각 표준 Amazon 조건에 대해 해당 조건을 선택합니다. 옵션은 [Amazon 조건 특성을 만들 때](./ob-creating-magento-attributes.md)추가한 조건 레이블입니다.<br><br>제품이 `Used` 또는 `Collectible` 조건에 있지만 더 이상 구분하지 않는 경우 단일 `Used` 또는 `Collectible` Amazon 조건에 매핑하고 다른 조건은 비워 둘 수 있습니다. 이 메서드는 모든 `Used` 또는 `Collectible` 조건을 단일 Amazon 사용 또는 수집 가능 조건에 매핑합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
