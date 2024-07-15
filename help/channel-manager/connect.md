---
title: ' [!DNL Commerce] 서비스에 연결'
description: '채널 관리자를  [!DNL Commerce] 서비스에 연결하면  [!DNL Commerce] 인스턴스, 채널 관리자 및 기타 지원 서비스 간의 데이터 동기화 및 통신이 가능합니다.'
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# [!DNL Commerce] 서비스에 연결

[!DNL Commerce Services Connector]은(는) 채널 관리자 서비스를 Adobe Commerce 및 Magento Open Source 인스턴스와 통합합니다. 커넥터를 사용하면 [!DNL Commerce] 인스턴스, [!DNL Channel Manager] 및 기타 지원 서비스 간의 데이터 동기화 및 통신을 사용할 수 있습니다.

[!DNL Commerce Services Connector] 설정은 [!DNL Channel Manager], [!DNL Live Search] 및 [!DNL Product Recommendations]과(와) 같은 [Adobe Commerce SaaS 서비스](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html)를 사용하는 데 필요한 일회성 프로세스입니다. 다른 서비스에 대한 커넥터를 이미 구성한 경우 이 단계를 건너뜁니다.

## 요구 사항

- **Commerce 계정**-[!DNL Commerce] 인스턴스에 소프트웨어를 설치하려면 [!DNL Commerce] 플랫폼에 대한 소유자 또는 관리자 액세스 권한이 있는 계정이 있어야 합니다.

  계정 소유자 및 수퍼 사용자는 [!DNL Commerce] 인스턴스 또는 명령줄에서 [!DNL Commerce] CLI 명령 `admin:user:create`을(를) 사용하여 관리자 계정을 만들 수 있습니다.

- **Adobe Commerce 프로덕션 API 키**-이 [키](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey)를 사용하면 채널 관리자에 필요한 서비스에 API 액세스를 사용할 수 있습니다. 이 키에는 공개 및 비공개 자격 증명이 필요합니다.

>[!TIP]
>
>자격 증명을 제공하기 위해 [!DNL Commerce] 라이선스 소유자나 계정 소유자는 [액세스 공유](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)를 사용하거나 [API 키](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) 자격 증명을 신뢰할 수 있는 개발자에게 제공할 수 있습니다.

## [!DNL Commerce Services Connector] 구성

1. 스토어 서비스 구성을 엽니다.

   - 책임자에서 **[!UICONTROL Stores]**&#x200B;을(를) 선택합니다.

   - *[!UICONTROL Settings]*&#x200B;에서 **[!UICONTROL Configuration]**&#x200B;을(를) 선택합니다.

   - **[!UICONTROL Services]**&#x200B;을(를) 확장하고 **[!UICONTROL Commerce Services Connector]**&#x200B;을(를) 선택합니다.

1. Adobe Commerce 계정에서 프로덕션 API 키 자격 증명을 추가합니다.

   [!DNL Admin] 보기의 ![[!DNL Commerce Services Connector] 서비스](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > [!DNL Commerce] 인스턴스에 [!DNL Live Search] 또는 [!DNL Product Recommendations]과(와) 같은 다른 [!DNL Adobe Commerce] 서비스가 설치되어 있는 경우 자격 증명 정보가 인터페이스에 표시되고 추가 구성이 필요하지 않습니다.

1. Commerce Services가 Channel Manager 서비스로 데이터를 전송할 수 있도록 SaaS 프로젝트 및 데이터 공간을 구성합니다.

   [!DNL Admin] 보기의 ![[!DNL Commerce Services Connector] SaaS 식별자 구성](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

