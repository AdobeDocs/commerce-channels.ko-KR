---
title: Amazon 주문 보기
description: Adobe Commerce 또는 Magento Open Source 관리자에서 Amazon Marketplace 주문을 봅니다.
feature: Sales Channels, Orders
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Amazon 주문 보기

Amazon 주문을 보는 방법에는 _[!UICONTROL Recent Orders]_과(와)_[!UICONTROL All Orders]_&#x200B;이(가) 있습니다.

두 옵션 모두 Amazon에서 받은 기본 주문 정보를 보여 줍니다. 여기에는 다음이 포함됩니다.

- 구매 날짜
- 주문 번호
- 상태
- 구매자 이름
- 총계
- 주문 메모

_[!UICONTROL All Orders]_보기는 주문 검색에 대한 필터링 옵션을 추가합니다.

>[!NOTE]
>
>_[!UICONTROL Order Notes]_열을 제외하고_[!UICONTROL Amazon orders]_ 테이블은 Amazon에서 받은 주문 정보로 채워집니다. _주문 메모_ 열은 [!DNL Commerce]에 의해 주문 프로세스에 따라 업데이트됩니다.

## 최근 주문

[스토어 대시보드](./amazon-store-dashboard.md)의 _[!UICONTROL Recent Orders]_섹션에서 가장 최근 주문을 볼 수 있습니다.

![최근 주문](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### 최근 Amazon 주문 보기

1. 저장소 카드에서 **[!UICONTROL View Store]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Recent Orders]_섹션에서 주문을 봅니다.

1. 주문 세부 사항을 보려면 _[!UICONTROL Order Number]_열에서 Amazon 주문 번호를 클릭하십시오.

   주문에 대한 _[!UICONTROL Amazon Order Details]_페이지가 열립니다.

## 모든 주문 보기

_[!UICONTROL Amazon orders]_페이지에서 모든 Amazon 주문을 볼 수 있습니다(_[!UICONTROL All Orders]_ 보기라고도 함). Amazon 주문 테이블은 스토어 대시보드의 _[!UICONTROL Recent Orders]_섹션과 유사하지만 다음 필터 옵션을 사용하여 모든 Amazon 주문을 보고 주문 목록의 범위를 좁힐 수 있습니다.

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon 주문](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### 모든 Amazon 주문 보기

1. 저장소 카드에서 **[!UICONTROL View Store]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Recent Orders]_섹션에서&#x200B;**[!UICONTROL All Orders]**을(를) 클릭합니다.

1. 목록의 범위를 좁히거나 특정 주문 번호를 검색하려면 **[!UICONTROL Filter by]** 매개 변수를 완료하고 **[!UICONTROL Apply filters]**&#x200B;을(를) 클릭하십시오.

1. 주문 세부 사항을 보려면 _[!UICONTROL Order Number]_열에서 Amazon 주문 번호를 클릭하십시오.

   주문에 대한 _[!UICONTROL Amazon Order Details]_페이지가 열립니다.

## 필터 사용

_[!UICONTROL Filter by]_섹션의 주문 목록에 필터를 적용할 수 있습니다. 선택한 다음&#x200B;**[!UICONTROL Apply filters]**을(를) 클릭합니다. 적용된 필터가 주문 그리드 위에 나타납니다.

![Amazon 주문 보기용 필터](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### 적용된 필터 변경

- _[!UICONTROL Filter by]_섹션에서 필터를 추가하거나 변경할 수 있습니다.**[!UICONTROL Apply filters]**을(를) 클릭하여 주문 목록 및 주문 표 위에 표시되는 필터 옵션을 업데이트합니다.

- 필터에 대한 `x`을(를) 클릭하여 한 번에 하나씩 또는 **[!UICONTROL Clear all filters]**&#x200B;을(를) 클릭하여 한 번에 모두 필터를 제거할 수 있습니다. 필터를 제거하면 주문 그리드 위에 표시되는 주문 목록과 필터 옵션이 업데이트됩니다.

- 주문 목록이 길면 그리드 아래의 페이지 매김 컨트롤을 사용하여 더 많은 주문을 볼 수 있습니다.

>[!TIP]
>
>주문 보기에 대한 몇 가지 팁입니다.
>
>- 여러 Amazon 스토어 통합이 있는 경우 스토어 보기 간을 전환할 때 페이지 보기를 새로 고치면 현재 스토어에 대한 주문 목록과 페이지 매김 보기가 모두 업데이트될 수 있습니다.
>- 열을 기준으로 정렬하는 경우 정렬은 현재 목록 보기에만 적용됩니다. 목록을 필터링한 다음 보고 있는 페이지를 정렬하는 것이 좋습니다.
>- 보기 창의 너비에 따라 열에 텍스트가 겹칠 수 있습니다. 줄 바꿈할 텍스트의 열을 확장하려면 창 보기를 넓힙니다.
>- _[!UICONTROL Total]_을(를) 기준으로 필터링할 때는 정수를 기준으로 필터링하십시오. 소수를 입력하면 결과에 오류가 발생할 수 있습니다.

### 기본 열

| 열 | 설명 |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Filter by] | _[!UICONTROL All Orders]_보기에서만 사용할 수 있습니다.<br>다음을 기준으로 주문 목록 좁히기:<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | Amazon에서 받은 구매 날짜. |
| [!UICONTROL Order Number] | Amazon에서 생성 및 수신한 주문 번호. Amazon 주문 세부 사항 화면을 보려면 링크를 클릭합니다. |
| [!UICONTROL Status] | Amazon에서 받은 주문 상태. 옵션: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Amazon에서 받은 주문자의 이름입니다. |
| [!UICONTROL Grand Total] | Amazon에서 받은 주문의 총 통화 값입니다. |
| [!UICONTROL Order Notes] | [!DNL Commerce]에서 처리할 때 주문에 대해 가장 최근에 기록된 작업입니다. 정보에는 주문 가져오기 오류 및 주문 처리 업데이트가 포함되지만 이에 국한되지 않습니다.<br>**참고**: 이 필드는 [!DNL Commerce]에 의해 주문 처리로 업데이트됩니다. |
