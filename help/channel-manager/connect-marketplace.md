---
title: '연결 [!DNL Channel Manager] to [!DNL Walmart Marketplace]'
description: "Commerce 스토어 보기를  [!DNL Walmart Marketplace] 에 연결하여 Walmart Marketplace 판매에 대한 Commerce 제품 목록, 재고, 가격 및 주문을 관리할 수 있는 판매 채널을 만드십시오."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channels, Install, Integration
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# [!DNL Channel Manager]을(를) [!DNL Walmart Marketplace]에 연결

[!DNL Commerce] 인스턴스에 채널 관리자를 설치한 후 채널 관리자에서 영업 채널을 만들고 [!DNL Channel Manager]을(를) [!DNL Walmart Marketplace]에 연결하도록 자격 증명을 구성합니다.

1. 제품 목록에 대한 [!DNL Commerce] 스토어를 선택하여 [판매 채널을 만듭니다](#create-the-sales-channel).

1. [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace)을(를) 추가하여 [채널을  [!DNL Walmart Marketplace] 에 연결합니다.

1. [판매 채널 설정을 완료합니다](#complete-sales-channel-store-setup). [!DNL Walmart Marketplace] 제품 분류에 대한 목록, 인벤토리, 가격 및 주문을 관리합니다.

>[!NOTE]
>
>채널 관리자에는 Walmart 계정과 [!DNL Commerce] 스토어 보기 간에 일대일 연결이 필요합니다. 동일한 스토어 보기를 여러 Walmart 계정에 연결할 수 없습니다.

## 판매 채널 만들기

1. 관리자의 경우 **[!UICONTROL Marketing** > _채널&#x200B;_> {채널 관리자]**를 선택하여 **0}을(를) 엽니다.[!DNL Channel Manager]

1. **[!UICONTROL Marketplaces available to connect]** 섹션에서 **[!UICONTROL Get Started]**&#x200B;을(를) 선택합니다.

   ![새 [!DNL Walmart] 저장소를 [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}에 연결

1. 필요한 경우 [!DNL Walmart Marketplace Seller] 계정을 설정합니다.

1. 저장소 및 연결을 구성합니다.

   - **[!UICONTROL Add Credentials]**&#x200B;을(를) 선택합니다.

   - 마켓플레이스에서 판매하려는 제품을 제공하는 [!DNL Commerce] 스토어 보기를 선택하십시오.

     ![[!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}에서 [!DNL Commerce]과(와) [!DNL Walmart Marketplace] 간의 연결을 구성합니다.

   - 고유한 **[!UICONTROL store name]**&#x200B;을(를) 입력하십시오.

   - 제품 목록 및 주문 처리를 위해 **[!UICONTROL Adobe [!DNL Commerce] site]**&#x200B;을(를) 선택하십시오.

   - [!DNL Channel Manager]과(와) 관련된 알림을 받으려면 **[!UICONTROL email address]**&#x200B;을(를) 추가하십시오.

1. 채널을 [!DNL Walmart Marketplace]에 연결합니다.

   - [!DNL Walmart Marketplace Seller] 계정에서 [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key)에 대한 자격 증명을 추가합니다.

   - 자격 증명이 없는 경우 **[!UICONTROL Get API credentials]**&#x200B;을(를) 선택하여 [!DNL Walmart Marketplace Developer Portal]에서 자격 증명을 가져옵니다.

     개발자 포털에서 지역(미국 및 캐나다)을 선택한 다음 로그인합니다.

     ![[!DNL Walmart Marketplace] 계정 로그인](assets/walmart-marketplace-login-page.png){width="600"}

   - API 키 양식에서 [!UICONTROL Adobe Inc Production API key]에 대한 **[!UICONTROL Client ID]** 및 **[!UICONTROL Client Secret]** 값을 복사하여 보안 위치에 저장합니다.

     ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >[!DNL Adobe Inc] 키가 개발자 포털에 나열되지 않으면 **[!UICONTROL Add New Key for a Solution Provider]**&#x200B;을(를) 선택하여 권한을 구성하고 키를 생성합니다. 구성 세부 정보는 [생성 [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key)을 참조하십시오.

   - **[!UICONTROL Walmart Connection]** 정보에 자격 증명을 추가하려면 [!DNL Channel Manager](으)로 돌아갑니다.

     자격 증명을 추가할 때 Adobe은 클라이언트 암호를 숨기고 보안 저장소에 값을 저장합니다.

1. 구성을 적용하고 [!DNL Walmart marketplace]에 연결하려면 **[!UICONTROL Save Store]**&#x200B;을(를) 선택하십시오.

1. 연결한 후 **[!UICONTROL Channel Manager]** 저장소 페이지에서 [저장소 설정을 완료](complete-sales-channel-store-setup.md)합니다.

![첫 번째 저장소 설정](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### 연결 문제 해결

[!DNL Walmart]에 연결하지 못하면 [Walmart Marketplace FAQ](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"}에서 문제 해결 팁을 확인하십시오.

- [!DNL Walmart Developer Portal]에서 [!UICONTROL Adobe Inc.]의 프로덕션 API 키에 대한 올바른 자격 증명을 복사했는지 확인합니다.

- [!UICONTROL Walmart Adobe API key]에 대한 액세스 구성에 올바른 권한이 있는지 확인하십시오. [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key)을(를) 참조하십시오.

- [Walmart API 상태 페이지](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}에서 [!DNL Walmart API] 서비스를 사용할 수 있는지 확인하십시오.
