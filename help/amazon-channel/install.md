---
title: 확장 설치
description: ' [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] 을(를) 통합하고 [!DNL Amazon Marketplace]을 통해 판매하려면 Amazon Sales Channel 확장을 다운로드하여 설치합니다.'
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 확장 설치

>[!IMPORTANT]
>
>Adobe 상거래 및 Magento Open Source 2.4.x 버전에서는 [!DNL Amazon Sales Channel] 확장 4.0 이상 버전만 지원됩니다. 2.3.x 버전을 실행 중인 경우 [호환 Amazon 판매 채널 릴리스](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}에 대한 설명서를 참조하십시오. 버전 호환성에 대한 자세한 내용은 개발자 설명서에서 [가용성](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} 페이지를 참조하십시오.

[!UICONTROL Amazon Sales Channel] 확장은 상거래 카탈로그를 [!DNL Amazon Seller Accounts]과 통합하여 [!DNL Amazon Marketplace]를 통해 판매하는 기능을 설치 및 추가합니다. 추가 정보를 검토하려면 [!DNL Commerce Marketplace]의 [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) 페이지와 개발자 설명서에서 [릴리스 노트](https://devdocs.magento.com/extensions/amazon-sales/release-notes/)를 참조하십시오.

## 요구 사항

- **상거래 인스턴스**: 확장 [!DNL Amazon Sales Channel] 은 클라우드 인프라 버전 2.3.x 이상에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce가 있는 인스턴스에 설치할 수 있습니다. 2.1, 2.2 또는 1.x 릴리스에서 더 이상 지원되지 않습니다.
- **상거래 웹 계정**: API 키를 만들고 추적하는 데 사용되는 상거래 웹 계정이 있어야 합니다.
- **API 키**: Commerce 웹 계정을 통해 Amazon 판매 채널 API 키를 만듭니다. 다음은 이러한 단계입니다.

## 설치

이 프로세스에 Composer 사용에 대한 자세한 내용은 개발자 설명서의 [확장 설치](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} 지침을 참조하십시오.

1. [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}에 로그인합니다.

1. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]** 를 클릭합니다.

1. **[!UICONTROL Amazon Sales Channel]** 을(를) 찾아 선택합니다.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름 및 버전에 대해 **[!UICONTROL Technical Details]** 을 클릭합니다.

1. 이름 및 버전 정보를 사용하여 `composer.json` 파일의 서비스 커넥터 항목을 업데이트합니다.

   - 확장의 이름 및 버전을 `composer.json` 파일에 추가합니다.

   - [!DNL Commerce] 프로젝트 디렉토리로 이동하고 `composer.json` 파일을 업데이트합니다.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - [인증 키](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}를 입력합니다. 공개 키는 사용자 이름 입니다. 개인 키는 암호입니다.

   - 작성기가 프로젝트 종속성 업데이트를 완료하고 오류가 없는지 확인할 때까지 기다리십시오.


1. [확장](https://devdocs.magento.com/extensions/install/#verify-the-extension) {target=&quot;_blank&quot;}을 확인합니다.

## Amazon 영업 채널 API 키 추가

설치 후 [API 키](./amazon-verify-api-key.md)를 입력하여 구성을 완료합니다.

## Amazon 채널 구성 옵션 설정

Amazon 판매 채널을 구성하기 위한 다음 옵션이 있습니다. Amazon에서 온보딩 및 판매를 시작하기 위해 이러한 설정을 수정할 필요가 없습니다. 고급 관리자는 이러한 옵션을 고려해 보는 것이 좋습니다.

1. 관리자에 로그인합니다.

1. _관리_ 사이드바에서 **저장소** > _설정_ > **구성**&#x200B;으로 이동합니다.

1. **Sales Channel**&#x200B;을 클릭한 다음 **전역 설정**&#x200B;을 클릭합니다.

1. **로그 기록 지우기**&#x200B;에 대해 수집된 로그를 지우는 간격을 정의합니다.

   옵션에는 `Once Daily`, `Once Weekly` 및 `Once Monthly`(기본값)가 있습니다.

1. (선택 사항) **백그라운드 작업(CRON) 소스**&#x200B;에 대해 설정을 `Command Line (CLI) CRON`로 변경합니다.

   이 설정은 **_고급 사용자/관리자_**&#x200B;에 권장됩니다.

1. **[!UICONTROL Save Config]** 을 클릭합니다.

## 확장 업데이트

1. [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}에 로그인합니다.

1. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]** 를 클릭합니다.

1. **[!UICONTROL Amazon Sales Channel]** 을(를) 찾아 선택합니다.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름 및 버전에 대해 **[!UICONTROL Technical Details]** 을 클릭합니다.

1. 개발자 설명서에서 [확장 업그레이드 지침](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;}을 완료합니다.
