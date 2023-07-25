---
title: 운송 회사 매핑
description: '''일치하는 [DNL!에 대한 속성 매핑'' 기존 Commerce] 제품 [!DNL Walmart Marketplace] 다음 기간 동안 데이터 목록 및 동기화 [!DNL Channel Manager] 및 [!DNL Walmart].'''
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# 운송 회사 매핑

이전으로 [주문 선적 처리](process-orders.md#ship-an-order) 대상 [!DNL Walmart Marketplace] 주문, 월마트에서 선호하는 배송 운송업체를 해당 운송업체에 매핑 [!DNL Commerce] 운송 데이터가 서로 동기화되는 [!DNL Walmart] 및 [!DNL Commerce].

선호 통신사에 매핑되지 않는 상거래 통신사는 다음과 같이 레이블이 지정됩니다. *[!UICONTROL Other Carrier]* 날짜 [!DNL Walmart].

**전제 조건**

운송 회사를 매핑하기 전에 다음 작업을 완료하십시오.

1. 리뷰 [적시 납품을 위한 운송회사 방법 및 배송 모범 사례](https://sellerhelp.walmart.com/s/guide?article=000009473) 대상 [!DNL Walmart Marketplace].

1. 확인 [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) 및 [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) 의 구성 [!DNL Commerce] 을(를) 저장하여 의 구성을 최적화했는지 확인 [!DNL Walmart Marketplace sales].

## 운송 회사 매핑

1. 다음에서 **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** 페이지, 선택 **[!UICONTROL Channel Settings]**.

1. 날짜 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Shipping Carriers]**.

   ![운송 회사 매핑](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. 각 [!DNL Walmart] 기본 캐리어가 나열되면 [!DNL Commerce] 통신사를 사용할 수 있는 경우 드롭다운의 통신사 이름.

1. 선택 **[!UICONTROL Save]** 구성을 적용합니다.

