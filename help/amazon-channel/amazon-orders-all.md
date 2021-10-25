---
title: Amazon 주문 보기
description: Adobe Commerce 또는 Magento Open Source 관리자에서 Amazon Marketplace 주문을 봅니다.
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Amazon 주문 보기

Amazon 주문을 보는 방법에는 두 가지가 있습니다. _[!UICONTROL Recent Orders]_및_[!UICONTROL All Orders]_.

두 옵션 모두 다음을 포함하여 Amazon에서 수신한 기본 주문 정보를 보여줍니다.

- 구매 날짜
- 주문 번호
- 상태
- 구매자 이름
- 총계
- 주문 정보

_[!UICONTROL All Orders]_보기 는 주문 검색에 대한 필터링 옵션을 추가합니다.

>[!NOTE]
>
>제외 _[!UICONTROL Order Notes]_열,_[!UICONTROL Amazon orders]_ 표는 Amazon에서 받은 주문 정보로 채워집니다. 다음 _주문 정보_ 열 업데이트 기준 [!DNL Commerce] 를 주문 프로세스의 일부로 표시합니다.

## 최근 주문

에서 최근 주문을 볼 수 있습니다 _[!UICONTROL Recent Orders]_섹션 [대시보드 저장](./amazon-store-dashboard.md).

![최근 주문](assets/amazon-recent-orders-imported.png)

### 최근 Amazon 주문 보기

1. 클릭 **[!UICONTROL View Store]** 매장 카드 위에

1. 에서 주문 보기 _[!UICONTROL Recent Orders]_섹션을 참조하십시오.

1. 주문 세부 사항을 보려면 _[!UICONTROL Order Number]_열.

   다음 _[!UICONTROL Amazon Order Details]_주문 페이지가 열립니다.

## 모든 주문 보기

모든 Amazon 주문을 _[!UICONTROL Amazon orders]_페이지(이하 &quot;페이지&quot;라고도 함)_[!UICONTROL All Orders]_ 보기). Amazon 주문 테이블은 다음과 유사합니다 _[!UICONTROL Recent Orders]_섹션에 있는 저장소 대시보드의 모든 섹션을 볼 수 있지만 다음 필터 옵션을 사용하여 주문 목록의 범위를 좁힐 수 있습니다.

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon 주문](assets/amazon-orders-list-all.png)

### 모든 Amazon 주문 보기

1. 클릭 **[!UICONTROL View Store]** 매장 카드 위에

1. 클릭 **[!UICONTROL All Orders]** 에서 _[!UICONTROL Recent Orders]_섹션을 참조하십시오.

1. 목록의 범위를 좁히거나 특정 주문 번호를 검색하려면 **[!UICONTROL Filter by]** 매개 변수 및 클릭 **[!UICONTROL Apply filters]**.

1. 주문 세부 사항을 보려면 _[!UICONTROL Order Number]_열.

   다음 _[!UICONTROL Amazon Order Details]_주문 페이지가 열립니다.

## 필터 사용

필터를에서 주문 목록에 적용할 수 있습니다 _[!UICONTROL Filter by]_섹션을 참조하십시오. 선택한 후 을 클릭합니다&#x200B;**[!UICONTROL Apply filters]**. 적용된 필터가 주문 그리드 위에 나타납니다.

![Amazon 주문 보기를 위한 필터](assets/amazon-orders-filter-view.png)

### 적용된 필터 변경

- 에서 필터에 추가하거나 변경할 수 있습니다 _[!UICONTROL Filter by]_섹션을 참조하십시오. 클릭&#x200B;**[!UICONTROL Apply filters]**주문 목록 및 주문 그리드 위에 나타나는 필터 옵션을 갱신하려면 다음을 수행합니다.

- 필터를 한 번에 한 번씩 `x` 을 클릭하거나 **[!UICONTROL Clear all filters]**. 필터를 제거하면 주문 그리드 위에 나타나는 주문 목록과 필터 옵션이 업데이트됩니다.

- 주문 목록이 길면 그리드 아래의 페이지 매김 컨트롤을 사용하여 더 많은 주문을 볼 수 있습니다.

>[!TIP]
>
>주문 보기에 대한 몇 가지 팁입니다.
>
>- 여러 Amazon 스토어 통합이 있는 경우, 현재 저장소에 대한 주문 목록과 페이지 매김 보기를 모두 업데이트하는 데 저장소 보기 간을 전환할 때 페이지 보기를 새로 고쳐야 할 수 있습니다.
>- 열별로 정렬하면 정렬이 현재 목록 보기에만 적용됩니다. 목록을 필터링한 다음 보고 있는 페이지를 정렬하는 것이 가장 좋습니다.
>- 뷰 창의 너비에 따라 열에 텍스트가 겹칠 수 있습니다. 텍스트 줄바꿈용 열을 확장하려면 창 보기를 확장합니다.
>- 필터링 기준 _[!UICONTROL Total]_를 정수로 필터링합니다. 소수점 값을 입력하면 결과에 오류가 발생할 수 있습니다.


### 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Filter by] | 에서만 사용 가능 _[!UICONTROL All Orders]_보기.<br>다음을 기준으로 주문 목록 범위를 좁힙니다.<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | Amazon에서 받은 구매 날짜입니다. |
| [!UICONTROL Order Number] | Amazon에서 생성 및 수신된 주문 번호입니다. Amazon 주문 세부 사항 화면을 보려면 링크를 클릭합니다. |
| [!UICONTROL Status] | Amazon에서 받은 주문의 상태입니다. 옵션: `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | Amazon에서 받은 주문 대상자의 이름입니다. |
| [!UICONTROL Grand Total] | Amazon에서 받은 주문의 총 통화 값입니다. |
| [!UICONTROL Order Notes] | 처리 중인 주문에 대해 기록된 가장 최근 작업 [!DNL Commerce]. 정보는 주문 가져오기 오류 및 주문 처리 업데이트를 포함하지만 이에 국한되지 않습니다.<br>**참고**: 이 필드는 [!DNL Commerce] 를 주문 프로세스의 일부로 표시합니다. |
