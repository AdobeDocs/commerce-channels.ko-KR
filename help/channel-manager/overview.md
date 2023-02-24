---
title: '''소개 - [!DNL Channel Manager]`'
description: '''설치 및 사용 방법 알아보기 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source 스토어를 Walmart Marketplace와 통합하고 판매 채널을 만들어 마켓플레이스 목록, 가격 책정, 재고 및 매출을 상거래 관리자''와 원활하게 관리할 수 있습니다.'
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 소개 [!DNL Channel Manager]

[!DNL Channel Manager] 상인들은 Adobe Commerce 또는 Magento Open Source 제품 카탈로그를 와 통합하여 매출을 늘리고, 신규 고객에게 도달하며, 영업 운영을 간소화하고, 시간을 절약할 수 있도록 지원합니다 [!DNL Walmart Marketplace].

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-home.png)

[!DNL Channel Manager] 에서 판매하려는 Adobe Commerce 또는 Magento Open Source 상인 지원 [!DNL Walmart Marketplace] 다음을 [!DNL Commerce] 관리자. 사용 [!DNL Channel Manager] 설치, 저장 관리자 및 작업 직원이 관리할 수 있습니다. [!DNL Walmart Marketplace] 상거래 환경에서 판매, 재고 및 제품 가격이 원활하게 제공될 수 있습니다.

확장 관리자는 동일한 워크플로우 및 프로세스를 사용하여 두 가지 모두에서 판매량을 관리할 수 있으므로 작업을 간소화합니다 [!DNL Commerce] 상점 전선과 월마트 마켓플레이스

설치 및 구성 후 [!DNL Channel Manager]에서는 다음 기능을 사용하여 Walmart Marketplace 판매 주문을 관리할 수 있습니다.

* **목록 관리**-제품 목록을 사용자의 [!DNL Commerce] 기존 [!DNL Walmart Marketplace] 목록.

* **Inventory management**-머천트의 마켓플레이스 판매자 계정의 항목은 자동으로 동기화되고 [!DNL Commerce] 정확한 재고 수준을 보장할 수 있습니다.

* **가격 업데이트**—자동 가격 동기화를 통해 마켓플레이스 목록에 대한 정확한 가격을 유지합니다. Adobe Commerce에서 가격이 변경되면 변경 사항이 마켓플레이스에 반영됩니다.

* **주문 관리**—마켓플레이스에서 새 주문이 생성되면 [!DNL Channel Manager] 주문을 Adobe Commerce과 동기화하고 주문 승인을 마켓플레이스에 보냅니다. 이러한 승인에서는 각 주문에 대해 재고가 예약되어 있는지 확인합니다. 최종 단계는 의 [!DNL Commerce] 처리할 Order Management 시스템입니다.

* **배송 관리**—주문이 Adobe Commerce에서 출하된 것으로 표시되면, 출하 갱신은 [!DNL Walmart Marketplace]. 이 알림은 판매자가 이행 SLA 요구 사항을 충족하고 고객이 현재 주문에 대한 배송 업데이트 알림을 받을 수 있도록 해줍니다.

* **취소**- Adobe Commerce에서 주문이 취소되면, [!DNL Channel Manager] 업데이트된 주문 정보를 marketplace에 전송하여 해당 마켓플레이스 주문에 대한 작업을 복제합니다. 주문 취소가 완료되면 [!DNL Commerce] 반환된 품목 및 재고 갱신을 반영하도록 재고 수량 갱신을 자동으로 [!DNL Walmart Marketplace].

* **반환 및 반환**- Walmart Marketplace에서 Adobe Commerce 또는 Magento Open Source 판매 채널을 통해 주문되는 항목에 대한 반환을 요청하면, [!DNL Channel Manager] 반환 요청을 복제하기 위해 상거래 판매 채널 저장소에 반환 요청 정보를 보냅니다. 그런 다음, [!DNL Commerce] [환불 워크플로우](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow), 오프라인 메서드. 환불이 완료되면, [!DNL Channel Manager] 업데이트를 Walmart에 동기화하여 marketplace 판매자 계정의 반환 상태를 업데이트하여 환불을 반영할 수 있습니다.

## 에 대한 예상 지연 [!DNL Channel Manager] 작업

데이터 동기화 프로세스 간 [!DNL Channel Manager] 연결된 [!DNL Walmart Marketplace] 스토어를 완료하려면 시간이 필요합니다. 에 대한 예상 처리 시간 검토 [!DNL Channel Manager] 영업 채널 작업 계획을 지원하는 작업입니다.

**예상 지연 시간 [!DNL Channel Manager] 작업**

| **작업** | **설명** | **예상 지연** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 에 제품 추가 [!DNL Channel Manager] | 에서 제품 선택 [!DNL Commerce] 제품 카탈로그를 로 가져와서 [!DNL Channel Manager]. | **최대 5분**-전체 제품 카탈로그와 같이 제품을 많이 선택하면 가져오기 프로세스가 길어집니다. |
| 제품 일치 [!DNL Walmart Marketplace] | 에서 제품 목록을 선택합니다. [!DNL Channel Manager] 매칭으로 월마트로 보내주세요 | **최대 30분**-여러 제품을 선택하면 선택한 수량에 따라 대응 프로세스가 더 길어집니다. |
| 인벤토리 업데이트 | 상거래에 재고 수량이 변경되면 [!DNL Channel Manager] Walmart에 업데이트를 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변하면, [!DNL Channel Manager] Walmart에 업데이트를 동기화합니다. | **최대 5분** |
| Walmart에서 다음으로 주문 동기화 [!DNL Commerce] | 고객이 주문 [!DNL Commerce] Walmart Marketplace의 제품. 월마트는 주문을 [!DNL Channel Manager]. 순서는 주문 대시보드에 표시됩니다. | **최대 30분** |
| 작성 순서 [!DNL Commerce] Order Management | [!DNL Channel Manager] 만들기 [!DNL Commerce] Walmart 주문에서 주문하고 주문 대시보드를 업데이트하여 [!DNL Commerce] 주문 번호. | **최대 5분** |
| 의 배송 상태 업데이트 [!DNL Commerce] Order Management | 상거래 주문에서 배송되면, [!DNL Channel Manager] 주문 대시보드의 배송 상태를 업데이트하고 업데이트를 Walmart 마켓플레이스로 보내어 고객에게 알릴 수 있습니다. | **최대 5분** |
| Commerce Order Management에서 주문 취소 업데이트 | 상거래 주문이 취소되면 [!DNL Channel Manager] 주문 대시보드의 주문 상태를 업데이트하고 고객이 알림을 받을 수 있도록 업데이트를 Walmart 마켓플레이스로 보냅니다. 주문 취소가 완료되면 [!DNL Commerce] 반환된 품목을 반영하도록 재고 수량 업데이트. 그럼, [!DNL Channel Manager] 업데이트를에 동기화 [!DNL Walmart Marketplace]. | **최대 5분** |


