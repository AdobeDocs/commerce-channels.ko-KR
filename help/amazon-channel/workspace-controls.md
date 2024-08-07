---
title: Amazon 판매 채널 - Workspace 제어
description: Amazon Sales Channel은 목록을 찾고 정보를 보고 작업을 쉽게 적용할 수 있는 작업 영역 컨트롤을 제공합니다.
feature: Sales Channels
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Workspace 컨트롤

Amazon 영업 채널 [홈 페이지](./amazon-sales-channel-home.md)에는 필터, 기본 보기, 열, 내보내기 등 몇 가지 일반적인 작업 영역 컨트롤이 있습니다. 모든 페이지에 동일한 제어 옵션이 있는 것은 아닙니다.

![Amazon Sales Channel 작업 영역 컨트롤 예제](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## 작업

_[!UICONTROL Actions]_선택기는 사용자가 페이지에 사용할 수 있는 작업 목록을 제공합니다. 이 옵션을 선택하면 작업이 선택한 모든 항목에 적용됩니다. 특정 항목에 작업을 적용하려면 각 항목의 첫 번째 열에서 확인란을 선택하고_[!UICONTROL Actions]_&#x200B;에서 옵션을 선택합니다.

예를 들어 선택기가 _[!UICONTROL Attributes]_페이지에 표시되면_[!UICONTROL Re-import Product Attribute Values]_ 작업이 포함됩니다. 이 작업을 선택하면 해당 [!DNL Amazon Seller Central] 계정이 ping되고 왼쪽 열에서 선택한 각 Amazon 스토어 항목에 대한 [!DNL Commerce] 데이터가 새로 고쳐집니다.

![작업 메뉴 예제](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## 필터

_[!UICONTROL Filters]_컨트롤은 표에 표시된 데이터를 좁히는 옵션을 보여 줍니다. 필터 옵션은 열 컨트롤에서 선택한 열을 기준으로 합니다. 필터 옵션은 열 컨트롤에서 활성화된 열에 대해서만 표시됩니다.

필터 컨트롤에는 지정된 날짜에 대한 데이터 범위를 좁히는 동적 달력, 미리 정의된 선택 영역이 있는 열에 대한 드롭다운 메뉴, 사용자 지정 데이터를 포함할 수 있는 자유 텍스트 필드가 포함될 수 있습니다.

다음 예제에서는 다음 기준을 충족하는 주문만 표시하도록 주문 목록을 필터링하는 설정을 보여 줍니다.

- 2019/2/01 및 2019/2/07 사이에 수행된 주문
- 구매자 이름이 `Smith`인 주문 및
- `Shipped` 상태의 주문입니다.

필터링 옵션이 설정되어 있으면 **[!UICONTROL Apply Filters]**&#x200B;을(를) 클릭하여 나열된 데이터를 필터링합니다. Cancel을 클릭하여 적용하지 않고 Filters 컨트롤을 종료합니다.

![필터 컨트롤 예](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

데이터에 필터를 적용하면 **[!UICONTROL Active Filters]** 정보가 표시됩니다. ![필터 지우기 아이콘](assets/x-icon-clear-filters.png) 아이콘을 클릭하여 특정 필터 옵션을 지우거나 **[!UICONTROL Clear All]**&#x200B;을(를) 클릭하여 적용된 모든 필터를 지울 수 있습니다.

![활성 필터 예](assets/applied-filters-line.png){width="700"}

## 보기

View 컨트롤은 페이지의 기본 열을 기반으로 하므로 기본 보기라고 합니다. Columns 컨트롤을 사용하여 사용 가능한 열을 추가하거나 제거할 수 있습니다. 열을 사용자 지정하면 View 컨트롤에 보기를 사용자 지정 보기로 저장할 수 있습니다.

열이 추가되거나 페이지에서 제거되면 다음이 표시됩니다.

1. **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**&#x200B;을(를) 클릭합니다.

1. 보기의 이름을 입력합니다.

1. 사용자 지정 보기를 저장하려면 화살표 아이콘을 클릭합니다.

![보기 컨트롤 예제](assets/workspace-controls-view.png)

이 예제에서는 _Order Id_ 열이 Column 컨트롤에 추가되고 사용자 지정 보기로 저장됩니다. 사용자 지정 보기 이름을 저장한 후 보기 이름이 _기본 보기_&#x200B;에서 입력한 이름으로 변경되었습니다.

_[!UICONTROL View]_메뉴에서 원하는 보기를 선택하여 보기 사이를 전환할 수 있습니다.

사용자 지정 보기의 이름을 삭제하거나 변경하려면 연필 아이콘을 클릭합니다. 그런 다음 다른 이름을 입력하거나 휴지통 아이콘을 클릭하여 사용자 지정 보기를 삭제할 수 있습니다. 기본 보기는 삭제할 수 없습니다.

## 열

열 컨트롤을 사용하면 페이지 표시에서 데이터 열을 추가하거나 제거할 수 있습니다. 각 Amazon 판매 채널 페이지에는 미리 설정된 데이터 열 조합이 있지만 대부분의 페이지에는 추가 열이 있습니다. 사용할 수 있는 추가 열이 없는 경우에도 디스플레이에서 기본 열을 제거할 수 있습니다.

다음 예제에서는 열 컨트롤을 보여 줍니다. 선택한 옵션은 페이지에 표시되는 열 헤더에 해당합니다.

- 페이지에 데이터 열을 추가하려면 확인란을 선택합니다.
- 페이지에서 데이터 열을 제거하려면 확인란을 선택하지 마십시오.

![열 컨트롤 예](assets/workspace-controls-columns.png){width="400"}

확인란 변경 사항이 즉시 표시됩니다. 변경한 후 페이지를 종료하면 페이지가 기본 열 표시로 돌아갑니다. 정기적으로 변경하는 경우 열 변경 내용을 View 컨트롤에 사용자 지정 보기로 저장할 수 있습니다. 그런 다음 열을 수동으로 추가하거나 제거할 필요 없이 View 컨트롤에서 전환할 수 있습니다.

**[!UICONTROL Reset]**&#x200B;을(를) 클릭하여 옵션을 다시 기본 설정으로 설정하거나 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭하여 변경 없이 종료할 수 있습니다.

## 내보내기

내보내기 옵션을 사용하면 데이터를 서드파티 소프트웨어나 별도의 데이터베이스로 가져올 수 있는 데이터 파일로 내보낼 수 있습니다. 내보낸 데이터는 표시된 데이터로 제한됩니다. 필요한 경우 Export 컨트롤을 사용하기 전에 열을 추가하거나 제거해야 합니다.

데이터를 내보낼 준비가 되면 내보내기 형식 옵션을 선택하고 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.

- CSV - 일반 텍스트 데이터를 포함하는 쉼표로 구분된 값 파일
- Excel XML - XML 기반의 스프레드시트 데이터 형식(일반적으로 Excel 사용자에게 사용됨)

생성된 데이터 파일은 다운로드를 위해 지정된 폴더에 자동으로 저장됩니다.

![컨트롤 내보내기](assets/workspace-controls-export.png){width="250"}
