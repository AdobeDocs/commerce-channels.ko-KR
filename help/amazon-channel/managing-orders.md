---
title: 주문 관리
description: 주문 설정에서 주문 가져오기를 활성화하여 상거래 관리자에서 Amazon 주문을 보다 쉽게 관리할 수 있습니다.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 주문 관리

Amazon에서 받은 대로 Amazon 주문 정보를 [대시보드](./amazon-store-dashboard.md)의 _[!UICONTROL Recent Orders]_섹션이나_[!UICONTROL Amazon orders]_ 페이지(_[!UICONTROL All Orders]_보기라고도 함)에서 볼 수 있습니다.

Amazon 주문을 관리하는 방법은 [주문 설정](./order-settings.md#configure-order-settings)에서 주문 가져오기가 활성화되었는지 아니면 비활성화되었는지 여부에 따라 다릅니다.

## 주문 임포트가 활성화된 경우

[통합](./store-integration.md) 다음에 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정은 기본적으로 `Enabled`입니다. 이 설정을 사용하면 해당 [!DNL Commerce] 주문이 Amazon 주문에 대해 작성되어 [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} 워크플로우에서 관리할 수 있습니다.

>[!NOTE]
>
>주문 가져오기 설정에 관계없이 [스토어 통합](./store-integration.md) 이전에 [!DNL Amazon Seller Central] 계정에 있던 Amazon 주문은 가져오지 않습니다.

가져온 Amazon 주문은 다른 [!DNL Commerce] 스토어와 마찬가지로 [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} 워크플로우에서 관리됩니다. *[!UICONTROL Order Number]* 열에서 Amazon 주문 번호를 클릭하여 [[!DNL Commerce] 주문 프로세스](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}에서 순서를 엽니다. [Amazon 주문 보기](./amazon-orders-all.md)를 참조하십시오.

### 주문 가져오기 프로세스

주문이 Amazon에 배치되고 [주문 가져오기](./order-settings.md)가 활성화되어 있으면 다음 프로세스가 시작됩니다.

| 변경 | 작업 |
|---|---|
| Amazon에 주문이 있습니다. | <ul><li>Amazon은 주문 상태를 `Pending`로 설정합니다.</li><li>주문 정보가 [!DNL Commerce](으)로 전송됩니다.</li><li>주문이 [_Amazon 주문_ 테이블](./amazon-orders-all.md)에 추가되고 `Pending` 상태가 표시됩니다.</li></ul> |
| Amazon이 주문 상태를 `Unshipped`으로 변경합니다. | <ul><li>상태 변경이 [!DNL Commerce](으)로 전송됩니다.</li><li>[_Amazon 주문_ 테이블](./amazon-orders-all.md)에서 주문 상태가 `Unshipped`로 변경됩니다.</li><li>[[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}에서 해당 `Processing` 순서가 [!DNL Commerce] 상태로 만들어집니다.</li></ul> |
| [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}에서 [!DNL Commerce] 순서가 처리되고 상태가 `Shipped`로 변경됩니다. | <ul><li>[_Amazon 주문_ 테이블](./amazon-orders-all.md)에서 주문 상태가 `Shipped`로 변경됩니다.</li><li>다음 클론 작업에서 주문 상태는 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}에서 `Complete`으로 변경됩니다.</li></ul> |

### 주문 생성 차단기

해당 [!DNL Commerce] 순서를 만들지 못하는 시나리오가 몇 가지 있습니다. [!DNL Commerce] 다음 문제가 발생할 때 받은 주문에 대해서는 주문이 생성되지 않습니다.

| 시나리오 | 솔루션 |
|---|---|
| 항목이 [!DNL Commerce] 카탈로그에 없습니다. | [카탈로그](./creating-assigning-catalog-products.md) 의  [!DNL Commerce] 제품을 만들고  [제품](./creating-assigning-catalog-products.md) 에 수동으로 일치시킵니다. |
| 카탈로그의 항목을 사용할 수 없습니다. | [제품 상태](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;}가 활성화되어 있는지 확인합니다. |
| 주문품이 품절되었습니다. | 수량 및 소스에 대해 [제품 옵션](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;}을 업데이트하거나 구성합니다. |

주문을 가져올 수 없는 경우 화면 맨 위에 다음과 유사한 시스템 메시지가 나타납니다.

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

문제가 해결되면 다음 동기화 시 [!DNL Commerce] 순서가 만들어집니다.

## 주문 가져오기를 사용하지 않도록 설정한 경우

[!DNL Commerce]에서 Amazon 주문을 가져오고 관리하지 않으려는 경우 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정을 `Disabled`로 변경할 수 있습니다. 이 설정은 Amazon에서 새 주문을 받으면 해당 [!DNL Commerce] 주문이 만들어지지 않음을 의미합니다.

비활성화하면 Amazon에서 받은 주문 정보가 저장소 대시보드의 _[!UICONTROL Recent Orders]_섹션과_[!UICONTROL All Orders]_ 보기에 표시됩니다. 이 주문 정보는 보기 전용이며 [!DNL Amazon Seller Central]에서 이러한 주문을 관리해야 합니다. [!DNL Amazon Seller Central]에서 주문 세부 사항을 열려면 _[!UICONTROL Order Number]_열에서 Amazon 주문 번호를 클릭합니다.

또한 [Amazon 주문 보기](./amazon-orders-all.md), [Amazon 주문 세부 사항 보기](./amazon-order-details.md) 및 [일반적인 주문 처리 작업](./common-order-processing.md)을 참조하십시오.
