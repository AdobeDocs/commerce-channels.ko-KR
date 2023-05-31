---
title: Amazon 이행 워크플로우
description: Amazon 목록의 주문에 대한 이행은 주문 실행에서 배송까지의 특정 순서를 따릅니다.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon 이행 워크플로우

## 예: 판매자가 이행함

| 단계 | 설명 |
|----|----|
| 1 | **판매자가 이행한 주문이 Amazon에 있습니다.** Amazon이 다음 상태를 할당함: `Pending` 고객의 신용카드 정보가 확인될 때까지. 의 주문 `Pending` 상태는 자동으로 Amazon 판매 채널로 가져오지만 _[!UICONTROL Orders]_탭. |
| 2 | **Amazon에서 주문을 확인합니다.** 확인되면 Amazon에서 상태를 로 변경합니다. `Unshipped`. 이 상태 변경으로 주문이 Amazon 판매 채널에서 업데이트되고 _[!UICONTROL Orders]_탭. |
| 3 | **주문 세부 사항이 업데이트됩니다.** Amazon 판매 채널은 가격, 고객 이메일 및 고객 이름으로 주문 세부 사항을 업데이트합니다. 이 업데이트 중에 Amazon 주문에서 해당 [!DNL Commerce] order management 페이지에서 주문합니다. 다음 [!DNL Commerce] 주문 번호가 다음에 대한 주문 정보와 함께 표시됩니다. _[!UICONTROL Orders]_탭. |
| 4 | **새 고객 계정이 만들어집니다.** 주문 설정에 구성되어 있고 고객이 [!DNL Commerce] 데이터베이스에서 새 고객은 [!DNL Commerce] Amazon 주문의 해당 고객 정보를 사용하는 데이터베이스. 다음을 선택한 경우 `No Customer Creation (guest)` 순서 설정에서 순서는 다음을 따릅니다. [!DNL Commerce] 게스트 프로세스이며 데이터베이스에서 고객을 만들지 않습니다. 이 시점에서 [!DNL Commerce] 시스템은 ERP/OMS/WMS와 통합되며, 내부 주문 및 생성된 신규 주문의 통합에 따라 주문이 선택됩니다 [!DNL Commerce]. |
| 5 | **주문이 배송되었습니다.** 다음에서 [!DNL Commerce] 주문 처리 페이지에서 주문을 배송하고 추적 번호를 추가합니다. 모든 항목이 `Shipped` 상태:<ul><li>의 상태 [!DNL Commerce] 주문 변경 대상 `Complete`.</li><li>Amazon 판매 채널 주문의 상태가 (으)로 변경됩니다. `Shipped`.</li><li>추적 번호가 Amazon에 동기화되고 Amazon 주문 상태가 (으)로 변경됩니다. `Shipped`.</li><li>배송 알림은 다음 대상이 아닌 Amazon을 통해 고객에게 전송됩니다. [!DNL Commerce] (Amazon 정책에 따라). |

## 예: Amazon(FBA)에서 이행

| 단계 | 설명 |
|---|---|
| 1 | **Amazon 이행 주문은 Amazon에 배치됩니다.** |
| 2 | **주문을 가져왔습니다.** 주문이 할당된 후에야 Amazon 판매 채널로 주문을 가져올 수 있습니다. `Shipped` Amazon별 상태. Amazon은 이 제품에 대한 재고를 가지고 있으므로 창고/재고 관리에 방해가 되지 않도록 합니다. |
| 3 | **주문 세부 사항이 업데이트됩니다.** 에 구성된 경우 [주문 설정](./order-settings.md), Amazon 주문에서 해당하는 을 만듭니다. [!DNL Commerce] 주문 및 상태가 인 주문으로 생성 `Complete`. |
