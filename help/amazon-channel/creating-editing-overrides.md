---
title: Amazon 판매 채널 재정의 만들기 및 편집
description: Amazon Sales Channel 재정의를 사용하여 단일 Amazon 목록 또는 여러 목록에 변경 사항을 적용합니다.
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 0%

---

# 재정의 만들기 및 편집

목록을 만들고 재정의하거나 목록에 적용된 재정의를 편집하거나 제거할 수 있습니다. 재정의는 특정 목록에 대해 정의된 값을 설정합니다.

## 단일 목록에 대한 재정의 만들기

다음 _[!UICONTROL Create Override]_작업은에서 목록을 볼 때 사용할 수 있습니다._[!UICONTROL Inactive]_, _[!UICONTROL Active]_, 및_[!UICONTROL Ineligible]_ 탭.

1. 다음에서 목록 보기 _[!UICONTROL Products Listings]_페이지 (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, 및_[!UICONTROL Ineligible]_ 탭).

1. 다음에서 _[!UICONTROL Action]_열, 클릭&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**제품 목록 무시 페이지를 엽니다.

   ![Amazon 목록 재정의 만들기](assets/amazon-select-create-override.png){width="220"}

1. 올바른 목록이 표시되는지 확인하려면 다음을 확인하십시오. _[!UICONTROL Listing Details]_.

1. 생성 중인 재정의 유형을 결정합니다.

   목록에 대해 단일 대체 유형 또는 유형의 조합(가격, 처리 시간, 조건, 판매자 노트)을 정의할 수 있습니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 다음에 대해 정의된 가격 값 입력 **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 및 다음에 대해 정의된 시간 값(일)을 입력합니다. **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 올바른 옵션을 선택합니다. **[!UICONTROL Condition Override]**.
   - **판매자 메모** - 클릭 **[!UICONTROL Change Seller Notes]** 다음에 대한 메모 텍스트 입력 **[!UICONTROL Seller Notes Override]**.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지를 닫습니다. 목록의 상태가 다음으로 변경됩니다. `Relist in Progress`. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 목록은 에도 추가됩니다._[!UICONTROL Overrides]_ 탭.

다음 예제는 새 가격을 정의하는 재정의를 보여 줍니다. `$55`, 다음의 새로운 처리 시간 `1 day`, 의 새로운 조건 `Used; Like New`및 새 판매자 노트 텍스트입니다.

![Amazon 목록 재정의 예](assets/amazon-overrides-edit.png){width="600" zoomable="yes"}

## 단일 목록에 대한 재정의 편집 또는 제거 {#edit-override-single-listing}

다음 _[!UICONTROL Edit Overrides]_작업은에서 목록을 볼 때 사용할 수 있습니다._[!UICONTROL Overrides]_ 탭.

1. 다음에서 목록 보기: _[!UICONTROL Product Listings]_페이지 (_[!UICONTROL Overrides]_ 탭).

1. 다음에서 _[!UICONTROL Action]_열, 클릭&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 재정의 선택](assets/amazon-select-edit-overrides.png){width="125"}

1. 올바른 목록을 재정의하려면 다음을 확인하십시오. _[!UICONTROL Listing Details]_.

1. 을(를) 편집하려면 _[!UICONTROL Override]_설정에서 변경할 유형(가격, 처리 시간, 조건, 판매자 노트)의 섹션을 정의합니다.

   재정의 유형을 동일하게 유지하려면 `No Change To <override type>` (기본값). 이 설정은 이전에 정의된 재정의 값을 변경하지 않고 그대로 둡니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 다음에 대해 정의된 가격 값 입력 **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 및 다음에 대해 정의된 시간 값(일)을 입력합니다. **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 올바른 옵션을 선택합니다. **[!UICONTROL Condition Override]**.
   - **판매자 메모** - 클릭 **[!UICONTROL Change Seller Notes]** 다음에 대한 메모 텍스트 입력 **[!UICONTROL Seller Notes Override]**.

1. 재정의 유형을 제거하려면 **제거** 제거할 각 유형에 대해. 제거하지 않으면 이전에 정의한 값이 재정의에 그대로 유지됩니다.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지를 닫습니다. 목록의 상태가 다음으로 변경됩니다. `Relist in Progress`. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 아직 나열되지 않은 경우 목록도_[!UICONTROL Overrides]_ 탭.

에 피기백 _재정의 만들기_ 예. 다음 예제는 새 가격을 정의하는 이전에 만든 재정의에 대한 편집을 보여 줍니다. `$50`는 처리 시간 재정의를 제거하고 이전 조건 및 판매자 노트 재정의를 유지합니다.

