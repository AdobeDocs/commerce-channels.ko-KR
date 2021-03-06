---
title: 작업 공간 컨트롤
description: Amazon Sales Channel은 작업 공간 컨트롤을 제공하여 목록을 찾고 정보를 보고 작업을 쉽게 적용할 수 있습니다.
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# 작업 공간 컨트롤

Amazon 영업 채널 [홈 페이지](./amazon-sales-channel-home.md) 에는 필터, 기본 보기, 열 및 내보내기를 포함한 몇 가지 일반적인 작업 영역 컨트롤이 있습니다. 일부 페이지에 동일한 제어 옵션이 있는 것은 아닙니다.

![Amazon Sales Channel 작업 공간 제어 예](assets/amazon-workspace-controls.png)

## 작업

다음 _[!UICONTROL Actions]_선택기는 사용자가 페이지에 사용할 수 있는 작업 목록을 제공합니다. 이 옵션을 선택하면 선택한 모든 항목에 작업이 적용됩니다. 특정 항목에 작업을 적용하려면 각 항목의 첫 번째 열에서 확인란을 선택하고 아래에서 옵션을 선택합니다_[!UICONTROL Actions]_.

예를 들어 선택기가 _[!UICONTROL Attributes]_페이지, 다음을 포함합니다_[!UICONTROL Re-import Product Attribute Values]_ 작업. 이 작업을 선택하면 해당 Ping [!DNL Amazon Seller Central] 계정 및 새로 고침 [!DNL Commerce] 왼쪽 열에서 선택된 각 Amazon 저장소 항목에 대한 데이터입니다.

![작업 메뉴 예](assets/amazon-sales-channel-home-actions-option.png)

## 필터

다음 _[!UICONTROL Filters]_컨트롤에는 테이블에 표시된 데이터 범위를 좁히기 위한 옵션이 표시됩니다. 필터 옵션은 열 컨트롤에서 선택한 열을 기준으로 합니다. 필터 옵션은 Columns 컨트롤에서 활성화된 열에 대해서만 표시됩니다.

필터 컨트롤에는 동적 달력이 포함되어 있어 지정된 날짜에 대한 데이터의 범위를 좁힐 수 있으며, 사전 정의된 선택 항목이 있는 열에 대한 드롭다운 메뉴 및 사용자 지정 데이터가 포함될 수 있는 자유 텍스트 필드를 포함할 수 있습니다.

다음 예는 다음 기준을 충족하는 주문만 표시하도록 주문 목록을 필터링하는 설정을 보여줍니다.

- 2/01/2019과 2/07/2019 사이에 수행한 주문
- 구매자가 `Smith`, 및
- 상태가 인 주문 `Shipped`.

필터링 옵션을 설정한 경우 **[!UICONTROL Apply Filters]** 나열된 데이터를 필터링하려면 다음을 수행하십시오. Cancel을 클릭하여 Filters 컨트롤을 적용하지 않고 종료합니다.

![필터 컨트롤 예](assets/workspace-controls-filters.png)

데이터에 필터를 적용하면 **[!UICONTROL Active Filters]** 정보가 표시됩니다. 을(를) 클릭합니다. ![필터 지우기 아이콘](assets/x-icon-clear-filters.png) 아이콘을 클릭하여 특정 필터 옵션을 지우거나 **[!UICONTROL Clear All]** 적용된 모든 필터를 지우려면

![활성 필터 예](assets/applied-filters-line.png)

## 보기

View 컨트롤은 페이지의 기본 열을 기반으로 하므로 Default View라는 이름이 지정됩니다. Columns 컨트롤을 사용하여 사용 가능한 열을 추가하거나 제거할 수 있습니다. 열을 사용자 지정할 때 보기를 View 컨트롤에서 사용자 지정 보기로 저장할 수 있습니다.

페이지에서 열을 추가 또는 제거한 경우 다음이 표시됩니다.

1. 클릭 **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**.

1. 볼 이름을 입력합니다.

1. 사용자 지정 보기를 저장하려면 화살표 아이콘을 클릭합니다.

![컨트롤 보기 예](assets/workspace-controls-view.png)

이 예에서 _주문 Id_ 열이 Column 컨트롤에 추가되고 사용자 지정 보기로 저장됩니다. 사용자 지정 보기 이름이 저장되면 보기의 이름이 _기본 보기_ 을 입력합니다.

에서 원하는 보기를 선택하여 보기 간에 전환할 수 있습니다 _[!UICONTROL View]_메뉴 아래의 제품에서 사용할 수 있습니다.

사용자 정의 뷰를 삭제하거나 이름을 변경하려면 연필 아이콘을 클릭합니다. 그런 다음 다른 이름을 입력하거나 휴지통 아이콘을 클릭하여 사용자 지정 보기를 삭제할 수 있습니다. 기본 보기는 삭제할 수 없습니다.

## 열

열 컨트롤을 사용하면 페이지 표시에서 데이터 열을 추가하거나 제거할 수 있습니다. 각 Amazon 판매 채널 페이지에는 사전 설정된 데이터 열 조합이 있지만 대부분의 페이지에는 사용 가능한 추가 열이 있습니다. 추가 열이 없는 경우에도 기본 열을 표시에서 제거할 수 있습니다.

다음 예제에서는 Columns 컨트롤을 보여 줍니다. 선택한 옵션은 페이지에 표시되는 열 헤더에 해당합니다.

- 페이지에 데이터 열을 추가하려면 확인란을 선택합니다.
- 페이지에서 데이터 열을 제거하려면 확인란을 선택하지 마십시오.

![열 컨트롤 예](assets/workspace-controls-columns.png)

확인란이 즉시 표시됩니다. 페이지를 변경하고 종료하면 페이지가 기본 열 표시로 돌아갑니다. 정기적으로 변경하는 경우 열 변경 내용을 View 컨트롤에서 사용자 정의 보기로 저장할 수 있습니다. 그런 다음 수동으로 열을 추가하거나 제거할 필요 없이 View 컨트롤에서 전환할 수 있습니다.

을(를) 클릭합니다 **[!UICONTROL Reset]** 옵션을 다시 기본 설정으로 설정하거나 **[!UICONTROL Cancel]** 를 입력하여 변경하지 않고 종료할 수 있습니다.

## 내보내기

내보내기 옵션을 사용하면 데이터를 타사 소프트웨어 또는 별도의 데이터베이스로 가져올 수 없는 데이터 파일로 내보낼 수 있습니다. 내보낸 데이터는 표시된 데이터로 제한됩니다. 필요한 경우 Export 컨트롤을 사용하기 전에 열을 추가하거나 제거해야 합니다.

데이터를 내보낼 준비가 되면 내보내기 형식 옵션을 선택하고 을(를) 클릭합니다 **[!UICONTROL Export]**.

- CSV - 일반 텍스트 데이터를 포함하는 쉼표로 구분된 값 파일입니다
- Excel XML - XML 기반의 스프레드시트 데이터 형식(일반적으로 Excel 사용자용으로 사용됨)입니다

생성된 데이터 파일은 다운로드하도록 지정된 폴더에 자동으로 저장됩니다.

![내보내기 제어](assets/workspace-controls-export.png)
