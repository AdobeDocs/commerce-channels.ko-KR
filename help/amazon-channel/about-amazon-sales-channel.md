---
title: Amazon 판매 채널 기본 정보
description: Amazon 판매 채널 확장을 사용하여 Adobe 상거래 또는 Magento Open Source을 Amazon Seller Central 계정과 원활하게 통합합니다.
exl-id: 11752491-d0da-4ff7-a0a7-d17d4fa1bfc9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Amazon 판매 채널 정보

Adobe 상거래를 위한 채널 관리자는 Amazon 영업 채널 확장을 제공하여 [!DNL Commerce] 관리자를 [!DNL Amazon Seller Central] 계정과 원활하게 통합합니다. [온보딩](./amazon-onboarding-home.md) 후 [!DNL Commerce]은(는) Amazon 스토어에 대한 Amazon 목록, 주문 및 인벤토리, 가격 책정 등을 관리하고 제어하기 위한 &quot;중앙 명령 센터&quot;가 됩니다.

[스토어 ](./store-integration.md) 통합은 인스턴스 [!DNL Commerce] 와 Amazon을 연결하여 두 플랫폼 간에 데이터를 동기화합니다. Amazon 영업 채널을 통해 다음을 수행할 수 있습니다.

- [](./amazon-onboarding-home.md) Adobe 상거래 또는 Magento Open Source에서 하나 이상의  [!DNL Amazon Seller Central] 계정을 온보딩하고 하나 이상의 계정을 통합합니다.

- 기존 Amazon 목록을 가져오고 동기화하고 [!DNL Commerce] 카탈로그의 제품에 일치시켜 중앙 집중식 제품 카탈로그를 만듭니다.

- [!DNL Commerce] 카탈로그에서 제품에 대한 Amazon 목록을 만들고 관리합니다.

- [!DNL Commerce] 및 Amazon에서 주문 조회 및 이행(출하), 주문 상태, 결제 및 환불 정보를 동기화합니다.

- [경쟁 가격](./competitive-price-analysis.md), [변경 사항 나열](./listing-changes-log.md) 및 [통신 문제](./communication-errors-log.md)에 대한 분석 및 오류에 대한 로그를 봅니다.

Amazon 스토어에 액세스하여 Amazon 판매 채널 [홈 페이지](./amazon-sales-channel-home.md)에서 이러한 모든 기능, 계정 정보, 목록, 주문 등을 보고 관리할 수 있습니다.

## 프로모션 및 가격

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 가격 목록을 [!DNL Commerce] 카탈로그 가격(또는 대체 가격 속성)으로 동기화합니다.

