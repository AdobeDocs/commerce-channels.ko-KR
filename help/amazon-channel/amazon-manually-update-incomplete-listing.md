---
title: Amazon 필수 정보 업데이트
description: Amazon 판매 채널은 Amazon에 필요한 정보가 누락된 Commerce 카탈로그 제품을 모니터링하는 미완료 탭을 제공합니다.
feature: Sales Channels, Merchandising, Catalog Management, Products
exl-id: f278cd50-8f04-452e-b9c2-c87820f9faf2
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# 필수 정보 업데이트(불완전한 목록)

_[!UICONTROL Incomplete]_탭에 표시되는 목록에는 목록 규칙에 정의된 Amazon 자격 요구 사항을 충족하지만 나열하기 전에 Amazon에 필요한 정보가 없는 [!DNL Commerce] 카탈로그 제품이 포함됩니다.

## 필수 정보 업데이트(Amazon 목록에 할당할 수 없음) {#update-required-info-unable-to-assign-to-amazon-listing}

1. [목록 관리](./managing-product-listings.md)의 _[!UICONTROL Incomplete]_탭에서 목록을 봅니다.

1. _[!UICONTROL Action]_열에서 업데이트할 목록에 대해&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**을(를) 클릭합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. **[!UICONTROL Assign ASIN]**&#x200B;의 경우 카탈로그 제품에 일치시킬 목록에 대해 Amazon에서 할당한 ASIN을 입력하십시오.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**&#x200B;을(를) 클릭합니다.

이제 목록이 카탈로그와 일치하고 크론 및 목록 설정에 따라 목록이 업데이트되고 Amazon에 게시됩니다. _[!UICONTROL Incomplete]_탭에서도 제거됩니다.

![목록 일치 항목 없음에 대해 ASIN을 수동으로 할당](assets/amazon-listing-update-assign-asin.png){width="600" zoomable="yes"}

## 필수 정보 업데이트(일치하는 항목이 여러 개 있음) {#update-required-info-multiple-matches-found}

1. [[!UICONTROL Manage Listings]](./managing-product-listings.md)의 _[!UICONTROL Incomplete]_탭에서 목록을 봅니다.

1. _작업_ 열에서 업데이트할 목록에 대해 **선택** > **필수 정보 업데이트**&#x200B;를 클릭합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. **[!UICONTROL Select Correct Amazon Listing]**&#x200B;의 경우 이 제품에 연결할 목록에 대해 올바른 ASIN을 선택하십시오.

   여기에 나열된 옵션에는 가능한 일치하는 것으로 식별되는 카탈로그 제품이 포함됩니다. 올바른 옵션이 없으면 `Manually Enter Correct ASIN`을(를) 선택하고 제품에 대한 ASIN을 수동으로 입력할 수 있습니다.

1. ASIN을 수동으로 입력하는 경우 **[!UICONTROL Manually Assign ASIN]**&#x200B;에 대한 올바른 ASIN을 입력하십시오.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**&#x200B;을(를) 클릭합니다.

![가능한 여러 일치 항목에서 수동으로 ASIN 선택](assets/amazon-listing-update-multiple-matches.png){width="600" zoomable="yes"}

## 필수 정보 업데이트(변형 있음) {#update-required-info-has-variants}

1. [[!UICONTROL Manage Listings]](./managing-product-listings.md)의 _[!UICONTROL Incomplete]_탭에서 목록을 봅니다.

1. _[!UICONTROL Action]_열에서 업데이트할 목록에 대해&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**을(를) 클릭합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. **[!UICONTROL Select Correct Amazon Listing]**&#x200B;의 경우 이 제품에 연결할 목록에 대해 올바른 ASIN을 선택하십시오.

   여기에 나열된 옵션에는 가능한 일치하는 것으로 식별되는 카탈로그 제품이 포함됩니다. 올바른 옵션이 없으면 `Manually Enter Correct ASIN`을(를) 선택하고 제품에 대한 ASIN을 수동으로 입력할 수 있습니다.

1. ASIN을 수동으로 입력하는 경우 **[!UICONTROL Manually Assign ASIN]**&#x200B;에 대한 올바른 ASIN을 입력하십시오.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]**&#x200B;을(를) 클릭합니다.

## 필수 정보 업데이트(조건 누락) {#update-required-info-missing-condition}

1. [목록 관리](./managing-product-listings.md)의 _[!UICONTROL Incomplete]_탭에서 목록을 봅니다.

1. _[!UICONTROL Action]_열에서 업데이트할 목록에 대해&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Update Required Info]**을(를) 클릭합니다.

1. Amazon 목록에 일치시키려는 카탈로그 제품 정보(SKU 및 제품 이름)를 검토합니다.

1. **[!UICONTROL Condition]**&#x200B;에 대해 적절한 조건을 선택하십시오.

   사용 가능한 옵션 목록은 [제품 목록 조건](./product-listing-condition.md) 설정에 따라 다릅니다.

1. 제품 일치를 저장하려면 **[!UICONTROL Save Listing Update]** 을 클릭합니다.

![누락된 상태를 수동으로 업데이트](assets/amazon-update-listing-missing-condition.png){width="600" zoomable="yes"}
