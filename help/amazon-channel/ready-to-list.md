---
title: 목록 준비
description: Amazon 판매 채널은 자격 조건을 충족하지만 자동으로 나열되지 않는 상거래 제품을 검토할 수 있도록 목록 준비 탭을 제공합니다.
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

_[!UICONTROL Ready to List]_탭에는 목록 설정을 충족하고&#x200B;**새**목록으로 Amazon에 게시할 준비가 된 [!DNL Commerce] 카탈로그 제품이 표시됩니다. 다른 목록 탭과 달리 이 탭이 [_[!UICONTROL Product Listings]_](./managing-product-listings.md) 페이지에 항상 나타나는 것은 아닙니다.

목록 설정의 [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이 `Do Not Automatically List Eligible Products`로 설정된 경우에만 _[!UICONTROL Ready to List]_탭이 나타납니다. 이 설정은 Amazon 판매 채널에 새 Amazon 목록을 수동으로 게시해야 한다고 알려줍니다.

[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이 `Automatically List Eligible Products`로 설정되면 Amazon 판매 채널에서 자격이 있는 카탈로그 제품에 대한 새 목록을 자동으로 게시합니다. 새 목록이 자동으로 게시되므로 _[!UICONTROL Ready to List]_탭이 표시되지 않습니다.

_[!UICONTROL Actions]_아래:

- **[!UICONTROL Publish Product to Amazon]**: 목록에 다시 게시하도록 선택합니다  [!DNL Amazon Marketplace]. [Amazon 목록 게시](./publish-listings-manually.md)를 참조하십시오

_[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래:

- **[!UICONTROL Publish On Amazon]**: 목록에 다시 게시하도록 선택합니다  [!DNL Amazon Marketplace]. [Amazon 목록 게시](./publish-listings-manually.md)를 참조하십시오.

- **[!UICONTROL View Details]**: Listing Activity  [Log](./product-listing-details.md#listing-activity-log),  [Competitor Pricing](./product-listing-details.md#buy-box-competitor-pricing) 및  [Lowered Competitor Pricing](./product-listing-details.md#lowest-competitor-pricing)을 포함하여 목록 세부 사항을 표시하도록 선택합니다. 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. [세부 정보 보기](./product-listing-details.md)를 참조하십시오.

수동으로 [새 목록을 Amazon](./publish-listings-manually.md)에 게시하는 옵션이 몇 가지 있습니다.

>[!NOTE]
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![목록 준비 완료](assets/amazon-ready-to-list.png)

## 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 을  [!DNL Amazon Standard Identification Number]의미합니다. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 제품의 [조건](./product-listing-condition.md)입니다. |
| [!UICONTROL Landed Price] | 제품 목록 가격과 배송료. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon에 의해 정의된 목록의 상태입니다. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을 클릭하고 옵션을 선택합니다.<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### 목록 준비 작업의 일반적인 원인

- **[!UICONTROL Ready to List]** - 제품이 Amazon ASIN과 일치하고 목록을 위해 예약되어 있습니다. 목록 설정에서 [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이 `Do Not Automatically List Eligible Products`로 설정된 경우 이 상태는 수동으로 나열할 준비가 된 제품을 나타냅니다.

- **[!UICONTROL List in Progress]** - 제품 목록이 Amazon에 제출되었으며 Amazon의 수락 확인을 기다리고 있습니다.
