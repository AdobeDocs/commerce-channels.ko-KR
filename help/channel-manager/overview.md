---
title: 정보 [!DNL Channel Manager]
description: 설치 및 사용 방법 알아보기 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source 스토어를 타사 마켓플레이스와 통합하고 판매 채널을 만들어 마켓플레이스 목록, 가격, 인벤토리 및 판매를 상거래 관리자와 원활하게 관리할 수 있습니다.
role: User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 9ccd205ccd4f4b3f4e6b9fed2c4d16893f4b0da8
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# 정보 [!DNL Channel Manager]

[!DNL Channel Manager] 은 Adobe Commerce 또는 Magento Open Source 제품 카탈로그를 와 통합하여 매출을 늘리고 새 고객에게 도달하도록 도와줍니다. [!DNL Walmart US Marketplace].

![[!DNL Channel Manager] 확장 관리자 보기](assets/channel-manager-home.png)

채널 관리자는 Walmart Marketplace에서 판매하려는 Adobe Commerce 또는 Magento Open Source 판매자를 지원합니다.

설치 및 구성 후 [!DNL Channel Manager], [!DNL Commerce] 관리자가 확장되어 관리할 수 있습니다 [!DNL Walmart Marketplace] 상거래 환경에서 원활하게 영업 운영 수행

* **목록 관리**-전자 상거래 카탈로그의 제품을 기존 Walmart Marketplace 목록에 일치시켜 제품 목록을 쉽게 게시합니다.

* **Inventory management**-머천트의 마켓플레이스 판매자 계정의 항목은 정확한 재고 수준을 보장하기 위해 상거래에서 자동으로 동기화되고 업데이트됩니다.

* **가격 업데이트**-자동 가격 동기화를 통해 시장 목록을 위한 정확한 가격 책정 유지 Adobe Commerce에서 가격이 변경되면 10분 이내에 변경 사항이 마켓플레이스에 반영됩니다.

* **주문 관리**-마켓플레이스에서 새로운 주문이 생성되면 Channel Manager는 주문을 Adobe Commerce과 동기화하고 주문 확인을 마켓플레이스에 보내 각 주문에 대해 재고가 예약되도록 합니다.

* **배송 관리**-Adobe Commerce에서 주문이 출하된 것으로 표시되면, 출하 갱신은 [!DNL Walmart Marketplace]. 이 알림은 판매자가 이행 SLA 요구 사항을 충족하고 고객이 현재 주문에 대한 배송 업데이트 알림을 받을 수 있도록 해줍니다.

* **취소**-Adobe Commerce에서 주문이 취소되면 Channel Manager는 업데이트된 주문 정보를 마켓플레이스에 전송하여 해당 마켓플레이스 주문에 대한 작업을 복제합니다.

## 채널 관리자 작업의 예상 지연

데이터 동기화 프로세스 간 [!DNL Channel Manager] 연결된 [!DNL Walmart Marketplace] 스토어를 완료하려면 시간이 필요합니다. 에 대한 예상 처리 시간 검토 [!DNL Channel Manager] 영업 채널 작업 계획을 지원하는 작업입니다.

**채널 관리자 작업의 예상 지연**

| **작업** | **설명** | **예상 지연** |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 채널 관리자에 제품 추가 | 상거래 제품 카탈로그에서 제품을 선택하고 채널 관리자로 가져옵니다. | **최대 5분**-전체 제품 카탈로그와 같이 제품을 많이 선택하면 가져오기 프로세스가 길어집니다. |
| Walmart Marketplace에서 제품 일치 | 채널 관리자에서 제품 목록을 선택하고 매칭하려면 Walmart로 보내십시오. | **최대 30분**-여러 제품을 선택하면 선택한 수량에 따라 대응 프로세스가 더 길어집니다. |
| 인벤토리 업데이트 | 상거래에 재고 수량이 변경되면 [!DNL Channel Manager] Walmart에 업데이트를 동기화합니다. | **최대 10분** |
| 가격 업데이트 | 제품 가격이 변경되면 Channel Manager 는 업데이트를 Walmart로 동기화합니다. | **최대 5분** |
| Walmart에서 Commerce로 주문 동기화 | 고객은 Walmart Marketplace에서 상거래 제품을 주문합니다. Walmart가 채널 관리자에게 주문을 보냅니다. 순서는 주문 대시보드에 표시됩니다. | **최대 30분** |
| Commerce Order Management에서 만든 순서 | 채널 관리자는 Mart 주문에서 상거래 주문을 만들고 상거래 주문 번호를 포함하도록 주문 대시보드를 업데이트합니다. | **최대 5분** |

