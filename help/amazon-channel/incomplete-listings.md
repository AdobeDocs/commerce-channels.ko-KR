---
title: 불완전한 Amazon 목록
description: Amazon 판매 채널은 [!UICONTROL Incomplete] 탭에서 불완전한 Amazon 목록의 자격 요구 사항을 식별하고 충족합니다.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 불완전한 Amazon 목록

다음 _[!UICONTROL Incomplete]_탭에 다음 항목이 나열됩니다. [!DNL Commerce] Amazon 자격 요구 사항을 충족하는 카탈로그 제품(에 정의됨) [규칙 나열](./listing-rules.md))에 있지만 Amazon에 필요한 정보(예: Amazon ASIN 또는 정의된 제품 조건)가 없습니다.

불완전 목록에는 네 가지 가능한 원인이 있으며, 각 원인은 해당 상태로 식별됩니다.

| 상태 | 이유 | 작업 |
|--- |--- |--- |
| 누락된 상태 | Amazon은 다양한 조건(예: _신규_, _재생_, _사용됨: 새것처럼_) 나열하려면 정의된 조건이 필요합니다. | 필요한 정보를 수동으로 업데이트 [조건 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 목록에 추가합니다. |
| Amazon 목록에 할당할 수 없음 | 이 목록을 카탈로그와 자동으로 일치시키지 못했습니다. 일치하는 항목이 없으면 Amazon Sales Channel에서 목록을 관리할 수 없습니다. | 필요한 정보를 수동으로 업데이트 [asin 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 목록에 일치시키기 위해 카탈로그 제품에 연결합니다. |
| 일치하는 항목이 여러 개 있습니다. | 이 목록을 카탈로그와 자동으로 일치시키지 못했습니다. 일치하는 항목이 여러 개 있는 경우 제품에 대해 올바른 일치 항목을 선택해야 합니다. | 필요한 정보를 수동으로 업데이트 [제품 일치 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) (제품 및 목록 포함) |
| 변형 있음 | 제품에 다른 크기 또는 색상으로 제공되는 티셔츠와 같은 변형이 있는 경우 카탈로그에서 변형을 선택하여 목록에 올바로 할당하고 대응해야 합니다 | 필요한 정보를 수동으로 업데이트 [올바른 변형 선택](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) 을(를) 할당하여 이 목록에 일치시킵니다. |

>[!NOTE]
>불완전한 목록이 카탈로그 제품과 올바르게 일치하면 목록이 _[!UICONTROL Incomplete]_을(를) 탭하고 을(를) 기반으로 Amazon에 게시합니다. [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정.

에서 사용 가능한 작업 _[!UICONTROL Incomplete]_탭에는 다음이 포함됩니다.

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Amazon 목록 데이터를 와(과) 일치시키기 위한 자동 프로세스를 시작하도록 선택합니다. [!DNL Commerce] 카탈로그. 제품이 자동으로 일치하지 않는 경우 다음을 다시 방문하십시오. [_[!UICONTROL Catalog Search]_](./catalog-search.md) 목록 작성에 있는 옵션입니다. 업데이트 후 목록이 자동으로 일치하지 않는 경우 _[!UICONTROL Catalog Search]_옵션에서 제품을 수동으로 일치시킬 수 있습니다. [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) 작업.

아래 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_열:

- **[!UICONTROL Update Required Info]**: 목록이 자동으로 카탈로그와 일치하지 않는 경우 선택합니다. 수동으로 다음을 수행할 수 있습니다. [카탈로그 제품을 목록에 일치](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), 수동으로 [asin 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) 카탈로그 일치 또는 [누락된 조건 할당](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) 목록을 만드는 중입니다.

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 정보를 보도록 선택합니다. [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격](./product-listing-details.md#buy-box-competitor-pricing), 및 [경쟁사 최저 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항을 변경할 수 없습니다. 다음을 참조하십시오 [세부 사항 보기](./product-listing-details.md).

>[!NOTE]
>
>목록을 처리 중인 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![불완전한 Amazon 목록](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Amazon 판매 채널 홈 페이지는 몇 가지 공통점을 공유합니다. [작업 영역 컨트롤](./workspace-controls.md) 을 사용하면 표시되는 데이터를 사용자 정의할 수 있습니다.

| 열 | 설명 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit). |
| [!UICONTROL ASIN] | 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품 이름. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) 제품. |
| [!UICONTROL Landed Price] | 제품의 목록 가격과 배송 가격을 더한 값입니다. |
| [!UICONTROL Amazon Quantity] | 제품이 Amazon에 활성 상태로 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon으로 정의된 목록의 상태. 위의 상태 표를 참조하십시오. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_열을 만들고 옵션을 선택합니다.<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
