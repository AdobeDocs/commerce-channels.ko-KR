---
title: "설치 [!DNL Amazon Sales Channel] 확장"
description: 을(를) 통합하려면 [!DNL Commerce] 카탈로그 [!DNL Amazon Seller Accounts] 다음을 통해 판매 [!DNL Amazon Marketplace], Amazon Sales Channel 확장 기능을 다운로드하여 설치합니다.
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 설치 [!DNL Amazon Sales Channel] 확장

>[!IMPORTANT]
>
>전용 [!DNL Amazon Sales Channel] 확장 4.0 이상 버전은 Adobe Commerce 및 Magento Open Source 2.4.x 버전에서 지원됩니다. 2.3.x 버전을 실행 중인 경우 [호환 가능한 Amazon sales channel 릴리스](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). 버전 호환성에 대한 자세한 내용은 [사용 가능](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 페이지를 참조하십시오.

다음 [!UICONTROL Amazon Sales Channel] 확장 프로그램은 상거래 카탈로그를 통합할 기능을 설치 및 추가합니다. [!DNL Amazon Seller Accounts] 을 통해 판매 [!DNL Amazon Marketplace]. 추가 정보를 검토하려면 [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) 페이지 위치 [!DNL Commerce Marketplace] 및 [릴리스 정보](release-notes.md).

## 요구 사항

- **상거래 인스턴스**: [!DNL Amazon Sales Channel] 확장은 cloud infrastructure 버전 2.3.x 이상의 Magento Open Source, Adobe Commerce 및 Adobe Commerce 인스턴스에 설치할 수 있습니다. 2.1, 2.2 또는 1.x 릴리스에서는 더 이상 지원되지 않습니다.
- **Commerce 웹 계정**: API 키를 만들고 추적하는 데 사용되는 Commerce 웹 계정이 있어야 합니다.
- **API 키**: Commerce 웹 계정을 통해 Amazon 판매 채널 API 키를 만듭니다. 다음 지침에는 다음 단계가 포함되어 있습니다.

## 설치

이 프로세스에 작성기를 사용하는 방법에 대한 자세한 내용은 [확장 설치](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 개발자 설명서의 지침.

1. 에 로그인합니다 [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. 다음을 클릭합니다. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**.

1. 찾기 및 선택 **[!UICONTROL Amazon Sales Channel]**.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름 및 버전에 대해 **[!UICONTROL Technical Details]**.

1. 이름 및 버전 정보를 사용하여 `composer.json` 파일.

   - 확장 이름 및 버전을 `composer.json` 파일.

   - 다음으로 이동 [!DNL Commerce] 프로젝트 디렉터리 및 업데이트 `composer.json` 파일.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 다음을 입력하십시오. [인증 키](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html). 공개 키는 사용자 이름이고 개인 키는 암호입니다.

   - Composer에서 프로젝트 종속성 업데이트를 마치고 오류가 없는지 확인할 때까지 기다립니다.

1. [확장 확인](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## Amazon 판매 채널 API 키 추가

설치 후 다음을 입력하십시오. [API 키](./amazon-verify-api-key.md) 구성을 완료합니다.

## Amazon 채널 구성 옵션 설정

Amazon 판매 채널을 구성하기 위한 다음과 같은 옵션이 있습니다. Amazon에서 온보딩 및 판매를 시작하기 위해 이러한 설정을 수정할 필요가 없습니다. 고급 관리자는 이러한 옵션을 고려하는 것이 좋습니다.

1. 관리자에 로그인합니다.

1. 다음에서 _관리자_ 사이드바, 이동 **스토어** > _설정_ > **구성**.

1. 클릭 **Sales Channel**, 그런 다음 **전역 설정**.

1. 대상 **로그 내역 지우기**&#x200B;수집된 로그를 지우는 간격을 정의합니다.

   옵션은 다음과 같습니다 `Once Daily`, `Once Weekly`, 및 `Once Monthly` (기본값).

1. (선택 사항) **백그라운드 작업(CRON) 소스**, 설정을 다음으로 변경 `Command Line (CLI) CRON`.

   이 설정은 다음 경우에 권장됩니다. **_고급 사용자/관리자_**.

1. 클릭 **[!UICONTROL Save Config]**.

## 확장 업데이트

1. 에 로그인합니다 [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. 다음을 클릭합니다. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**.

1. 찾기 및 선택 **[!UICONTROL Amazon Sales Channel]**.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름 및 버전에 대해 **[!UICONTROL Technical Details]**.

1. 다음을 완료합니다. [확장 업그레이드 지침](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 다음에서 _설치 안내서_.
