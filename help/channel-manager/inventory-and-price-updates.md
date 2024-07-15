---
title: 재고 및 가격 갱신
description: '''[!DNL Channel Manager]'' [!DNL Commerce] 스토어와 [!DNL Walmart Marketplace]  간의 인벤토리 및 가격 업데이트를 동기화하여  [!DNL Commerce] 관리자''에서 판매 채널 작업을 관리할 수 있습니다.'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# 재고 및 가격 업데이트

[!DNL Channel Manager]은(는) [!DNL Commerce] 제품 카탈로그의 제품에 대한 인벤토리 및 가격을 추적하고 연결된 판매 채널 및 [!DNL Walmart Marketplace]에 대한 업데이트를 동기화합니다. 동기화 작업은 제품 목록이 현재 재고 수량 및 가격을 반영하도록 합니다.


>[!IMPORTANT]
>
>[!DNL Channel Manager]을(를) 설치하고 구성한 후에는 모든 재고, 가격 및 주문 업데이트가 자동으로 동기화됩니다. Walmart Marketplace에서 이미 판매하고 있는 경우 제품 및 주문 데이터를 업데이트하는 다른 통합을 비활성화해야 합니다. [!DNL Channel Manager]을(를) Live Marketplace 저장소에 연결하기 전에 [!DNL Commerce] 상점 첫 화면의 재고 재고 수준과 가격이 정확한지 확인하고 [!DNL Walmart Marketplace]의 데이터와 일치하는지 확인하십시오.


## 인벤토리 업데이트

[!DNL Commerce]에서 제품 재고 수준이 변경되면 [!DNL Channel Manager]에서 [!DNL Walmart Marketplace]에 동기화됩니다. 인벤토리 업데이트가 판매 채널 전반에서 [!DNL Walmart marketplace]에 동기화되는 데 최대 10분이 걸릴 수 있습니다.

* **제품 카탈로그의 재고 수량에 대한 업데이트**—[수동 재고 수량 변경](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), 환불 또는 취소로 인해 [!DNL Commerce] 재고 수량이 변경되면 [!DNL Channel Manager]에서 연결된 채널과 [!DNL Walmart Marketplace]에 변경 내용을 동기화합니다.

* **재고 수량을 줄여 [!DNL Walmart Marketplace]개의 주문을 반영합니다**—[!DNL Walmart Marketplace] 주문이 [!DNL Channel Manager]에 동기화된 후 [!DNL Channel Manager]에서 [!DNL Commerce] 주문 시스템으로 업데이트를 보냅니다. [!DNL Commerce]은(는) 주문에 따라 재고 수량을 조정합니다. 그런 다음 업데이트된 수량이 [!DNL Walmart Marketplace]에 동기화됩니다. 동기화 작업이 완료될 때까지 판매 채널 목록 및 [!DNL Walmart]에서 다른 수량을 볼 수 있습니다.

>[!IMPORTANT]
>
>[!DNL Walmart Marketplace] 주문이 [!DNL Channel Manager]에 동기화되면 재고 수량 및 주문 정보는 [!DNL Commerce]에서 시작된 환불 및 취소에 대해서만 업데이트됩니다. 주문이 [!DNL Walmart marketplace]에서 환불 또는 취소된 경우 [!DNL Commerce]에서 변경 내용을 처리하여 [!DNL Commerce]의 재고 수량 및 주문 정보의 정확성을 확인합니다.

## 가격 업데이트

[!DNL Commerce]에서 제품 가격이 변경되면 [!DNL Channel Manager]에서 업데이트를 [!DNL Walmart Marketplace]에 동기화합니다. 가격 변경 내용이 [!DNL Walmart Marketplace] 목록에 표시되는 데 최대 5분이 걸릴 수 있습니다.

### 연결된 제품의 가격 관리

1. [!UICONTROL Admin]에서 **[!UICONTROL Catalog > Products]**&#x200B;을(를) 선택합니다.
1. 제품 그리드에서 업데이트할 제품을 찾은 다음 **[!UICONTROL Edit]**&#x200B;을(를) 선택합니다.
1. 필요에 따라 가격을 검토하고 업데이트합니다.
1. 변경 내용을 **[!UICONTROL Save]**&#x200B;합니다.

[!DNL Commerce]에서 제품 가격 구성 관리에 대한 도움말은 [가격 관리](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html)를 참조하십시오.
