---
title: 일반적인 주문 처리 작업
description: 해당 [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] 관리자를 사용합니다.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 일반적인 주문 처리 작업

[[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}에서는 구매자 전자 메일, 주문(배송) 이행, 대변/환불 발행, 주석 추가 등을 포함하여 Amazon 주문을 관리할 수 있습니다. Amazon 주문을 관리하려면, Amazon 주문이 수신될 때 해당 [!DNL Commerce] 주문이 생성되도록 [**Amazon 주문 가져오기**](./order-settings.md) 설정을 `Enabled`로 설정해야 합니다. Amazon 주문 정보는 저장소 대시보드의 *[!UICONTROL Recent Orders]* 섹션에 표시됩니다.

활성화되면 Amazon 주문에 대해 해당 [!DNL Commerce] 주문이 만들어지며 Amazon 주문 번호는 _[!UICONTROL Order Number]_열에 표시됩니다. 해당 [!DNL Commerce] 순서가 생성된 경우 주문 번호를 클릭하여 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} 페이지에서 순서를 엽니다. 다른 [[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}에서처럼 주문을 관리할 수 있습니다.

[!DNL Commerce] 주문 번호가 _[!UICONTROL Recent Orders]_정보와 함께 표시되지 않습니다. [!DNL Commerce] 주문 번호는 저장소 대시보드에서 주문 번호를 클릭하고 [[!DNL Commerce] 주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}에서 주문을 열 때만 표시됩니다. [!DNL Commerce] 순서를 보면 Amazon 주문 번호가&#x200B;*[!UICONTROL Payment & Shipping Method]*섹션에 표시됩니다. 또한 주문 배송 상태에 따라&#x200B;*[!UICONTROL View or Cancel Amazon Order]*및&#x200B;*[!UICONTROL View all Amazon Orders]*옵션이 포함되어 있습니다.

[미출하 주문 취소](./cancel-unshipped-order.md)를 참조하십시오.

![상거래 주문의 Amazon 주문 정보](assets/amazon-order-number-payment-info.png)

Amazon 주문을 처리할 때 Amazon 영업 채널은 주문 정보를 업데이트하고 [!DNL Amazon Seller Central] 계정과 동기화합니다. 기본 설정은 Amazon과 Amazon 판매 채널 간에 주문 정보를 동기화하는 빈도를 결정합니다.

일반적인 [!DNL Commerce] [주문 처리](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} 작업은 다음과 같습니다.

- [작업 순서](https://docs.magento.com/user-guide/sales/order-actions.html) 지정{target=&quot;_blank&quot;}
- [주문 검색](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [주문](https://docs.magento.com/user-guide/sales/order-processing.html) 처리{target=&quot;_blank&quot;}
   - [주문](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order) 보기{target=&quot;_blank&quot;}
   - [주문](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order) 처리{target=&quot;_blank&quot;}
   - [주문 및 계정 정보](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [주소 정보](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [결제 및 배송 방법](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [순서가 지정된](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered) 항목 검토{target=&quot;_blank&quot;}
- [신용/환급](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;} 발급
- [주문](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;} 이행/배송
- [송장](https://docs.magento.com/user-guide/sales/invoice-create.html) 만들기{target=&quot;_blank&quot;}
- [미출하 주문 취소](./cancel-unshipped-order.md)

>[!NOTE]
>
>주문이 `Unshipped` 상태인 경우 [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) 페이지에서 [Amazon 주문](./cancel-unshipped-order.md)을 취소할 수 있습니다. 주문이 배송된 경우에는 취소할 수 없습니다.

[상거래 주문 관리](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}를 참조하십시오.
