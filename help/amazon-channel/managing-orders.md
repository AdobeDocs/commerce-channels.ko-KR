---
title: 주문 관리
description: 주문 설정에서 주문 가져오기를 활성화하여 Commerce 관리자의 Amazon 주문을 보다 쉽게 관리할 수 있습니다.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 주문 관리

Amazon에서 받은 Amazon 주문 정보를에서 볼 수 있습니다. _[!UICONTROL Recent Orders]_의 섹션 [대시보드 저장](./amazon-store-dashboard.md) 또는_[!UICONTROL Amazon orders]_ 페이지(또한 _[!UICONTROL All Orders]_view).

Amazon 주문 관리 방법은 주문에서 주문 가져오기의 활성화 여부에 따라 다릅니다. [주문 설정](./order-settings.md#configure-order-settings).

## 주문 가져오기가 활성화된 경우

다음 이후 [스토어 통합](./store-integration.md), [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정: `Enabled` 기본적으로. 이 설정으로, 해당 [!DNL Commerce] 주문은 Amazon 주문에 대해 생성되며 [[!DNL Commerce] 주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 워크플로입니다.

>[!NOTE]
>
>주문 가져오기 설정에 관계없이, 사이트에 있었던 Amazon 주문 [!DNL Amazon Seller Central] 다음 이전 계정 [스토어 통합](./store-integration.md) 은(는) 가져오지 않습니다.

가져온 Amazon 주문은 [[!DNL Commerce] 주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workflow, just like your other [!DNL Commerce] stores. Click the Amazon order number in the *[!UICONTROL Order Number]* column to open the order in the [[!DNL Commerce] order process](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target="_blank"}. 다음을 참조하십시오 [Amazon 주문 보기](./amazon-orders-all.md).

### 주문 가져오기 프로세스

주문이 Amazon에 접수되고 [주문 가져오기](./order-settings.md) 이(가) 활성화되면 다음 프로세스가 시작됩니다.

| 변경 | 작업 |
|---|---|
| 주문이 Amazon에 접수됩니다. | <ul><li>Amazon이 주문 상태를 다음으로 설정 `Pending`.</li><li>주문 정보가 (으)로 전송됨 [!DNL Commerce].</li><li>주문이 다음에 추가됨 [_Amazon 주문_ 표](./amazon-orders-all.md) 포함 `Pending` 상태.</li></ul> |
| Amazon이 주문 상태를 다음으로 변경 `Unshipped`. | <ul><li>상태 변경 사항이 (으)로 전송됨 [!DNL Commerce].</li><li>다음에서 [_Amazon 주문_ 표](./amazon-orders-all.md), 주문 상태가 다음으로 변경됨 `Unshipped`.</li><li>다음에서 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}, 해당 [!DNL Commerce] 주문은 `Processing` 상태.</li></ul> |
| 위치 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}, [!DNL Commerce] 주문이 처리되고 상태가 다음으로 변경됨 `Shipped`. | <ul><li>다음에서 [_Amazon 주문_ 표](./amazon-orders-all.md), 주문 상태가 다음으로 변경됨 `Shipped`.</li><li>다음 cron 작업에서 주문 상태가 다음으로 변경됩니다. `Complete` 다음에서 [[!DNL Commerce] 주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}.</li></ul> |

### 주문 생성 차단기

해당 항목이 생성되지 않게 하는 몇 가지 시나리오가 있습니다 [!DNL Commerce] 주문. [!DNL Commerce] 다음 문제가 발생할 때 수신되는 주문에 대해서는 주문이 생성되지 않습니다.

| 시나리오 | 솔루션 |
|---|---|
| 항목이 다음에 존재하지 않음 [!DNL Commerce] 카탈로그. | [제품 만들기](./creating-assigning-catalog-products.md) (으)로 [!DNL Commerce] 카탈로그 및 [수동 일치](./creating-assigning-catalog-products.md) 제품에 적용합니다. |
| 카탈로그의 항목이 비활성화되었습니다. | 다음을 확인하십시오. [제품 상태](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} 이(가) 활성화되었습니다. |
| 주문한 상품이 품절입니다. | 업데이트 또는 구성 [제품 옵션](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){target="_blank"} 수량 및 출처의 경우. |

주문을 가져올 수 없는 경우 화면 상단에 다음과 유사한 시스템 메시지가 나타납니다.

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

문제가 해결되면 [!DNL Commerce] 다음 동기화 시 순서가 만들어집니다.

## 주문 가져오기가 비활성화됨

에서 Amazon 주문을 가져오고 관리하지 않으려는 경우 [!DNL Commerce], 다음을 변경할 수 있습니다. [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) 설정 `Disabled`. 이 설정은 Amazon에서 새 주문을 받으면 [!DNL Commerce] 주문이 생성되지 않습니다.

비활성화되면 Amazon에서 받은 주문 정보가 _[!UICONTROL Recent Orders]_섹션( 스토어 대시보드 및 )을 참조하십시오_[!UICONTROL All Orders]_ 보기. 이 주문 정보는 보기 전용이며 다음 위치에서 이러한 주문을 관리해야 합니다. [!DNL Amazon Seller Central]. 주문 세부 사항을 열려면 [!DNL Amazon Seller Central]에서 Amazon 주문 번호 를 클릭합니다. _[!UICONTROL Order Number]_열.

참조: [Amazon 주문 보기](./amazon-orders-all.md), [Amazon 주문 세부 사항 보기](./amazon-order-details.md), 및 [일반적인 주문 처리 작업](./common-order-processing.md).
