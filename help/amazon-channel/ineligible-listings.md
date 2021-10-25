---
title: 부적격 목록
description: Amazon 영업 채널은 [!UICONTROL Ineligible] 항목을 관리하는 데 도움이 되는 탭은 현재 목록 규칙에 따라 목록으로 사용할 수 없습니다.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 부적격 목록

다음 _[!UICONTROL Ineligible]_탭에는 현재 Amazon에 게시되었지만 현재 목록 규칙을 기준으로 나열할 수 없는 모든 제품의 목록이 표시됩니다. 이전 제품이 적격이고 목록 규칙이 수정되어 부적합하면 제품 관련 수량이 0으로 감소하고 제품이 로 표시됩니다_&#x200B;부적당하&#x200B;_. 그러나 여전히 [!DNL Amazon Seller Account].

제품을 _[!UICONTROL Ineligible]_탭, [목록 규칙 수정](./listing-rules.md) 을 클릭하여 제품에서 자격을 부여할 수 있습니다.

에서 사용 가능한 작업 _[!UICONTROL Ineligible]_에는 다음이 포함되어 있습니다.

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: 선택한 모든 목록을 [!DNL Amazon Marketplace]. 자세한 내용은 [Amazon 목록 종료](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: 목록의 무시 설정을 변경하려면 선택합니다. 자세한 내용은 [무시](./overrides.md) 또는 [무시 편집 또는 제거](./creating-editing-overrides.md#edit-override-single-listing).

아래 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열:

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 사항을 표시하도록 선택합니다 [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격 책정](./product-listing-details.md#buy-box-competitor-pricing), 및 [가장 낮은 경쟁업체 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. 자세한 내용은 [세부 사항 보기](./product-listing-details.md).

- **[!UICONTROL Create Override]**: 무시를 만들고 이 목록에 적용하도록 선택합니다. 자세한 내용은 [무시 만들기](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: 카탈로그 제품에 할당된 ASIN을 수정하도록 선택합니다. 이 작업은 카탈로그의 제품이 잘못된 ASIN과 일치한 경우 사용됩니다. 자세한 내용은 [지정된 ASIN 편집](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: 동일한 카탈로그 제품에서 Amazon 목록을 만드는 데 사용할 수 있는 별칭 SKU를 만들도록 선택합니다. 자세한 내용은 [별칭 판매자 SKU 만들기](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: 주문과 연관된 이행 방법을 변경하도록 선택합니다. 자세한 내용은 [설정별 충족됨 구성](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: 목록에서 목록을 제거하도록 선택합니다 [!DNL Amazon Marketplace]. 자세한 내용은 [Amazon 목록 종료](./end-listings-manually.md).

>[!NOTE]
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![부적격 Amazon 목록](assets/amazon-ineligible-listings.png)

Amazon 영업 채널 홈 페이지는 다음과 같은 몇 가지 일반적인 [작업 영역 컨트롤](./workspace-controls.md) 표시되는 데이터를 사용자 지정할 수 있습니다.

## 기본 열

| 열 | 설명 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) Analytics Premium이 있어야 합니다. |
| [!UICONTROL Landed Price] | 제품 목록 가격과 배송료. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고 다음 옵션을 선택합니다.<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[무시 만들기](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
