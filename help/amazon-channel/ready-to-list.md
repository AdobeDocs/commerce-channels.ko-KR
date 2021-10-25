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

다음 _[!UICONTROL Ready to List]_탭에 [!DNL Commerce] 목록 설정을 충족하고 Marketing Cloud를 Adobe Analytics에&#x200B;**새**목록. 다른 목록 탭과 달리 이 탭이 항상 [_[!UICONTROL Product Listings]_](./managing-product-listings.md) 페이지.

다음 _[!UICONTROL Ready to List]_탭이 [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) 에서 목록 설정은 `Do Not Automatically List Eligible Products`. 이 설정은 Amazon 판매 채널에 새 Amazon 목록을 수동으로 게시해야 한다고 알려줍니다.

When [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) 가 로 설정되어 있습니다. `Automatically List Eligible Products`, Amazon 영업 채널은 해당 카탈로그 제품에 대한 새 목록을 자동으로 게시합니다. 새 목록이 자동으로 게시되므로 _[!UICONTROL Ready to List]_탭이 표시되지 않습니다.

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: 목록을 [!DNL Amazon Marketplace]. 자세한 내용은 [Amazon 목록 게시](./publish-listings-manually.md)

아래 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열:

- **[!UICONTROL Publish On Amazon]**: 목록을 [!DNL Amazon Marketplace]. 자세한 내용은 [Amazon 목록 게시](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 사항을 표시하도록 선택합니다 [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격 책정](./product-listing-details.md#buy-box-competitor-pricing), 및 [가장 낮은 경쟁업체 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항에서는 변경할 수 없습니다. 자세한 내용은 [세부 사항 보기](./product-listing-details.md).

수동으로 수행할 수 있는 옵션이 몇 가지 있습니다 [Amazon에 새 목록 게시](./publish-listings-manually.md).

>[!NOTE]
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![목록 준비 완료](assets/amazon-ready-to-list.png)

## 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) Analytics Premium이 있어야 합니다. |
| [!UICONTROL Landed Price] | 제품 목록 가격과 배송료. |
| [!UICONTROL Amazon Quantity] | Amazon에 제품이 활발히 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon에 의해 정의된 목록의 상태입니다. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고 다음 옵션을 선택합니다.<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### 목록 준비 작업의 일반적인 원인

- **[!UICONTROL Ready to List]** - 제품이 Amazon ASIN과 일치하고 목록을 위해 예약되어 있습니다. If [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) 에서 목록 설정은 `Do Not Automatically List Eligible Products`, 이 상태는 수동으로 나열할 준비가 된 제품을 나타냅니다.

- **[!UICONTROL List in Progress]** - 제품 목록이 Amazon에 제출되었으며 Amazon의 수락 확인을 기다리고 있습니다.
