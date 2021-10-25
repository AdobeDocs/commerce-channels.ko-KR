---
title: Amazon 이행 워크플로우
description: Amazon 목록의 주문에 대한 이행은 주문 제출에서 배송에 이르는 특정 시퀀스를 따릅니다.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon 이행 워크플로우

## 예: 상인에 대한 이행

| 단계 | 설명 |
|----|----|
| 1 | **Amazon에 상인이 이행된 주문이 제출됩니다.** Amazon이 상태 지정 `Pending` 고객의 신용 카드 정보가 확인될 때까지. 주문 `Pending` 상태는 자동으로 Amazon 판매 채널로 가져오지만 _[!UICONTROL Orders]_탭. |
| 2개 | **이 순서는 Amazon에 의해 확인됩니다.** 확인되면 Amazon이 상태를 로 변경합니다. `Unshipped`. 이 상태가 변경되면 주문은 Amazon 판매 채널에서 업데이트되고 _[!UICONTROL Orders]_탭. |
| 3 | **주문 세부 사항이 업데이트됩니다.** Amazon 판매 채널은 가격, 고객 이메일 및 고객 이름으로 주문 세부 사항을 업데이트합니다. 이 업데이트 중에 Amazon 순서는 해당 [!DNL Commerce] order management 페이지의 순서. 다음 [!DNL Commerce] 주문 번호는 _[!UICONTROL Orders]_탭. |
| 4 | **새 고객 계정이 만들어집니다.** 주문 설정에 구성되었으며 고객이 [!DNL Commerce] 데이터베이스에서 새 고객이 생성되면 [!DNL Commerce] Amazon 주문의 해당 고객 정보를 사용하는 데이터베이스입니다. 선택한 경우 `No Customer Creation (guest)` 주문 설정에서 순서는 [!DNL Commerce] 데이터베이스에 고객을 만들지 않고 게스트 프로세스를 수행합니다. 이 시점에서 [!DNL Commerce] 시스템은 ERP/OMS/WMS와 통합되며, 내부에 배치되고 생성되는 새로운 주문의 통합 시 주문이 선택됩니다 [!DNL Commerce]. |
| 5개 | **주문품이 배송됩니다** 에서 [!DNL Commerce] 주문 처리 페이지에서 주문을 출하하고 추적 번호를 추가합니다. 모든 항목이 `Shipped` 상태:<ul><li>의 상태 [!DNL Commerce] 주문 변경 `Complete`.</li><li>Amazon 판매 채널 주문 상태가 `Shipped`.</li><li>추적 번호가 Amazon에 동기화되고 Amazon의 주문 상태가 `Shipped`.</li><li>배송 알림은 고객이 아닌 Amazon을 통해 고객에게 전송됩니다 [!DNL Commerce] (Amazon의 정책에 따라) |

## 예: Amazon(FBA)에 의해 처리됨

| 단계 | 설명 |
|---|---|
| 1 | **Amazon 이행 주문이 Amazon에 배치됩니다.** |
| 2개 | **주문을 가져옵니다.** 주문이 할당될 때까지 해당 주문은 Amazon 판매 채널로 가져오지 않습니다 `Shipped` Amazon의 상태입니다. Amazon은 이 제품에 대한 인벤토리가 있으므로 웨어하우스/재고 관리에 대한 간섭을 방지합니다. |
| 3 | **주문 세부 사항이 업데이트됩니다.** 에 구성된 경우 [순서 설정](./order-settings.md)로 지정하는 경우 Amazon 순서에 따라 [!DNL Commerce] 주문 및 상태 `Complete`. |
