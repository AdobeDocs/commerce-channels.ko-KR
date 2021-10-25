---
title: 일반적인 주문 처리 작업
description: 해당 [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] 관리자.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 일반적인 주문 처리 작업

[[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}은 구매자에게 전자 메일을 보내고, 주문(배송), 대변/환불 발행, 주석 추가 등을 포함하여 Amazon 주문을 관리할 수 있습니다. Amazon 주문을 관리하려면 [**Amazon 주문 가져오기**](./order-settings.md) 설정은 `Enabled` 따라서 [!DNL Commerce] 주문은 Amazon 주문이 수신되면 생성됩니다. Amazon 주문 정보는 *[!UICONTROL Recent Orders]* 저장소 대시보드의 섹션.

활성화되면 해당 [!DNL Commerce] Amazon 주문에 대한 주문이 생성되며, Amazon 주문 번호는 _[!UICONTROL Order Number]_열. 해당하는 경우 [!DNL Commerce] 주문이 생성되면 주문 번호를 클릭하여 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} 페이지. 다른 주문처럼 주문을 관리할 수 있습니다 [[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

다음 [!DNL Commerce] 주문 번호가 _[!UICONTROL Recent Orders]_정보. 다음 [!DNL Commerce] 주문 번호는 저장소 대시보드에서 주문 번호를 클릭하고 주문을 여는 경우에만 표시됩니다 [[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. 를 볼 때 [!DNL Commerce] 순서대로 Amazon 주문 번호가&#x200B;*[!UICONTROL Payment & Shipping Method]*섹션을 참조하십시오. 여기에는 다음 옵션도 포함되어 있습니다&#x200B;*[!UICONTROL View or Cancel Amazon Order]*및&#x200B;*[!UICONTROL View all Amazon Orders]*주문 배송 상태에 따라 다릅니다.

자세한 내용은 [미출하 주문 취소](./cancel-unshipped-order.md).

![상거래 주문의 Amazon 주문 정보](assets/amazon-order-number-payment-info.png)

Amazon 주문을 처리할 때 Amazon 영업 채널은 주문 정보를 업데이트하고 와 동기화합니다 [!DNL Amazon Seller Central] 계정이 필요합니다. 기본 설정은 Amazon과 Amazon 판매 채널 간에 주문 정보를 동기화하는 빈도를 결정합니다.

공통 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} 작업은 다음과 같습니다.

- [주문 작업](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [주문 검색](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [주문 보기](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [주문 및 계정 정보](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [주소 정보](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [결제 및 배송 방법](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [주문된 항목 검토](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [신용/환급 발행](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [주문 이행/운송](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [송장 생성](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [미출하 주문 취소](./cancel-unshipped-order.md)

>[!NOTE]
>
>주문이 포함된 경우 `Unshipped` 상태, [Amazon 주문 취소](./cancel-unshipped-order.md) on [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 페이지. 주문이 배송된 경우에는 취소할 수 없습니다.

자세한 내용은 [상거래 주문 관리](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
