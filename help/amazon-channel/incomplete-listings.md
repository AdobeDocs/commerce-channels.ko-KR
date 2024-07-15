---
title: 불완전한 Amazon 목록
description: Amazon 판매 채널에서는 불완전한 Amazon 목록에 대한 자격 요구 사항을 식별하고 충족하는 데 도움이 되는 [!UICONTROL Incomplete] 탭을 제공합니다.
feature: Sales Channels, Products
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 불완전한 Amazon 목록

_[!UICONTROL Incomplete]_탭에는 Amazon 자격 요구 사항([목록 규칙](./listing-rules.md)에 정의됨)을 충족하지만 Amazon에 필요한 정보(Amazon ASIN 또는 정의된 제품 조건 등)가 없는 [!DNL Commerce] 카탈로그 제품이 나열됩니다.

불완전 목록에는 네 가지 가능한 원인이 있으며, 각 원인은 해당 상태로 식별됩니다.

| 상태 | 이유 | 작업 |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 누락된 상태 | Amazon은 정의된 조건이 필요한 다양한 조건(예: _신규_, _재생_, _사용: 신규_)의 목록을 허용합니다. | 필수 정보를 업데이트하고 수동으로 [조건을 목록에 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)하세요. |
| Amazon 목록에 할당할 수 없음 | 이 목록을 카탈로그와 자동으로 일치시키지 못했습니다. 일치하는 항목이 없으면 Amazon Sales Channel에서 목록을 관리할 수 없습니다. | 필수 정보를 업데이트하고 목록에 일치시키기 위해 카탈로그 제품에 수동으로 [ASIN을 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing)합니다. |
| 일치하는 항목이 여러 개 있습니다. | 이 목록을 카탈로그와 자동으로 일치시키지 못했습니다. 일치하는 항목이 여러 개 있는 경우 제품에 대해 올바른 일치 항목을 선택해야 합니다. | 필수 정보를 업데이트하고 제품 및 목록에 대해 수동으로 [제품 일치 항목을 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)합니다. |
| 변형 있음 | 제품에 다른 크기 또는 색상으로 제공되는 티셔츠와 같은 변형이 있는 경우 카탈로그에서 변형을 선택하여 목록에 올바로 할당하고 대응해야 합니다 | 필요한 정보를 업데이트하고 수동으로 [올바른 변형을 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants)하여 할당하고 이 목록에 일치시키십시오. |

>[!NOTE]
>불완전한 목록이 카탈로그 제품과 올바르게 일치하면 목록이 _[!UICONTROL Incomplete]_탭에서 이동하고 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정에 따라 Amazon에 게시됩니다.

_[!UICONTROL Incomplete]_탭에서 사용할 수 있는 작업은 다음과 같습니다.

_[!UICONTROL Actions]_에서:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Amazon 목록 데이터를 [!DNL Commerce] 카탈로그와 일치시키는 자동 프로세스를 시작하도록 선택하십시오. 제품이 자동으로 일치하지 않는 경우 목록 기록에서 [_[!UICONTROL Catalog Search]_](./catalog-search.md) 옵션을 다시 방문하십시오. _[!UICONTROL Catalog Search]_옵션을 업데이트한 후 목록이 자동으로 일치하지 않으면 [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 작업에서 제품을 수동으로 일치시킬 수 있습니다.

_[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래:

- **[!UICONTROL Update Required Info]**: 목록이 자동으로 카탈로그와 일치하지 않는 경우 선택합니다. 카탈로그 제품을 목록에 수동으로 [일치](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), 카탈로그 일치 항목에 수동으로 [ASIN 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 또는 목록에 대해 [누락된 조건 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition)할 수 있습니다.

- **[!UICONTROL View Details]**: [활동 로그 나열](./product-listing-details.md#listing-activity-log), [경쟁업체 가격 Buy Box](./product-listing-details.md#buy-box-competitor-pricing), [경쟁업체 최저 가격 설정](./product-listing-details.md#lowest-competitor-pricing)을 포함한 목록 세부 정보를 보려면 선택하십시오. 이 작업은 보기 전용입니다. 목록 세부 사항을 변경할 수 없습니다. [세부 정보 보기](./product-listing-details.md)를 참조하세요.

>[!NOTE]
>
>목록을 처리 중인 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![불완전한 Amazon 목록](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Amazon 판매 채널 홈 페이지는 표시되는 데이터를 사용자 지정할 수 있도록 해 주는 몇 가지 일반적인 [작업 영역 컨트롤](./workspace-controls.md)을 공유합니다.

| 열 | 설명 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit). |
| [!UICONTROL ASIN] | 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]을(를) 나타냅니다. ASIN은 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품 이름. |
| [!UICONTROL Condition] | 제품의 [조건](./product-listing-condition.md). |
| [!UICONTROL Landed Price] | 제품의 목록 가격과 배송 가격을 더한 값입니다. |
| [!UICONTROL Amazon Quantity] | 제품이 Amazon에 활성 상태로 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon으로 정의된 목록의 상태. 위의 상태 표를 참조하십시오. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을(를) 클릭하고 옵션을 선택하십시오.<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
