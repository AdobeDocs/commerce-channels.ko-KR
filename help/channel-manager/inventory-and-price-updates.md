---
title: 재고 및 가격 갱신
description: '[!DNL Channel Manager] 다음 기간 동안 재고 및 가격 업데이트 동기화: [!DNL Commerce] 저장 및 [!DNL Walmart Marketplace] 를 통해 판매 채널 작업을 관리할 수 있습니다. [!DNL Commerce] 관리자'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 재고 및 가격 업데이트

[!DNL Channel Manager] 에서 제품에 대한 인벤토리 및 가격 추적 [!DNL Commerce] 제품 카탈로그 및 연결된 판매 채널에 대한 업데이트 동기화 [!DNL Walmart Marketplace]. 동기화 작업은 제품 목록이 현재 재고 수량 및 가격을 반영하도록 합니다.


>[!IMPORTANT]
>
>다음 이후 [!DNL Channel Manager] 가 설치되고 구성되면 모든 재고, 가격 및 주문 업데이트가 자동으로 동기화됩니다. Walmart Marketplace에서 이미 판매하고 있는 경우 제품 및 주문 데이터를 업데이트하는 다른 통합을 비활성화해야 합니다. 그런 다음 재고의 재고 수준과 가격을 확인합니다. [!DNL Commerce] storefront는 정확하고 다음의 데이터와 일치합니다. [!DNL Walmart Marketplace] 연결하기 전에 [!DNL Channel Manager] 라이브 마켓플레이스 스토어로 이동합니다.


## 인벤토리 업데이트

에서 제품 재고 수준이 변경되는 경우 [!DNL Commerce], [!DNL Channel Manager] 에 대한 업데이트 동기화 [!DNL Walmart Marketplace]. 재고 업데이트가 판매 채널 전반에서 로 동기화되는 데 최대 10분이 걸릴 수 있습니다. [!DNL Walmart marketplace].

* **제품 카탈로그의 재고 수량 업데이트**- 다음과 같은 경우 [!DNL Commerce] 다음 이유로 재고 수량이 변경됨: [수동 재고 수량 변경](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html), 환불 또는 취소 [!DNL Channel Manager] 연결된 채널에 변경 내용을 동기화합니다. [!DNL Walmart Marketplace].

* **재고 수량을 줄여 반영합니다. [!DNL Walmart Marketplace] 주문 수**- 다음 이후 [!DNL Walmart Marketplace] 동기화 순서 [!DNL Channel Manager], [!DNL Channel Manager] 업데이트를 (으)로 전송합니다. [!DNL Commerce] 시스템 주문. [!DNL Commerce] 주문에 따라 재고 수량을 조정합니다. 그런 다음 업데이트된 수량이에 동기화됩니다. [!DNL Walmart Marketplace]. 동기화 작업이 완료될 때까지 판매 채널 목록에서 다른 수량을 볼 수 있습니다. [!DNL Walmart].

>[!IMPORTANT]
>
>다음 이후 [!DNL Walmart Marketplace] 동기화 순서 [!DNL Channel Manager], 재고 수량 및 주문 정보는 다음에 시작된 환불 및 취소에 대해서만 업데이트됩니다. [!DNL Commerce]. 주문이 다음 항목에서 환불 또는 취소된 경우 [!DNL Walmart marketplace], 변경 내용 처리 [!DNL Commerce] 의 정확성을 기하기 위하여 [!DNL Commerce] 재고 수량 및 주문 정보.

## 가격 업데이트

에서 제품 가격이 변경되는 경우 [!DNL Commerce], [!DNL Channel Manager] 업데이트를 로 동기화합니다. [!DNL Walmart Marketplace]. 가격 변경 사항이 페이지에 표시되는 데 최대 5분이 걸릴 수 있습니다. [!DNL Walmart Marketplace] 나열 중.

### 연결된 제품의 가격 관리

1. 다음에서 [!UICONTROL Admin], 선택 **[!UICONTROL Catalog > Products]**.
1. 제품 그리드에서 업데이트할 제품을 찾아 선택합니다. **[!UICONTROL Edit]**.
1. 필요에 따라 가격을 검토하고 업데이트합니다.
1. **[!UICONTROL Save]** 거스름돈

에서 제품 가격 구성 관리에 대한 도움말 [!DNL Commerce], 참조 [가격 관리](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
