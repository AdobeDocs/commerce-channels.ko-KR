---
title: Walmart Marketplace 연결 관리
description: '''API 자격 증명을 업데이트하여 [DNL! Commerce] 스토어 보기 및 [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] 제품 목록 작성 및 재고, 가격, 주문 및 다음 기간 동안의 배송 데이터 동기화 [!DNL Commerce] 월마트도요'
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 운송 회사 매핑

이전으로 [주문 선적 처리](process-orders.md#ship-an-order) 대상 [!DNL Walmart Marketplace] 주문, 월마트에서 선호하는 배송 운송업체를 해당 운송업체에 매핑 [!DNL Commerce] 운송 데이터가 서로 동기화되는 [!DNL Walmart] 및 [!DNL Commerce].

선호 통신사에 매핑되지 않는 상거래 통신사는 다음과 같이 레이블이 지정됩니다. *[!UICONTROL Other Carrier]* 날짜 [!DNL Walmart].

**전제 조건**

리뷰 [Walmart 요구 사항](walmart-requirements.md) 대상: [!DNL Marketplace Seller account].

## 연결 자격 증명 업데이트

1. 다음에서 [!UICONTROL Listings] sales channel 스토어에 대한 페이지에서 **[!UICONTROL Channel Settings]**.

1. 날짜 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Walmart Connection]**.

1. 자격 증명을 수정하려면 을 선택합니다 **[!UICONTROL Change Credentials]**

   ![연결을 승인하도록 Walmart API 자격 증명 업데이트](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. 다음을 입력합니다. **[!UICONTROL Walmart Client ID]** 및 **[!UICONTROL Walmart Client Secret]**.

1. 선택 **[!UICONTROL Save]** 구성을 적용합니다.
