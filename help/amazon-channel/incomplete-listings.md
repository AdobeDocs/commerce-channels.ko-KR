---
title: 불완전한 목록
description: Amazon 영업 채널은 [!UICONTROL Incomplete] 불완전한 Amazon 목록에 대한 자격 요구 사항을 식별하고 충족하는 데 도움이 되는 탭입니다.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 불완전한 목록

다음 _[!UICONTROL Incomplete]_탭 목록 [!DNL Commerce] Amazon 자격 요구 사항(에 정의됨)을 충족하는 카탈로그 제품 [목록 규칙](./listing-rules.md))이지만 Amazon에 필요한 정보(예: Amazon ASIN 또는 정의된 제품 조건)가 없습니다.

불완전한 목록에 대해 각각 해당 상태로 식별되는 네 가지 가능한 원인이 있습니다.

| 상태 | 이유 | 작업 |
|--- |--- |--- |
| 누락된 조건 | Amazon은 다양한 조건(예: _새로 만들기_, _새로 고친_, _사용: 좋아요 새로_) 목록은 정의된 조건이 필요합니다. | 필수 정보 업데이트 및 수동 업데이트 [조건 지정](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 목록에 추가합니다. |
| Amazon 목록에 할당할 수 없음 | 이 목록을 카탈로그에 자동으로 일치시키지 못했습니다. 일치하는 항목이 없으면 Amazon Sales Channel에서 목록을 관리할 수 없습니다 | 필수 정보 업데이트 및 수동 업데이트 [ASIN 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 목록에 일치시킬 카탈로그 제품으로 이동합니다. |
| 여러 일치 항목 찾음 | 이 목록을 카탈로그에 자동으로 일치시키지 못했습니다. 가능한 일치 항목이 여러 개 있는 경우 제품에 대한 올바른 일치 항목을 선택해야 합니다. | 필수 정보 업데이트 및 수동 업데이트 [제품 일치 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 참조하십시오. |
| 변형 있음 | 제품에 다른 크기 또는 색상으로 사용할 수 있는 티셔츠 등의 변형이 있는 경우 카탈로그의 변형을 선택하여 목록에 올바르게 지정하고 일치시켜야 합니다 | 필수 정보 업데이트 및 수동 업데이트 [올바른 변형 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) 을 추가하여 이 목록에 을 지정합니다. |

>[!NOTE]
>불완전한 목록이 카탈로그 제품과 제대로 일치하면 목록이 _[!UICONTROL Incomplete]_탭하고 을 기반으로 Amazon에 게시됩니다. [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정.

에서 사용 가능한 작업 _[!UICONTROL Incomplete]_에는 다음이 포함되어 있습니다.

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Amazon 목록 데이터를 [!DNL Commerce] 카탈로그 제품이 자동으로 일치하지 않는 경우 을 다시 방문하십시오 [_[!UICONTROL Catalog Search]_](./catalog-search.md) 목록의 옵션. 목록을 업데이트한 후 목록이 자동으로 일치하지 않는 경우 _[!UICONTROL Catalog Search]_옵션을 선택하면 [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 작업.

아래 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열:

- **[!UICONTROL Update Required Info]**: 목록이 카탈로그에 자동으로 일치하지 않는 경우를 선택합니다. 수동으로 수행할 수 있습니다 [카탈로그 제품을 목록에 연결](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), 수동으로 [ASIN 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 카탈로그 일치 또는 [누락된 조건 지정](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 참조하십시오.

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 사항을 표시하도록 선택합니다 [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격 책정](./product-listing-details.md#buy-box-competitor-pricing), 및 [가장 낮은 경쟁업체 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. 자세한 내용은 [세부 사항 보기](./product-listing-details.md).

>[!NOTE]
>
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![불완전한 Amazon 목록](assets/amazon-incomplete-listings.png)

Amazon 영업 채널 홈 페이지는 다음과 같은 몇 가지 일반적인 [작업 영역 컨트롤](./workspace-controls.md) 표시되는 데이터를 사용자 지정할 수 있습니다.

| 열 | 설명 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) Analytics Premium이 있어야 합니다. |
| [!UICONTROL Landed Price] | 제품 목록 가격과 배송료. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon에 의해 정의된 목록의 상태입니다. 위의 상태 표를 참조하십시오. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고 다음 옵션을 선택합니다.<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
