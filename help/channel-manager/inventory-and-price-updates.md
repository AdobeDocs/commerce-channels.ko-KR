---
title: 재고 및 가격 업데이트
description: '"[!DNL Channel Manager] 상거래 스토어와 가격 업데이트 동기화 [!DNL Walmart Marketplace] 상거래 관리자에서 영업 채널 작업을 관리할 수 있습니다."'
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# 재고 및 가격 업데이트

Channel Manager는 게시된 제품에 대한 재고 및 가격을 추적하고 Channel Manager 및 Walmart Marketplace에 변경 사항을 동기화하여 제품 목록의 현재 재고 수량 및 가격을 반영합니다.**

## 인벤토리 업데이트

재고 수준이 변경되면 Channel Manager는 Commerce 제품 카탈로그와 Walmart Marketplace 간에 업데이트를 동기화하여 Channel Manager와 Walmart Marketplace에서 모두 현재 재고 수량을 표시합니다.

채널 관리자 및 Walmart Marketplace에 재고 변경 사항을 표시하는 데 최대 5분이 걸릴 수 있습니다.

* **제품 카탈로그의 재고 수량에 대한 업데이트**&#x200B;월마트에서 팔릴 상품에 대해 상거래 주식이 변동되면 [수동 재고 수량 변경](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html) 또는 주문 환불 또는 취소를 통해 Channel Manager 는 연결된 영업 채널과 [!DNL Walmart Marketplace].

* **Walmart Marketplace 주문을 반영하도록 재고 수량을 줄입니다**-Walmart Marketplace 주문이 채널 관리자에게 동기화되면 채널 관리자는 상거래 주문 시스템에 업데이트를 보냅니다. 상거래는 주문에 따라 주식 수량을 조정합니다. 그런 다음 업데이트된 수량이 Walmart Marketplace에 동기화됩니다. 동기화 작업이 완료될 때까지 Channel Manager 및 Marketplace에 표시되는 재고 수량에 일부 차이가 있을 수 있습니다.

>[!IMPORTANT]
>
> Walmart Marketplace 주문이 채널 관리자에게 동기화되면 재고 수량 및 기타 주문 처리 정보는 Commerce에서 시작된 환불 및 취소에 대해서만 업데이트됩니다. Walmart Marketplace에서 주문이 반환되거나 취소된 경우 상거래 재고 수량 및 주문 정보가 정확한지 확인하기 위해 상거래 변경을 처리합니다.

## 가격 업데이트

Commerce에서 제품 가격이 변경되면 Channel Manager는 상거래 제품 카탈로그에서 Walmart Marketplace로 업데이트를 동기화합니다. 재고 변경 사항을 표시하는 데 최대 5분이 걸릴 수 있습니다.

### 게시된 제품에 대한 가격 관리

1. 에서 [!UICONTROL Admin], 선택 **[!UICONTROL Catalog > Products]**.
1. 제품 그리드에서 업데이트할 제품을 찾아 선택합니다 **[!UICONTROL Edit]**.
1. 필요에 따라 가격을 검토하고 업데이트합니다.
1. **[!UICONTROL Save]** 변경 사항입니다.

채널 관리자는 채널 스토어에 대한 가격 업데이트를 동기화하고 [!DNL Walmart Marketplace]. 이 작업은 최대 5분이 걸릴 수 있습니다.

Commerce에서 제품 가격 구성을 관리하는 방법에 대한 자세한 내용은 [가격 관리](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
