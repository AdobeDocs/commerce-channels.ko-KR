---
title: 필수 정보 업데이트(불완전한 목록)
description: Amazon 영업 채널은 Amazon에 필요한 정보가 없는 상거래 카탈로그 제품을 모니터링하는 불완전한 탭을 제공합니다.
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# 필수 정보 업데이트(불완전한 목록)

다음에 표시되는 목록 _[!UICONTROL Incomplete]_탭에 포함 [!DNL Commerce] 목록 규칙에 정의된 대로 Amazon 자격 요구 사항을 충족하지만 나열하기 전에 Amazon에 필요한 정보가 없는 카탈로그 제품.

## 필수 정보 업데이트(Amazon 목록에 할당할 수 없음) {#update-required-info-unable-to-assign-to-amazon-listing}

1. 다음에서 목록을 봅니다. _[!UICONTROL Incomplete]_탭 [목록 관리](./managing-product-listings.md).

1. 에서 _[!UICONTROL Action]_열,**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록을 표시합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토하십시오.

1. 대상 **[!UICONTROL Assign ASIN]**&#x200B;를 입력한 다음 카탈로그 제품에 일치시킬 목록에 대해 Amazon에서 지정한 ASIN을 입력합니다.

1. 제품 일치 항목을 저장하려면 **[!UICONTROL Save Listing Update]**.

이제 목록이 카탈로그와 일치하고 목록이 크론 및 목록 설정에 따라 Amazon에 업데이트되고 게시됩니다. 또한 _[!UICONTROL Incomplete]_탭.

![목록 일치 없음에 대해 ASIN을 수동으로 지정](assets/amazon-listing-update-assign-asin.png)

## 필수 정보 업데이트(일치하는 항목이 여러 개 있음) {#update-required-info-multiple-matches-found}

1. 다음에서 목록을 봅니다. _[!UICONTROL Incomplete]_탭 [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. 에서 _작업_ 열, **선택** > **업데이트 필수 정보** 업데이트하려는 목록을 표시합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토하십시오.

1. 대상 **[!UICONTROL Select Correct Amazon Listing]**&#x200B;을(를) 선택하고 이 제품에 일치시킬 목록에 대한 올바른 ASIN을 선택합니다.

   여기에 나열된 옵션에는 가능한 일치로 식별되는 카탈로그 제품이 포함됩니다. 이 선택 사항이 모두 올바른 경우 `Manually Enter Correct ASIN` 및에 대해 ASIN을 수동으로 입력합니다.

1. 수동으로 ASIN을 입력하는 경우, 올바른 ASIN을 입력하십시오. **[!UICONTROL Manually Assign ASIN]**.

1. 제품 일치 항목을 저장하려면 **[!UICONTROL Save Listing Update]**.

![가능한 여러 일치 항목 중에서 ASIN을 수동으로 선택합니다.](assets/amazon-listing-update-multiple-matches.png)

## 필수 정보 업데이트(변형 있음) {#update-required-info-has-variants}

1. 다음에서 목록을 봅니다. _[!UICONTROL Incomplete]_탭 [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. 에서 _[!UICONTROL Action]_열,**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록을 표시합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토하십시오.

1. 대상 **[!UICONTROL Select Correct Amazon Listing]**&#x200B;을(를) 선택하고 이 제품에 일치시킬 목록에 대한 올바른 ASIN을 선택합니다.

   여기에 나열된 옵션에는 가능한 일치로 식별되는 카탈로그 제품이 포함됩니다. 어떤 옵션도 올바르지 않으면 `Manually Enter Correct ASIN` 및에 대해 ASIN을 수동으로 입력합니다.

1. 수동으로 ASIN을 입력하는 경우, 올바른 ASIN을 입력하십시오. **[!UICONTROL Manually Assign ASIN]**.

1. 제품 일치 항목을 저장하려면 **[!UICONTROL Save Listing Update]**.

![가능한 변형 일치에서 ASIN을 수동으로 선택합니다.](assets/amazon-listing-update-multiple-matches.png)

## 필수 정보 업데이트(조건 없음) {#update-required-info-missing-condition}

1. 다음에서 목록을 봅니다. _[!UICONTROL Incomplete]_탭 [목록 관리](./managing-product-listings.md).

1. 에서 _[!UICONTROL Action]_열,**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록을 표시합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토하십시오.

1. 대상 **[!UICONTROL Condition]**&#x200B;를 클릭하고 적절한 조건을 선택합니다.

   사용 가능한 옵션 목록은 [제품 목록 조건](./product-listing-condition.md) 설정.

1. 제품 일치 항목을 저장하려면 **[!UICONTROL Save Listing Update]** .

![누락된 조건을 수동으로 업데이트](assets/amazon-update-listing-missing-condition.png)
