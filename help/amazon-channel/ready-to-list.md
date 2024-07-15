---
title: Amazon 판매 채널 - [!UICONTROL Ready to List]
description: Amazon 판매 채널에서는 자격 조건을 충족하지만 자동으로 나열되지 않는 Commerce 제품을 검토할 수 있도록 목록 준비 탭을 제공합니다.
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

_[!UICONTROL Ready to List]_탭에는 목록 설정을 충족하고&#x200B;**새**목록으로 Amazon에 게시할 준비가 된 [!DNL Commerce] 카탈로그 제품이 표시됩니다. 다른 목록 탭과 달리 이 탭은 [_[!UICONTROL Product Listings]_](./managing-product-listings.md) 페이지에 항상 나타나지는 않습니다.

_[!UICONTROL Ready to List]_탭은 목록 설정의 [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이(가) `Do Not Automatically List Eligible Products`(으)로 설정된 경우에만 나타납니다. 이 설정은 새 Amazon 목록을 수동으로 게시해야 함을 Amazon 판매 채널에 알려줍니다.

[**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이(가) `Automatically List Eligible Products`(으)로 설정되면 Amazon 판매 채널에서 적격 카탈로그 제품에 대한 새 목록을 자동으로 게시합니다. 새 목록이 자동으로 게시되므로 _[!UICONTROL Ready to List]_탭이 표시되지 않습니다.

_[!UICONTROL Actions]_에서:

- **[!UICONTROL Publish Product to Amazon]**: 목록을 [!DNL Amazon Marketplace]에 다시 게시하도록 선택합니다. [Publish 및 Amazon 목록](./publish-listings-manually.md)을 참조하세요.

_[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래:

- **[!UICONTROL Publish On Amazon]**: 목록을 [!DNL Amazon Marketplace]에 다시 게시하도록 선택합니다. [Publish 및 Amazon 목록](./publish-listings-manually.md)을 참조하세요.

- **[!UICONTROL View Details]**: [활동 로그 나열](./product-listing-details.md#listing-activity-log), [경쟁업체 가격 Buy Box](./product-listing-details.md#buy-box-competitor-pricing), [경쟁업체 최저 가격 설정](./product-listing-details.md#lowest-competitor-pricing)을 포함한 목록 세부 정보를 보려면 선택하십시오. 이 작업은 보기 전용입니다. 목록 세부 사항을 변경할 수 없습니다. [세부 정보 보기](./product-listing-details.md)를 참조하세요.

수동으로 [Amazon에 새 목록을 게시](./publish-listings-manually.md)하는 옵션이 몇 가지 있습니다.

>[!NOTE]
>목록이 처리 중인 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![나열 준비](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## 기본 열

| 열 | 설명 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit). |
| [!UICONTROL ASIN] | 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]을(를) 나타냅니다. ASIN은 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품 이름. |
| [!UICONTROL Condition] | 제품의 [조건](./product-listing-condition.md). |
| [!UICONTROL Landed Price] | 제품의 목록 가격과 배송 가격을 더한 값입니다. |
| [!UICONTROL Amazon Quantity] | 제품이 Amazon에 활성 상태로 나열될 때 사용할 수 있는 수량입니다. |
| [!UICONTROL Status] | Amazon으로 정의된 목록의 상태. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을(를) 클릭하고 옵션을 선택하십시오.<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### 목록 목록을 작성할 준비가 된 일반적인 원인

- **[!UICONTROL Ready to List]** - 제품이 Amazon ASIN과 일치하며 나열 예정입니다. 목록 설정의 [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md)이(가) `Do Not Automatically List Eligible Products`(으)로 설정된 경우 이 상태는 수동으로 나열할 준비가 된 제품을 나타냅니다.

- **[!UICONTROL List in Progress]** - 제품 목록이 Amazon에 제출되었으며 Amazon의 수락 확인을 기다리는 중입니다.
