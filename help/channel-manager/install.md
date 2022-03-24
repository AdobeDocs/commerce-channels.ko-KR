---
title: 설치 [!DNL Channel Manager]
description: 채널 관리자 확장을 설치합니다.
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# 채널 관리자 설치

를 검토합니다. [전제 조건](onboard.md#prerequisites) 채널 관리자를 설치하기 전에 필요한 정보를 수집합니다.

## 최소 안정성 설정 업데이트

확장을 설치하기 전에 `minimum-stability` 요구 사항 `composer.json` 파일을 만들면 Composer를 사용하여 채널 관리자의 이전 버전을 설치할 수 있습니다.

구성을 업데이트하려면 다음 줄을 `composer.json` 파일.

```json
{
   "minimum-stability": "alpha",
   "prefer-stable": true
}
```

## 확장 설치

채널 관리자 설치 지침은 Adobe Commerce 또는 Magento Open Source이 온프레미스 또는 클라우드 인프라에 배포되는지 여부에 따라 다릅니다.

- 설치 [온-프레미스 인스턴스](#install-on-an-on-premises-instance).

- 설치 [[!DNL Adobe Commerce] 클라우드 인프라 인스턴스](#install-adobe-commerce-on-cloud-infrastructure)

두 방법 모두 명령줄 인터페이스(CLI)를 사용해야 합니다.

>[!NOTE]
>
>설치 도움말 [!DNL Commerce] CLI를 사용하는 소프트웨어 [일반 CLI 설치](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}.

### 온-프레미스 인스턴스에 설치

다음 지침에 따라 Adobe Commerce 및 Magento Open Source 플랫폼에 설치합니다.

1. 에 로그인합니다. [!DNL Commerce] 서버로 [권한이 있는 사용자](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;} - 쓰기 [!DNL Commerce] 파일 시스템.

1. 웹 사이트를 [유지 모드](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}.

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 에서 [!DNL Commerce] 프로젝트 루트 디렉토리, 채널 관리자를 추가합니다. `composer.json`.

   ```bash
    $ composer require magento/channel-manager --no-update
   ```

1. 메시지가 표시되면 [!DNL Commerce] 계정이 필요합니다.

   공개 키는 사용자 이름 입니다. 개인 키는 암호입니다.

1. 종속성을 업데이트하고 확장을 설치합니다.

   ```bash
   $ composer update
   ```

   다음 `composer update` 명령은 모든 종속성을 업데이트합니다. 채널 관리자와 관련된 종속성만 업데이트하려면 대신 이 명령을 사용하십시오. `composer update magento/channel-manager`.

1. 작성기가 프로젝트 종속성 업데이트를 완료하고 오류를 해결할 때까지 기다립니다.

1. 설치 확인

   ```bash
   $ bin/magento module:status channel-manager
   ```

   샘플 응답:

   ```terminal
   Module is disabled
   ```

1. 확장을 등록합니다.

   ```bash
   $ bin/magento setup:upgrade
   ```

1. 메시지가 표시되면 다시 컴파일하십시오 [!DNL Commerce] 프로젝트.

   ```bash
   $ bin/magento setup:di:compile
   ```

1. 확장이 활성화되어 있는지 확인합니다.

   ```bash
   $ bin/magento module:status channel-manager
   ```

   샘플 응답:

   ```bash
   Module is enabled
   ```

1. 캐시를 지웁니다.

   ```bash
   $ bin/magento cache:clean
   ```

1. 유지 관리 모드를 비활성화합니다.

   ```bash
    $ bin/magento maintenance:disable
   ```

### 클라우드 인프라 인스턴스에 Adobe Commerce 설치

클라우드 인스턴스에 확장을 추가할 때 개발 분기에서 작업합니다.

분기 사용에 대한 자세한 내용은 [분기 만들기 시작](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted)Adobe Commerce 개발자 설명서의 {target=&quot;_blank&quot;}.

설치하는 동안 확장 이름(`&lt;VendorName>\_&lt;ComponentName>`)이 자동으로 [app/etc/config.php](https://devdocs-beta.magento.com/guides/v2.3/config-guide/config/config-php.html){target=&quot;_blank&quot;} 파일입니다. 파일을 직접 편집할 필요는 없습니다.

1. 로컬 워크스테이션에서 클라우드 프로젝트 루트 디렉토리로 변경합니다.

1. 개발 만들기 또는 체크아웃 [분기](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}.

1. 작성기 이름을 사용하여 확장을 `require` 섹션 `composer.json` 파일.

   ```bash
   $ composer require magento/channel-manager --no-update
   ```

1. 코드 변경 사항을 추가, 커밋 및 푸시할 때 변경 사항을 `composer.lock` 및 `composer.json` 파일.

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 빌드 및 배포가 완료되면 SSH를 사용하여 원격 환경에 로그인하고 확장이 올바르게 설치되었는지 확인하십시오.

   ```bash
   $ bin/magento module:status channel-manager
   ```

   샘플 응답:

   ```terminal
   Module is enabled
   ```

1. 설치가 성공적으로 완료되면 [!UICONTROL Admin] to [commerce Services 커넥터 구성](connect.md).

   >[!NOTE]
   >
   >채널 관리자를 새 릴리스로 업데이트하는 방법에 대한 지침은 [모듈 및 확장 업그레이드](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}.


## 문제 해결

채널 관리자 설치 프로세스 중에 발생하는 오류를 해결하려면 다음 정보를 사용하십시오.

### 잘못된 작성기 키

만약 [액세스 키](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html)작성기 리포지토리를 인증하는 데 사용된 {target=&quot;_blank&quot;}이 잘못되었거나 작성기 리포지토리에 연결되어 있지 않습니다 [!DNL MAGE ID] 등록 [!DNL Channel Manager] 서비스, 다음 오류가 표시됩니다.


```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

주요 구성을 확인합니다.

1. 의 위치 찾기 `auth.json` 파일:

   ```bash
   $ composer config –global home
   ```

1. 보기 `auth.json` 파일.

   ```bash
   $ cat /path/to/auth.json
   ```

1. auth.json의 자격 증명이 일치하는지 확인합니다 [이미지 ID와 연결된 키](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html)채널 관리자 서비스에 등록하는 데 사용되는 {target=&quot;_blank&quot;}입니다.

### PHP에 메모리가 부족합니다.

시스템에 PHP에 대해 할당된 메모리가 부족한 경우 다음 오류가 표시됩니다.

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

다음 방법 중 하나를 사용하여 메모리 문제를 해결하십시오.

- [PHP의 메모리 제한 증가](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit)환경의 {target=&quot;_blank&quot;} `php.ini` 파일. 또한 상거래 인스턴스에 [권장 값](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)다른 PHP 설정에 대해 {target=&quot;_blank&quot;}.

- 명령줄에서 메모리 제한을 지정합니다.

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   For example:

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### 보기 누락

실종에 대한 오류가 발생하면 `process_catalog_exporter_view` 채널 관리자를 설치하는 동안 [인덱서 새로 고침](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}.

```bash
php bin/magento indexer:refresh
```

### 클라우드 배포 오류

클라우드에 확장을 배포하는 데 문제가 있는 경우 다음을 참조하십시오. [확장 배포 실패](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}.
