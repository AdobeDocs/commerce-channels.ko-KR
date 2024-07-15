---
title: 온보드 [!DNL Channel Manager]
description: '몇 가지 온보딩 단계를 완료하여 인스턴스를  [!DNL Channel Manager] 서비스에 연결하십시오.'
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---


# [!DNL Channel Manager] 온보드

Channel Manager 온보딩 프로세스를 완료한 후 Adobe Commerce에서 Walmart Marketplace 채널 판매 운영을 액세스, 구성 및 관리할 수 있습니다. 채널 관리자는 [!UICONTROL Commerce Admin Marketing] 메뉴의 [!UICONTROL Channel Manager] 옵션에서 사용할 수 있습니다.

관리자 보기의 ![[!DNL Channel Manager] 옵션](assets/channel-manager-admin-view.png){width="500"}

## 요구 사항

Channel Manager 사용 요구 사항을 검토하고 필요한 계정 정보와 자격 증명을 수집하여 확장을 다운로드, 설치 및 구성합니다.

- **[Walmart Marketplace 요구 사항](walmart-requirements.md)**-Channel Manager와 통합하기 위한 요구 사항(예: [판매자 계정 설정](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) 및 통합을 활성화하기 위한 API 키 생성)을 충족하는지 확인하십시오.

- **Commerce 계정 정보** - [!DNL Channel Manager]을(를) 다운로드하고 설치하려면 [Commerce 계정](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html)이 필요합니다. [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 인스턴스에 대한 소유자 또는 관리자 액세스 권한이 있는 계정 ID 및 자격 증명이 필요합니다.

   - **[!UICONTROL My Account - Magento settings]**&#x200B;에서 ID를 가져오려면 **MAGE ID**-[[!DNL Commerce] 계정에 로그인](https://account.magento.com/customer/account/login/)하십시오.

     [!DNL Commerce] 계정 설정의 ![[!DNL MAGEID]](assets/mageid-my-commerce-account.png){width="250"}

   - **액세스 키-** [!DNL Commerce] 작성기 저장소 `([!DNL repo.magento.com]`에서 [!DNL Commerce] 확장을 다운로드하기 위한 인증 키를 가져옵니다.

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Adobe Commerce 및 Magento Open Source 프로젝트에서 소유자는 [공유 액세스](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)를 설정하여 신뢰할 수 있는 직원과 서비스 공급자가 소유자 또는 라이선스 소유자 계정의 자격 증명을 사용하여 확장을 다운로드할 수 있도록 할 수 있습니다.

     클라우드 인프라 프로젝트의 [!DNL Adobe Commerce]에 대해 소프트웨어 설치 관리자에게는 [!DNL Commerce] 인스턴스에 대한 다음 액세스 권한이 있어야 합니다.

      - 클라우드 프로젝트에 대한 수퍼 유저 액세스
      - 특정 환경에 대한 관리자 액세스
      - 작성기 저장소에 액세스할 수 있는 권한이 있는 [!DNL Adobe Commerce] 계정

     *Cloud Infrastructure의 Commerce 안내서*&#x200B;에서 [사용자 액세스 관리](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html)를 참조하십시오.

- **작성기 및[!DNL Commerce CLI]**&#x200B;을(를) 사용하는 경험입니다. [!DNL Adobe Commerce] 또는 [!DNL Magento Open Source] 플랫폼에서 이러한 도구를 사용하여 확장을 설치하고 관리하는 방법에 대한 자세한 내용은 *설치 안내서*&#x200B;의 [확장 설치](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)를 참조하십시오.

- **[[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-[!DNL Commerce] 사이트에 대해 [!DNL Amazon Sales Channel]을(를) 활성화한 경우 [!DNL Channel Manager]을(를) 설치하기 전에 [!DNL Commerce] 플랫폼에 버전 4.4.2 이상이 설치되어 있는지 확인하십시오.

- Adobe Commerce 및 Magento Open Source에 대한 **[!DNL Inventory Management]확장**

  재고 및 주문 관리에 Channel Manager를 사용할 계획이라면 Adobe Commerce 및 Magento Open Source 인스턴스에 Inventory management 확장 기능이 설치 및 활성화되어 있어야 합니다. 일반적으로 이 확장은 Adobe Commerce 및 [!DNL Magento Open Source] 2.3.x 이상에서 기본적으로 설치되고 활성화됩니다.

  2.2.x에서 Commerce을 업그레이드했거나 Inventory management을 사용하지 않도록 설정한 경우 필요한 모듈을 포함하도록 설치를 업데이트합니다. *Inventory management 안내서*&#x200B;에서 [Inventory management 설치](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)를 참조하십시오.

### 시스템 요구 사항

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7.3 / 7.4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [작성기 1.x 이상](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] 버전 4.4.2 이상](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-[!DNL Commerce] 사이트에 대해 [!DNL Amazon Sales Channel]을(를) 활성화한 경우 [!DNL Channel Manager]을(를) 설치하기 전에 [!DNL Commerce] 플랫폼에 버전 4.4.2가 설치되어 있는지 확인하십시오.
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### 지원되는 플랫폼

- ECE(Adobe Commerce on Cloud) : 2.4.x
- Adobe Commerce 온-프레미스(EE) : 2.4.x
- Magento Open Source 2.4.x

## 온보딩 단계

1. [월마트 판매자 계정을 설정합니다](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [확장 설치 [!DNL Channel Manager] 2}.](install.md)

1. [Commerce 서비스에 연결](connect.md) - Channel Manager를 Commerce 인스턴스 및 기타 지원 서비스와 통합합니다.

1. [스토어를  [!DNL Walmart Marketplace]](connect-marketplace.md)에 연결 [!DNL Commerce] 합니다.

1. [스토어 설정 완료](complete-sales-channel-store-setup.md).
