---
title: ' [!DNL Channel Manager] 소개'
description: 'Adobe Commerce 및 Magento Open Source 스토어를 Walmart Marketplace와 통합하고 판매 채널을 만들어 Commerce 관리자로부터 마켓플레이스 목록, 가격, 인벤토리 및 판매를 원활하게 관리하는  [!DNL Channel Manager] 의 설치 및 사용 방법에 대해 알아봅니다.'
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---


# [!DNL Channel Manager] 소개

[!DNL Channel Manager]은(는) Adobe Commerce 또는 Magento Open Source 제품 카탈로그를 [!DNL Walmart Marketplace]과(와) 통합하여 판매자가 매출을 늘리고, 신규 고객에게 도달하고, 판매 운영을 간소화하고, 시간을 절약할 수 있도록 지원합니다.

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager]은(는) [!DNL Commerce] 관리자를 확장하여 [!DNL Walmart Marketplace]에서 판매하려는 Adobe Commerce 또는 Magento Open Source 판매자를 지원합니다. [!DNL Channel Manager]이(가) 설치되면 스토어 관리자 및 운영 직원은 Commerce 환경에서 [!DNL Walmart Marketplace] 판매, 인벤토리 및 제품 가격을 원활하게 관리할 수 있습니다.

확장된 관리자는 동일한 워크플로우 및 프로세스를 사용하여 [!DNL Commerce] 상점 및 월마트 마켓플레이스에서 판매를 관리할 수 있으므로 운영을 간소화합니다.

[!DNL Channel Manager]을(를) 설치하고 구성한 후 다음 기능을 사용하여 Walmart Marketplace 판매 주문을 관리할 수 있습니다.

* **목록 관리**-[!DNL Commerce] 카탈로그의 제품을 기존 [!DNL Walmart Marketplace] 목록에 일치시켜 제품 목록을 쉽게 연결합니다.

* 판매자의 마켓플레이스 판매자 계정에 있는 **Inventory management**-항목은 정확한 재고 수준을 보장하기 위해 [!DNL Commerce]에서 자동으로 동기화되고 업데이트됩니다.

* **가격 업데이트**—자동 가격 동기화를 통해 마켓플레이스 목록에 대한 정확한 가격을 유지하세요. Adobe Commerce에서 가격이 변경되면 변경 사항이 마켓플레이스에 반영됩니다.

* **주문 관리**—마켓플레이스에서 새 주문이 만들어지면 [!DNL Channel Manager]에서 주문을 Adobe Commerce과 동기화하고 주문 승인을 마켓플레이스로 보냅니다. 이 승인은 각 주문에 대해 재고가 예약되어 있음을 보장합니다. 마지막 단계는 처리를 위해 [!DNL Commerce] Order Management 시스템에서 해당 주문을 만드는 것입니다.

* **배송 관리**—주문이 Adobe Commerce에서 배송된 것으로 표시되면 배송 업데이트가 [!DNL Walmart Marketplace](으)로 전송됩니다. 이 알림을 통해 판매자는 이행 SLA 요구 사항을 충족하고 고객은 현재 주문에 대한 배송 업데이트 알림을 받을 수 있습니다.

* **취소**—Adobe Commerce에서 주문이 취소되면 [!DNL Channel Manager]이(가) 업데이트된 주문 정보를 마켓플레이스로 전송하여 해당 마켓플레이스 주문에 대한 작업을 복제합니다. 주문 취소가 완료되면 반품된 항목을 반영하도록 [!DNL Commerce] 재고 수량 업데이트가 자동으로 [!DNL Walmart Marketplace]에 동기화됩니다.

* **반환 및 반환**—Walmart Marketplace에서 Adobe Commerce 또는 Magento Open Source 판매 채널을 통해 주문한 항목에 대한 반환을 요청하면 [!DNL Channel Manager]에서 반환 요청 정보를 Commerce 판매 채널 스토어로 보내 반환 요청을 복제합니다. 그런 다음 [!DNL Commerce] [환불 워크플로우](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow), 오프라인 메서드를 사용하여 환불을 처리할 수 있습니다. 환불이 완료된 후 [!DNL Channel Manager]은(는) 업데이트를 월마트에 동기화하여 마켓플레이스 판매자 계정의 반환 상태를 업데이트하여 환불을 반영할 수 있습니다.

## [!DNL Channel Manager] 작업에 필요한 대기 시간

[!DNL Channel Manager]과(와) 연결된 [!DNL Walmart Marketplace] 저장소 간의 데이터 동기화 프로세스를 완료하려면 시간이 필요합니다. [!DNL Channel Manager] 작업에 대한 예상 처리 시간을 검토하여 판매 채널 작업이 제대로 작동하도록 계획합니다.

**[!DNL Channel Manager]개 작업에 대한 예상 대기 시간**

| **작업** | **설명** | **지연이 예상됨** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| [!DNL Channel Manager]에 제품 추가 | [!DNL Commerce] 제품 카탈로그에서 제품을 선택하고 [!DNL Channel Manager](으)로 가져오십시오. | **최대 5분**-전체 제품 카탈로그 등 여러 제품을 선택하는 경우 가져오기 프로세스가 더 오래 걸립니다. |
| [!DNL Walmart Marketplace]의 제품 일치 | [!DNL Channel Manager]에서 제품 목록을 선택하고 일치시킬 Walmart로 보내십시오. | **최대 30분**-제품을 많이 선택하면 선택한 수량에 따라 일치 프로세스가 더 오래 걸립니다. |
| 인벤토리 업데이트 | Commerce에서 재고 수량이 변경되면 [!DNL Channel Manager]에서 업데이트를 Walmart로 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변경되면 [!DNL Channel Manager]에서 업데이트를 Walmart에 동기화합니다. | **최대 5분** |
| Walmart에서 [!DNL Commerce](으)로 동기화 주문 | 고객이 Walmart Marketplace에서 [!DNL Commerce] 제품을 주문합니다. 월마트가 주문을 [!DNL Channel Manager](으)로 보냅니다. 주문이 주문 대시보드에 표시됩니다. | **최대 30분** |
| [!DNL Commerce] Order Management에서 만들어진 순서 | [!DNL Channel Manager]이(가) Walmart 주문에서 [!DNL Commerce] 주문을 만들고 [!DNL Commerce] 주문 번호를 포함하도록 주문 대시보드를 업데이트합니다. | **최대 5분** |
| [!DNL Commerce] Order Management의 배송 상태 업데이트 | Commerce에서 주문이 배송되면 [!DNL Channel Manager]이(가) 주문 대시보드에서 배송 상태를 업데이트하고 고객에게 알릴 수 있도록 업데이트를 월마트 마켓플레이스로 보냅니다. | **최대 5분** |
| Commerce Order Management의 주문 취소 업데이트 | Commerce에서 주문이 취소되면 [!DNL Channel Manager]에서 주문 대시보드의 주문 상태를 업데이트하고 고객에게 알릴 수 있도록 업데이트를 Walmart 마켓플레이스로 보냅니다. 주문 취소가 완료되면 반환된 항목을 반영하도록 [!DNL Commerce] 재고 수량이 업데이트됩니다. 그런 다음 [!DNL Channel Manager]이(가) 업데이트를 [!DNL Walmart Marketplace](으)로 동기화합니다. | **최대 5분** |


