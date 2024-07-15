---
title: ' [!DNL Amazon Sales Channel] 확장 설치'
description: ' [!DNL Commerce] 카탈로그를  [!DNL Amazon Seller Accounts] 과(와) 통합하고  [!DNL Amazon Marketplace]을(를) 통해 판매하려면 Amazon Sales Channel 확장을 다운로드하여 설치하십시오.'
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 010a95d7be29354515cf4dcbf5d557eebaa40ed6
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 확장 설치

>[!IMPORTANT]
>
>Adobe Commerce 및 Magento Open Source 2.4.x 버전에서는 [!DNL Amazon Sales Channel] 확장 4.0 이상 버전만 지원됩니다. 2.3.x 버전을 실행 중인 경우 [호환 Amazon 판매 채널 릴리스](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html)에 대한 설명서를 참조하십시오. 버전 호환성에 대한 자세한 내용은 개발자 설명서에서 [가용성](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 페이지를 참조하십시오.

[!UICONTROL Amazon Sales Channel] 확장은 Commerce 카탈로그를 [!DNL Amazon Seller Accounts]과(와) 통합하여 [!DNL Amazon Marketplace]을(를) 통해 판매하는 기능을 설치 및 추가합니다. 추가 정보를 검토하려면 [!DNL Commerce Marketplace]의 [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) 페이지와 [릴리스 정보](release-notes.md)를 참조하세요.

## 요구 사항

- **Commerce 인스턴스**: [!DNL Amazon Sales Channel] 확장은 cloud infrastructure 버전 2.3.x 이상의 Magento Open Source, Adobe Commerce 및 Adobe Commerce을 사용하는 인스턴스에 설치할 수 있습니다. 2.1, 2.2 또는 1.x 릴리스에서는 더 이상 지원되지 않습니다.
- **Commerce 웹 계정**: API 키를 만들고 추적하는 데 사용되는 Commerce 웹 계정이 있어야 합니다.
- **API 키**: Commerce 웹 계정을 통해 Amazon 판매 채널 API 키를 만듭니다. 다음 지침에는 다음 단계가 포함되어 있습니다.

## 설치

이 프로세스에 작성기를 사용하는 방법에 대한 자세한 내용은 개발자 설명서에서 [확장 설치](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 지침을 참조하십시오.

1. [Commerce Marketplace](https://marketplace.magento.com/customer/account/)에 로그인합니다.

1. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Amazon Sales Channel]**&#x200B;을(를) 찾아 선택합니다.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름과 버전을 보려면 **[!UICONTROL Technical Details]**&#x200B;을(를) 클릭하십시오.

1. 이름 및 버전 정보를 사용하여 `composer.json` 파일의 서비스 커넥터 항목을 업데이트하십시오.

   - `composer.json` 파일에 확장 이름 및 버전을 추가하십시오.

   - [!DNL Commerce] 프로젝트 디렉터리로 이동하고 `composer.json` 파일을 업데이트합니다.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - [인증 키](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html)를 입력하십시오. 공개 키는 사용자 이름이고 개인 키는 암호입니다.

   - Composer에서 프로젝트 종속성 업데이트를 마치고 오류가 없는지 확인할 때까지 기다립니다.

1. [확장을 확인합니다](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## Amazon 판매 채널 API 키 추가

설치 후 구성을 완료하려면 [API 키](./amazon-verify-api-key.md)를 입력하십시오.

## Amazon 채널 구성 옵션 설정

Amazon 판매 채널을 구성하기 위한 다음과 같은 옵션이 있습니다. Amazon에서 온보딩 및 판매를 시작하기 위해 이러한 설정을 수정할 필요가 없습니다. 고급 관리자는 이러한 옵션을 고려하는 것이 좋습니다.

1. 관리자에 로그인합니다.

1. _관리자_ 사이드바에서 **스토어** > _설정_ > **구성**(으)로 이동합니다.

1. **Sales Channel**&#x200B;을 클릭한 다음 **전역 설정**&#x200B;을 클릭합니다.

1. **로그 기록 지우기**&#x200B;에 대해 수집된 로그를 지우는 간격을 정의합니다.

   옵션에는 `Once Daily`, `Once Weekly` 및 `Once Monthly`(기본값)이 포함됩니다.

1. (선택 사항) **CRON(백그라운드 작업) Source**&#x200B;의 경우 설정을 `Command Line (CLI) CRON`(으)로 변경하십시오.

   이 설정은 **_고급 사용자/관리자_**&#x200B;에게 권장됩니다.

1. **[!UICONTROL Save Config]**&#x200B;을(를) 클릭합니다.

## 확장 업데이트

1. [Commerce Marketplace](https://marketplace.magento.com/customer/account/)에 로그인합니다.

1. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Amazon Sales Channel]**&#x200B;을(를) 찾아 선택합니다.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름과 버전을 보려면 **[!UICONTROL Technical Details]**&#x200B;을(를) 클릭하십시오.

1. _설치 안내서_&#x200B;에서 [확장 업그레이드 지침](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)을 완료합니다.
