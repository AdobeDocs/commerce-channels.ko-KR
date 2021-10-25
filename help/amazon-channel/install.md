---
title: 확장 설치
description: 를 통합하려면 [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] 그리고 [!DNL Amazon Marketplace]Amazon Sales Channel 확장을 다운로드하여 설치합니다.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 확장 설치

>[!IMPORTANT]
>
>전용 [!DNL Amazon Sales Channel] 확장 4.0 이상 버전은 Adobe Commerce 및 Magento Open Source 2.4.x 버전에서 지원됩니다. 2.3.x 버전을 실행하는 경우 [호환 가능한 Amazon 판매 채널 릴리스](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}. 버전 호환성에 대한 자세한 내용은 [사용 가능](https://devdocs.magento.com/release/availability.html)개발자 설명서의 {target=&quot;_blank&quot;} 페이지입니다.

다음 [!UICONTROL Amazon Sales Channel] extension에서 Commerce 카탈로그를 와 통합하는 기능을 설치하고 추가합니다. [!DNL Amazon Seller Accounts] 팔다 [!DNL Amazon Marketplace]. 추가 정보를 검토하려면 [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) 페이지 [!DNL Commerce Marketplace] 그리고 [릴리스 노트](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) 개발자 설명서에서 를 참조하십시오.

## 요구 사항

- **상거래 인스턴스**: 다음 [!DNL Amazon Sales Channel] 확장은 클라우드 인프라 버전 2.3.x 이상에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce이 있는 인스턴스에 설치할 수 있습니다. 2.1, 2.2 또는 1.x 릴리스에서 더 이상 지원되지 않습니다.
- **상거래 웹 계정**: API 키를 만들고 추적하는 데 사용되는 상거래 웹 계정이 있어야 합니다.
- **API 키**: Commerce 웹 계정을 통해 Amazon 판매 채널 API 키를 만듭니다. 다음은 이러한 단계입니다.

## 설치

이 프로세스에 작성기 사용에 대한 자세한 내용은 [확장 설치](https://devdocs.magento.com/extensions/install/)개발자 설명서의 {target=&quot;_blank&quot;} 지침입니다.

1. 에 로그인합니다. [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. 을(를) 클릭합니다. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**.

1. 찾기 및 선택 **[!UICONTROL Amazon Sales Channel]**.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름과 버전을 보려면 **[!UICONTROL Technical Details]**.

1. 이름 및 버전 정보를 사용하여 `composer.json` 파일.

   - 확장의 이름 및 버전을 `composer.json` 파일.

   - 로 이동합니다. [!DNL Commerce] 프로젝트 디렉토리 및 업데이트 `composer.json` 파일.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 을(를) 입력합니다. [인증 키](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}. 공개 키는 사용자 이름 입니다. 개인 키는 암호입니다.

   - 작성기가 프로젝트 종속성 업데이트를 완료하고 오류가 없는지 확인할 때까지 기다리십시오.


1. [확장 확인](https://devdocs.magento.com/extensions/install/#verify-the-extension){target=&quot;_blank&quot;}.

## Amazon 영업 채널 API 키 추가

설치 후 다음을 입력합니다 [API 키](./amazon-verify-api-key.md) 구성을 완료합니다.

## Amazon 채널 구성 옵션 설정

Amazon 판매 채널을 구성하기 위한 다음 옵션이 있습니다. Amazon에서 온보딩 및 판매를 시작하기 위해 이러한 설정을 수정할 필요가 없습니다. 고급 관리자는 이러한 옵션을 고려해 보는 것이 좋습니다.

1. 관리자에 로그인합니다.

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **스토어** > _설정_ > **구성**.

1. 클릭 **Sales Channel**, 그런 다음 **전역 설정**.

1. 대상 **로그 기록 지우기**&#x200B;를 사용하여 수집된 로그를 지우는 간격을 정의합니다.

   옵션은 다음과 같습니다 `Once Daily`, `Once Weekly`, 및 `Once Monthly` (기본값)

1. (선택 사항) **배경 작업(CRON) 소스**&#x200B;를 입력하여 설정을 로 변경합니다. `Command Line (CLI) CRON`.

   이 설정은 **_고급 사용자/관리자_**.

1. 클릭 **[!UICONTROL Save Config]**.

## 확장 업데이트

1. 에 로그인합니다. [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;}.

1. 을(를) 클릭합니다. **[!UICONTROL Marketplace]** 탭을 클릭한 다음 **[!UICONTROL My Purchases]**.

1. 찾기 및 선택 **[!UICONTROL Amazon Sales Channel]**.

1. 확장 페이지에서 버전을 선택합니다.

1. 구성 요소 이름과 버전을 보려면 **[!UICONTROL Technical Details]**.

1. 을(를) 완료합니다 [확장 업그레이드 지침](https://devdocs.magento.com/extensions/install/#upgrade-an-extension)개발자 설명서의 {target=&quot;_blank&quot;}.
