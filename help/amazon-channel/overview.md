---
title: " [!DNL Amazon Sales Channel] 소개"
description: "[!DNL Amazon Sales Channel]을(를) 사용하면 판매자가  [!DNL Amazon Marketplace]에서 제품을 원활하게 판매할 수 있습니다."
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 소개

Adobe Commerce 또는 Magento Open Source 판매자의 경우 [!DNL Amazon Sales Channel] 확장을 사용하여 상점과 세계 최대 규모의 글로벌 인터넷 쇼핑 대상을 통합할 수 있습니다. 이 확장을 사용하면 [!DNL Commerce]을(를) [!DNL Amazon Seller Central] 계정에 연결하고 카탈로그 및 주문 데이터의 자동화 및 동기화를 모두 제공하여 Amazon 판매를 수행할 수 있습니다. 모든 Amazon 목록을 완벽하게 관리하고, 간단하거나 지능적인 가격 책정 규칙을 구현하고, 단일 [!DNL Commerce] 대시보드를 통해 주문 및 인벤토리를 유지 관리합니다.

[온보딩](./amazon-onboarding-home.md) 후 [!DNL Commerce]은(는) Amazon 목록, 주문 및 인벤토리, Amazon 스토어의 가격 책정 등을 관리하고 제어하는 &quot;중앙 명령 센터&quot;가 됩니다. [스토어 통합](./store-integration.md)을 통해 [!DNL Commerce] 인스턴스와 Amazon을 연결하여 두 플랫폼 간에 데이터를 동기화합니다. Amazon sales channel을 통해 다음과 같은 작업을 수행할 수 있습니다.

- [온보딩](./amazon-onboarding-home.md), Adobe Commerce 또는 Magento Open Source과 하나 이상의 [!DNL Amazon Seller Central] 계정을 통합합니다.

- 기존 Amazon 목록을 가져와서 동기화하고 [!DNL Commerce] 카탈로그의 제품에 일치시켜 중앙 집중식 제품 카탈로그를 만듭니다.

- [!DNL Commerce] 카탈로그의 제품에 대한 Amazon 목록을 만들고 관리합니다.

- 주문 상태, 결제 및 환불 정보를 동기화하여 [!DNL Commerce] 및 Amazon에서 주문 조회 및 처리(배송)를 수행합니다.

- [경쟁사 가격](./competitive-price-analysis.md), [변경 내용 나열](./listing-changes-log.md) 및 [통신 문제](./communication-errors-log.md)에 대한 분석 및 오류에 대한 로그를 봅니다.

Amazon 스토어에 액세스하여 Amazon 판매 채널 [홈 페이지](./amazon-sales-channel-home.md)에서 이러한 모든 기능, 계정 정보, 목록, 주문 등을 보고 관리할 수 있습니다.

## 프로모션 및 가격

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- Amazon 목록 가격을 [!DNL Commerce] 카탈로그 가격(또는 대체 가격 특성)에 동기화합니다.

