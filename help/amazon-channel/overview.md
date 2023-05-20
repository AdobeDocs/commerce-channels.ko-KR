---
title: "[!DNL Amazon Sales Channel] 사용 안내서"
description: "[!DNL Amazon Sales Channel] 상인이 제품에서 원활하게 판매할 수 있도록 합니다. [!DNL Amazon Marketplace]."
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 74e58c95479b624ad9993d613776b4d33c492080
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 사용 안내서

[!DNL Amazon Sales Channel] 상인이 제품에서 원활하게 판매할 수 있도록 합니다. [!DNL Amazon Marketplace].

Adobe Commerce 또는 Magento Open Source 판매자는 [!DNL Amazon Sales Channel] 세계 최대의 글로벌 인터넷 쇼핑 목적지와 매장을 통합하는 확장. 이 확장 기능을 통해 다음을 연결하여 Amazon 판매 가능 [!DNL Commerce] (으)로 [!DNL Amazon Seller Central] 카탈로그 및 주문 데이터의 자동화 및 동기화를 모두 제공하는 계정. 모든 Amazon 목록을 완벽하게 관리하고, 단순하거나 지능적인 가격 규칙을 구현하며, 단일 솔루션을 통해 주문 및 재고를 유지 관리할 수 있습니다. [!DNL Commerce] 대시보드입니다.

시작하는 것은 쉽습니다. 짧은 온보딩 프로세스를 통해 [!DNL Amazon Seller Central] 계정 및 Amazon sales channel 스토어 및 [!DNL Commerce] 카탈로그로 Amazon 목록, 주문, 재고 및 이행을 관리합니다. 중앙 대시보드에는 모든 Amazon 판매 채널 스토어 통합 및 Amazon 목록에 대한 상태 업데이트가 표시됩니다. 전 세계의 새로운 고객에게 도달 [!DNL Amazon Marketplace] 단순화되고 자동화된 프로세스를 통해 새로운 시스템을 구축하는 데 드는 비용과 수고를 거의 또는 전혀 최소화할 수 있습니다.

통합 후 [!DNL Amazon Seller Central] 계정, [!DNL Amazon Sales Channel] 확장을 사용하면 계정을 관리하고 다음 간 데이터를 동기화할 수 있습니다. [!DNL Commerce] 그리고 Amazon. 목록을 만들고, 프로모션을 관리하고, 가격을 설정하고, 인벤토리와 이행을 직접 관리할 수 있습니다. [!DNL Commerce] 관리자. 이러한 옵션에는 동일한 품목에 대한 Amazon 가격을 모니터링하고 가격을 자동으로 조정하여 보다 경쟁력있게 조정하는 가격 책정 규칙이 포함됩니다.

## 안내서 개요

이 안내서에서는 몇 가지 기본 사항을 검토합니다. [!DNL Amazon Seller Central] 정보, Amazon 판매 채널을 설정하기 위한 요구 사항. 또한 온보딩 및 통합 프로세스, 사용 가능한 스토어, 제품, 가격 및 기타 옵션, 그리고 Amazon 판매 채널을 사용하여 의 목록 및 판매를 관리하는 방법에 대한 세부 정보가 포함되어 있습니다. [!DNL Amazon Marketplace]. 왼쪽 레일을 사용하여 다양한 기능을 탐색하고 세부 정보 및 절차에 액세스하기 위해 드릴다운합니다.

| 영역 | 설명 |
|----|----|
| [Amazon 판매 채널 정보](./about-amazon-sales-channel.md) | Amazon 영업 채널 기본 사항, 주요 기능, 모범 사례 등에 대해 자세히 알아보십시오. |
| [Amazon 판매 채널 온보드](./amazon-onboarding-home.md) | Amazon 스토어를 신속하게 만들고 와 통합 [!DNL Amazon Seller Central]. Amazon 판매 채널을 가동하여 판매를 시작하십시오. |
| [Amazon sales channel 홈](./amazon-sales-channel-home.md) | Amazon 판매 채널 홈 페이지와 사용 가능한 옵션 및 작업에 대해 자세히 알아보십시오. Amazon 스토어에 대한 요약 정보를 보고 스토어 세부 정보 및 설정에 액세스할 수 있습니다. |
| [속성 관리](./attributes-view.md) | Amazon sales channel은 [!DNL Commerce] 제품 특성을 사용하는 카탈로그 및 Amazon. 이러한 속성을 만들고, 매핑하고, 관리하는 방법에 대해 자세히 알아보십시오. |
| [스토어 설정 관리](./ob-store-review.md) | 목록 설정, 주문 설정, 목록 및 가격책정 규칙을 포함한 스토어 설정을 조회하고 수정합니다. |
| [목록 관리](./managing-product-listings.md) | Amazon 마켓플레이스를 통해 판매하면서 목록(설정, 규칙 및 가격)을 업데이트, 추가 및 관리할 수 있습니다. 스토어 및 목록 설정 생성 및 수정에 대해 자세히 알아보십시오. |
| [주문 및 이행 관리](./managing-orders.md) | Amazon 판매 채널은 Amazon 및 를 통한 주문 이행 및 납품을 지원합니다. [!DNL Commerce]. Amazon을 통해, 을 통해 직접 구현에 대해 자세히 알아보십시오. [!DNL Commerce]및 order management 옵션. |
| [로그 및 보고서 보기](./amazon-logs-reports.md) | Amazon과 간의 추적된 오류 및 상호 작용에 대해 자세히 알아보십시오. [!DNL Commerce]. |

## 추가 Adobe Commerce 설명서

- [Adobe Commerce 사용 안내서](https://docs.magento.com/user-guide/){target="_blank"}
- [Adobe Commerce 개발자 안내서](https://devdocs.magento.com/){target="_blank"}
