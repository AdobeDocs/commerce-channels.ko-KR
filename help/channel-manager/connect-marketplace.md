---
title: 영업 채널을 [!DNL Walmart Marketplace]
description: 판매 채널을 구성하고 Walmart Marketplace에 연결합니다.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 7a400bf0b09e65d5375dc15c6a1e004d0fef0592
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 영업 채널을 [!DNL Walmart Marketplace]

에 채널 관리자를 설치한 후 [!DNL Commerce] 예를 들어 Commerce store를 Walmart Marketplace에 연결합니다.

1. [영업 채널 만들기](#create-the-sales-channel) 제품 목록에 대해 상거래 저장소를 선택하여 기본 설정을 지정합니다.

1. [채널을 [!DNL Walmart Marketplace] Walmart API 자격 증명을 추가하여](#connect-the-channel-to-walmart-marketplace).

1. [영업 채널 설정 완료](#complete-store-setup) Walmart Marketplace 제품에 대한 목록, 재고, 가격 및 주문을 관리하려면

## 영업 채널 만들기

1. 열기 [!DNL Channel Manager].

   - Admin에서 **[!UICONTROL Marketing** > _채널&#x200B;_> **채널 관리자]**.

1. 에서 **[!UICONTROL Marketplaces available to connect]** 섹션, **[!UICONTROL Get Started]**.

   ![새 Walmart 스토어에 연결 [!DNL Channel Manager]](assets/channel-manager-home.png)

1. 필요한 경우 Walmart Marketplace 판매자 계정을 설정합니다.

1. 저장소 및 연결을 구성합니다.

   - 선택 **[!UICONTROL Add Credentials]**.

   - 설정 [!UICONTROL Connect New Walmart Store] 양식에서 상거래 스토어 보기를 선택하여 마켓플레이스에 연결합니다.

      ![상거래 및 연결 구성 [!DNL Walmart Marketplace] 변환 전: [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - 고유 항목 입력 **[!UICONTROL store name]**.

   - 을(를) 선택합니다 **[!UICONTROL Adobe Commerce site]** 제품 목록

   - 추가 **[!UICONTROL email address]** 와 관련된 서비스 알림을 수신하려면 [!DNL Channel Manager].

1. 채널을 [!DNL Walmart Marketplace].

   - 에 대한 자격 증명을 추가합니다. [[!DNL Walmart Marketplace Adobe Production API key]](walmart-prerequisites.md#generate-a-walmart-marketplace-production-api-key) 다음 [!DNL Walmart Marketplace Seller] 계정이 필요합니다.

   - 자격 증명이 없는 경우 **[!UICONTROL Get API credentials]** 그들을 [!DNL Walmart Marketplace Developer Portal].

      메시지가 표시되면 지역(미국 및 캐나다)을 선택한 다음 로그인합니다.

      ![[!DNL Walmart Marketplace] 계정 로그인](assets/walmart-marketplace-login-page.png)

   - API 키 양식에서 를 복사하여 저장합니다 **[!UICONTROL Client ID]** 및 **[!UICONTROL Client Secret]** 값 [!UICONTROL Adobe Inc Production API key] 보안 위치에 배치합니다.

      ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >만약 [!DNL Adobe Inc] 키가 Developer Portal에 나열되지 않은 경우 **[!UICONTROL Add New Key for a Solution Provider]** 권한을 구성하고 키를 생성하기 위해 구성에 대한 자세한 내용은 [생성 [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key).

   - 로 돌아가기 [!DNL Channel Manager] 자격 증명을 **[!UICONTROL Walmart Connection]** 정보.

      자격 증명을 추가할 때 [!DNL Channel Manager]에서는 Adobe이 클라이언트 암호를 숨기고 보안 저장소에 값을 저장합니다.

1. 선택 **[!UICONTROL Save Store]** 구성을 적용하고 [!DNL Walmart marketplace].

1. 연결 후 [저장소 설정 완료](complete-store-setup.md) 에서 **[!UICONTROL Channel Manager]** 목록 저장 페이지.

![첫 번째 저장소 설정](assets/channel-manager-setup-first-store.png)

### 연결 문제 해결

Walmart와의 연결이 실패하면 [Walmart Marketplace FAQ](https://developer.walmart.com/faq/us/faq-auth/)문제 해결 팁은 {target=&quot;_blank&quot;} 입니다.

- 에서 [!DNL Walmart Developer Portal]에서 프로덕션 API 키에 대한 올바른 자격 증명을 복사했는지 확인합니다. [!UICONTROL Adobe Inc.]

- Walmart Adobe API 키에 대한 액세스 구성에 올바른 권한이 있는지 확인합니다. 자세한 내용은 [월마트 사전 요구 사항](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key).

- 에서 [!DNL Walmart API] 서비스는 [Walmart API 상태 페이지](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
