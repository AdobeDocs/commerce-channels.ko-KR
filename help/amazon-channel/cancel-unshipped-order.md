---
title: 미출하 주문 취소
description: Amazon [!DNL Seller Central] 계정을 통해 보류 중 또는 부분적으로 출하된(미출하) 주문을 취소합니다.
exl-id: a6df09b7-7f62-47e5-a2d3-1761802255d0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 미출하 주문 취소

Amazon 주문은 `Unshipped` 상태인 경우에만 취소할 수 있습니다. 주문이 보류 중이거나 일부 출하(미출하)된 경우 [!DNL Amazon Seller Central] 계정을 통해서만 주문을 취소할 수 있습니다. 품목이 출하된 경우 반품 및 교환도 [!DNL Amazon Seller Central] 계정에서 처리해야 합니다.

>[!NOTE]
>
>주문 취소 이외의 작업의 경우
>
>- [주문 가져오기](./order-settings.md)가 활성화되어 있으면 주문은 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}에서 관리됩니다.
>- [주문 가져오기](./order-settings.md)가 비활성화되어 있으면 [!DNL Amazon Seller Central]에서 주문을 관리해야 합니다.


## `Unshipped` 상태의 주문 취소

1. 스토어 카드에서 **[!UICONTROL View Store]** 을 클릭합니다.

1. 저장소 대시보드의 _[!UICONTROL Recent Orders]_섹션에서 주문 번호를 클릭합니다.

   _[!UICONTROL Amazon Order Details]_페이지가 나타납니다.

1. 헤더 막대에서 **[!UICONTROL Cancel Order]** 을 클릭합니다.

   이 옵션은 `Unshipped` 상태의 주문에 대해서만 나타납니다.

1. **[!UICONTROL Reason for cancellation]**&#x200B;에 대해 옵션을 선택합니다.

1. **[!UICONTROL Confirm]** 을 클릭합니다.

   주문이 취소되고 주문 세부 정보에 따라 상태가 `Canceled`으로 업데이트됩니다.

취소 알림이 [!DNL Amazon Seller Central] 계정으로 전송되고 주문과 연결된 고객에게도 알림이 표시됩니다. 해당하는 [!DNL Commerce] 주문이 있는 경우 상태가 `Complete`로 변경됩니다.
