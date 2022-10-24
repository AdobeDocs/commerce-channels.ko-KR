---
title: 운송 회사 매핑
description: '일치하는 [DNL! 기존 제품에 대한 상거래 [!DNL Walmart Marketplace] 목록 및 데이터 동기화 [!DNL Channel Manager] 및 [!DNL Walmart]'
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 3f6039ad78ff500c31129bee12d65e291e226567
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# 운송 회사 매핑

시작하기 전에 [프로세스 주문 출하](process-orders.md#ship-an-order) 대상 [!DNL Walmart Marketplace] 주문에서 Walmart 기본 배송 운송선을 해당 운송회사에 매핑합니다. [!DNL Commerce] 전송 데이터를 [!DNL Walmart] 및 [!DNL Commerce].

기본 통신사에 매핑되지 않는 상거래 통신사에는 *[!UICONTROL Other Carrier]* on [!DNL Walmart].

**전제 조건**

운송 회사를 매핑하기 전에 다음 작업을 완료하십시오.

1. 를 검토합니다. [정시 배송을 위한 운송 회사 방법 및 운송 우수 사례](https://sellerhelp.walmart.com/s/guide?article=000009473) 대상 [!DNL Walmart Marketplace].

1. 확인 [[!UICONTROL Shipping Carrier]](https://docs.magento.com/user-guide/shipping/carriers.html) 및 [[!UICONTROL Shipping Settings]](https://docs.magento.com/user-guide/configuration/sales/shipping-settings.html) 구성 [!DNL Commerce] 를 저장하여 구성을 [!DNL Walmart Marketplace sales].

## 운송 회사 매핑

1. 에서 **[!UICONTROL Listings]** 또는 **[!UICONTROL Orders]** 페이지를 선택하고 **[!UICONTROL Channel Settings]**.

1. 설정 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Shipping Carriers]**.

   ![운송 회사 매핑](assets/map-shipping-carriers.png)

1. 각 [!DNL Walmart] 나열된 선호 반송파 목록에서 [!DNL Commerce] 통신사를 사용할 수 있는 경우 드롭다운에서 통신사 이름입니다.

1. 선택 **[!UICONTROL Save]** 구성을 적용하려면

