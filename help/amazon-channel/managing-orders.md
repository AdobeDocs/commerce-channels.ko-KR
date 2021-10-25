---
title: 주문 관리
description: 주문 설정에서 주문 가져오기를 활성화하여 상거래 관리자에서 Amazon 주문을 보다 쉽게 관리할 수 있습니다.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 1d1b888db4de4f6e3658af768cd6f5cf30828788
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 주문 관리

Amazon에서 받은 대로 Amazon 주문 정보를 _[!UICONTROL Recent Orders]_섹션 [대시보드 저장](./amazon-store-dashboard.md) 또는_[!UICONTROL Amazon orders]_ 페이지(라고 함) _[!UICONTROL All Orders]_보기).

Amazon 주문을 관리하는 방법은 주문 가져오기가 [주문 설정](./order-settings.md#configure-order-settings).

## 주문 임포트가 활성화된 경우

후 [스토어 통합](./store-integration.md), [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정 `Enabled` 기본적으로 제공됩니다. 이 설정을 사용하면 해당 [!DNL Commerce] 주문은 Amazon 주문에 대해 만들어지며 [[!DNL Commerce] 주문](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} 워크플로입니다.

>[!NOTE]
>
>주문 가져오기 설정에 관계없이, [!DNL Amazon Seller Central] 이전 계정 [스토어 통합](./store-integration.md) 가져올 수 없습니다.

가져온 Amazon 주문은 [[!DNL Commerce] 주문](https://docs.magento.com/user-guide/sales/orders.html)다른 워크플로우처럼 {target=&quot;_blank&quot;} 워크플로우입니다 [!DNL Commerce] 상점들. 에서 Amazon 주문 번호를 클릭합니다 *[!UICONTROL Order Number]* 열에서 순서를 엽니다. [[!DNL Commerce] 주문 프로세스](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;}. 자세한 내용은 [Amazon 주문 보기](./amazon-orders-all.md).

### 주문 가져오기 프로세스

Amazon에서 주문이 이행되면 [주문 가져오기](./order-settings.md) 이 활성화되어 있으면 다음 프로세스가 시작됩니다.

| 변경 | 작업 |
|---|---|
| Amazon에 주문이 있습니다. | <ul><li>Amazon에서 주문 상태를 로 설정합니다. `Pending`.</li><li>주문 정보는 [!DNL Commerce].</li><li>다음에 주문이 추가됩니다. [_Amazon 주문_ 표](./amazon-orders-all.md) 사용 `Pending` 상태.</li></ul> |
| Amazon이 주문 상태를 `Unshipped`. | <ul><li>상태 변경이에 전송됩니다. [!DNL Commerce].</li><li>에서 [_Amazon 주문_ 표](./amazon-orders-all.md)로 설정되면 주문 상태가 `Unshipped`.</li><li>에서 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, 해당 [!DNL Commerce] 주문은 `Processing` 상태.</li></ul> |
| in [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}, [!DNL Commerce] 순서는 처리되고 상태는 `Shipped`. | <ul><li>에서 [_Amazon 주문_ 표](./amazon-orders-all.md)로 설정되면 주문 상태가 `Shipped`.</li><li>다음 클론 작업에서 주문 상태가 `Complete` 에서 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;}.</li></ul> |

### 주문 생성 차단기

해당 항목을 만들 수 없는 몇 가지 시나리오가 있습니다 [!DNL Commerce] 주문. [!DNL Commerce] 다음 문제가 발생할 때 받은 주문에 대해서는 주문이 생성되지 않습니다.

| 시나리오 | 솔루션 |
|---|---|
| 항목이 [!DNL Commerce] 카탈로그 | [제품 만들기](./creating-assigning-catalog-products.md) 다음 위치에서 [!DNL Commerce] 카탈로그 및 [수동 일치](./creating-assigning-catalog-products.md) 제품에 적용됩니다. |
| 카탈로그의 항목을 사용할 수 없습니다. | 다음을 확인합니다. [제품 상태](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target=&quot;_blank&quot;}이 활성화되었습니다. |
| 주문품이 품절되었습니다. | 업데이트 또는 구성 [제품 옵션](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html)수량 및 소스에 대해 {target=&quot;_blank&quot;}. |

주문을 가져올 수 없는 경우 화면 맨 위에 다음과 유사한 시스템 메시지가 나타납니다.

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

문제가 해결되면 [!DNL Commerce] 다음 동기화 시 순서가 만들어집니다.

## 주문 가져오기를 사용하지 않도록 설정한 경우

에서 Amazon 주문을 가져오고 관리하지 않으려는 경우 [!DNL Commerce]를 변경할 수 있습니다 [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정 `Disabled`. 이 설정은 Amazon에서 새 주문을 받으면, [!DNL Commerce] 주문은 만들어지지 않습니다.

비활성화하면 Amazon에서 받은 주문 정보가 _[!UICONTROL Recent Orders]_저장소 대시보드의 섹션 및_[!UICONTROL All Orders]_ 보기. 이 주문 정보는 보기 전용이며, [!DNL Amazon Seller Central]. 주문 세부 사항을 열려면 [!DNL Amazon Seller Central]에서 Amazon 주문 번호를 클릭합니다. _[!UICONTROL Order Number]_열.

참조 - [Amazon 주문 보기](./amazon-orders-all.md), [Amazon 주문 세부 사항 보기](./amazon-order-details.md), 및 [일반적인 주문 처리 작업](./common-order-processing.md).
