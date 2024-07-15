---
title: 일반적인 Amazon 주문 처리 작업
description: Amazon 주문에 대해 생성된 해당  [!DNL Commerce] 주문을 사용하여 [!UICONTROL Commerce] 관리자의 주문 활동 및 처리를 관리하십시오.
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 일반적인 Amazon 주문 처리 작업

[Commerce 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)를 통해 구매자에게 이메일 전송, 주문 이행(배송), 크레딧/환불 발급, 댓글 추가 등 Amazon 주문을 관리할 수 있습니다. Amazon 주문을 관리하려면 Amazon 주문이 수신될 때 해당 [!DNL Commerce]개의 주문이 생성되도록 [**Amazon 주문 가져오기**](./order-settings.md) 설정을 `Enabled`(으)로 설정해야 합니다. Amazon 주문 정보는 스토어 대시보드의 *[!UICONTROL Recent Orders]* 섹션에 표시됩니다.

사용하도록 설정하면 Amazon 주문에 대해 해당 [!DNL Commerce]개의 주문이 만들어지고 _[!UICONTROL Order Number]_열에 Amazon 주문 번호가 표시됩니다. 해당 [!DNL Commerce] 순서가 만들어지면 주문 번호를 클릭하여 [Commerce 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) 페이지에서 주문을 엽니다. 다른 [[!DNL Commerce] 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)를 수행할 때 주문을 관리할 수 있습니다.

[!DNL Commerce] 주문 번호가 _[!UICONTROL Recent Orders]_정보와 함께 표시되지 않습니다. Commerce 주문 번호는 스토어 대시보드에서 주문 번호를 클릭하고 [Commerce 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)에서 주문을 여는 경우에만 표시됩니다. [!DNL Commerce] 주문을 볼 때&#x200B;*[!UICONTROL Payment & Shipping Method]*섹션에 Amazon 주문 번호가 나타납니다. 주문 배송 상태에 따라&#x200B;*[!UICONTROL View or Cancel Amazon Order]*및&#x200B;*[!UICONTROL View all Amazon Orders]*에 대한 옵션도 포함됩니다.

[배송되지 않은 주문 취소](./cancel-unshipped-order.md)를 참조하세요.

![Commerce 순서의 Amazon 주문 정보](assets/amazon-order-number-payment-info.png){width="500"}

Amazon 주문을 처리할 때 Amazon 판매 채널은 주문 정보를 업데이트하고 [!DNL Amazon Seller Central] 계정과 동기화합니다. 크론 설정에 따라 Amazon과 Amazon 판매 채널 간에 주문 정보가 동기화되는 빈도가 결정됩니다.

일반적인 Commerce [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) 작업은 다음과 같습니다.

- [작업 순서 지정](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [검색 순서 지정](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [주문 보기](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [주문 및 계정 정보](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [주소 정보](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [결제 및 배송 방법](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [순서가 지정된 항목 검토](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [크레딧/환불하기](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [주문 이행/배송](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [인보이스 만들기](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [선적되지 않은 주문 취소](./cancel-unshipped-order.md)

>[!NOTE]
>
>주문이 `Unshipped` 상태인 경우 [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 페이지에서 [Amazon 주문을 취소](./cancel-unshipped-order.md)할 수 있습니다. 주문이 발송된 경우 취소할 수 없습니다.

[Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations)을(를) 참조하십시오.
