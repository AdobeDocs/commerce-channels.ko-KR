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
| 1 | **Amazon에 상인이 이행된 주문이 제출됩니다.** Amazon은 고객의 신용 카드 정보가 확인될  `Pending` 때까지 상태를 지정합니다. `Pending` 상태의 주문은 Amazon 판매 채널로 자동으로 가져오지만 _[!UICONTROL Orders]_탭에는 표시되지 않습니다. |
| 2개 | **이 순서는 Amazon에 의해 확인됩니다.** 확인되면 Amazon이 상태를 로 변경합니다 `Unshipped`. 이 상태가 변경되면 Amazon 판매 채널에서 주문이 업데이트되고 _[!UICONTROL Orders]_탭에 표시됩니다. |
| 1 | **주문 세부 사항이 업데이트됩니다.** Amazon 판매 채널은 가격, 고객 이메일 및 고객 이름으로 주문 세부 사항을 업데이트합니다. 이 업데이트 중에 Amazon 순서는 주문 관리 페이지에서 해당 [!DNL Commerce] 순서를 만듭니다. [!DNL Commerce] 주문 번호는 _[!UICONTROL Orders]_탭에 주문 정보와 함께 표시됩니다. |
| 4 | **새 고객 계정이 만들어집니다.** 주문 설정에 구성되어 있고 고객이 데이터베이스에  [!DNL Commerce] 없는 경우 Amazon 순서의 해당 고객  [!DNL Commerce] 정보를 사용하여 새 고객이 데이터베이스에 생성됩니다. 주문 설정에서 `No Customer Creation (guest)`을(를) 선택한 경우 이 순서는 [!DNL Commerce] 게스트 프로세스를 따르며 데이터베이스에 고객을 만들지 않습니다. 이때 [!DNL Commerce] 시스템이 ERP/OMS/WMS와 통합된 경우, [!DNL Commerce] 내부에 배치되고 생성되는 새 주문의 통합에 따라 주문이 선택됩니다. |
| 5개 | **주문품이 배송됩니다** 주문  [!DNL Commerce] 처리 페이지에서 주문을 출하하고 추적 번호를 추가합니다. 모든 항목이 `Shipped` 상태로 표시된 경우:<ul><li>[!DNL Commerce] 주문 상태가 `Complete`로 변경됩니다.</li><li>Amazon 판매 채널 주문 상태가 `Shipped`으로 변경됩니다.</li><li>추적 번호가 Amazon에 동기화되고 Amazon의 순서 상태가 `Shipped`으로 변경됩니다.</li><li>배송 알림은 [!DNL Commerce](Amazon의 정책에 따라)이 아니라 Amazon을 통해 고객에게 전송됩니다. |

## 예: Amazon(FBA)에 의해 처리됨

| 단계 | 설명 |
|---|---|
| 1 | **Amazon 이행 주문이 Amazon에 배치됩니다.** |
| 2개 | **주문을 가져옵니다.** 이 주문은 Amazon에서 상태를 지정할 때까지 Amazon 판매 채널 `Shipped` 으로 가져오지 않습니다. Amazon은 이 제품에 대한 인벤토리가 있으므로 웨어하우스/재고 관리에 대한 간섭을 방지합니다. |
| 1 | **주문 세부 사항이 업데이트됩니다.** 주문  [설정에](./order-settings.md) 구성된 경우 Amazon 순서는 해당  [!DNL Commerce] 순서를 생성하고 상태가  `Complete`인 주문으로 만들어집니다. |
