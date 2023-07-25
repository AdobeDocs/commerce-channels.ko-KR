---
title: '소개 - [!DNL Channel Manager]'
description: '설치 및 사용 방법 알아보기 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source 스토어를 Walmart Marketplace와 통합하고 판매 채널을 만들어 상거래 관리자로부터 시장 목록, 가격, 인벤토리 및 판매를 원활하게 관리할 수 있습니다.'
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# 소개 [!DNL Channel Manager]

[!DNL Channel Manager] Adobe Commerce 또는 Magento Open Source 제품 카탈로그를 와 통합하여 판매자가 매출을 증가시키고, 신규 고객에게 도달하며, 판매 운영을 간소화하고, 시간을 절약할 수 있도록 지원합니다. [!DNL Walmart Marketplace].

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager] 은 을 판매하려는 Adobe Commerce 또는 Magento Open Source 판매자를 지원합니다. [!DNL Walmart Marketplace] 를 확장하여 [!DNL Commerce] 관리자. 포함 [!DNL Channel Manager] 설치, 저장소 관리자 및 운영 담당자가 관리할 수 있음 [!DNL Walmart Marketplace] 상거래 환경에서 매출, 재고, 제품 가격 책정 과정이 원활하게 이루어집니다.

확장된 관리자는 판매자가 동일한 워크플로우 및 프로세스를 사용하여 두 플랫폼 모두로부터 판매를 관리할 수 있으므로 운영을 간소화합니다 [!DNL Commerce] 상점 및 월마트 마켓플레이스.

설치 및 구성 후 [!DNL Channel Manager], 다음 기능을 사용하여 Walmart Marketplace 판매 주문을 관리할 수 있습니다.

* **목록 관리**-에서 제품을 일치시켜 제품 목록을 쉽게 연결할 수 있습니다. [!DNL Commerce] 기존 카탈로그로 [!DNL Walmart Marketplace] 목록.

* **Inventory management**-판매자의 마켓 플레이스 판매자 계정의 항목은에서 자동으로 동기화되고 업데이트됩니다. [!DNL Commerce] 정확한 재고 레벨을 보장합니다.

* **가격 업데이트**—자동 가격 동기화를 통해 시장 목록에 대한 정확한 가격 책정 유지 Adobe Commerce에서 가격이 변경되면 변경 사항이 마켓플레이스에 반영됩니다.

* **주문 관리**—마켓플레이스에서 새 주문이 생성되면 [!DNL Channel Manager] 주문을 Adobe Commerce과 동기화하고 주문 승인을 마켓플레이스로 보냅니다. 이 승인은 각 주문에 대해 재고가 예약되어 있음을 보장합니다. 마지막 단계는 [!DNL Commerce] 처리를 위한 Order Management 시스템

* **배송 관리**—Adobe Commerce에서 주문이 출하됨으로 표시되면 선적 업데이트가 [!DNL Walmart Marketplace]. 이 알림을 통해 판매자는 이행 SLA 요구 사항을 충족하고 고객은 현재 주문에 대한 배송 업데이트 알림을 받을 수 있습니다.

* **취소**- Adobe Commerce에서 주문이 취소되는 경우 [!DNL Channel Manager] 업데이트된 주문 정보를 마켓플레이스에 전송하여 해당 마켓플레이스 주문에 대한 작업을 복제합니다. 주문 취소가 완료되면 [!DNL Commerce] 반품된 품목을 반영하는 재고 수량 갱신 및 재고 갱신은 자동으로 다음과 동기화됩니다. [!DNL Walmart Marketplace].

* **반환 및 환불**—Walmart Marketplace에서 Adobe Commerce 또는 Magento Open Source 판매 채널을 통해 주문한 품목의 반품을 요청할 때, [!DNL Channel Manager] 반환 요청을 복제하기 위해 반환 요청 정보를 Commerce 판매 채널 스토어에 보냅니다. 그런 다음 다음을 사용하여 환불을 처리할 수 있습니다. [!DNL Commerce] [환불 워크플로우](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow), 오프라인 메서드. 환불이 완료된 후, [!DNL Channel Manager] 시장 판매자 계정의 반환 상태를 업데이트하여 환불을 반영할 수 있도록 업데이트를 Walmart에 동기화합니다.

## 다음에 대한 예상 지연 시간: [!DNL Channel Manager] 작업

다음 간 데이터 동기화 프로세스 [!DNL Channel Manager] 및 연결된 [!DNL Walmart Marketplace] 스토어를 완료하려면 시간이 좀 필요합니다. 다음에 대한 예상 처리 시간 검토 [!DNL Channel Manager] 영업 채널 운영 계획을 세우는 데 도움이 되는 작업.

**다음에 대한 예상 지연 시간: [!DNL Channel Manager] 작업**

| **작업** | **설명** | **예상 지연** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 에 제품 추가 [!DNL Channel Manager] | 에서 제품 선택 [!DNL Commerce] 제품 카탈로그 및 가져오기 [!DNL Channel Manager]. | **최대 5분**-전체 제품 카탈로그 등 여러 제품을 선택하는 경우 가져오기 시간이 오래 걸립니다. |
| 제품 일치 [!DNL Walmart Marketplace] | 에서 제품 목록 선택 [!DNL Channel Manager] 짝짓기를 위해 월마트로 보내요. | **최대 30분**-많은 제품을 선택하는 경우 선택한 수량에 따라 일치 프로세스가 오래 걸립니다. |
| 인벤토리 업데이트 | Commerce에서 재고 수량이 변경되면 [!DNL Channel Manager] 업데이트를 Walmart에 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변경될 때, [!DNL Channel Manager] 업데이트를 Walmart에 동기화합니다. | **최대 5분** |
| Walmart에서 (으)로 동기화 주문 [!DNL Commerce] | 고객 주문 a [!DNL Commerce] 월마트 마켓플레이스의 제품. 월마트가 주문서를 [!DNL Channel Manager]. 주문이 주문 대시보드에 표시됩니다. | **최대 30분** |
| 주문 생성일: [!DNL Commerce] Order Management | [!DNL Channel Manager] 에서 [!DNL Commerce] Walmart 주문에서 주문하고 다음을 포함하도록 주문 대시보드를 업데이트합니다. [!DNL Commerce] 주문 번호. | **최대 5분** |
| 의 배송 상태 업데이트 [!DNL Commerce] Order Management | 주문이 Commerce에서 발송되면, [!DNL Channel Manager] 주문 대시보드에서 배송 상태를 업데이트하고 고객에게 알릴 수 있도록 업데이트를 Walmart marketplace로 보냅니다. | **최대 5분** |
| Commerce Order Management의 주문 취소 업데이트 | Commerce에서 주문이 취소되면 [!DNL Channel Manager] 주문 대시보드에서 주문 상태를 업데이트하고 고객에게 알릴 수 있도록 업데이트를 Walmart marketplace로 보냅니다. 주문 취소가 완료되면 [!DNL Commerce] 반품된 품목을 반영하도록 재고 수량이 업데이트됩니다. 그런 다음, [!DNL Channel Manager] 업데이트를 로 동기화합니다. [!DNL Walmart Marketplace]. | **최대 5분** |


