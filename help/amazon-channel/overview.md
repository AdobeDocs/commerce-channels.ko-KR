---
title: '[!DNL Amazon Sales Channel] 사용 안내서'
description: '[!DNL Channel manager] for Adobe Commerce provides the Amazon sales channel extension to enable merchants to seamlessly sell products in the [!DNL Amazon Marketplace].'
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 55e3376f3a1462446cb27a7f0d926202c7542334
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 사용 안내서

[!DNL Channel manager] Adobe Commerce용 Commerce는 판매자가 Amazon Marketplace에서 제품을 원활하게 판매할 수 있도록 Amazon 판매 채널 확장을 제공합니다.

Adobe 상거래 또는 Magento Open Source 매상인 경우 [!DNL Amazon Sales Channel] 확장 프로그램을 사용하여 스토어를 세계에서 가장 큰 글로벌 인터넷 쇼핑 대상과 통합할 수 있습니다. 이 확장을 사용하면 [!DNL Commerce]을(를) [!DNL Amazon Seller Central] 계정과 연결하고 카탈로그 및 주문 데이터의 자동화 및 동기화를 모두 제공하여 Amazon 매출을 활성화할 수 있습니다. 모든 Amazon 목록을 완벽하게 관리하고, 단순 또는 지능형 가격 규칙을 구현하며, 단일 [!DNL Commerce] 대시보드를 통해 주문 및 인벤토리를 유지 관리합니다.

시작하는 것은 쉽습니다. 짧은 온보딩 프로세스는 [!DNL Amazon Seller Central] 계정을 만들고 Amazon 판매 채널 저장소 및 [!DNL Commerce] 카탈로그와 통합하여 Amazon 목록, 주문, 재고 및 이행을 관리하는 방법을 안내합니다. 중앙 대시보드에는 모든 Amazon 판매 채널 저장소 통합 및 Amazon 목록에 대한 상태 업데이트가 표시됩니다. 새로운 시스템을 설정하는 데 드는 비용과 노고에 상관없이 글로벌 [!DNL Amazon Marketplace] 의 신규 고객에게 도달할 수 있습니다.

[!DNL Amazon Seller Central] 계정을 통합한 후 [!DNL Amazon Sales Channel] 확장을 사용하여 계정을 관리하고 [!DNL Commerce] 와 Amazon 간에 데이터를 동기화할 수 있습니다. 이 기능을 사용하면 [!DNL Commerce] 관리자를 통해 목록을 만들고, 판촉을 관리하고, 가격을 설정하고, 재고 및 이행을 직접 관리할 수 있습니다. 이러한 옵션에는 동일한 항목에 대한 Amazon 가격을 모니터링하고 보다 경쟁력 있게 가격을 자동으로 조정하는 가격 규칙이 포함됩니다.

## 안내서 개요

이 안내서에서는 Amazon 판매 채널 설정을 위한 요구 사항인 몇 가지 기본 [!DNL Amazon Seller Central] 정보를 검토합니다. 또한 온보딩 및 통합 프로세스, 사용 가능한 스토어, 제품, 가격 및 기타 옵션, Amazon 판매 채널을 사용하여 [!DNL Amazon Marketplace]에서 목록 및 매출을 관리하는 방법에 대한 세부 정보도 포함되어 있습니다. 왼쪽 레일을 사용하여 다양한 기능을 탐색하고 세부 정보 및 절차에 액세스할 수 있습니다.

| 영역 | 설명 |
|----|----|
| [Amazon 판매 채널 기본 정보](./about-amazon-sales-channel.md) | Amazon 영업 채널의 기본 사항, 주요 기능, 모범 사례 등에 대해 자세히 알아보십시오. |
| [온보드 Amazon 영업 채널](./amazon-onboarding-home.md) | Amazon 스토어를 신속하게 만들고 [!DNL Amazon Seller Central]과 통합합니다. Amazon 판매 채널을 가동하고 판매 시작 모드로 전환하십시오. |
| [Amazon 영업 채널 홈](./amazon-sales-channel-home.md) | Amazon 판매 채널 홈 페이지와 사용 가능한 옵션 및 작업에 대해 자세히 알아보십시오. Amazon 저장소에 대한 요약 정보를 보고 저장소 세부 사항 및 설정에 액세스할 수 있습니다. |
| [속성 관리](./attributes-view.md) | Amazon 판매 채널은 제품 특성을 사용하여 [!DNL Commerce] 카탈로그와 Amazon 사이에 제품을 매핑합니다. 이러한 속성을 만들고, 매핑하고, 관리하는 방법에 대해 자세히 알아봅니다. |
| [저장소 설정 관리](./ob-store-review.md) | 목록 설정, 주문 설정, 목록 및 가격 규칙을 포함하여 저장소 설정을 보고 수정합니다. |
| [목록 관리](./managing-product-listings.md) | Amazon Marketplace를 통해 판매할 때 목록(설정, 규칙 및 가격)을 업데이트, 추가 및 관리할 수 있습니다. 저장소 및 목록 설정을 만들고 수정하는 방법에 대해 자세히 알아보십시오. |
| [주문 및 이행 관리](./managing-orders.md) | Amazon 판매 채널은 Amazon 및 [!DNL Commerce]을 통한 주문 이행 및 선적을 지원합니다. [!DNL Commerce] 및 Order Management 옵션을 통해 직접 Amazon을 통해 충족시키는 방법에 대해 자세히 알아보십시오. |
| [로그 및 보고서 보기](./amazon-logs-reports.md) | Amazon과 [!DNL Commerce] 간의 추적된 오류 및 상호 작용에 대해 자세히 알아보십시오. |

## 추가 Adobe 상거래 설명서

- [Adobe 상거래 사용 안내서](https://docs.magento.com/user-guide/){:target=&quot;_blank&quot;}
- [Adobe 상거래 개발자 안내서](https://devdocs.magento.com/){:target=&quot;_blank&quot;}
