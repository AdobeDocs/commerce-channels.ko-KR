---
title: '''연결 대상 [!DNL Commerce] services'
description: '''채널 관리자 연결 대상 [!DNL Commerce] 서비스 를 통해 데이터 동기화 및 통신 가능 [!DNL Commerce] 인스턴스, 채널 관리자 및 기타 지원 서비스'''
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 7e7a3e854bbc6062e2d15c1962ddf787451e7275
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 연결 대상 [!DNL Commerce] 서비스

다음 [!DNL Commerce Services Connector] 채널 관리자 서비스를 Adobe Commerce 및 Magento Open Source 인스턴스와 통합합니다. 커넥터를 사용하면 [!DNL Commerce] 인스턴스, [!DNL Channel Manager], 및 기타 지원 서비스.

[!DNL Commerce Services Connector] 설정은 [Adobe Commerce SaaS 서비스](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html)다음과 같은 {target=&quot;_blank&quot;} [!DNL Channel Manager], [!DNL Live Search], 및 [!DNL Product Recommendations]. 다른 서비스에 대한 커넥터를 이미 구성한 경우 이 단계를 건너뜁니다.

## 요구 사항

- **상거래 계정**-소프트웨어를 설치하려면 [!DNL Commerce] 인스턴스에 대한 소유자 또는 관리자 액세스 권한이 있는 계정이 있어야 합니다 [!DNL Commerce] 플랫폼.

   계정 소유자 및 슈퍼 사용자는 [!DNL Commerce] 인스턴스 또는 를 사용하여 명령줄에서 [!DNL Commerce] CLI 명령 `admin:user:create`.

- **Adobe Commerce 프로덕션 API 키**-이것 [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} 채널 관리자에서 필요한 서비스에 대한 API 액세스를 사용할 수 있습니다. 이 키에 대한 공개 및 개인 자격 증명이 필요합니다.

>[!TIP]
>
>자격 증명을 제공하려면 [!DNL Commerce] 라이선스 소유자 또는 계정 소유자에 대한 옵션 [공유 액세스](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} 또는 [API 키](https://docs.magento.com/user-guide/system/saas.html#apikey)신뢰할 수 있는 개발자에 대한 {target=&quot;_blank&quot;} 자격 증명.

## 구성 [!DNL Commerce Services Connector]

1. 저장소 서비스 구성을 엽니다.

   - 관리자에서 을(를) 선택합니다. **[!UICONTROL Stores]**.

   - 아래 *[!UICONTROL Settings]*, 선택 **[!UICONTROL Configuration]**.

   - 확장 **[!UICONTROL Services]** 을(를) 선택합니다. **[!UICONTROL Commerce Services Connector]**.

1. Adobe Commerce 계정에서 프로덕션 API 키 자격 증명을 추가합니다.

   ![[!DNL Commerce Services Connector] 의 서비스 [!DNL Admin] 보기](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 만약 [!DNL Commerce] 인스턴스에 다른 인스턴스가 있습니다. [!DNL Adobe Commerce] 과 같은 서비스 [!DNL Live Search] 또는 [!DNL Product Recommendations] 설치된 경우 자격 증명 정보가 인터페이스에 표시되고 추가 구성이 필요하지 않습니다.

1. Commerce Services가 채널 관리자 서비스로 데이터를 전송할 수 있도록 SaaS 프로젝트 및 데이터 공간을 구성합니다.

   ![[!DNL Commerce Services Connector] 에서 SaaS 식별자 구성 [!DNL Admin] 보기](assets/commerce-services-connector-saas-config.png)

