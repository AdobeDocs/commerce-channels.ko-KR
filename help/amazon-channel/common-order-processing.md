---
title: 일반적인 주문 처리 작업
description: 해당 항목 사용 [!DNL Commerce] 주문 활동 및 처리를 관리하기 위해 Amazon 주문에 대해 생성된 주문 [!UICONTROL Commerce] 관리자.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 일반적인 주문 처리 작업

[[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} 은(는) 구매자에게 이메일 전송, 주문 이행(배송), 크레딧/환불 발급, 댓글 추가 등을 포함하여 Amazon 주문을 관리할 수 있습니다. Amazon 주문을 관리하려면 [**Amazon 주문 가져오기**](./order-settings.md) 설정을 로 설정해야 합니다. `Enabled` 이에 해당됨 [!DNL Commerce] 주문은 Amazon 주문이 수신되면 생성됩니다. Amazon 주문 정보는 *[!UICONTROL Recent Orders]* 섹션 을 참조하십시오.

활성화하면 해당 [!DNL Commerce] 주문은 Amazon 주문에 대해 생성되며 Amazon 주문 번호는 _[!UICONTROL Order Number]_열. 해당하는 경우 [!DNL Commerce] 주문이 생성되면 주문 번호를 클릭하여 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

다음 [!DNL Commerce] 주문 번호가 _[!UICONTROL Recent Orders]_정보. 다음 [!DNL Commerce] 주문 번호는 스토어 대시보드에서 주문 번호를 클릭하고 주문을 여는 경우에만 표시됩니다. [[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}. 를 볼 때 [!DNL Commerce] order를 입력하면 Amazon 주문 번호가&#x200B;*[!UICONTROL Payment & Shipping Method]*섹션. 또한 다음과 같은 옵션이 포함되어 있습니다.*[!UICONTROL View or Cancel Amazon Order]*및&#x200B;*[!UICONTROL View all Amazon Orders]*주문 배송 상태에 따라 달라질 수 있습니다.

다음을 참조하십시오 [미출하 주문 취소](./cancel-unshipped-order.md).

![상거래 주문의 Amazon 주문 정보](assets/amazon-order-number-payment-info.png)

Amazon 주문을 처리할 때 Amazon 판매 채널은 주문 정보를 업데이트하고 와 동기화합니다. [!DNL Amazon Seller Central] 계정입니다. 크론 설정에 따라 Amazon과 Amazon 판매 채널 간에 주문 정보가 동기화되는 빈도가 결정됩니다.

공통 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} 작업에는 다음이 포함됩니다.

- [주문 작업](https://docs.magento.com/user-guide/sales/order-actions.html){target="_blank"}
- [주문 검색](https://docs.magento.com/user-guide/sales/orders-search.html){target="_blank"}
- [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}
   - [주문 보기](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target="_blank"}
   - [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target="_blank"}
   - [주문 및 계정 정보](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target="_blank"}
   - [주소 정보](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target="_blank"}
   - [결제 및 배송 방법](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target="_blank"}
   - [순서가 지정된 항목 검토](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target="_blank"}
- [대변/환불 발행](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target="_blank"}
- [주문 이행/배송](https://docs.magento.com/user-guide/sales/shipments-create.html){target="_blank"}
- [송장 만들기](https://docs.magento.com/user-guide/sales/invoice-create.html){target="_blank"}
- [선적되지 않은 주문 취소](./cancel-unshipped-order.md)

>[!NOTE]
>
>주문이 있는 경우 `Unshipped` 상태, 다음을 수행할 수 있습니다. [Amazon 주문 취소](./cancel-unshipped-order.md) 다음에 있음 [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 페이지를 가리키도록 업데이트하는 중입니다. 주문이 발송된 경우 취소할 수 없습니다.

다음을 참조하십시오 [상거래 주문 관리](https://docs.magento.com/user-guide/sales/order-management.html){target="_blank"}.
