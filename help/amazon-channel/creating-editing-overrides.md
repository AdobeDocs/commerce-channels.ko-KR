---
title: Amazon 판매 채널 재정의 만들기 및 편집
description: Amazon Sales Channel 재정의를 사용하여 단일 Amazon 목록 또는 여러 목록에 변경 사항을 적용합니다.
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# 재정의 만들기 및 편집

목록을 만들고 재정의하거나 목록에 적용된 재정의를 편집하거나 제거할 수 있습니다. 재정의는 특정 목록에 대해 정의된 값을 설정합니다.

## 단일 목록에 대한 재정의 만들기

_[!UICONTROL Inactive]_,_[!UICONTROL Active]_ 및 _[!UICONTROL Ineligible]_탭에서 목록을 볼 때_[!UICONTROL Create Override]_ 작업을 사용할 수 있습니다.

1. _[!UICONTROL Products Listings]_페이지에서 목록을 봅니다(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_및_[!UICONTROL Ineligible]_ 탭).

1. _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**을(를) 클릭하여 제품 목록 무시 페이지를 엽니다.

   ![Amazon 목록 재정의 만들기](assets/amazon-select-create-override.png){width="220"}

1. 올바른 목록을 보려면 _[!UICONTROL Listing Details]_을(를) 확인하십시오.

1. 생성 중인 재정의 유형을 결정합니다.

   목록에 대해 단일 대체 유형 또는 유형의 조합(가격, 처리 시간, 조건, 판매자 노트)을 정의할 수 있습니다.

   - **가격** - **[!UICONTROL Change Listing Price]**&#x200B;을(를) 클릭하고 **[!UICONTROL Price Override]**&#x200B;에 대해 정의된 가격 값을 입력하십시오.
   - **처리 시간** - **[!UICONTROL Change Handling Time]**&#x200B;을(를) 클릭하고 **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력하십시오.
   - **조건** - **[!UICONTROL Change Condition]**&#x200B;을(를) 클릭하고 **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택하십시오.
   - **판매자 메모** - **[!UICONTROL Change Seller Notes]**&#x200B;을(를) 클릭하고 **[!UICONTROL Seller Notes Override]**&#x200B;에 대한 메모 텍스트를 입력하십시오.

1. **[!UICONTROL Save Listing Override]**&#x200B;을(를) 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`(으)로 변경됩니다. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 목록은_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

다음 예제에서는 새 가격 `$55`, 새 처리 시간 `1 day`, 새 조건 `Used; Like New` 및 새 판매자 메모 텍스트를 정의하는 재정의를 보여 줍니다.

![Amazon 목록 재정의 예](assets/amazon-overrides-edit.png){width="600" zoomable="yes"}

## 단일 목록에 대한 재정의 편집 또는 제거 {#edit-override-single-listing}

_[!UICONTROL Overrides]_탭에서 목록을 볼 때_[!UICONTROL Edit Overrides]_ 작업을 사용할 수 있습니다.

1. _[!UICONTROL Product Listings]_페이지에서 목록을 봅니다(_[!UICONTROL Overrides]_ 탭).

1. _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**을(를) 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 재정의 선택](assets/amazon-select-edit-overrides.png){width="125"}

1. 올바른 목록을 재정의하려면 _[!UICONTROL Listing Details]_을(를) 확인하십시오.

1. _[!UICONTROL Override]_설정을 편집하려면 변경할 유형(가격, 처리 시간, 조건, 판매자 노트)의 섹션을 정의하세요.

   재정의 형식을 동일하게 유지하려면 `No Change To <override type>`(기본값)을(를) 선택합니다. 이 설정은 이전에 정의된 재정의 값을 변경하지 않고 그대로 둡니다.

   - **가격** - **[!UICONTROL Change Listing Price]**&#x200B;을(를) 클릭하고 **[!UICONTROL Price Override]**&#x200B;에 대해 정의된 가격 값을 입력하십시오.
   - **처리 시간** - **[!UICONTROL Change Handling Time]**&#x200B;을(를) 클릭하고 **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력하십시오.
   - **조건** - **[!UICONTROL Change Condition]**&#x200B;을(를) 클릭하고 **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택하십시오.
   - **판매자 메모** - **[!UICONTROL Change Seller Notes]**&#x200B;을(를) 클릭하고 **[!UICONTROL Seller Notes Override]**&#x200B;에 대한 메모 텍스트를 입력하십시오.

1. 재정의 형식을 제거하려면 제거할 각 형식에 대해 **제거**&#x200B;를 클릭하십시오. 제거하지 않으면 이전에 정의한 값이 재정의에 그대로 유지됩니다.

1. **[!UICONTROL Save Listing Override]**&#x200B;을(를) 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`(으)로 변경됩니다. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 아직 나열되지 않은 경우 목록이_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