![무시 편집 또는 제거](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## 여러 목록의 재정의 편집 또는 제거 {#edit-override-multiple-listings}

다음 _[!UICONTROL Edit Listing Overrides]_작업은 다음에서 사용할 수 있습니다._[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_, 및 _[!UICONTROL Ineligible]_탭.

>[!NOTE]
>
>여러 목록에 대한 재정의를 수정하고 있으므로 _[!UICONTROL Listing Details]_섹션은 단일 목록을 수정할 때처럼 표시되지 않습니다.

1. 다음에서 목록 보기: _[!UICONTROL Products Listings]_페이지 (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_, 및 _[!UICONTROL Ineligible]_탭).

1. 수정할 각 목록에 대해 왼쪽 열에서 확인란을 선택합니다.

1. 아래 _[!UICONTROL Actions]_, 클릭&#x200B;**[!UICONTROL Edit Listing Overrides]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지가 열립니다.

   ![Amazon 목록 재정의 선택](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. 을(를) 편집하려면 _[!UICONTROL Override]_설정에서 변경할 유형(가격, 처리 시간, 조건, 판매자 노트)의 섹션을 정의합니다.

   재정의를 동일하게 유지하려면 다음을 선택합니다. `No Change To <override type>` (기본값). 이 설정은 이전에 정의된 재정의 값을 변경하지 않고 그대로 둡니다.

   - **가격** - 클릭 **[!UICONTROL Change Listing Price]** 다음에 대해 정의된 가격 값 입력 **[!UICONTROL Price Override]**.
   - **처리 시간** - 클릭 **[!UICONTROL Change Handling Time]** 및 다음에 대해 정의된 시간 값(일)을 입력합니다. **[!UICONTROL Handling Time Override]**.
   - **조건** - 클릭 **[!UICONTROL Change Condition]** 올바른 옵션을 선택합니다. **[!UICONTROL Condition Override]**.
   - **판매자 메모** - 클릭 **[!UICONTROL Change Seller Notes]** 다음에 대한 메모 텍스트 입력 **[!UICONTROL Seller Notes Override]**.

1. 재정의 유형을 제거하려면 **[!UICONTROL Remove]** 제거할 각 유형에 대해. 제거하지 않으면 이전에 정의한 값이 재정의에 그대로 유지됩니다.

1. 클릭 **[!UICONTROL Save Listing Override]**.

   다음 _[!UICONTROL Product Listing Overrides]_페이지를 닫습니다. 목록의 상태가 (으)로 변경됩니다. `Relist in Progress`. 변경 사항은 다음 데이터 동기화와 함께 Amazon에 게시됩니다(cron 설정에 구성된 대로). 아직 나열되지 않은 경우 목록도_[!UICONTROL Overrides]_ 탭.

### 재정의 유형

| 오버라이드 | 설명 |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | 가격 재정의는 목록의 가격을 정의합니다. 이 무시는 무시가 제거될 때까지 모든 자동화된 설정에 우선합니다.<br><br>제품의 가격을 오버라이드하려면 **[!UICONTROL Change Listing Price]** 다음에 대한 새 가격을 입력합니다. **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | 처리 시간 재정의는 제품을 처리하고 출하하는 데 걸리는 시간(일)을 정의합니다. 처리 시간 재정의는 재정의가 제거될 때까지 모든 자동화된 처리 시간 설정 및 기본 처리 시간 설정에 우선합니다.<br><br>에 있는 값 _[!UICONTROL Handling Time Override]_box는에 정의된 기본 처리 시간입니다. [목록 설정](./listing-settings.md) 또는 정의된 재정의 처리 시간. 처리 시간 무시를 제거하면 목록 설정에 정의된 처리 시간이 기본값으로 설정됩니다.<br><br>처리 시간 재정의를 정의하려면 다음을 선택합니다.**[!UICONTROL Change Handling Time]**다음에 대한 새 처리 시간(일)을 입력합니다.**[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | 목록 조건을 재정의하려면 **[!UICONTROL Change Condition]** 새 조건 선택 **조건 재정의**. |
| [!UICONTROL Seller Notes Override] | 다음 이외의 조건으로 정의된 카탈로그의 제품 `New`, 판매자 노트를 추가하여 잠재적 구매자에게 제품 및 상태에 대해 자세히 설명할 수 있습니다. 다음에 대한 판매자 메모 재정의를 입력할 수 있습니다. `New` 조건 제품이지만 Amazon에 메모가 표시되지 않습니다.<br><br>판매자 노트를 대체하려면 다음을 선택합니다. **[!UICONTROL Change Seller Notes]** 다음에 대한 새 메모 입력 **[!UICONTROL Seller Notes Override]**. |
