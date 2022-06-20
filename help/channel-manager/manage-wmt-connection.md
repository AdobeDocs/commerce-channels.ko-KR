---
title: Walmart Marketplace 연결 관리
description: API 자격 증명을 업데이트하여 [DNL! Commerce] 저장소 보기 및 [!DNL Walmart Marketplace]. 상거래 제품 목록을 연결하고 상거래 제품 목록과 월마트 간에 재고, 가격, 주문 및 배송 데이터를 동기화하려면 연결이 필요합니다.
source-git-commit: 97128dcf45d7672e958c771f88389aba40c6e39e
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# 운송 회사 매핑

시작하기 전에 [프로세스 주문 출하](process-orders.md#ship-an-order) 대상 [!DNL Walmart Marketplace] 주문에서 Walmart 기본 배송 운송선을 해당 운송회사에 매핑합니다. [!DNL Commerce] 전송 데이터를 [!DNL Walmart] 및 [!DNL Commerce].

기본 통신사에 매핑되지 않는 상거래 통신사에는 *[!UICONTROL Other Carrier]* on [!DNL Walmart].

**전제 조건**

검토 [월마트 요구 사항](walmart-requirements.md) 대상 [!DNL Marketplace Seller account].

## 연결 자격 증명 업데이트

1. 설정 [!UICONTROL Listings] 영업 채널 저장소 페이지에서 **[!UICONTROL Channel Settings]**.

1. 설정 **[!UICONTROL Channel Settings]**, 선택 **[!UICONTROL Walmart Connection]**.

1. 자격 증명을 수정하려면 **[!UICONTROL Change Credentials]**

   ![연결을 승인하도록 Walmart API 자격 증명을 업데이트합니다](assets/update-connection-credentials.png)

1. 을(를) 입력합니다. **[!UICONTROL Walmart Client ID]** 및 **[!UICONTROL Walmart Client Secret]**.

1. 선택 **[!UICONTROL Save]** 구성을 적용하려면