_재정의 만들기_ 예제를 피기백합니다. 다음 예제에서는 새 가격 `$50`을(를) 정의하고 처리 시간 재정의를 제거하며 이전 조건 및 판매자 노트 재정의를 유지하는 이전에 만든 재정의에 대한 편집 방법을 보여 줍니다.

![재정의 편집 또는 제거](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## 여러 목록의 재정의 편집 또는 제거 {#edit-override-multiple-listings}

_[!UICONTROL Edit Listing Overrides]_작업은_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ 및 _[!UICONTROL Ineligible]_탭에서 사용할 수 있습니다.

>[!NOTE]
>
>여러 목록에 대한 재정의를 수정하고 있으므로 _[!UICONTROL Listing Details]_섹션이 단일 목록을 수정할 때처럼 표시되지 않습니다.

1. _[!UICONTROL Products Listings]_페이지(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ 및 _[!UICONTROL Ineligible]_탭)에서 목록을 봅니다.

1. 수정할 각 목록에 대해 왼쪽 열에서 확인란을 선택합니다.

1. _[!UICONTROL Actions]_에서&#x200B;**[!UICONTROL Edit Listing Overrides]**을(를) 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 재정의 선택](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. _[!UICONTROL Override]_설정을 편집하려면 변경할 유형(가격, 처리 시간, 조건, 판매자 노트)의 섹션을 정의하세요.

   재정의를 동일하게 유지하려면 `No Change To <override type>`(기본값)을(를) 선택합니다. 이 설정은 이전에 정의된 재정의 값을 변경하지 않고 그대로 둡니다.

   - **가격** - **[!UICONTROL Change Listing Price]**&#x200B;을(를) 클릭하고 **[!UICONTROL Price Override]**&#x200B;에 대해 정의된 가격 값을 입력하십시오.
   - **처리 시간** - **[!UICONTROL Change Handling Time]**&#x200B;을(를) 클릭하고 **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력하십시오.
   - **조건** - **[!UICONTROL Change Condition]**&#x200B;을(를) 클릭하고 **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택하십시오.
   - **판매자 메모** - **[!UICONTROL Change Seller Notes]**&#x200B;을(를) 클릭하고 **[!UICONTROL Seller Notes Override]**&#x200B;에 대한 메모 텍스트를 입력하십시오.

1. 재정의 형식을 제거하려면 제거할 각 형식에 대해 **[!UICONTROL Remove]**&#x200B;을(를) 클릭합니다. 제거하지 않으면 이전에 정의한 값이 재정의에 그대로 유지됩니다.

1. **[!UICONTROL Save Listing Override]**&#x200B;을(를) 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`(으)로 변경됩니다. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 아직 나열되지 않은 경우 목록이_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

### 재정의 유형

| 오버라이드 | 설명 |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | 가격 재정의는 목록의 가격을 정의합니다. 이 무시는 무시가 제거될 때까지 모든 자동화된 설정에 우선합니다.<br><br>제품 가격을 재정의하려면 **[!UICONTROL Change Listing Price]**&#x200B;을(를) 선택하고 **[!UICONTROL Price Override]**&#x200B;의 새 가격을 입력하십시오. |
| [!UICONTROL Handling Time Override] | 처리 시간 재정의는 제품을 처리하고 출하하는 데 걸리는 시간(일)을 정의합니다. 처리 시간 재정의는 재정의가 제거될 때까지 모든 자동화된 처리 시간 설정 및 기본 처리 시간 설정에 우선합니다.<br><br>_[!UICONTROL Handling Time Override]_상자에 있는 값은 [설정 나열](./listing-settings.md)에 정의된 기본 처리 시간 또는 정의된 재정의 처리 시간입니다. 처리 시간 무시를 제거하면 목록 설정에 정의된 처리 시간이 기본값으로 설정됩니다.<br><br>처리 시간 재정의를 정의하려면&#x200B;**[!UICONTROL Change Handling Time]**을(를) 선택하고&#x200B;**[!UICONTROL Handling Time Override]**의 새 처리 시간(일)을 입력하십시오. |
| [!UICONTROL Condition Override] | 목록 조건을 재정의하려면 **[!UICONTROL Change Condition]**&#x200B;을(를) 선택하고 **조건 재정의**&#x200B;에서 새 조건을 선택합니다. |
| [!UICONTROL Seller Notes Override] | `New` 이외의 조건으로 정의된 카탈로그의 제품에 대해 판매자 메모를 추가하여 잠재적 구매자에게 제품 및 해당 조건을 자세히 설명할 수 있습니다. `New` 조건 제품에 대한 판매자 메모 재정의를 입력할 수 있지만 Amazon은 메모를 표시하지 않습니다.<br><br>판매자 메모를 재정의하려면 **[!UICONTROL Change Seller Notes]**&#x200B;을(를) 선택하고 **[!UICONTROL Seller Notes Override]**&#x200B;에 대한 새 메모를 입력하십시오. |
