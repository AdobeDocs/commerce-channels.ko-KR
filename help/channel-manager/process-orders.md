---
title: 주문 처리
description: 배송 및 취소 지침 [!DNL Walmart Marketplace] Adobe Commerce 및 Magento Open Source의 주문.'
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# 주문 처리

다음 이후 [!DNL Walmart Marketplace] 주문이 확인되었으며 정상적으로 (으)로 전송되었습니다. [!DNL Channel Manager], 다음을 사용합니다. [상거래 주문 관리](https://docs.magento.com/user-guide/sales/orders-workspace.html) 주문을 처리합니다.

채널 관리자가에 대한 업데이트를 동기화합니다. [!DNL Walmart Marketplace] 주문 상태 및 운송 정보를 [!DNL Commerce] 에서 추적한 데이터와 일치 [!DNL Walmart Marketplace].

* **주문 배송**-월마트는 모든 배송에 대해 추적 번호가 필요합니다. 일부 품목이 품절된 경우 부분 선적을 생성하여 현재 사용 가능한 품목을 발송할 수 있습니다. 출하를 제출하면 주문 업데이트가 [!DNL Walmart Marketplace]. 그러면 월마트는 고객에게 주문 현황 및 배송 내역을 알립니다.

* **주문 취소**-다음을 취소할 때 [!DNL Walmart Marketplace] 주문, 월마트는 고객에게 보낸 주문 취소 통지에 포함된 취소 사유를 요구합니다. 취소 사유도 [!DNL Commerce] 주문 결제 정보. 취소를 실행하면 재고 갱신이 [!DNL Walmart Marketplace]. 그러면 월마트는 고객에게 주문 현황 및 배송 내역을 알립니다.

   매점에서 전체 주문을 취소해야 합니다. [!DNL Commerce] 은(는) 부분 취소를 허용하지 않습니다.

* **환불 요청**-배송된 주문에 대해 Walmart Marketplace 반품이 요청되면 [!UICONTROL Status details] 에는 반환에 대한 링크가 포함되어 있습니다. 반품 및 환불은 다음 위치에서 관리됩니다. [반환](return-refund-orders.md) 대시보드입니다.

상거래 주문이 처리되는 경우 및 [!DNL Channel Manager] 에 대한 선적, 부분 선적 및 취소 업데이트를 성공적으로 동기화합니다. [!DNL Walmart Marketplace]주문 처리가 완료되었습니다. 출하된 주문에 대한 반품 요청 및 환불은 [반환](return-refund-orders.md) 대시보드입니다.

>[!NOTE]
>
> 주문 업데이트를 동기화하는 데 최대 5분이 소요될 수 있습니다. [!DNL Walmart Marketplace]. 주문 상태를 확인하려면 [!DNL Channel Manager] 주문 페이지.

## 주문 배송

1. 책임자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 판매 채널 스토어의 눈 모양 아이콘을 선택하여 스토어 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, 선택 **[!UICONTROL Orders]**.

1. 주문 테이블에서 다음을 선택하여 출하할 주문을 엽니다. **상거래 주문 번호**.

1. 다음을 선택하여 주문의 전체 또는 일부에 대한 납품을 생성하고 실행합니다. **[!UICONTROL Ship]**.

   ![다음에 대한 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-detail-with-external-order-id.png)

   * 운송 회사를 선택하고 다음을 선택하여 추적 번호를 추가합니다. **[!UICONTROL Add tracking number]**.

      ![다음에 대한 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-shipment-add-tracking-number.png)


   * 필요에 따라 나머지 선적 양식을 작성하십시오. 다음을 참조하십시오 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 자세한 지침은 을 참조하십시오.

1. 배송을 제출한 후 다음을 추적합니다. [주문 상태](manage-orders.md#about-order-status) 위치: [!DNL Channel Manager] 업데이트가 (으)로 전송되었는지 확인 [!DNL Walmart Marketplace].

주문이 배송된 후 다음 항목에서 전체 또는 부분 환불을 처리할 수 있습니다. [!DNL Channel Manager] (이)에서 받은 반환 요청을 기반으로 주문에 포함된 항목 [!DNL Walmart Marketplace]. 다음을 참조하십시오 [반품 및 환불 주문](return-refund-orders.md).

## 주문 취소

1. 책임자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 판매 채널 스토어의 눈 모양 아이콘을 선택하여 스토어 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, 선택 *[!UICONTROL *Orders]**.

1. Orders 테이블에서 [주문 세부 사항 페이지](manage-orders.md#view-order-detail) 을(를) 선택하여 **상거래 주문 번호** 주문 취소를 위해.

   ![다음에 대한 상거래 주문 세부 사항 보기[!DNL Walmart Marketplace]주문](assets/order-detail-with-external-order-id.png)

1. 주문을 취소합니다.

   * 선택 **취소** 주문 세부 사항 메뉴에서

   * 다음에서 [!UICONTROL Cancel Order] 양식을 선택하고 **취소 이유**.
   ![다음에 대한 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/cancel-order-reason-selector.png)

   * 선택 **주문 취소**.


1. 취소를 제출한 후 [주문 상태](manage-orders.md#about-order-status) 위치: [!DNL Channel Manager] 업데이트가 (으)로 전송되었는지 확인 [!DNL Walmart Marketplace].

## 주문 오류 수정

다음 항목에서 주문 동기화 프로세스 중 오류가 발생할 수 있습니다. [!DNL Walmart Marketplace]또는 선적, 부분 선적 및 취소에 대한 주문 갱신 프로세스 동안.

출하, 부분 출하 또는 취소 갱신의 동기화 작업이 실패할 경우 [!DNL Channel Manager] 주문 페이지에 _오류_ 주문 상태. 배송 정보와 주문 취소 정보가 Walmart Marketplace 계정에 정확하게 반영되도록 하려면 [!DNL Walmart Marketplace] 저장.


