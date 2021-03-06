---
title: 온보드 [!DNL Channel Manager]
description: '''인스턴스를 [!DNL Channel Manager] 몇 가지 온보딩 단계를 완료하여 서비스를 제공합니다.'''
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 638ba8c595652e66aa5f15f5207855c6d2b872d7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 온보드 [!DNL Channel Manager]

온보딩을 완료하면 [!UICONTROL Channel Manager] 옵션 [!UICONTROL Commerce Admin Marketing] 메뉴 아래의 제품에서 사용할 수 있습니다.

![[!DNL Channel Manager] 관리자 보기의 옵션](assets/channel-manager-admin-view.png)

## 온보딩 개요

1. [설치 [!DNL Channel Manager] 확장](install.md).

1. [구성 [!DNL Commerce Services Connector]](connect.md) 채널 관리자를 Commerce 인스턴스 및 기타 지원 서비스와 통합합니다.

1. [연결 [!DNL Commerce] 저장 위치 [!DNL Walmart Marketplace]](connect.md).

1. [저장소 설정 완료](complete-store-setup.md).

## 요구 사항

- 을(를) 충족하는지 확인합니다. [Walmart Marketplace 요구 사항](walmart-requirements.md) 를 채널 관리자와 통합합니다.

- **상거래 계정 정보**- 다운로드 및 설치 [!DNL Channel Manager] 를 사용하려면 [상거래 계정](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. 에 대한 소유자 또는 관리자 액세스 권한이 있는 계정 ID 및 자격 증명이 필요합니다 [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 인스턴스.

   - **이미지 ID**-[로그인](https://account.magento.com/customer/account/login/) 변환 후 [!DNL Commerce] 계정이 있어야 **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] on [!DNL Commerce] 계정 설정](assets/mageid-my-commerce-account.png)

   - **액세스 키-** 다운로드할 인증 키 가져오기 [!DNL Commerce] 확장 프로그램 [!DNL Commerce] 작성기 저장소 `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Adobe Commerce 및 Magento Open Source 프로젝트에서 소유자는 [공유 액세스](https://docs.magento.com/user-guide/magento/magento-account-share.html) 를 사용하여 신뢰할 수 있는 직원 및 서비스 공급자가 소유자 또는 라이선스 소유자 계정의 자격 증명을 사용하여 확장을 다운로드할 수 있습니다.

      대상 [!DNL Adobe Commerce] 클라우드 인프라 프로젝트에서 소프트웨어 설치 관리자는 [!DNL Commerce] 인스턴스:

      - 클라우드 프로젝트에 대한 슈퍼 사용자 액세스 권한
      - 특정 환경에 대한 관리자 액세스 권한
      - an [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 작성기 리포지토리에 액세스할 수 있는 권한이 있는 계정

      자세한 내용은 [사용자 액세스 관리](https://devdocs.magento.com/cloud/project/user-admin.html).


- **작성기 및 를 사용한 경험[!DNL Commerce CLI]** -참조 [일반 CLI 설치](https://devdocs.magento.com/extensions/install/)다음 도구를 사용하여 확장을 설치 및 관리하는 방법에 대한 자세한 내용은 target=&quot;_blank&quot;} 를 참조하십시오. [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 플랫폼.

- [[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-활성화한 경우 [!DNL Amazon Sales Channel] 에 대해 [!DNL Commerce] 사이트, [!DNL Commerce] 설치하기 전에 플랫폼에 버전 4.4.2가 설치되어 있습니다. [!DNL Channel Manager].

- [!DNL Inventory Management] Adobe Commerce 및 Magento Open Source 확장

   재고 및 Order Management에 채널 관리자를 사용할 계획이라면 Adobe Commerce 및 Magento Open Source 인스턴스에 Inventory management 확장이 설치 및 활성화되어 있어야 합니다. 일반적으로 이 확장은 Adobe Commerce 및 Magento Open Source 2.3.x 이상에서 기본적으로 설치 및 활성화됩니다.

   Commerce를 2.2.x에서 업그레이드했거나 Inventory management을 비활성화한 경우 필수 모듈을 포함하도록 설치를 업데이트해야 합니다. 자세한 내용은 [Inventory management 설치](https://devdocs.magento.com/extensions/inventory-management/) ( Adobe Commerce 개발자 설명서).

### 시스템 요구 사항

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x 이상](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-활성화한 경우 [!DNL Amazon Sales Channel] 에 대해 [!DNL Commerce] 사이트, [!DNL Commerce] 설치하기 전에 플랫폼에 버전 4.4.2가 설치되어 있습니다. [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### 지원되는 플랫폼

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce 온-프레미스(EE) : 2.4.x
- Magento Open Source 2.4.x
