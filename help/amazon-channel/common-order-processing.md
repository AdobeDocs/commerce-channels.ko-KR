---
title: 일반적인 Amazon 주문 처리 작업
description: 해당 항목 사용 [!DNL Commerce] 주문 활동 및 처리를 관리하기 위해 Amazon 주문에 대해 생성된 주문 [!UICONTROL Commerce] 관리자.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 6d221c2c2e9a37a42e9d660aceb3c525fedc511d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# 일반적인 Amazon 주문 처리 작업

[상거래 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) 은(는) 구매자에게 이메일 전송, 주문 이행(배송), 크레딧/환불 발급, 댓글 추가 등을 포함하여 Amazon 주문을 관리할 수 있습니다. Amazon 주문을 관리하려면 [**Amazon 주문 가져오기**](./order-settings.md) 설정을 로 설정해야 합니다. `Enabled` 이에 해당됨 [!DNL Commerce] 주문은 Amazon 주문이 수신되면 생성됩니다. Amazon 주문 정보는 *[!UICONTROL Recent Orders]* 섹션 을 참조하십시오.

활성화하면 해당 [!DNL Commerce] 주문은 Amazon 주문에 대해 생성되며 Amazon 주문 번호는 _[!UICONTROL Order Number]_열. 해당하는 경우 [!DNL Commerce] 주문이 생성되면 주문 번호를 클릭하여 [상거래 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) 페이지를 가리키도록 업데이트하는 중입니다. 다른 작업을 수행하는 것처럼 주문을 관리할 수 있습니다. [[!DNL Commerce] 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

다음 [!DNL Commerce] 주문 번호가 _[!UICONTROL Recent Orders]_정보. 상거래 주문 번호는 스토어 대시보드에서 주문 번호를 클릭하고 주문을 여는 경우에만 표시됩니다. [상거래 주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). 를 볼 때 [!DNL Commerce] order를 입력하면 Amazon 주문 번호가&#x200B;*[!UICONTROL Payment & Shipping Method]*섹션. 또한 다음과 같은 옵션이 포함되어 있습니다.*[!UICONTROL View or Cancel Amazon Order]*및&#x200B;*[!UICONTROL View all Amazon Orders]*주문 배송 상태에 따라 달라질 수 있습니다.

다음을 참조하십시오 [미출하 주문 취소](./cancel-unshipped-order.md).

![상거래 주문의 Amazon 주문 정보](assets/amazon-order-number-payment-info.png){width="500"}

Amazon 주문을 처리할 때 Amazon 판매 채널은 주문 정보를 업데이트하고 와 동기화합니다. [!DNL Amazon Seller Central] 계정입니다. 크론 설정에 따라 Amazon과 Amazon 판매 채널 간에 주문 정보가 동기화되는 빈도가 결정됩니다.

일반 상거래 [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) 작업에는 다음이 포함됩니다.

- [주문 작업](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [주문 검색](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [주문 보기](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [주문 및 계정 정보](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [주소 정보](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [결제 및 배송 방법](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [순서가 지정된 항목 검토](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [대변/환불 발행](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [주문 이행/배송](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [송장 만들기](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [선적되지 않은 주문 취소](./cancel-unshipped-order.md)

>[!NOTE]
>
>주문이 있는 경우 `Unshipped` 상태, 다음을 수행할 수 있습니다. [Amazon 주문 취소](./cancel-unshipped-order.md) 다음에 있음 [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 페이지를 가리키도록 업데이트하는 중입니다. 주문이 발송된 경우 취소할 수 없습니다.

다음을 참조하십시오 [상거래 주문 관리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
