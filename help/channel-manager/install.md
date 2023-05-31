---
title: '설치 [!DNL Channel Manager]'
description: '설치[!DNL Channel Manager] 확장명.'
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---


# 설치 [!DNL Channel Manager]

리뷰 [요구 사항](onboard.md#requirements) Channel Manager를 설치하기 전에 필요한 정보를 수집합니다.

## 확장 설치

Channel Manager 설치 지침은 Adobe Commerce 또는 Magento Open Source이 온프레미스에 배포되었는지 또는 클라우드 인프라에 배포되었는지에 따라 다릅니다.

- 에 설치 [온-프레미스 인스턴스](#install-on-an-on-premises-instance).

- 에 설치 [[!DNL Adobe Commerce] 클라우드 인프라 인스턴스에서](#install-adobe-commerce-on-cloud-infrastructure)

두 방법 모두 명령줄 인터페이스(CLI)를 사용해야 합니다.

>[!NOTE]
>
>설치에 대한 도움말 [!DNL Commerce] CLI를 사용하는 소프트웨어는 [확장 설치](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### 온-프레미스 인스턴스에 설치

다음 지침에 따라 설치하십시오. [!DNL Channel Manager] Adobe Commerce 및 온-프레미스 인스턴스에 Magento Open Source.

1. 에 로그인합니다 [!DNL Commerce] 서버 as a [권한이 있는 사용자](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) 에 쓰기 [!DNL Commerce] 파일 시스템.

1. 웹 사이트 입력 [유지 관리 모드](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 다음에서 [!DNL Commerce] 프로젝트 루트 디렉터리, 채널 관리자 추가 `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. 메시지가 표시되면 [!DNL Commerce] 계정입니다.

   공개 키는 사용자 이름이고 개인 키는 암호입니다.

1. 종속성을 업데이트하고 확장을 설치합니다.

   ```bash
   composer update magento/channel-manager
   ```

   다음 `composer update` 명령은에 필요한 종속성만 업데이트합니다. [!DNL Channel Manager]. 모든 종속성을 업데이트하려면 이 명령을 대신 사용하십시오. `composer update`.

1. 작성기가 프로젝트 종속성 업데이트를 완료하고 오류를 해결할 때까지 기다립니다.

1. 모듈 설치 확인:

   - 모듈 상태를 확인합니다.

      ```bash
      bin/magento module:status Magento_SalesChannels
      ```

      샘플 응답:

      ```terminal
      Module is enabled
      ```

   - 모듈이 활성화되지 않은 경우 활성화합니다.

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. 확장을 등록합니다.

   ```bash
   bin/magento setup:upgrade
   ```

1. 메시지가 표시되면 [!DNL Commerce] 프로젝트.

   ```bash
   bin/magento setup:di:compile
   ```

1. 캐시를 정리합니다.

   ```bash
   bin/magento cache:clean
   ```

1. 유지 관리 모드를 비활성화합니다.

   ```bash
   bin/magento maintenance:disable
   ```

### 클라우드 인프라 인스턴스의 Adobe Commerce에 설치

클라우드 인스턴스에 확장을 추가할 때 개발 분기에서 작동합니다.

분기 사용에 대한 도움말은 를 참조하십시오. [분기 만들기 시작](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) 다음에서 _클라우드 인프라의 Commerce 안내서_.

설치하는 동안 확장 이름(`magento\channel-manager`)가 [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) 파일. 파일을 직접 편집할 필요는 없습니다.

1. 로컬 워크스테이션에서 클라우드 프로젝트 루트 디렉터리로 변경합니다.

1. 개발 만들기 또는 체크 아웃 [분기](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. 작성기 이름을 사용하여 확장자를 `require` 의 섹션 `composer.json` 파일.

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. 종속성을 업데이트하고 확장을 설치합니다.

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   다음 `composer update` 명령은에 필요한 종속성만 업데이트합니다. [!DNL Channel Manager]. 모든 종속성을 업데이트하려면 이 명령을 대신 사용하십시오. `composer update`.

1. 코드 변경 사항 추가, 커밋 및 푸시 - 두 항목에 대한 변경 사항 포함 `composer.lock` 및 `composer.json` 파일.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m "Install channel manager extension" 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 빌드 및 배포 프로세스가 완료되면 SSH를 사용하여 원격 환경에 로그인하고 확장이 올바르게 설치되었는지 확인합니다.

```bash
   bin/magento module:status Magento_SalesChannels
```

샘플 응답:

```terminal
Module is enabled
```

모듈이 비활성화되면 [로컬 환경에서 활성화합니다.](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) 변경 사항을 배포합니다.


1. 확장을 성공적으로 설치한 후에에 로그인합니다 [!UICONTROL Admin] 끝 [commerce Services 커넥터 구성](connect.md).

   >[!NOTE]
   >
   >Channel Manager를 새 릴리스로 업데이트하는 방법은 다음을 참조하십시오. [모듈 및 확장 업그레이드](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## 문제 해결

다음 정보를 사용하여 Channel Manager 설치 프로세스 중에 발생하는 오류를 해결하십시오.

### 잘못된 작성기 키

다음과 같은 경우 [액세스 키](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) 작성기 리포지토리에 인증하는 데 사용되었거나, [!DNL MAGE ID] 을(를) 등록하는 데 사용됨 [!DNL Channel Manager] 서비스에서 다음 오류가 표시됩니다.

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

주요 구성 확인:

1. 의 위치 찾기 `auth.json` 파일:

   ```bash
   $ composer config –global home
   ```

1. 보기 `auth.json` 파일.

   ```bash
   $ cat /path/to/auth.json
   ```

1. auth.json의 자격 증명이 일치하는지 확인 [mage ID와 연결된 키](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) 채널 관리자 서비스를 등록하는 데 사용됩니다.

### PHP에 필요한 메모리가 부족합니다.

시스템에 PHP에 충분한 메모리가 할당되지 않은 경우 다음 오류가 표시됩니다.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

다음 방법 중 하나를 사용하여 메모리 문제를 해결하십시오.

- [PHP에 대한 메모리 제한 늘이기](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) 환경 `php.ini` 파일. 또한 Commerce 인스턴스에 [권장 값](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) 다른 PHP 설정용.

- 명령줄에서 메모리 제한을 지정합니다.

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   예:

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### 보기 누락

누락에 대해 오류를 발견하면 `process_catalog_exporter_view` channel Manager 설치 중에 다음을 시도해 보십시오. [인덱서를 새로 고치는 중](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### 클라우드 배포 오류

확장을 클라우드에 배포하는 데 발생하는 문제는 다음을 참조하십시오. [확장 배포 실패](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