- Amazon 목록에서 MSRP [타격 가격 책정](./listing-price.md#configure-listing-price-settings)을(를) 활성화하여 고객 가치 제안을 높이십시오.

- Amazon 목록에서 [MAP(Minimum Advertised Price)](./listing-price.md#configure-listing-price-settings)을(를) 활성화하고 관리합니다.

- Amazon 가격에서 추가 [VAT 세금](./listing-price.md#configure-listing-price-settings)을(를) 구성합니다.

- [재고/수량 설정](./stock-quantity.md#configure-stock--quantity-settings)에서 &quot;사용 가능한 수량&quot;에 대한 사용자 지정 값을 설정하여 Amazon 목록에 표시하여 구매자 긴급도를 높이십시오.

## 가격 규칙

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 매일 판매하거나 계절별 프로모션을 위한 Amazon 가격을 관리하려면 스택이 가능하고 유연하며 복잡한 [가격 규칙](./pricing-products.md)을 만드십시오.

- 최저가와 최고 가격을 보호하려면 [층](./floor-price.md) 및 [천정](./optional-ceiling-price.md) 가격을 만드세요.

- 다른 Amazon 경쟁사([가장 낮은 경쟁사](./lowest-competitor-pricing.md) 및 [Buy Box](./buy-box-competitor-pricing.md) 가격)와 비교하여 제품 가격을 자동으로 조정하는 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)을(를) 만들고 관리합니다.

## 카탈로그 피드 관리

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 기존 Amazon 목록(제품)을 가져와서 기존 목록과 일치시키거나 [!DNL Commerce] 카탈로그에 제품을 만드십시오.

- Publish 목록을 만들려면 [!DNL Commerce] 제품을 AmazonAmazon 에 게시합니다.

- 개별 가격, 처리 시간, 조건 및 판매자 메모 메시지를 설정하려면 [overrides](./creating-editing-overrides.md)를 만드십시오.

- Amazon 목록에서 [특성](./attributes-view.md)을(를) 가져와서 매핑하면 [!DNL Commerce] 카탈로그의 제품과 자동으로 일치합니다.

- Amazon 목록을 [!DNL Commerce] 카탈로그와 일치시키려면 여러 검색 매개 변수를 설정하십시오.

- [목록 규칙](./listing-rules.md)을(를) 정의하여 [!DNL Commerce] 제품 중 어떤 제품이 Amazon에 나열될 수 있는지 결정합니다.

- 새 Amazon 목록의 기본 [처리 시간](./product-listing-actions.md)을 설정합니다.

- [!DNL Commerce] 특성을 기준으로 목록 조건을 일치시키십시오.

- 각 조건 유형에 대해 판매자 노트를 추가합니다(선택 사항).

- Amazon 목록을 [!DNL Commerce] 카탈로그로 가져올 때 수량 임계값을 구현합니다.

- 권장 [목록 개선 사항](./listing-improvements.md)을 봅니다.

## Order Management 및 고객 서비스

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- Amazon 및 [!DNL Commerce]에서 주문을 지원하고 처리합니다.

- Amazon 주문을 [가져오거나](./order-settings.md#configure-order-settings) [!DNL Commerce](으)로 가져오거나 Amazon에 남깁니다.

- 주문 가져오기 및 관리를 위해 Amazon 주문과 연결할 [!DNL Commerce] 웹 사이트 스토어를 정의합니다.

- [이행 설정](./fulfilled-by.md)에 따라 [!DNL Commerce] 및/또는 Amazon에서 주문을 보고, 취소하고, 배송합니다.

- [!DNL Commerce] 내의 사용자 지정 상태에 Amazon 주문 상태를 매핑합니다(선택 사항).

- 주문 오류를 보고 관리하여 문제를 해결하고 고객과 연결합니다.

- 주문 추적 데이터를 [!DNL Amazon Seller Central] 계정에 보냅니다.

- [주문 취소](./cancel-unshipped-order.md) 및 이유 응답을 선택하십시오.

- Amazon 주문에 대한 [최근 주문](./amazon-store-dashboard.md) 정보를 봅니다.

## 보고

[!DNL Amazon Sales Channel] 확장을 사용하면 다음에 대한 보고서 정보를 검토할 수 있습니다.

- 활성, 비활성, 적격 및 미완료 상태별 목록.

- 선적 대기 중인 주문.

- 가장 최근 주문입니다.

- 제품/목록 피드 변경 사항(예: 가격 및 수량)을 검토하기 위해 Amazon [목록 변경 사항 로그](./listing-changes-log.md).

- 제품 [Buy Box](./buy-box-competitor-pricing.md) 경쟁업체 가격 데이터입니다.

- 제품 [경쟁업체 최저 가격](./lowest-competitor-pricing.md) 데이터.

## 글로벌 영업 지원

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 여러 [!DNL Amazon Marketplace] 지역(국가)을 관리합니다.

- [Commerce 통화 구성 도구](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html)를 사용하여 여러 통화를 지원합니다.

- 제품 위치 및 Amazon 이행 센터에서 발송을 관리합니다.

## 고객 관리

Amazon 주문과 연결된 [고객 데이터를 가져오기](./order-settings.md#configure-order-settings)하여 [!DNL Commerce] 고객 데이터베이스를 빌드합니다. [!DNL Amazon Marketplace] 목록 및 [!DNL Commerce] 상점을 통해 확장된 고객 목록을 통해 마케팅 잠재력을 높이십시오.


시작하는 것은 쉽습니다. 짧은 온보딩 프로세스를 통해 [!DNL Amazon Seller Central] 계정을 만들고 Amazon 판매 채널 스토어 및 [!DNL Commerce] 카탈로그와 통합하여 Amazon 목록, 주문, 인벤토리 및 이행을 관리할 수 있습니다. 중앙 대시보드에는 모든 Amazon 판매 채널 스토어 통합 및 Amazon 목록에 대한 상태 업데이트가 표시됩니다. 간소화된 자동화된 프로세스를 통해 글로벌 [!DNL Amazon Marketplace]의 새로운 고객에게 도달하십시오. 새로운 시스템을 설정하는 데 드는 비용과 수고를 조금도 줄이십시오.

[!DNL Amazon Seller Central] 계정을 통합한 후 [!DNL Amazon Sales Channel] 확장을 사용하면 계정을 관리하고 [!DNL Commerce]과(와) Amazon 간에 데이터를 동기화할 수 있습니다. [!DNL Commerce] 관리자를 통해 목록을 만들고, 프로모션을 관리하고, 가격을 설정하고, 인벤토리 및 이행 상태를 직접 관리할 수 있습니다. 이러한 옵션에는 동일한 품목에 대한 Amazon 가격을 모니터링하고 가격을 자동으로 조정하여 보다 경쟁력있게 조정하는 가격 책정 규칙이 포함됩니다.

