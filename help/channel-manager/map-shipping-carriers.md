---
title: 운송 회사 매핑
description: '''일치하는 [DNL!에 대한 속성 매핑'' Commerce] 제품을 기존 [!DNL Walmart Marketplace] 목록에 추가 및  [!DNL Channel Manager] 과(와) [!DNL Walmart] 간의 데이터 동기화'''
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# 운송 회사 매핑

[!DNL Walmart Marketplace]개 주문에 대해 [주문 배송 처리](process-orders.md#ship-an-order)를 수행하기 전에, [!DNL Walmart]과(와) [!DNL Commerce] 간에 배송 데이터를 동기화할 수 있도록 Walmart의 기본 배송 업체를 [!DNL Commerce]의 해당 운송업체에 매핑하십시오.

기본 설정 통신사에 매핑되지 않은 Commerce 통신사는 [!DNL Walmart]에서 *[!UICONTROL Other Carrier]*(으)로 레이블이 지정됩니다.

**필수 구성 요소**

운송 회사를 매핑하기 전에 다음 작업을 완료하십시오.

1. [!DNL Walmart Marketplace]의 정시 게재에 대한 [통신사 방법 및 배송 모범 사례](https://sellerhelp.walmart.com/s/guide?article=000009473)를 검토하십시오.

1. [!DNL Commerce] 저장소에서 [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) 및 [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) 구성을 확인하여 [!DNL Walmart Marketplace sales]에 대한 구성을 최적화했는지 확인하십시오.

## 운송 회사 매핑

1. **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** 페이지에서 **[!UICONTROL Channel Settings]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Channel Settings]**&#x200B;에서 **[!UICONTROL Shipping Carriers]**&#x200B;을(를) 선택합니다.

   ![운송회사 매핑](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. 나열된 각 [!DNL Walmart] 기본 통신사에 대해 통신사가 있는 경우 드롭다운에서 [!DNL Commerce] 통신사 이름을 선택합니다.

1. 구성을 적용하려면 **[!UICONTROL Save]**&#x200B;을(를) 선택하십시오.

