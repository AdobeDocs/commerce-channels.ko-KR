---
title: 불완전한 목록
description: Amazon 판매 채널은 불완전한 Amazon 목록에 대한 자격 조건을 확인하고 충족하는 데 도움이 되는 [!UICONTROL Incomplete] 탭을 제공합니다.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 불완전한 목록

_[!UICONTROL Incomplete]_탭에는 Amazon 자격 요구 사항([목록 규칙](./listing-rules.md)에 정의됨)을 충족하지만 Amazon에 필요한 정보(예: Amazon ASIN 또는 정의된 제품 조건)가 없는 [!DNL Commerce] 카탈로그 제품이 나열됩니다.

불완전한 목록에 대해 각각 해당 상태로 식별되는 네 가지 가능한 원인이 있습니다.

| 상태 | 이유 | 작업 |
|--- |--- |--- |
| 누락된 조건 | Amazon은 다양한 조건(예: _New_, _Repancreated_, _사용됨: New_)와 마찬가지로 정의된 조건이 필요합니다. | 필수 정보를 업데이트하고 수동으로 [목록에 조건](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)을 지정하십시오. |
| Amazon 목록에 할당할 수 없음 | 이 목록을 카탈로그에 자동으로 일치시키지 못했습니다. 일치하는 항목이 없으면 Amazon Sales Channel에서 목록을 관리할 수 없습니다 | 필요한 정보를 업데이트하고 수동으로 [목록에 일치시킬 ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing)을 카탈로그 제품에 할당합니다. |
| 여러 일치 항목 찾음 | 이 목록을 카탈로그에 자동으로 일치시키지 못했습니다. 가능한 일치 항목이 여러 개 있는 경우 제품에 대한 올바른 일치 항목을 선택해야 합니다. | 필요한 정보를 업데이트하고 수동으로 [제품 및 목록에 대한 제품 일치](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)를 선택합니다. |
| 변형 있음 | 제품에 다른 크기 또는 색상으로 사용할 수 있는 티셔츠 등의 변형이 있는 경우 카탈로그의 변형을 선택하여 목록에 올바르게 지정하고 일치시켜야 합니다 | 필요한 정보를 업데이트하고 수동으로 [이 목록에 할당하고 일치시킬 올바른 변형](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants)을 선택하십시오. |

>[!NOTE]
>불완전한 목록이 카탈로그 제품과 제대로 일치하면 목록이 _[!UICONTROL Incomplete]_탭에서 이동하고 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정에 따라 Amazon에 게시됩니다.

_[!UICONTROL Incomplete]_탭에서 사용할 수 있는 작업은 다음과 같습니다.

_[!UICONTROL Actions]_아래:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Amazon 목록 데이터를 카탈로그에 일치시키는 자동 프로세스를 시작하도록  [!DNL Commerce] 선택합니다. 제품이 자동으로 일치하지 않는 경우 목록 설정에서 [_[!UICONTROL Catalog Search]_](./catalog-search.md) 옵션을 다시 방문하십시오. _[!UICONTROL Catalog Search]_옵션을 업데이트한 후 목록이 자동으로 일치하지 않는 경우 [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 작업에서 제품을 수동으로 일치시킬 수 있습니다.

_[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래:

- **[!UICONTROL Update Required Info]**: 목록이 카탈로그에 자동으로 일치하지 않는 경우를 선택합니다. 수동으로 [카탈로그 제품을 목록](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)에 일치시키거나, 수동으로 [카탈로그 일치에 ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing)을 할당하거나, 목록에 누락된 조건](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)을 할당할 수 있습니다.[

- **[!UICONTROL View Details]**: Listing Activity  [Log](./product-listing-details.md#listing-activity-log),  [Competitor Pricing](./product-listing-details.md#buy-box-competitor-pricing) 및  [Lowered Competitor Pricing](./product-listing-details.md#lowest-competitor-pricing)을 포함하여 목록 세부 사항을 표시하도록 선택합니다. 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. [세부 정보 보기](./product-listing-details.md)를 참조하십시오.

>[!NOTE]
>
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![불완전한 Amazon 목록](assets/amazon-incomplete-listings.png)

Amazon 판매 채널 홈 페이지는 표시되는 데이터를 사용자 지정할 수 있는 몇 가지 일반적인 [작업 공간 컨트롤](./workspace-controls.md)을 공유합니다.

| 열 | 설명 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 을  [!DNL Amazon Standard Identification Number]의미합니다. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 제품의 [조건](./product-listing-condition.md)입니다. |
| [!UICONTROL Landed Price] | 제품 목록 가격과 배송료. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon에 의해 정의된 목록의 상태입니다. 위의 상태 표를 참조하십시오. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을 클릭하고 옵션을 선택합니다.<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
