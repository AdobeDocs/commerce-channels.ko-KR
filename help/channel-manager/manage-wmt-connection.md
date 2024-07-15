---
title: Walmart Marketplace 연결 관리
description: '''API 자격 증명을 업데이트하여 [DNL! Commerce] 스토어 보기 및  [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] 제품 목록을 보고  [!DNL Commerce] 과(와) 월마트 간에 재고, 가격, 주문 및 배송 데이터를 동기화합니다.'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 운송 회사 매핑

[!DNL Walmart Marketplace]개 주문에 대해 [주문 배송 처리](process-orders.md#ship-an-order)를 수행하기 전에, [!DNL Walmart]과(와) [!DNL Commerce] 간에 배송 데이터를 동기화할 수 있도록 Walmart의 기본 배송 업체를 [!DNL Commerce]의 해당 운송업체에 매핑하십시오.

기본 설정 통신사에 매핑되지 않은 Commerce 통신사는 [!DNL Walmart]에서 *[!UICONTROL Other Carrier]*(으)로 레이블이 지정됩니다.

**필수 구성 요소**

[!DNL Marketplace Seller account]에 대한 [Walmart 요구 사항](walmart-requirements.md)을 검토합니다.

## 연결 자격 증명 업데이트

1. 판매 채널 스토어의 [!UICONTROL Listings] 페이지에서 **[!UICONTROL Channel Settings]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Channel Settings]**&#x200B;에서 **[!UICONTROL Walmart Connection]**&#x200B;을(를) 선택합니다.

1. 자격 증명을 수정하려면 **[!UICONTROL Change Credentials]**&#x200B;을(를) 선택합니다.

   ![연결을 승인하도록 Walmart API 자격 증명 업데이트](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. **[!UICONTROL Walmart Client ID]** 및 **[!UICONTROL Walmart Client Secret]**&#x200B;을(를) 입력하십시오.

1. 구성을 적용하려면 **[!UICONTROL Save]**&#x200B;을(를) 선택하십시오.
