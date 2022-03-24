---
title: 'Sales Channel 연결 대상 [!DNL Walmart Marketplace] '
description: 판매 채널을 구성하고 Walmart Marketplace에 연결합니다.
source-git-commit: ff87f31fec7a689385a93b8cab260fd93ff15f90
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 연결 대상 [!DNL Walmart Marketplace]

에 채널 관리자를 설치한 후 [!DNL Commerce] 예를 들어 Commerce store를 Walmart Marketplace에 연결합니다.

1. 판매 채널을 [제품 목록을 위한 상거래 스토어 선택](#select-the-commerce-store-for-the-sales-channel).

1. [채널을 [!DNL Walmart Marketplace] Walmart API 자격 증명을 추가하여](#connect-the-channel-to-walmart-marketplace).

1. [영업 채널 설정 완료](#complete-store-setup) 채널 관리자에서 목록, 인벤토리, 가격 책정 및 판매를 관리할 수 있습니다.

## 영업 채널 만들기

1. 채널 관리자를 엽니다.

   - Admin에서 **[!UICONTROL Marketing** > _채널&#x200B;_> **채널 관리자]**.

   - 선택 **[!UICONTROL Connect New Store]**.

      ![전자 상거래 스토어에 연결 [!DNL Walmart Marketplace] 변환 전: [!DNL Channel Manager]](assets/connect-commerce-store-to-marketplace.png)


1. 저장소 및 연결을 구성합니다.

   - 고유 항목 입력 **[!UICONTROL store name]**.

   - 을(를) 선택합니다 **[!UICONTROL Adobe Commerce site]** 제품 목록

   - 추가 **[!UICONTROL email address]** 와 관련된 서비스 알림을 수신하려면 [!DNL Channel Manager].

      ![상거래 및 연결 구성 [!DNL Walmart Marketplace] 변환 전: [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)


## Walmart Marketplace에 채널 연결

1. 에 대한 자격 증명을 추가합니다. [!DNL Walmart Marketplace Adobe Production API key] 다음 [!DNL Walmart Marketplace Seller] 계정이 필요합니다.

   - 자격 증명이 없는 경우 **[!UICONTROL Get API credentials]** 그들을 [!DNL Walmart Marketplace Developer Portal].

      메시지가 표시되면 지역(미국 및 캐나다)을 선택한 다음 로그인합니다.

      ![[!DNL Walmart Marketplace] 계정 로그인](assets/walmart-marketplace-login-page.png)

   - API 키 양식에서 를 복사하여 저장합니다 **[!UICONTROL Client ID]** 및 **[!UICONTROL Client Secret]** 값 [!UICONTROL Adobe Inc Production API key] 보안 위치에 배치합니다.

      ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >표시되지 않으면 [!DNL Adobe Inc] Developer Portal에서 **[!UICONTROL Add New Key for a Solution Provider]** 권한을 구성하고 키를 생성하기 위해 구성에 대한 자세한 내용은 [생성 [!DNL Walmart Marketplace API Key]](overview.md#generate-a-walmart-marketplace-api-key).

   - 로 돌아가기 [!DNL Channel Manager] 자격 증명을 **[!UICONTROL Walmart Connection]** 정보.

      자격 증명을 추가할 때 [!DNL Channel Manager]에서는 Adobe이 클라이언트 암호를 숨기고 보안 저장소에 값을 저장합니다.

1. [!UICONTROL Save] 연결을 설정할 구성입니다.

   연결 후 채널을 **[!UICONTROL Channel Manager > Marketplace Stores]**.

   ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/manage-connected-stores.png)


### 연결 문제 해결

Walmart와의 연결이 실패하면 [Walmart Marketplace FAQ](https://developer.walmart.com/faq/us/faq-auth/)문제 해결 팁은 {target=&quot;_blank&quot;} 입니다.

- 에서 [!DNL Walmart Developer Portal]에서 프로덕션 API 키에 대한 올바른 자격 증명을 복사했는지 확인합니다. [!UICONTROL Adobe Inc.]

- Walmart Adobe API 키에 대한 액세스 구성에 올바른 권한이 있는지 확인합니다. 자세한 내용은 [월마트 사전 요구 사항](overview.md#walmart-prerequisites).

- Walmart API 서비스가 [Walmart API 상태 페이지](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.


## 저장소 설정 완료

상거래 스토어를 [!DNL Walmart Marketplace]를 입력하면 [!DNL Channel Manager Stores] 보기.

저장소 설정을 완료하려면

1. 관리자에서 **[!UICONTROL Marketing** > **채널 관리자**].

   ![[!DNL Walmart Marketplace API key] 구성 페이지](assets/connect-commerce-store-config.png)

1. 저장소 항목 행에서 연필 아이콘을 선택하여 연결된 판매 채널을 엽니다.

1. 영업 채널 작업을 시작합니다.

   - 상거래 카탈로그의 제품을 채널 관리자에 추가합니다

   - 제품 일치를 사용하여 Walmart에 제품 게시

   - 재고 및 가격 보기 및 관리

   - 상거래 관리자에서 Walmart 주문을 보고 관리합니다
