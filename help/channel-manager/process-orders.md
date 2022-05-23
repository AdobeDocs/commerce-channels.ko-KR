---
title: 주문 처리
description: '운송 및 취소에 대한 지침 [!DNL Walmart Marketplace] 주문: Adobe Commerce 및 Magento Open Source.'
source-git-commit: 5670639697550b2d7fee67dd29be9c6278d5782b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# 주문 처리

Adobe Commerce 및 Magento Open Source Order Management를 사용하여 [!DNL Commerce] 판매 저장, 프로세스 [!DNL Walmart Marketplace] 유사한 워크플로우를 사용하여 Commerce에서 주문.

Commerce에서 순서를 처리할 때 채널 관리자는 업데이트를 [!DNL Walmart Marketplace]. 이 업데이트를 통해 Commerce의 제품 인벤토리 및 주문 상태가 [!DNL Walmart Marketplace] 및 는 Walmart에 주문 상태와 배송 정보를 고객에게 전송하도록 알립니다.

>[!NOTE]
>
> 주문 업데이트를 동기화하려면 최대 5분이 걸릴 수 있습니다 [!DNL Walmart Marketplace]. 주문 상태를 확인하려면 [!DNL Channel Manager] 주문.

## 주문 배송

상거래 주문을 출하할 때 [[!DNL Commerce Order Management] 배송 워크플로우](https://docs.magento.com/user-guide/sales/order-ship.html). 주문을 제출하면 업데이트가 [!DNL Walmart Marketplace]. 그리고 나서, 월마트는 고객에게 주문 상태와 배송 세부 사항을 알려준다.

**전제 조건**

주문 배송 전에 [채널 배송 설정 및 통신사 구성](map-shipping-carriers.md) 모임 [!DNL Walmart Marketplace requirements].

### 선적을 생성 및 실행합니다

배송 시 [!DNL Walmart Marketplace] 주문 위치 [!DNL Commerce]로 지정하는 경우 추적 번호를 추가해야 합니다. 고객은 발송자로부터 받은 선적 통지에서 추적 번호를 받습니다 [!DNL Walmart].

1. 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 열다 [!UICONTROL Channel Manager Marketplace Stores] 페이지.

1. 판매 채널 저장소에 대한 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, * 선택[!UICONTROL *Orders]**.

1. Orders 테이블에서, **상거래 주문 번호**.

1. 선택을 통해 주문의 전체 또는 일부에 대한 선적을 생성하고 실행합니다 **[!UICONTROL Ship]**.

   - 운송 회사를 선택하고 추적 번호를 추가하려면 **[!UICONTROL Add tracking number]**.

   - 필요에 따라 나머지 배송 양식을 작성하십시오. 자세한 내용은 [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) 자세한 지침

1. 출하를 실행한 후, [주문 상태](manage-orders.md#about-order-status) in [!DNL Channel Manager] 업데이트를에 보냈는지 확인하려면 [!DNL Walmart Marketplace].

## 주문 취소

취소 시 [!DNL Walmart Marketplace] 주문, 월마트는 취소 이유가 필요합니다. 주문 취소가 Walmart로 갱신되면, 취소 사유는 고객에게 발송된 취소 통지에 포함됩니다.

취소 사유는에 표시됩니다 [!DNL Commerce] 주문 결제 정보.

1. 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 열다 [!UICONTROL Channel Manager Marketplace Stores] 페이지.

1. 판매 채널 저장소에 대한 눈 아이콘을 선택하여 저장소 보기를 엽니다.

1. 보려면 [!DNL Walmart Marketplace] 주문, * 선택[!UICONTROL *Orders]**.

1. 주문 테이블에서 주문 세부 사항 페이지를 열고 **상거래 주문 번호** 취소하시려면

   ![Walmart Marketplace 주문에 대한 상거래 주문 세부 사항 보기](assets/order-detail-with-external-order-id.png)

1. 주문을 취소하세요.

   - 선택 **취소** 주문 세부 사항 메뉴에서 를 선택합니다.

   - 주문 취소 양식에서 **취소 이유**.

      ![Walmart Marketplace 주문에 대한 상거래 주문 세부 사항 보기](assets/order-detail-with-external-order-id.png)

   - 선택 **주문 취소**.

1. 업데이트가 로 전송되었는지 확인 [!DNL Walmart Marketplace] 다음을 확인하여 [주문 상태](manage-orders.md#about-order-status) in [!DNL Channel Manager].
