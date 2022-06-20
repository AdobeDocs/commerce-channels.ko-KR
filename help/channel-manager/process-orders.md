---
title: 주문 처리
description: '운송 및 취소에 대한 지침 [!DNL Walmart Marketplace] 주문: Adobe Commerce 및 Magento Open Source.'
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: aeb3e4883a92f8dbd1725a70102401ad733ee391
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 주문 처리

후 [!DNL Walmart Marketplace] 주문은 확인되었으며 성공적으로 [!DNL Channel Manager], [상거래 주문 관리](https://docs.magento.com/user-guide/sales/orders-workspace.html) 주문 처리

채널 관리자는 업데이트를 [!DNL Walmart Marketplace] 상거래 주문 상태 및 배송 정보가 [!DNL Walmart Marketplace].

* **주문 선적**&quot;월마트는 모든 배송에 대한 추적 번호가 필요합니다. 일부 품목이 재고가 없는 경우 부분 선적을 생성하여 현재 사용 가능한 품목을 발송할 수 있습니다. 출하를 실행한 후 주문 갱신은 [!DNL Walmart Marketplace]. 그리고 나서, 월마트는 고객에게 주문 상태와 배송 세부 사항을 알려준다.

* **주문 취소**-취소 시 [!DNL Walmart Marketplace] 주문, 월마트는 고객에게 발송되는 주문 취소 공지에 포함된 취소 사유가 필요합니다. 취소 사유는에 표시됩니다 [!DNL Commerce] 주문 결제 정보. 취소를 실행하면 재고 갱신은 [!DNL Walmart Marketplace]. 그리고 나서, 월마트는 고객에게 주문 상태와 배송 세부 사항을 알려준다.

   창고에서 전체 주문을 취소하셔야 합니다 상거래에 의해 부분 취소를 허용하지 않습니다.

상거래 주문이 처리되고 [!DNL Channel Manager] 선적, 부분 선적 및 취소 업데이트를 성공적으로 동기화합니다. [!DNL Walmart Marketplace]로 설정되면 주문 처리가 완료됩니다.

>[!NOTE]
>
> 주문 업데이트를 동기화하려면 최대 5분이 걸릴 수 있습니다 [!DNL Walmart Marketplace]. 주문 상태를 확인하려면 [!DNL Channel Manager] 주문 페이지.

## 주문 배송

1. 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 판매 채널 저장소에 대한 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, * 선택[!UICONTROL *Orders]**.

1. Orders 테이블에서, **상거래 주문 번호**.

1. 선택을 통해 주문의 전체 또는 일부에 대한 선적을 생성하고 실행합니다 **[!UICONTROL Ship]**.

   ![전자 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-detail-with-external-order-id.png)

   * 운송 회사를 선택하고 을(를) 선택하여 추적 번호를 추가합니다 **[!UICONTROL Add tracking number]**.

      ![전자 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-shipment-add-tracking-number.png)


   * 필요에 따라 나머지 배송 양식을 작성하십시오. 자세한 내용은 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 자세한 지침

1. 출하를 실행한 후, [주문 상태](manage-orders.md#about-order-status) in [!DNL Channel Manager] 업데이트를에 보냈는지 확인하려면 [!DNL Walmart Marketplace].

## 주문 취소

1. 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. 판매 채널 저장소에 대한 눈 아이콘을 선택하여 저장소 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, * 선택[!UICONTROL *Orders]**.

1. 주문 테이블에서 주문 세부 사항 페이지를 열고 **상거래 주문 번호** 취소하시려면

   ![전자 상거래 주문 세부 사항 보기[!DNL Walmart Marketplace]주문](assets/order-detail-with-external-order-id.png)

1. 주문을 취소하세요.

   * 선택 **취소** 주문 세부 사항 메뉴에서 를 선택합니다.

   * 설정 [!UICONTROL Cancel Order] 양식을 선택하고 **취소 이유**.
   ![전자 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/cancel-order-reason-selector.png)

   * 선택 **주문 취소**.


1. 취소를 제출한 후 다음을 추적합니다 [주문 상태](manage-orders.md#about-order-status) in [!DNL Channel Manager] 업데이트를에 보냈는지 확인하려면 [!DNL Walmart Marketplace].

## 주문 오류 수정

Order 동기화 프로세스 중에 [!DNL Walmart Marketplace]또는 출하, 부분 출하 및 취소에 대한 주문 갱신 프로세스 중에

선적, 부분 선적 또는 취소 갱신에 대한 동기화 작업이 실패하면 [!DNL Channel Manager] 주문 페이지에 _오류_ 주문 상태. 배송 정보 및 주문 취소 정보가 Walmart Marketplace 계정에 정확하게 반영되도록 하려면, [!DNL Walmart Marketplace] 저장.


