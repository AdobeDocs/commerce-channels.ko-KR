---
title: 온보드 [!DNL Channel Manager]
description: '인스턴스를 [!DNL Channel Manager] 몇 가지 온보딩 단계를 완료하여 서비스를 제공합니다.'
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# 온보드 [!DNL Channel Manager]

Channel Manager 온보딩 프로세스를 완료한 후 Adobe Commerce에서 Walmart Marketplace 채널 판매 운영을 액세스, 구성 및 관리할 수 있습니다. 채널 관리자는 다음에서 사용할 수 있습니다. [!UICONTROL Channel Manager] 옵션 [!UICONTROL Commerce Admin Marketing] 메뉴 아래의 제품에서 사용할 수 있습니다.

![[!DNL Channel Manager] 관리자 보기의 옵션](assets/channel-manager-admin-view.png){width="500"}

## 요구 사항

Channel Manager 사용 요구 사항을 검토하고 필요한 계정 정보와 자격 증명을 수집하여 확장을 다운로드, 설치 및 구성합니다.

- **[Walmart Marketplace 요구 사항](walmart-requirements.md)**-다음을 포함한 Channel Manager와의 통합 요구 사항을 충족하는지 확인합니다. [판매자 계정 설정](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) 통합을 사용하려면 API 키를 생성합니다.

- **상거래 계정 정보**-다운로드 및 설치 [!DNL Channel Manager] 을(를) 필요로 함 [상거래 계정](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html). 에 대한 소유자 또는 관리자 액세스 권한이 있는 계정 ID 및 자격 증명이 필요합니다. [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 인스턴스.

   - **이미지 ID**-[로그인](https://account.magento.com/customer/account/login/) (으)로 [!DNL Commerce] ID를 가져올 계정 **[!UICONTROL My Account - Magento settings]**.

     ![[!DNL MAGEID] 날짜 [!DNL Commerce] 계정 설정](assets/mageid-my-commerce-account.png){width="250"}

   - **액세스 키-** 다운로드할 인증 키 가져오기 [!DNL Commerce] 의 확장 [!DNL Commerce] 작성기 저장소 `([!DNL repo.magento.com]`).

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Adobe Commerce 및 Magento Open Source 프로젝트에서 소유자는 을 설정할 수 있습니다 [공유 액세스](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) 신뢰할 수 있는 직원 및 서비스 공급자가 소유자 또는 라이선스 소유자 계정의 자격 증명을 사용하여 확장을 다운로드할 수 있도록 합니다.

     대상 [!DNL Adobe Commerce] 클라우드 인프라 프로젝트의 소프트웨어 설치 관리자는에 대한 다음 액세스 권한이 있어야 합니다. [!DNL Commerce] 인스턴스:

      - 클라우드 프로젝트에 대한 수퍼 유저 액세스
      - 특정 환경에 대한 관리자 액세스
      - an [!DNL Adobe Commerce] 작성기 저장소에 액세스할 수 있는 권한이 있는 계정

     다음을 참조하십시오 [사용자 액세스 관리](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) 다음에서 *클라우드 인프라의 Commerce 안내서*.

- **작성기 및 를 사용한 경험[!DNL Commerce CLI]**-참조 [확장 설치](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 다음에서 *설치 안내서* 에서 이러한 도구를 사용하여 확장을 설치하고 관리하는 방법에 대한 자세한 내용 [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 플랫폼.

- **[[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-를 활성화한 경우 [!DNL Amazon Sales Channel] 에 대한 [!DNL Commerce] sites에서 다음을 확인합니다. [!DNL Commerce] 설치하기 전에 platform에 버전 4.4.2 이상이 설치되어 있습니다. [!DNL Channel Manager].

- **[!DNL Inventory Management]Adobe Commerce 및 Magento Open Source 확장**

  재고 및 주문 관리에 Channel Manager를 사용할 계획이라면 Adobe Commerce 및 Magento Open Source 인스턴스에 Inventory management 확장 기능이 설치 및 활성화되어 있어야 합니다. 일반적으로 이 확장은 Adobe Commerce에 기본적으로 설치되고 활성화됩니다. [!DNL Magento Open Source] 2.3.x 이상

  Commerce를 2.2.x에서 업그레이드했거나 Inventory management을 사용하지 않도록 설정한 경우 필요한 모듈을 포함하도록 설치를 업데이트합니다. 다음을 참조하십시오 [Inventory management 설치](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html) 다음에서 *Inventory management 안내서*.

### 시스템 요구 사항

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7.3 / 7.4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [Composer 1.x 이상](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-를 활성화한 경우 [!DNL Amazon Sales Channel] 에 대한 [!DNL Commerce] sites에서 다음을 확인합니다. [!DNL Commerce] 설치하기 전에 platform에 버전 4.4.2가 설치되어 있습니다 [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### 지원되는 플랫폼

- ECE(Adobe Commerce on Cloud) : 2.4.x
- Adobe Commerce 온-프레미스(EE) : 2.4.x
- Magento Open Source 2.4.x

## 온보딩 단계

1. [Walmart 판매자 계정 설정](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [설치 [!DNL Channel Manager] 확장](install.md).

1. [상거래 서비스에 연결](connect.md) Commerce 인스턴스 및 기타 지원 서비스와 Channel Manager 통합

1. [연결 [!DNL Commerce] 저장 위치: [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [스토어 설정 완료](complete-sales-channel-store-setup.md).