- Amazon 목록에서 MSRP [Strike-through pricing](./listing-price.md#configure-listing-price-settings)을 활성화하여 고객 가치 제안을 늘립니다.

- Amazon 목록에서 [최소 광고 가격(MAP)](./listing-price.md#configure-listing-price-settings)을 활성화하고 관리합니다.

- Amazon 가격에서 추가 [VAT 세금](./listing-price.md#configure-listing-price-settings)을 구성합니다.

- Amazon 목록과 함께 표시하려면 [재고/수량 설정](./stock-quantity.md#configure-stock--quantity-settings)에서 &quot;사용 가능한 수량&quot;에 대한 사용자 지정 값을 설정하여 구매자 긴급성을 높입니다.

## 가격 규칙

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 스택할 수 있고 유연하며 복잡한 [가격 책정 규칙](./pricing-products.md)을 만들어 매일의 판매 또는 계절별 판촉에 대한 Amazon 가격을 관리합니다.

- [floor](./floor-price.md) 및 [ceiling](./optional-ceiling-price.md) 가격을 만들어 가장 저렴하고 높은 가격을 보호합니다.

- 다른 Amazon 경쟁업체와 비교하여 제품 가격을 자동으로 조정하는 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)을 만들고 관리합니다([가장 낮은 경쟁업체](./lowest-competitor-pricing.md) 및 [Buy Box](./buy-box-competitor-pricing.md) 가격).

## 카탈로그 피드 관리

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 기존 Amazon 목록(제품)을 가져와서 기존 와 일치시키거나 [!DNL Commerce] 카탈로그에서 제품을 만듭니다.

- Amazon에 [!DNL Commerce] 제품을 게시하여 Amazon 목록을 만듭니다.

- [을(를) 만들어 개별 가격, 처리 시간, 조건 및 판매자 메모 메시지를 설정합니다.](./creating-editing-overrides.md)

- Amazon 목록에서 제품 [속성](./attributes-view.md)을 가져와 매핑하여 [!DNL Commerce] 카탈로그의 제품과 자동으로 일치시킵니다.

- Amazon 목록을 [!DNL Commerce] 카탈로그에 일치시키려면 여러 검색 매개 변수를 설정합니다.

- [목록 규칙](./listing-rules.md)을 정의하여 Amazon에 나열할 수 있는 [!DNL Commerce] 제품을 결정할 수 있습니다.

- 새 Amazon 목록에 대한 기본 [처리 시간](./product-listing-actions.md)을 설정합니다.

- [!DNL Commerce] 속성을 기준으로 목록 조건을 일치시킵니다.

- 각 조건 유형에 대해 판매자 노트를 추가합니다(선택 사항).

- Amazon 목록을 [!DNL Commerce] 카탈로그로 가져올 때 수량 임계값을 구현합니다.

- 권장 [목록 개선 사항](./listing-improvements.md)을 봅니다.

## 주문 관리 및 고객 서비스

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- Amazon 및 [!DNL Commerce]에서 주문을 지원 및 처리합니다.

- [](./order-settings.md#configure-order-settings) Amazon 주문 [!DNL Commerce] 을 Amazon에 가져오거나 둡니다.

- 주문을 가져오고 관리하기 위해 Amazon 주문과 연결할 [!DNL Commerce] 웹 사이트 저장소 중 하나를 정의합니다.

- [이행 설정](./fulfilled-by.md)에 따라 [!DNL Commerce] 및/또는 Amazon에서 주문을 보고, 취소하고 출하합니다.

- Amazon 주문 상태를 [!DNL Commerce] 내의 사용자 지정 상태에 매핑합니다(선택 사항).

- 주문 오류를 보고 관리하여 문제를 해결하고 고객과 연결할 수 있습니다.

- 주문 추적 데이터를 [!DNL Amazon Seller Central] 계정에 보냅니다.

- [주문 취소 ](./cancel-unshipped-order.md) 및 사유 응답을 선택합니다.

- Amazon 주문에 대한 [최근 주문](./amazon-store-dashboard.md) 정보를 봅니다.

## 보고

[!DNL Amazon Sales Channel] 확장을 사용하면 다음에 대한 보고서 정보를 검토할 수 있습니다.

- 활성, 비활성, 적격 및 불완전 상태의 상태별 목록

- 선적을 기다리는 주문.

- 가장 최근 주문입니다.

- Amazon [listing changes log](./listing-changes-log.md)를 입력하여 제품/목록 피드 변경 사항(예: 가격 및 수량)을 검토합니다.

- 제품 [Buy Box](./buy-box-competitor-pricing.md) 경쟁업체 가격 책정 데이터.

- 제품 [가장 낮은 경쟁업체 가격 ](./lowest-competitor-pricing.md) 데이터.

## 글로벌 영업 지원

[!DNL Amazon Sales Channel] 확장을 사용하면 다음 작업을 수행할 수 있습니다.

- 여러 [!DNL Amazon Marketplace] 지역(국가)을 관리합니다.

- [[!DNL Commerce] 통화 변환 도구](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;}를 사용하여 여러 통화를 지원합니다.

- 제품 위치 및 Amazon 이행 센터에서 출하를 관리합니다.

## 고객 관리

Amazon 주문과 연결된 고객 데이터](./order-settings.md#configure-order-settings)를 가져오기 통해 [!DNL Commerce] 고객 데이터베이스를 구축합니다. [ [!DNL Amazon Marketplace] 목록 및 [!DNL Commerce] 스토어를 통해 이 확장된 고객 목록을 통해 마케팅 가능성을 높일 수 있습니다.
