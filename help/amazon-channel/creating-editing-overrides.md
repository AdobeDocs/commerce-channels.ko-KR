---
title: 무시 만들기 및 편집
description: Amazon Sales Channel 무시를 사용하여 변경 사항을 단일 Amazon 목록 또는 여러 목록에 적용합니다.
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 무시 만들기 및 편집

목록을 만들고 재정의하거나 목록에 적용된 무시를 편집하거나 제거할 수 있습니다. 재정의하여 특정 목록에 대해 정의된 값을 설정합니다.

## 단일 목록에 대한 무시 만들기

_[!UICONTROL Create Override]_작업은_[!UICONTROL Inactive]_, _[!UICONTROL Active]_및_[!UICONTROL Ineligible]_ 탭의 목록을 볼 때 사용할 수 있습니다.

1. _[!UICONTROL Products Listings]_페이지(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_및_[!UICONTROL Ineligible]_ 탭)에서 목록을 봅니다.

1. _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**를 클릭하여 제품 목록 무시 페이지를 엽니다.

   ![Amazon 목록 무시 만들기](assets/amazon-select-create-override.png)

1. 올바른 목록을 보고 있는지 확인하려면 _[!UICONTROL Listing Details]_을(를) 확인합니다.

1. 만들고 있는 재정의 유형을 결정합니다.

   단일 대체 유형이나 목록의 유형 조합(가격, 처리 시간, 조건, 판매자 노트)을 정의할 수 있습니다.

   - **가격**  -  **[!UICONTROL Change Listing Price]** 을 클릭하고 정의된 가격 값을  **[!UICONTROL Price Override]**&#x200B;입력합니다.
   - **처리 시간**  -  **[!UICONTROL Change Handling Time]** 을 클릭하고  **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력합니다.
   - **조건**  -  **[!UICONTROL Change Condition]** 을(를) 클릭하고  **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택합니다.
   - **판매자 노트**  -  **[!UICONTROL Change Seller Notes]** 을 클릭하고 노트 텍스트를  **[!UICONTROL Seller Notes Override]**&#x200B;입력합니다.

1. **[!UICONTROL Save Listing Override]** 을 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`으로 변경됩니다. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 목록이_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

다음 예제에서는 새 가격 `$55`, 새 처리 시간 `1 day`, 새 조건 `Used; Like New` 및 새 판매자 메모 텍스트를 정의하는 재지정을 보여 줍니다.

![Amazon 목록 무시 예](assets/amazon-overrides-edit.png)

## 단일 목록에 대한 무시 편집 또는 제거 {#edit-override-single-listing}

_[!UICONTROL Edit Overrides]_작업은_[!UICONTROL Overrides]_ 탭에서 목록을 볼 때 사용할 수 있습니다.

1. _[!UICONTROL Product Listings]_페이지(_[!UICONTROL Overrides]_ 탭)에서 목록을 봅니다.

1. _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**를 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 무시 선택](assets/amazon-select-edit-overrides.png)

1. 올바른 목록을 재정의하려면 _[!UICONTROL Listing Details]_을(를) 확인합니다.

1. _[!UICONTROL Override]_설정을 편집하려면 변경할 유형의 섹션을 정의합니다(가격, 처리 시간, 조건, 판매자 노트).

   대체 유형을 동일하게 유지하려면 `No Change To <override type>` (기본값)을 선택합니다. 이 설정은 이전에 정의한 재정의 값을 그대로 둡니다.

   - **가격**  -  **[!UICONTROL Change Listing Price]** 을 클릭하고 정의된 가격 값을  **[!UICONTROL Price Override]**&#x200B;입력합니다.
   - **처리 시간**  -  **[!UICONTROL Change Handling Time]** 을 클릭하고  **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력합니다.
   - **조건**  -  **[!UICONTROL Change Condition]** 을 클릭하고  **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택합니다.
   - **판매자 노트**  -  **[!UICONTROL Change Seller Notes]** 을 클릭하고 노트 텍스트를  **[!UICONTROL Seller Notes Override]**&#x200B;입력합니다.

1. 재정의 유형을 제거하려면 제거할 각 유형에 대해 **제거**&#x200B;를 클릭합니다. 제거하지 않으면 이전에 정의한 값이 재정의에 유지됩니다.

1. **[!UICONTROL Save Listing Override]** 을 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`으로 변경됩니다. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 아직 나열되지 않은 경우 목록이_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

_Override_ 예제를 만들 때 피기백합니다. 다음 예제에서는 `$50`의 새 가격을 정의하고 처리 시간 무시를 제거하고 이전 조건 및 판매자 메모 무시를 유지하는 이전에 만든 무시를 편집하는 방법을 보여 줍니다.

![무시 편집 또는 제거](assets/amazon-overrides-edit-2.png)
__

