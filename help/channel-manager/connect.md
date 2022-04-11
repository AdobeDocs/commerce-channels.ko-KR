---
title: 연결 대상 [!DNL Commerce] 서비스
description: 채널 관리자를 다음으로 연결 [!DNL Commerce] 서비스 를 통해 데이터 동기화 및 통신 가능 [!DNL Commerce] 인스턴스, 채널 관리자 및 기타 지원 서비스.
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 연결 대상 [!DNL Commerce] 서비스

Commerce Services Connector는 채널 관리자 서비스를 Adobe Commerce 및 Magento Open Source 인스턴스와 통합합니다. 커넥터를 사용하면 [!DNL Commerce] 인스턴스, [!DNL Channel Manager], 및 기타 지원 서비스.

Commerce Services 커넥터 설정은 Adobe을 사용하는 데 필요한 일회성 프로세스입니다 [Commerce SaaS 서비스](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html)다음과 같은 {target=&quot;_blank&quot;} [!DNL Channel Manager], [!DNL Live Search], 및 [!DNL Product Recommendations]. 다른 서비스에 대한 커넥터를 이미 구성한 경우 이 단계를 건너뜁니다.

## 전제 조건

- **상거래 계정**-상거래 인스턴스에 소프트웨어를 설치하려면 상거래 플랫폼에 대한 소유자 또는 관리자 액세스 권한이 있는 계정이 있어야 합니다.

   계정 소유자 및 관리자 사용자는 상거래 인스턴스 또는 명령줄에서 [!DNL Commerce] CLI 명령 `admin:user:create`.

- **Adobe Commerce 프로덕션 API 키**-이것 [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} 채널 관리자에서 필요한 서비스에 대한 API 액세스를 사용할 수 있습니다. 이 키에 대한 공개 및 개인 자격 증명이 필요합니다.

>[!TIP]
>
>자격 증명을 제공하기 위해 전자 상거래 라이선스 소유자 또는 계정 소유자는 다음 옵션을 사용할 수 있습니다 [공유 액세스](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} 또는 [API 키](https://docs.magento.com/user-guide/system/saas.html#apikey)신뢰할 수 있는 개발자에 대한 {target=&quot;_blank&quot;} 자격 증명.

## Commerce Services 커넥터 구성

1. 저장소 서비스 구성을 엽니다.

   - 관리자에서 을(를) 선택합니다. **[!UICONTROL Stores]**.

   - 아래 *[!UICONTROL Settings]*, 선택 **[!UICONTROL Configuration]**.

   - 확장 **[!UICONTROL Services]** 을(를) 선택합니다. **[!UICONTROL Commerce Services Connector]**.

1. Adobe Commerce 계정에서 프로덕션 API 키 자격 증명을 추가합니다.

   ![[!DNL Commerce Service Connector] 의 서비스 [!DNL Admin] 보기](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 만약 [!DNL Commerce] 인스턴스에 다른 인스턴스가 있습니다. [!DNL Adobe Commerce] 과 같은 서비스 [!DNL Live Search] 또는 [!DNL Product Recommendations] 설치된 경우 자격 증명 정보가 인터페이스에 표시되고 추가 구성이 필요하지 않습니다.

1. Commerce Services가 채널 관리자 서비스로 데이터를 전송할 수 있도록 SaaS 프로젝트 및 데이터 공간을 구성합니다.

   ![[!DNL Commerce Service Connector] 에서 SaaS 식별자 구성 [!DNL Admin] 보기](assets/commerce-services-connector-saas-config.png)

