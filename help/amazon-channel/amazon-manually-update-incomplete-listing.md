---
title: 필수 정보 업데이트(불완전한 목록)
description: Amazon 판매 채널은 Amazon에 필요한 정보가 누락된 상거래 카탈로그 제품을 모니터링하는 미완료 탭을 제공합니다.
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# 필수 정보 업데이트(불완전한 목록)

목록에 표시된 목록 _[!UICONTROL Incomplete]_탭에 다음 포함: [!DNL Commerce] 목록 규칙에 정의된 Amazon 자격 요구 사항을 충족하지만 나열하기 전에 Amazon에 필요한 정보가 누락된 카탈로그 제품.

## 필수 정보 업데이트(Amazon 목록에 할당할 수 없음) {#update-required-info-unable-to-assign-to-amazon-listing}

1. 에서 목록 보기 _[!UICONTROL Incomplete]_의 탭 [목록 관리](./managing-product-listings.md).

1. 다음에서 _[!UICONTROL Action]_열, 클릭&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록에 대해 설명합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. 대상 **[!UICONTROL Assign ASIN]**&#x200B;카탈로그 제품에 일치시킬 목록에 대해 Amazon에서 할당한 ASIN을 입력합니다.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**.

이제 목록이 카탈로그와 일치하고 크론 및 목록 설정에 따라 목록이 업데이트되고 Amazon에 게시됩니다. 또한 에서도 제거됩니다. _[!UICONTROL Incomplete]_탭.

![목록 일치 없음에 대해 ASIN 수동 할당](assets/amazon-listing-update-assign-asin.png)

## 필수 정보 업데이트(일치하는 항목이 여러 개 있음) {#update-required-info-multiple-matches-found}

1. 에서 목록 보기 _[!UICONTROL Incomplete]_의 탭 [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. 다음에서 _작업_ 열, 클릭 **선택** > **필수 정보 업데이트** 업데이트하려는 목록에 대해 설명합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. 대상 **[!UICONTROL Select Correct Amazon Listing]**&#x200B;이 제품에 일치시킬 목록에 대해 올바른 ASIN을 선택합니다.

   여기에 나열된 옵션에는 가능한 일치하는 것으로 식별되는 카탈로그 제품이 포함됩니다. 올바른 옵션이 없으면 다음을 선택할 수 있습니다. `Manually Enter Correct ASIN` 제품에 대한 ASIN을 수동으로 입력합니다.

1. ASIN을 수동으로 입력하는 경우 올바른 ASIN을 입력합니다 **[!UICONTROL Manually Assign ASIN]**.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**.

![가능한 여러 일치 항목에서 수동으로 ASIN 선택](assets/amazon-listing-update-multiple-matches.png)

## 필수 정보 업데이트(변형 있음) {#update-required-info-has-variants}

1. 에서 목록 보기 _[!UICONTROL Incomplete]_의 탭 [[!UICONTROL Manage Listings]](./managing-product-listings.md).

1. 다음에서 _[!UICONTROL Action]_열, 클릭&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록에 대해 설명합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. 대상 **[!UICONTROL Select Correct Amazon Listing]**&#x200B;이 제품에 일치시킬 목록에 대해 올바른 ASIN을 선택합니다.

   여기에 나열된 옵션에는 가능한 일치하는 것으로 식별되는 카탈로그 제품이 포함됩니다. 올바른 옵션이 없으면 다음을 선택할 수 있습니다. `Manually Enter Correct ASIN` 제품에 대한 ASIN을 수동으로 입력합니다.

1. ASIN을 수동으로 입력하는 경우 올바른 ASIN을 입력합니다 **[!UICONTROL Manually Assign ASIN]**.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**.

![가능한 변형 일치에서 ASIN 수동 선택](assets/amazon-listing-update-multiple-matches.png)

## 필수 정보 업데이트(조건 누락) {#update-required-info-missing-condition}

1. 에서 목록 보기 _[!UICONTROL Incomplete]_의 탭 [목록 관리](./managing-product-listings.md).

1. 다음에서 _[!UICONTROL Action]_열, 클릭&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**업데이트하려는 목록에 대해 설명합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. 대상 **[!UICONTROL Condition]**&#x200B;적절한 조건을 선택합니다.

   사용 가능한 옵션 목록은 다음에 따라 다릅니다 [제품 목록 조건](./product-listing-condition.md) 설정.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]** .

![누락된 조건 수동 업데이트](assets/amazon-update-listing-missing-condition.png)