## 여러 목록에 대한 무시 편집 또는 제거 {#edit-override-multiple-listings}

_[!UICONTROL Edit Listing Overrides]_작업은_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ 및 _[!UICONTROL Ineligible]_탭에서 사용할 수 있습니다.

>[!NOTE]
>
>여러 목록에 대한 재정의를 수정하려고 하므로 단일 목록을 수정할 때 _[!UICONTROL Listing Details]_섹션이 그대로 표시되지 않습니다.

1. _[!UICONTROL Products Listings]_페이지(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_ 및 _[!UICONTROL Ineligible]_탭)에서 목록을 봅니다.

1. 수정할 각 목록에 대해 왼쪽 열에서 확인란을 선택합니다.

1. _[!UICONTROL Actions]_아래에서&#x200B;**[!UICONTROL Edit Listing Overrides]**를 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 무시 선택](assets/amazon-actions-edit-listing-overrides.png)

1. _[!UICONTROL Override]_설정을 편집하려면 변경할 유형의 섹션을 정의합니다(가격, 처리 시간, 조건, 판매자 노트).

   무시를 동일하게 유지하려면 `No Change To <override type>` (기본값)을 선택합니다. 이 설정은 이전에 정의한 재정의 값을 그대로 둡니다.

   - **가격**  -  **[!UICONTROL Change Listing Price]** 을 클릭하고 정의된 가격 값을  **[!UICONTROL Price Override]**&#x200B;입력합니다.
   - **처리 시간**  -  **[!UICONTROL Change Handling Time]** 을 클릭하고  **[!UICONTROL Handling Time Override]**&#x200B;에 대해 정의된 시간 값(일)을 입력합니다.
   - **조건**  -  **[!UICONTROL Change Condition]** 을 클릭하고  **[!UICONTROL Condition Override]**&#x200B;에 대한 올바른 옵션을 선택합니다.
   - **판매자 노트**  -  **[!UICONTROL Change Seller Notes]** 을 클릭하고 노트 텍스트를  **[!UICONTROL Seller Notes Override]**&#x200B;입력합니다.

1. 재정의 유형을 제거하려면 제거할 각 유형에 대해 **[!UICONTROL Remove]** 을 클릭합니다. 제거하지 않으면 이전에 정의한 값이 재정의에 유지됩니다.

1. **[!UICONTROL Save Listing Override]** 을 클릭합니다.

   _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록 상태가 `Relist in Progress`으로 변경됩니다. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 아직 나열되지 않은 경우 목록이_[!UICONTROL Overrides]_ 탭에도 추가됩니다.

### 무시 유형

| 무시 | 설명 |
|--- |--- |
| [!UICONTROL Price Override] | 가격 대체는 목록의 가격을 정의합니다. 이 재정의는 재정의가 제거될 때까지 모든 자동화된 설정보다 우선합니다.<br><br>제품 가격을 대체하려면 가격 **[!UICONTROL Change Listing Price]** 을 선택하고 신규 가격을  **[!UICONTROL Price Override]**&#x200B;입력합니다. |
| [!UICONTROL Handling Time Override] | 처리 시간은 제품을 처리하고 출하하는 데 걸리는 시간(일)을 정의합니다. 처리 시간 재정의는 재정의가 제거될 때까지 모든 자동화된 처리 시간 설정에 우선합니다.<br><br>상자에  _[!UICONTROL Handling Time Override]_있는 값은 목록 설정에 정의된 기본 처리 시간 또는  [정의된 ](./listing-settings.md) 무시 처리 시간입니다. 처리 시간 대체를 제거하면 기본적으로 목록 설정에 정의된 처리 시간이 표시됩니다.<br><br>처리 시간 대체를 정의하려면 을(**[!UICONTROL Change Handling Time]**를) 선택하고 새 처리 시간(일)을&#x200B;**[!UICONTROL Handling Time Override]**입력합니다. |
| [!UICONTROL Condition Override] | 목록 조건을 무시하려면 **[!UICONTROL Change Condition]**&#x200B;을 선택하고 **조건 무시**&#x200B;에서 새 조건을 선택합니다. |
| [!UICONTROL Seller Notes Override] | 카탈로그의 제품에 대해 `New` 이외의 조건으로 정의된 경우, 판매자 메모를 추가하여 제품과 해당 조건을 잠재 구매자에게 자세히 설명할 수 있습니다. `New` 조건 제품에 대해 판매자 노트 대체를 입력할 수 있지만 Amazon에 노트가 표시되지 않습니다.<br><br>판매자 노트를 대체하려면  **[!UICONTROL Change Seller Notes]** 을 선택하고 새 노트를 입력합니다  **[!UICONTROL Seller Notes Override]**. |
