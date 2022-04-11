---
title: 재고 및 가격 업데이트
description: '`[!DNL Channel Manager] 상거래 스토어와 가격 업데이트 동기화 [!DNL Walmart Marketplace] Commerce Admin에서 영업 채널 작업을 관리할 수 있습니다.'
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 재고 및 가격 업데이트

[!DNL Channel Manager] 의 제품에 대한 인벤토리 및 가격 추적 [!DNL Commerce] 제품 카탈로그 및 동기화는 연결된 영업 채널 및 [!DNL Walmart Marketplace]. 동기화는 제품 목록에 현재 재고 수량 및 가격이 반영되도록 합니다.

## 인벤토리 업데이트

제품 재고 수준이 [!DNL Commerce], [!DNL Channel Manager] 영업 채널 및 [!DNL Walmart Marketplace]. 판매 채널 간에 인벤토리 업데이트를 동기화하려면 최대 10분이 걸릴 수 있습니다 [!DNL Walmart marketplace].

* **제품 카탈로그의 재고 수량에 대한 업데이트**-When [!DNL Commerce] 다음 이유로 인해 재고 수량 변경 [수동 재고 수량 변경](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html), 환불 또는 취소, [!DNL Channel Manager] 연결된 채널 및 [!DNL Walmart Marketplace].

* **반영하도록 재고 수량 감소 [!DNL Walmart Marketplace] 주문**-다음 항목 후 [!DNL Walmart Marketplace] 주문 동기화 대상 [!DNL Channel Manager], [!DNL Channel Manager] 에서 업데이트를에 보냅니다. [!DNL Commerce] 주문 시스템. [!DNL Commerce] 주문에 따라 재고 수량을 조정합니다. 그런 다음 업데이트된 수량이 [!DNL Walmart Marketplace]. 동기화 작업이 완료될 때까지 판매 채널 목록 및 [!DNL Walmart].

>[!IMPORTANT]
>
> 후 [!DNL Walmart Marketplace] 주문 동기화 대상 [!DNL Channel Manager], 재고 수량 및 주문 정보는 [!DNL Commerce]. 주문에서 환불 또는 취소되는 경우 [!DNL Walmart marketplace]에서 변경 내용을 처리합니다. [!DNL Commerce] 의 정확성을 보장하다 [!DNL Commerce] 재고 수량 및 주문 정보.

## 가격 업데이트

제품 가격이 [!DNL Commerce], [!DNL Channel Manager] 업데이트를에 동기화 [!DNL Walmart Marketplace]. 가격 변경이에 표시되는 데 최대 5분이 걸릴 수 있습니다 [!DNL Walmart Marketplace] 목록.

### 게시된 제품에 대한 가격 관리

1. 에서 [!UICONTROL Admin], 선택 **[!UICONTROL Catalog > Products]**.
1. 제품 그리드에서 업데이트할 제품을 찾아 선택합니다 **[!UICONTROL Edit]**.
1. 필요에 따라 가격을 검토하고 업데이트합니다.
1. **[!UICONTROL Save]** 변경 사항입니다.

의 제품 가격 구성 관리에 대한 도움말입니다. [!DNL Commerce]를 참조하십시오. [가격 관리](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}.
