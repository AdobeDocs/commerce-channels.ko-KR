---
title: Amazon 주문 관리
description: 주문 설정에서 주문 가져오기를 활성화하여 Commerce 관리자로부터 Amazon 주문을 보다 쉽게 관리할 수 있습니다.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Amazon 주문 관리

Amazon에서 받은 Amazon 주문 정보는 [스토어 대시보드](./amazon-store-dashboard.md)의 _[!UICONTROL Recent Orders]_섹션 또는_[!UICONTROL Amazon orders]_ 페이지에서 볼 수 있습니다(_[!UICONTROL All Orders]_보기라고도 함).

Amazon 주문을 관리하는 방법은 [주문 설정](./order-settings.md#configure-order-settings)에서 주문 가져오기를 사용할 수 있는지 여부에 따라 다릅니다.

## 주문 가져오기가 활성화된 경우

[스토어 통합](./store-integration.md) 후 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정은 기본적으로 `Enabled`입니다. 이 설정을 사용하면 Amazon 주문에 대해 해당 [!DNL Commerce]개의 주문이 만들어지고 [[!DNL Commerce] 주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 워크플로우에서 관리할 수 있습니다.

>[!NOTE]
>
>주문 가져오기 설정에 관계없이 [스토어 통합](./store-integration.md) 이전에 [!DNL Amazon Seller Central] 계정에 있었던 Amazon 주문은 가져오지 않습니다.

가져온 Amazon 주문은 다른 [!DNL Commerce] 스토어와 마찬가지로 [[!DNL Commerce] 주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 워크플로우에서 관리됩니다. *[!UICONTROL Order Number]* 열에서 Amazon 주문 번호를 클릭하여 [[!DNL Commerce] 주문 프로세스](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions)에서 주문을 엽니다. [Amazon 주문 보기](./amazon-orders-all.md)를 참조하세요.

### 주문 가져오기 프로세스

Amazon에서 주문하고 [주문 가져오기](./order-settings.md)를 사용하도록 설정하면 다음 프로세스가 시작됩니다.

| 변경 | 작업 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 주문이 Amazon에 접수됩니다. | <ul><li>Amazon에서 주문 상태를 `Pending`(으)로 설정합니다.</li><li>주문 정보를 [!DNL Commerce](으)로 보냅니다.</li><li>주문이 `Pending` 상태의 [_Amazon 주문_ 테이블](./amazon-orders-all.md)에 추가됩니다.</li></ul> |
| Amazon에서 주문 상태를 `Unshipped`(으)로 변경합니다. | <ul><li>상태 변경 내용이 [!DNL Commerce](으)로 전송되었습니다.</li><li>[_Amazon 주문_ 테이블](./amazon-orders-all.md)에서 주문 상태가 `Unshipped`(으)로 변경됩니다.</li><li>[[!DNL Commerce] 주문 워크플로우](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)에서 `Processing` 상태로 해당 [!DNL Commerce] 주문이 만들어집니다.</li></ul> |
| [[!DNL Commerce] 주문 워크플로](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)에서 [!DNL Commerce] 주문이 처리되고 상태가 `Shipped`(으)로 변경됩니다. | <ul><li>[_Amazon 주문_ 테이블](./amazon-orders-all.md)에서 주문 상태가 `Shipped`(으)로 변경됩니다.</li><li>다음 cron 작업에서 주문 상태가 [[!DNL Commerce] 주문 워크플로](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)의 `Complete`(으)로 변경됩니다.</li></ul> |

### 주문 생성 차단기

해당 [!DNL Commerce] 순서가 만들어지지 않도록 하는 시나리오가 몇 가지 있습니다. 다음 문제가 발생할 때 받은 주문에 대해 [!DNL Commerce]개의 주문이 만들어지지 않습니다.

| 시나리오 | 솔루션 |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 항목이 [!DNL Commerce] 카탈로그에 없습니다. | [!DNL Commerce] 카탈로그에 [제품을 만들고](./creating-assigning-catalog-products.md) 제품에 [수동으로 일치](./creating-assigning-catalog-products.md)합니다. |
| 카탈로그의 항목이 비활성화되었습니다. | [제품 상태](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html)가 활성화되어 있는지 확인하십시오. |
| 주문한 상품이 품절입니다. | 수량 및 출처에 대한 [제품 옵션](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html)을 업데이트하거나 구성하십시오. |

주문을 가져올 수 없는 경우 화면 상단에 다음과 유사한 시스템 메시지가 나타납니다.

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

문제가 해결되면 다음 동기화 시 [!DNL Commerce] 순서가 만들어집니다.

## 주문 가져오기가 비활성화됨

[!DNL Commerce]에서 Amazon 주문을 가져오고 관리하지 않으려면 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정을 `Disabled`(으)로 변경할 수 있습니다. 이 설정은 Amazon에서 새 주문을 받으면 해당 [!DNL Commerce]개의 주문이 만들어지지 않음을 의미합니다.

비활성화하면 Amazon에서 받은 주문 정보가 스토어 대시보드의 _[!UICONTROL Recent Orders]_섹션과_[!UICONTROL All Orders]_ 보기에 나타납니다. 이 주문 정보는 보기 전용이며 [!DNL Amazon Seller Central]에서 이러한 주문을 관리해야 합니다. [!DNL Amazon Seller Central]에서 주문 세부 사항을 열려면 _[!UICONTROL Order Number]_열에서 Amazon 주문 번호를 클릭합니다.

[Amazon 주문 보기](./amazon-orders-all.md), [Amazon 주문 세부 사항 보기](./amazon-order-details.md) 및 [일반적인 주문 처리 작업](./common-order-processing.md)도 참조하세요.
