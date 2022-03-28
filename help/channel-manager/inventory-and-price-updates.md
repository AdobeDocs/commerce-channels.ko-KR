---
title: 재고 및 가격 업데이트
description: '`[!DNL Channel Manager] 상거래 스토어와 가격 업데이트 동기화 [!DNL Walmart Marketplace] Commerce Admin에서 영업 채널 작업을 관리할 수 있습니다.'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a1944052f02968c36495275cd5ddfb2ca43ce967
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 재고 및 가격 업데이트

[!DNL Channel Manager] 채널 저장소에서 제품에 대한 인벤토리 및 가격을 추적합니다. 재고 또는 가격이 변경되면 두 가지 모두에 대한 동기화가 업데이트됩니다 [!DNL Channel Manager] 및 [!DNL Walmart Marketplace] 제품 목록에 현재 재고 수량 및 가격을 반영하도록 했습니다.

## 인벤토리 업데이트

재고 수준이 변경되면 Channel Manager는 Commerce와 Walmart Marketplace 간에 업데이트를 동기화하여 Channel Manager와 Walmart Marketplace의 재고 수량이 올바른지 확인합니다.

채널 관리자와 마켓플레이스 간에 인벤토리 업데이트를 동기화하는 데 최대 10분이 걸릴 수 있습니다.

* **제품 카탈로그의 재고 수량에 대한 업데이트**-다음 이유로 인해 상거래 주식이 변경되는 경우 [수동 재고 수량 변경](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html)채널 관리자는 연결된 채널 및 [!DNL Walmart Marketplace].

* **Walmart Marketplace 주문을 반영하도록 재고 수량을 줄입니다**-Walmart Marketplace 주문이 채널 관리자에게 동기화되면 채널 관리자는 상거래 주문 시스템에 업데이트를 보냅니다. 상거래는 주문에 따라 주식 수량을 조정합니다. 그런 다음 업데이트된 수량이 Walmart Marketplace에 동기화됩니다. 동기화 작업이 완료될 때까지 Channel Manager와 Marketplace의 수량 차이를 볼 수 있습니다.

>[!IMPORTANT]
>
> Walmart Marketplace 주문이 채널 관리자에게 동기화되면 Commerce에서 시작된 환불 및 취소에 대해서만 재고 수량 및 주문 정보가 업데이트됩니다. Walmart Marketplace에서 주문이 반환되거나 취소되는 경우 상거래 재고 수량 및 주문 정보의 정확성을 위해 상거래 변경을 처리합니다.

## 가격 업데이트

Commerce에서 제품 가격이 변경되면 Channel Manager는 [!DNL Commerce] 제품 카탈로그를 로 [!DNL Walmart Marketplace]. 마켓플레이스에서 가격 변경을 표시하는 데 최대 5분이 걸릴 수 있습니다.

### 게시된 제품에 대한 가격 관리

1. 에서 [!UICONTROL Admin], 선택 **[!UICONTROL Catalog > Products]**.
1. 제품 그리드에서 업데이트할 제품을 찾아 선택합니다 **[!UICONTROL Edit]**.
1. 필요에 따라 가격을 검토하고 업데이트합니다.
1. **[!UICONTROL Save]** 변경 사항입니다.

Commerce에서 제품 가격 구성을 관리하는 방법에 대한 자세한 내용은 [가격 관리](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
