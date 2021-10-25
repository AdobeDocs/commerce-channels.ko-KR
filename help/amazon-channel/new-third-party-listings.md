---
title: 새로운 타사 목록
description: 전자 상거래 카탈로그의 제품에 일치시켜 새 Amazon 목록을 관리합니다.
exl-id: ace9d334-d1d1-4f4b-88c8-60a9e7d1d17c
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 새로운 타사 목록

다음 _[!UICONTROL New Third Party]_탭에는 사용자의 제품에 일치하지 않는 기존 Amazon 목록이 표시됩니다 [!DNL Commerce] 카탈로그 수량, 가격 책정, 처리 시간 등에 대한 목록 관리를 사용하려면 각 Amazon 목록을 [!DNL Commerce] 카탈로그 목록에 을 지정할 수 있는 옵션이 몇 가지 있습니다 [!DNL Commerce] 카탈로그

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL Create New Catalog Product(s)]**: Amazon 목록의 정보를 사용하여 [!DNL Commerce] 카탈로그 이 프로세스는 자동으로 새 카탈로그 제품에 Amazon 목록을 일치시킵니다. 자세한 내용은 [카탈로그 제품 만들기 및 할당](./creating-assigning-catalog-products.md).

- **[!UICONTROL Attempt Automatic Match]**: 현재 목록을 기준으로 선택한 목록에 대해 자동 일치를 시도하도록 선택합니다 [카탈로그 검색](./catalog-search.md) 목록 설정에 있는 옵션. 을 수정하는 경우 _[!UICONTROL Catalog Search]_옵션, 이 작업을 사용하면 일치 프로세스를 다시 시도할 수 있습니다.

아래 _[!UICONTROL Select]_:

- **[!UICONTROL Assign Catalog Product]**: 목록을 의 제품과 일치시키도록 선택합니다 [!DNL Commerce] 카탈로그를 수동으로 표시합니다. 자세한 내용은 [카탈로그 제품 만들기 및 할당](./creating-assigning-catalog-products.md).

- **[!UICONTROL Create New Catalog Product]**: Amazon 목록의 정보를 사용하여 [!DNL Commerce] 카탈로그 이 프로세스는 자동으로 새 카탈로그 제품에 Amazon 목록을 일치시킵니다. 자세한 내용은 [카탈로그 제품 만들기 및 할당](./creating-assigning-catalog-products.md).

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 사항을 표시하도록 선택합니다 [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격 책정](./product-listing-details.md#buy-box-competitor-pricing), 및 [가장 낮은 경쟁업체 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. 자세한 내용은 [세부 사항 보기](./product-listing-details.md).

>[!NOTE]
>
>진행 중인 목록이 있는 경우 목록 수를 나타내는 메시지가 탭 위에 표시됩니다.

![새로운 타사 목록](assets/amazon-listings-new-third-party.png)

Amazon 영업 채널 홈 페이지는 다음과 같은 몇 가지 일반적인 [작업 영역 컨트롤](./workspace-controls.md) 표시되는 데이터를 사용자 지정할 수 있습니다.

## 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) Analytics Premium이 있어야 합니다. |
| [!UICONTROL Listing Price] | 가격 출처 및 적용 가능한 가격책정 규칙에 의해 정의된 대로 품목의 목록 가격을 식별합니다. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon에 의해 정의된 목록의 상태입니다. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고 다음 옵션을 선택합니다.<ul><li>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)</li><li>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
