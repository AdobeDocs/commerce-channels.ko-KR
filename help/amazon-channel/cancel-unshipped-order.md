---
title: 미출하 주문 취소
description: Amazon을 통해 보류 중이거나 부분적으로 배송된(미배송) 주문을 취소합니다. [!DNL Seller Central] 계정입니다.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# 미출하 주문 취소

Amazon 주문이 다음에 있는 경우에만 취소할 수 있습니다. `Unshipped` 상태. 주문이 보류 중이거나 부분적으로 출하(미출하)된 경우 주문을 통해서만 취소할 수 있습니다. [!DNL Amazon Seller Central] 계정입니다. 제품이 배송된 경우 반품과 교환도 다음 위치에서 처리되어야 합니다. [!DNL Amazon Seller Central] 계정.

>[!NOTE]
>
>주문 취소 이외의 작업의 경우:
>
>- 다음을 보유한 경우: [주문 가져오기](./order-settings.md) 활성화됨, 주문은 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}.
>- If [주문 가져오기](./order-settings.md) 이(가) 비활성화되어 있음에서 주문을 관리해야 합니다. [!DNL Amazon Seller Central].


## 다음 위치에서 주문 취소 `Unshipped` 상태

1. 클릭 **[!UICONTROL View Store]** 가게 카드에서요.

1. 다음에서 _[!UICONTROL Recent Orders]_스토어 대시보드의 섹션에서 주문 번호를 클릭합니다.

   다음 _[!UICONTROL Amazon Order Details]_페이지가 나타납니다.

1. 클릭 **[!UICONTROL Cancel Order]** 헤더 막대에서.

   이 옵션은 의 주문에 대해서만 나타납니다. `Unshipped` 상태.

1. 대상 **[!UICONTROL Reason for cancellation]**&#x200B;옵션을 선택합니다.

1. 클릭 **[!UICONTROL Confirm]**.

   주문이 취소되고 상태가 (으)로 업데이트됩니다. `Canceled` 주문 세부 사항.

취소 알림이 (으)로 전송됩니다 [!DNL Amazon Seller Central] 계정과 해당 주문과 연관된 고객에게도 알림이 전송됩니다. 해당 항목의 상태 [!DNL Commerce] 주문(있는 경우) `Complete`.
