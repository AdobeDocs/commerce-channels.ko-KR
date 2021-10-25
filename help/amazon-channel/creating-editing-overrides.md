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

다음 _[!UICONTROL Create Override]_작업은 목록을 볼 때 사용할 수 있습니다_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, 및_[!UICONTROL Ineligible]_ 탭.

1. 에서 목록 보기 _[!UICONTROL Products Listings]_페이지 (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, 및_[!UICONTROL Ineligible]_ 탭).

1. 에서 _[!UICONTROL Action]_열,**[!UICONTROL Select]**>**[!UICONTROL Create Override]**제품 목록 무시 페이지를 엽니다.

   ![Amazon 목록 무시 만들기](assets/amazon-select-create-override.png)

1. 올바른 목록을 보고 있는지 확인하려면 _[!UICONTROL Listing Details]_.

1. 만들고 있는 재정의 유형을 결정합니다.

   단일 대체 유형이나 목록의 유형 조합(가격, 처리 시간, 조건, 판매자 노트)을 정의할 수 있습니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 에 대해 정의된 가격 값을 입력합니다. **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 에 대해 정의된 시간 값(일)을 입력합니다 **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 그리고 **[!UICONTROL Condition Override]**.
   - **판매자 노트** - 클릭 **[!UICONTROL Change Seller Notes]** 메모에 대한 **[!UICONTROL Seller Notes Override]**.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 목록은 또한_[!UICONTROL Overrides]_ 탭.

다음 예에서는 `$55`, 의 새로운 처리 시간 `1 day`, 의 새로운 조건 `Used; Like New`, 새 판매자 노트 텍스트.

![Amazon 목록 무시 예](assets/amazon-overrides-edit.png)

## 단일 목록에 대한 무시 편집 또는 제거 {#edit-override-single-listing}

다음 _[!UICONTROL Edit Overrides]_작업은 목록을 볼 때 사용할 수 있습니다_[!UICONTROL Overrides]_ 탭.

1. 다음 위치에서 목록 보기 _[!UICONTROL Product Listings]_페이지 (_[!UICONTROL Overrides]_ 탭).

1. 에서 _[!UICONTROL Action]_열,**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 무시 선택](assets/amazon-select-edit-overrides.png)

1. 올바른 목록을 재정의하려면 _[!UICONTROL Listing Details]_.

1. 을 편집하려면 _[!UICONTROL Override]_설정을 사용하여 변경할 유형의 섹션을 정의합니다(가격, 처리 시간, 조건, 판매자 노트).

   무시 유형을 동일하게 유지하려면 `No Change To <override type>` (기본값) 이 설정은 이전에 정의한 재정의 값을 그대로 둡니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 에 대해 정의된 가격 값을 입력합니다. **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 에 대해 정의된 시간 값(일)을 입력합니다 **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 그리고 다음 옵션을 선택합니다. **[!UICONTROL Condition Override]**.
   - **판매자 노트** - 클릭 **[!UICONTROL Change Seller Notes]** 메모에 대한 **[!UICONTROL Seller Notes Override]**.

1. 무시 유형을 제거하려면 **제거** 제거할 각 유형에 대해 제거하지 않으면 이전에 정의한 값이 재정의에 유지됩니다.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록의 상태가 `Relist in Progress`. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 아직 나열되지 않은 경우 목록도_[!UICONTROL Overrides]_ 탭.

피기백 _무시 만들기_ 예. 다음 예제에서는 새 가격을 정의하는 이전에 생성한 재정의에 대한 편집을 보여 줍니다 `$50`를 지정하면 처리 시간 재정의가 제거되고 이전 조건 및 판매자 메모 재정의가 유지됩니다.

![무시 편집 또는 제거](assets/amazon-overrides-edit-2.png)
__

## 여러 목록에 대한 무시 편집 또는 제거 {#edit-override-multiple-listings}

다음 _[!UICONTROL Edit Listing Overrides]_작업은_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_, 및 _[!UICONTROL Ineligible]_탭.

>[!NOTE]
>
>여러 목록에 대한 재정의를 수정하기 때문에 _[!UICONTROL Listing Details]_단일 목록을 수정할 때처럼 섹션이 표시되지 않습니다.

1. 에서 목록 보기 _[!UICONTROL Products Listings]_페이지 (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_, 및 _[!UICONTROL Ineligible]_탭).

1. 수정할 각 목록에 대해 왼쪽 열에서 확인란을 선택합니다.

1. 아래 _[!UICONTROL Actions]_를 클릭합니다.**[!UICONTROL Edit Listing Overrides]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 무시 선택](assets/amazon-actions-edit-listing-overrides.png)

1. 을 편집하려면 _[!UICONTROL Override]_설정을 사용하여 변경할 유형의 섹션을 정의합니다(가격, 처리 시간, 조건, 판매자 노트).

   무시를 동일하게 유지하려면 `No Change To <override type>` (기본값) 이 설정은 이전에 정의한 재정의 값을 그대로 둡니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 에 대해 정의된 가격 값을 입력합니다. **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 에 대해 정의된 시간 값(일)을 입력합니다 **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 그리고 다음 옵션을 선택합니다. **[!UICONTROL Condition Override]**.
   - **판매자 노트** - 클릭 **[!UICONTROL Change Seller Notes]** 메모에 대한 **[!UICONTROL Seller Notes Override]**.

1. 무시 유형을 제거하려면 **[!UICONTROL Remove]** 제거할 각 유형에 대해 제거하지 않으면 이전에 정의한 값이 재정의에 유지됩니다.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 닫힙니다. 목록 상태가 `Relist in Progress`. 변경 사항이 다음 데이터 동기화를 사용하여 Amazon에 게시됩니다(크론 설정에 구성된 대로). 아직 나열되지 않은 경우 목록도_[!UICONTROL Overrides]_ 탭.

### 무시 유형

| 무시 | 설명 |
|--- |--- |
| [!UICONTROL Price Override] | 가격 대체는 목록의 가격을 정의합니다. 이 재정의는 재정의가 제거될 때까지 모든 자동화된 설정보다 우선합니다.<br><br>제품 가격을 변경하려면 **[!UICONTROL Change Listing Price]** 새 가격 입력 **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | 처리 시간은 제품을 처리하고 출하하는 데 걸리는 시간(일)을 정의합니다. 처리 시간 재정의는 재정의가 제거될 때까지 모든 자동화된 처리 시간 설정에 우선합니다.<br><br>에 있는 값 _[!UICONTROL Handling Time Override]_상자는 [목록 설정](./listing-settings.md) 또는 정의된 재정의 처리 시간을 지정합니다. 처리 시간 대체를 제거하면 기본적으로 목록 설정에 정의된 처리 시간이 표시됩니다.<br><br>처리 시간 무시를 정의하려면&#x200B;**[!UICONTROL Change Handling Time]**에 대한 새 처리 시간(일)을 입력합니다.**[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | 목록 조건을 재정의하려면 **[!UICONTROL Change Condition]** 새 조건을 선택하고 **조건 무시**. |
| [!UICONTROL Seller Notes Override] | 카탈로그에 있는 제품 중 이외의 조건으로 정의된 제품의 경우 `New`를 추가할 수 있습니다. 판매자 메모를 추가하여 제품과 해당 조건을 잠재 구매자에게 자세히 설명합니다. 판매자 노트 대체를 입력할 수 있습니다 `New` 조건 제품이지만 Amazon에 노트가 표시되지 않습니다.<br><br>판매자 노트를 재정의하려면 **[!UICONTROL Change Seller Notes]** 다음에 대한 새 메모를 입력합니다. **[!UICONTROL Seller Notes Override]**. |
