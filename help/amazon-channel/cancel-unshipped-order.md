---
title: 미출하 주문 취소
description: Amazon을 통해 보류 중이거나 부분적으로 출하된(미출하) 주문 취소 [!DNL Seller Central] 계정이 필요합니다.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 미출하 주문 취소

Amazon 주문은 `Unshipped` 상태. 주문이 보류 중이거나 일부 출하(미출하)된 경우, 주문을 통해 취소할 수 있습니다 [!DNL Amazon Seller Central] 계정이 필요합니다. 품목이 출하된 경우 반품 및 교환도 반드시 [!DNL Amazon Seller Central] 계정.

>[!NOTE]
>
>주문 취소 이외의 작업의 경우
>
>- 만약 [주문 가져오기](./order-settings.md) 활성화되면, 주문은 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.
>- If [주문 가져오기](./order-settings.md) 이 비활성화되어 있으면에서 주문을 관리해야 합니다. [!DNL Amazon Seller Central].


## 주문 취소 `Unshipped` 상태

1. 클릭 **[!UICONTROL View Store]** 매장 카드 위에

1. 에서 _[!UICONTROL Recent Orders]_저장소 대시보드의 섹션에서 주문 번호를 클릭합니다.

   다음 _[!UICONTROL Amazon Order Details]_페이지가 나타납니다.

1. 클릭 **[!UICONTROL Cancel Order]** 헤더 막대에서 클릭합니다.

   이 옵션은 의 주문에 대해서만 나타납니다 `Unshipped` 상태.

1. 대상 **[!UICONTROL Reason for cancellation]**&#x200B;옵션을 선택합니다.

1. 클릭 **[!UICONTROL Confirm]**.

   주문은 취소되고 상태는 로 업데이트됩니다. `Canceled` 주문 세부 사항

취소 알림이 [!DNL Amazon Seller Central] 계정 및 주문과 연관된 고객도 알림을 받습니다. 해당 의 상태 [!DNL Commerce] order를으로 변경할 경우 `Complete`.
