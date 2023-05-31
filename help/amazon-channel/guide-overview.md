---
title: '[!DNL Amazon Sales Channel] 가이드'
description: 다음에 대한 포괄적인 정보 [!DNL Amazon sales channel] Adobe Commerce 및 Magento Open Source 관리자(설치 및 온보딩 포함)
seo-title: Adobe Commerce Amazon Sales Channel Guide
seo-description: Describes how to use [!DNL Amazon sales channel] with Adobe Commerce or Magento Open Source.
exl-id: ad3e2353-313b-4c40-800a-b1ef5f0d8235
source-git-commit: 901d856067cd9d236727edc8bde354820791c411
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 안내서

이 안내서는 Adobe Commerce 및 Magento Open Source 관리자를 위한 것입니다. 여기에는 의 설치 및 온보딩에 대한 자세한 정보가 포함되어 있습니다 [!DNL Amazon sales channel], 서비스 구성 및 관리. 이는 핵심 상거래 구성 및 기능에 대한 기본적인 이해를 전제로 합니다.

[!DNL Amazon sales channel] 에는 관리자를 위한 두 가지 영역이 있습니다.

* 관리자: 이 영역을 사용하여 구성 UI 및 보고에 액세스합니다.
* 명령줄 인터페이스: 이 도구를 사용하여 설치 및 백엔드 구성 작업을 실행합니다.

이 안내서에서는 몇 가지 기본 사항을 검토합니다. [!DNL Amazon Seller Central] 정보, Amazon 판매 채널을 설정하기 위한 요구 사항. 또한 온보딩 및 통합 프로세스, 사용 가능한 스토어, 제품, 가격 및 기타 옵션, 그리고 Amazon 판매 채널을 사용하여 의 목록 및 판매를 관리하는 방법에 대한 세부 정보가 포함되어 있습니다. [!DNL Amazon Marketplace]. 왼쪽 레일을 사용하여 다양한 기능을 탐색하고 세부 정보 및 절차에 액세스하기 위해 드릴다운합니다.

>[!NOTE]
>
>이 안내서에서는 Adobe Commerce 및 Magento Open Source의 핵심 기능을 다루지 않습니다.

| 영역 | 설명 |
|----|----|
| [Amazon 판매 채널 소개](./overview.md) | Amazon 영업 채널 기본 사항, 주요 기능, 모범 사례 등에 대해 자세히 알아보십시오. |
| [Amazon 판매 채널 온보드](./amazon-onboarding-home.md) | Amazon 스토어를 신속하게 만들고 와 통합 [!DNL Amazon Seller Central]. Amazon 판매 채널을 가동하여 판매를 시작하십시오. |
| [Amazon sales channel 홈](./amazon-sales-channel-home.md) | Amazon 판매 채널 홈 페이지와 사용 가능한 옵션 및 작업에 대해 자세히 알아보십시오. Amazon 스토어에 대한 요약 정보를 보고 스토어 세부 정보 및 설정에 액세스할 수 있습니다. |
| [속성 관리](./attributes-view.md) | Amazon sales channel은 [!DNL Commerce] 제품 특성을 사용하는 카탈로그 및 Amazon. 이러한 속성을 만들고, 매핑하고, 관리하는 방법에 대해 자세히 알아보십시오. |
| [스토어 설정 관리](./ob-store-review.md) | 목록 설정, 주문 설정, 목록 및 가격책정 규칙을 포함한 스토어 설정을 조회하고 수정합니다. |
| [목록 관리](./managing-product-listings.md) | Amazon 마켓플레이스를 통해 판매하면서 목록(설정, 규칙 및 가격)을 업데이트, 추가 및 관리할 수 있습니다. 스토어 및 목록 설정 생성 및 수정에 대해 자세히 알아보십시오. |
| [주문 및 이행 관리](./managing-orders.md) | Amazon 판매 채널은 Amazon 및 를 통한 주문 이행 및 납품을 지원합니다. [!DNL Commerce]. Amazon을 통해, 을 통해 직접 구현에 대해 자세히 알아보십시오. [!DNL Commerce]및 order management 옵션. |
| [로그 및 보고서 보기](./amazon-logs-reports.md) | Amazon과 간의 추적된 오류 및 상호 작용에 대해 자세히 알아보십시오. [!DNL Commerce]. |

## 추가 설명서

| 설명서 리소스 | 설명 |
|----------------------- | ----------- |
| [Adobe Commerce 2.4 Merchant 설명서](https://experienceleague.adobe.com/docs/commerce-admin/user-guides/home.html) | Adobe Commerce 및 Magento Open Source 모두를 위한 판매자 중심 설명서 |
| [Adobe Commerce 설명서를 위한 서비스](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) | 판매자가 비즈니스의 주요 구성 요소를 스토어와 통합하는 데 도움이 되는 서비스 컬렉션을 지원하는 설명서입니다. |
| [클라우드 인프라의 Commerce 안내서](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/overview.html) | 관리되고 자동화된 호스팅 클라우드 플랫폼에서의 Adobe Commerce 배포에 대한 단계별 절차. |
| [Adobe Commerce 2.4 운영 안내서](https://experienceleague.adobe.com/docs/commerce-operations/operational-guides/home.html) | Adobe Commerce 및 Magento Open Source 플랫폼에 배포된 프로젝트를 개발, 배포 및 유지 관리하기 위한 개념, 프로세스, 도구 및 모범 사례에 대한 시스템 설명서입니다. |
| [Adobe Commerce 2.4 개발자 설명서](https://developer.adobe.com/commerce/docs) | Adobe Commerce 또는 Magento Open Source을 빌드하고 사용자 지정하는 데 사용되는 개발자 중심의 설명서 |

{style="table-layout:auto"}

## 지원

이 안내서에서 다루지 않는 정보가 필요하거나 질문이 있는 경우 다음 리소스를 사용하십시오.

* [도움말 센터](https://support.magento.com/hc/en-us)- 다음을 참조하십시오. [!DNL Amazon Sales Channel]-관련 문제 해결 문서.
* [지원 티켓](https://support.magento.com/hc/en-us/articles/360000913794#submit-ticket)- 추가 지원을 받으려면 티켓을 제출합니다.
