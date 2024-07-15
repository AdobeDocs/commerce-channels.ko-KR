---
title: 배송되지 않은 Amazon 주문 취소
description: Amazon [!DNL Seller Central] 계정을 통해 보류 중이거나 부분적으로 배송된(배송되지 않은) 주문을 취소합니다.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 배송되지 않은 Amazon 주문 취소

Amazon 주문은 `Unshipped` 상태인 경우에만 취소할 수 있습니다. 주문이 보류 중이거나 부분적으로 배송된 경우(배송되지 않은 경우) [!DNL Amazon Seller Central] 계정을 통해서만 주문을 취소할 수 있습니다. 항목이 배송된 경우 반품과 교환도 [!DNL Amazon Seller Central] 계정에서 처리해야 합니다.

>[!NOTE]
>
>주문 취소 이외의 작업의 경우:
>
>- [주문 가져오기](./order-settings.md)를 사용하도록 설정한 경우 주문은 [[!DNL Commerce] 주문 워크플로우](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)에서 관리됩니다.
>- [주문 가져오기](./order-settings.md)를 사용하지 않도록 설정한 경우 [!DNL Amazon Seller Central]에서 주문을 관리해야 합니다.

## `Unshipped` 상태에서 주문 취소

1. 저장소 카드에서 **[!UICONTROL View Store]**&#x200B;을(를) 클릭합니다.

1. 스토어 대시보드의 _[!UICONTROL Recent Orders]_섹션에서 주문 번호를 클릭합니다.

   _[!UICONTROL Amazon Order Details]_페이지가 나타납니다.

1. 헤더 표시줄에서 **[!UICONTROL Cancel Order]**&#x200B;을(를) 클릭합니다.

   이 옵션은 `Unshipped` 상태의 주문에만 나타납니다.

1. **[!UICONTROL Reason for cancellation]**&#x200B;에 대해 옵션을 선택하십시오.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   주문이 취소되고 주문 세부 정보에서 상태가 `Canceled`(으)로 업데이트됩니다.

취소 알림이 [!DNL Amazon Seller Central] 계정으로 전송되며 해당 주문과 연계된 고객에게도 알림이 전송됩니다. 해당 [!DNL Commerce] 주문(있는 경우)의 상태가 `Complete`(으)로 변경됩니다.
