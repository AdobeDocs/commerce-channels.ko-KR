---
title: '연결 [!DNL Channel Manager] 끝 [!DNL Walmart Marketplace]'
description: '"상거래 스토어 보기를 다음으로 연결" [!DNL Walmart Marketplace] Walmart Marketplace 판매에 대한 상거래 제품 목록, 재고, 가격 및 주문을 관리할 수 있는 판매 채널을 만듭니다."'
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 연결 [!DNL Channel Manager] 끝 [!DNL Walmart Marketplace]

에 Channel Manager 설치 후 [!DNL Commerce] 예를 들어 Channel Manager에서 영업 채널을 만들고 연결할 자격 증명을 구성합니다 [!DNL Channel Manager] 끝 [!DNL Walmart Marketplace].

1. [판매 채널 만들기](#create-the-sales-channel) 을(를) 선택하여 [!DNL Commerce] 제품 목록을 저장합니다.

1. [채널을 다음으로 연결 [!DNL Walmart Marketplace] 를 추가하여 [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [판매 채널 설정 완료](#complete-sales-channel-store-setup) 목록, 재고, 가격책정 및 주문을 관리하려면 [!DNL Walmart Marketplace] 제품 분류.

>[!NOTE]
>
>Channel Manager는 Walmart 계정과 [!DNL Commerce] 스토어 뷰. 동일한 스토어 보기를 여러 Walmart 계정에 연결할 수 없습니다.

## 판매 채널 만들기

1. 관리자에서 를 엽니다 [!DNL Channel Manager] 을(를) 선택하여 **[!UICONTROL Marketing** > _채널&#x200B;_> **채널 관리자]**.

1. 다음에서 **[!UICONTROL Marketplaces available to connect]** 섹션, 선택 **[!UICONTROL Get Started]**.

   ![새로 연결 [!DNL Walmart] 저장 위치: [!DNL Channel Manager]](assets/channel-manager-home.png)

1. 필요한 경우 다음을 설정하십시오. [!DNL Walmart Marketplace Seller] 계정입니다.

1. 저장소 및 연결을 구성합니다.

   - 선택 **[!UICONTROL Add Credentials]**.

   - 다음 항목 선택 [!DNL Commerce] 마켓플레이스에서 판매하려는 제품을 제공하는 스토어 보기.

      ![다음 간 연결 구성 [!DNL Commerce] 및 [!DNL Walmart Marketplace] 출처: [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - 고유 항목 입력 **[!UICONTROL store name]**.

   - 다음 항목 선택 **[!UICONTROL Adobe [!DNL Commerce] site]** 제품 목록 및 주문 처리용.

   - 관련 알림을 받으려면 [!DNL Channel Manager], 추가 **[!UICONTROL email address]**.

1. 채널을 다음으로 연결 [!DNL Walmart Marketplace].

   - 에 대한 자격 증명 추가 [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) (으)로부터 [!DNL Walmart Marketplace Seller] 계정입니다.

   - 자격 증명이 없는 경우 [!DNL Walmart Marketplace Developer Portal] 을(를) 선택하여 **[!UICONTROL Get API credentials]**.

      개발자 포털에서 지역(미국 및 캐나다)을 선택한 다음 로그인합니다.

      ![[!DNL Walmart Marketplace] 계정 로그인](assets/walmart-marketplace-login-page.png)

   - API 키 양식에서 을(를) 복사하여 저장합니다. **[!UICONTROL Client ID]** 및 **[!UICONTROL Client Secret]** 값: [!UICONTROL Adobe Inc Production API key] 안전한 장소로.

      ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >다음과 같은 경우 [!DNL Adobe Inc] 키가 개발자 포털에 나열되지 않으면 다음을 선택합니다. **[!UICONTROL Add New Key for a Solution Provider]** 을 클릭하여 권한을 구성하고 키를 생성합니다. 구성에 대한 자세한 내용은 [생성 [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - 다음으로 돌아가기: [!DNL Channel Manager] 에 자격 증명을 추가하려면 **[!UICONTROL Walmart Connection]** 정보.

      자격 증명을 추가할 때 Adobe은 클라이언트 암호를 숨기고 보안 저장소에 값을 저장합니다.

1. 선택 **[!UICONTROL Save Store]** 구성을 적용하고 [!DNL Walmart marketplace].

1. 연결에 성공하면 [스토어 설정 완료](complete-sales-channel-store-setup.md) 다음에서 **[!UICONTROL Channel Manager]** 페이지를 저장합니다.

![첫 번째 스토어 설정](assets/channel-manager-setup-first-store.png)

### 연결 문제 해결

에 연결된 경우 [!DNL Walmart] 실패, 다음을 참조하십시오. [월마트 마켓플레이스 FAQ](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"} 문제 해결 팁입니다.

- 다음에서 [!DNL Walmart Developer Portal], 의 프로덕션 API 키에 대한 올바른 자격 증명을 복사했는지 확인합니다. [!UICONTROL Adobe Inc.]

- 에 대한 액세스 구성 확인 [!UICONTROL Walmart Adobe API key] 은(는) 올바른 권한을 갖습니다. 다음을 참조하십시오 [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- 다음을 확인합니다. [!DNL Walmart API] 서비스는 다음 위치에서 사용할 수 있습니다. [Walmart API 상태 페이지](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"}.
