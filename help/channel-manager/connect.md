---
title: '연결 대상 [!DNL Commerce] 서비스'
description: '채널 관리자 연결 대상: [!DNL Commerce] 를 사용하여 데이터 동기화 및 [!DNL Commerce] 인스턴스, 채널 관리자 및 기타 지원 서비스.'
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# 연결 대상 [!DNL Commerce] 서비스

다음 [!DNL Commerce Services Connector] 는 채널 관리자 서비스를 Adobe Commerce 및 Magento Open Source 인스턴스와 통합합니다. 커넥터는 커넥터 간의 데이터 동기화 및 통신을 가능하게 합니다 [!DNL Commerce] 인스턴스, [!DNL Channel Manager]및 기타 지원 서비스.

[!DNL Commerce Services Connector] 설치는 을(를) 사용하는 데 필요한 일회성 프로세스입니다. [Adobe Commerce SaaS 서비스](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) 과 같은 [!DNL Channel Manager], [!DNL Live Search], 및 [!DNL Product Recommendations]. 다른 서비스에 대한 커넥터를 이미 구성한 경우 이 단계를 건너뜁니다.

## 요구 사항

- **상거래 계정**-에 소프트웨어 설치 [!DNL Commerce] 인스턴스에 대한 소유자 또는 관리자 액세스 권한이 있는 계정이 있어야 합니다. [!DNL Commerce] 플랫폼.

  계정 소유자 및 수퍼 사용자는 [!DNL Commerce] 인스턴스 또는 를 사용하는 명령줄에서 [!DNL Commerce] CLI 명령 `admin:user:create`.

- **Adobe Commerce 프로덕션 API 키**-이 [key](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) 채널 관리자에 필요한 서비스에 대한 API 액세스를 활성화합니다. 이 키에는 공개 및 비공개 자격 증명이 필요합니다.

>[!TIP]
>
>자격 증명을 제공하려면 다음을 수행하십시오. [!DNL Commerce] 라이선스 소유자 또는 계정 소유자에게 다음 옵션이 있음: [액세스 공유](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)또는 다음을 제공합니다. [API 키](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) 신뢰할 수 있는 개발자의 자격 증명입니다.

## 구성 [!DNL Commerce Services Connector]

1. 스토어 서비스 구성을 엽니다.

   - 책임자에서 을(를) 선택합니다. **[!UICONTROL Stores]**.

   - 아래 *[!UICONTROL Settings]*, 선택 **[!UICONTROL Configuration]**.

   - 확장 **[!UICONTROL Services]** 및 선택 **[!UICONTROL Commerce Services Connector]**.

1. Adobe Commerce 계정에서 프로덕션 API 키 자격 증명을 추가합니다.

   ![[!DNL Commerce Services Connector] 의 서비스 [!DNL Admin] 보기](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > 다음의 경우 [!DNL Commerce] 인스턴스에 다른 항목이 있습니다. [!DNL Adobe Commerce] 다음과 같은 서비스 [!DNL Live Search] 또는 [!DNL Product Recommendations] 자격 증명 정보가 설치되고 인터페이스에 표시되므로 더 이상 구성할 필요가 없습니다.

1. Commerce Services에서 채널 관리자 서비스로 데이터를 전송할 수 있도록 SaaS 프로젝트 및 데이터 공간을 구성합니다.

   ![[!DNL Commerce Services Connector] 의 SaaS 식별자 구성 [!DNL Admin] 보기](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

