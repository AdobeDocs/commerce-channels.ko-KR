---
title: "소개 [!DNL Amazon Sales Channel]"
description: "[!DNL Amazon Sales Channel] 상인이 제품에서 원활하게 판매할 수 있도록 합니다. [!DNL Amazon Marketplace]."
redirect_from: /sales-channels/amazon/amazon-sales-channel.html
role: Admin, User, Leader
exl-id: a4a6f446-7029-4c92-bce3-5b857cc33056
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# 소개 [!DNL Amazon Sales Channel]

Adobe Commerce 또는 Magento Open Source 판매자는 [!DNL Amazon Sales Channel] 세계 최대의 글로벌 인터넷 쇼핑 목적지와 매장을 통합하는 확장. 이 확장 기능을 통해 다음을 연결하여 Amazon 판매 가능 [!DNL Commerce] (으)로 [!DNL Amazon Seller Central] 카탈로그 및 주문 데이터의 자동화 및 동기화를 모두 제공하는 계정. 모든 Amazon 목록을 완벽하게 관리하고, 단순하거나 지능적인 가격 규칙을 구현하며, 단일 솔루션을 통해 주문 및 재고를 유지 관리할 수 있습니다. [!DNL Commerce] 대시보드입니다.

다음 이후 [온보딩](./amazon-onboarding-home.md), [!DNL Commerce] 는 Amazon 스토어의 Amazon 목록, 주문 및 재고, 가격을 관리 및 제어하는 &quot;중앙 관리 센터&quot;가 됩니다. [스토어 통합](./store-integration.md) 다음 연결: [!DNL Commerce] 인스턴스와 Amazon을 사용하여 두 플랫폼 간에 데이터를 동기화할 수 있습니다. Amazon sales channel을 통해 다음과 같은 작업을 수행할 수 있습니다.

- [온보드](./amazon-onboarding-home.md) 하나 이상 통합 [!DNL Amazon Seller Central] Adobe Commerce 또는 Magento Open Source을 사용하는 계정.

- 기존 Amazon 목록을 가져와서 동기화하고 [!DNL Commerce] 카탈로그, 중앙 집중식 제품 카탈로그 만들기

- 의 제품에 대한 Amazon 목록 만들기 및 관리 [!DNL Commerce] 카탈로그.

- 주문 조회 및 이행(출하) [!DNL Commerce] 및 Amazon, 주문 상태, 결제 및 환불 정보를 동기화합니다.

- 분석 로그 및 오류 보기 [경쟁 가격](./competitive-price-analysis.md), [변경 내용 나열](./listing-changes-log.md), 및 [커뮤니케이션 문제](./communication-errors-log.md).

Amazon 스토어에 액세스하여 Amazon 판매 채널에서 이러한 모든 기능, 계정 정보, 목록, 주문 등을 보고 관리합니다 [홈 페이지](./amazon-sales-channel-home.md).

## 프로모션 및 가격

포함 [!DNL Amazon Sales Channel] 확장 기능을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

- 가격 책정 대상 Amazon 동기화 [!DNL Commerce] 카탈로그 가격(또는 대체 가격 속성).

- MSRP 사용 [특별 할인 가격](./listing-price.md#configure-listing-price-settings) Amazon 을 참조하십시오.

- 활성화 및 관리 [최소 광고 가격(MAP)](./listing-price.md#configure-listing-price-settings) Amazon 목록에서 참조할 수 있습니다.

- 추가 구성 [부가세](./listing-price.md#configure-listing-price-settings) Amazon 가격에서.

- 에서 &quot;사용 가능한 수량&quot;에 대한 사용자 지정 값 설정 [재고 / 수량 설정](./stock-quantity.md#configure-stock--quantity-settings) Amazon 목록을 표시하여 구매자 긴급도를 높일 수 있습니다.

## 가격 규칙

포함 [!DNL Amazon Sales Channel] 확장 기능을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

- 스택이 가능하고 유연하며 복잡한 환경 조성 [가격 규칙](./pricing-products.md) 일상적인 판매 또는 시즌 프로모션에 대한 Amazon 가격을 관리하십시오.

- 만들기 [floor](./floor-price.md) 및 [천장](./optional-ceiling-price.md) 최저 및 최고 가격을 보호하기 위한 가격.

- 만들기 및 관리 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md) 다른 Amazon 경쟁업체와 비교하여 제품 가격을 자동으로 조정([가장 낮은 경쟁자](./lowest-competitor-pricing.md) 및 [Buy Box](./buy-box-competitor-pricing.md) 가격).

## 카탈로그 피드 관리

포함 [!DNL Amazon Sales Channel] 확장 기능을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

- 기존 Amazon 목록(제품)을 가져와서 기존 목록에 일치시키거나 [!DNL Commerce] 카탈로그.

- 게시 [!DNL Commerce] Amazon 목록을 만들기 위해 Amazon에 제품을 보냅니다.

- 만들기 [재정의](./creating-editing-overrides.md) 개별 가격, 처리 시간, 조건 및 판매자 메모 메시지를 설정할 수 있습니다.

- 제품 가져오기 및 매핑 [속성](./attributes-view.md) 과(와) 의 제품이 자동으로 일치하도록 Amazon 목록에서 [!DNL Commerce] 카탈로그.

- 여러 검색 매개 변수를 설정하여 Amazon 목록을 [!DNL Commerce] 카탈로그.

- 정의 [규칙 나열](./listing-rules.md) 을(를) 확인하여 [!DNL Commerce] 제품은 Amazon에 나열될 수 있습니다.

- 기본값 설정 [처리 시간](./product-listing-actions.md) 새 Amazon 목록.

- 다음을 기준으로 목록 조건 일치 [!DNL Commerce] 특성.

- 각 조건 유형에 대해 판매자 노트를 추가합니다(선택 사항).

- Amazon 목록을 로 가져올 때 수량 임계값 구현 [!DNL Commerce] 카탈로그.

- 권장 사항 보기 [목록 개선 사항](./listing-improvements.md).

## Order Management 및 고객 서비스

포함 [!DNL Amazon Sales Channel] 확장 기능을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

- Amazon 및 의 지원 및 처리 주문 [!DNL Commerce].

- [가져오기](./order-settings.md#configure-order-settings) 내 Amazon 주문 [!DNL Commerce] 아니면 Amazon에 두십시오.

- 다음 중 하나를 정의합니다. [!DNL Commerce] 주문 가져오기 및 관리를 위해 Amazon 주문과 연결할 웹 사이트 스토어.

- 주문 조회, 취소 및 출하 출처 [!DNL Commerce] 및/또는 다음에 따라 Amazon [이행 설정](./fulfilled-by.md).

- 내에서 Amazon 주문 상태를 사용자 정의 상태에 매핑 [!DNL Commerce] (선택 사항).

- 주문 오류를 보고 관리하여 문제를 해결하고 고객과 연결합니다.

- 주문 추적 데이터를 다음으로 전송 [!DNL Amazon Seller Central] 계정입니다.

- [주문 취소](./cancel-unshipped-order.md) 사유 응답을 선택합니다.

- 보기 [최근 주문](./amazon-store-dashboard.md) Amazon 주문에 대한 정보입니다.

## 보고

포함 [!DNL Amazon Sales Channel] 확장에서는 다음에 대한 보고서 정보를 검토할 수 있습니다.

- 활성, 비활성, 적격 및 미완료 상태별 목록.

- 선적 대기 중인 주문.

- 가장 최근 주문입니다.

- Amazon [변경 로그 나열](./listing-changes-log.md) 제품/목록 피드 변경 사항(예: 가격 및 수량)을 검토하려면

- 제품 [Buy Box](./buy-box-competitor-pricing.md) 경쟁업체 가격 데이터.

- 제품 [경쟁사 최저 가격](./lowest-competitor-pricing.md) 데이터.

## 글로벌 영업 지원

포함 [!DNL Amazon Sales Channel] 확장 기능을 사용하여 다음과 같은 작업을 수행할 수 있습니다.

- 다중 관리 [!DNL Amazon Marketplace] 지역(국가).

- 다음을 사용하여 여러 통화 지원 [상거래 통화 구성 도구](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-configuration.html).

- 제품 위치 및 Amazon 이행 센터에서 발송을 관리합니다.

## 고객 관리

빌드 [!DNL Commerce] 고객 데이터베이스 기준 [고객 데이터 가져오기](./order-settings.md#configure-order-settings) Amazon 주문과 연계되었습니다. 다음을 통해 확장된 고객 목록을 통해 마케팅 잠재력을 키우십시오. [!DNL Amazon Marketplace] 목록 및 [!DNL Commerce] 가게 앞이야


시작하는 것은 쉽습니다. 짧은 온보딩 프로세스를 통해 [!DNL Amazon Seller Central] 계정 및 Amazon sales channel 스토어 및 [!DNL Commerce] 카탈로그로 Amazon 목록, 주문, 재고 및 이행을 관리합니다. 중앙 대시보드에는 모든 Amazon 판매 채널 스토어 통합 및 Amazon 목록에 대한 상태 업데이트가 표시됩니다. 전 세계의 새로운 고객에게 도달 [!DNL Amazon Marketplace] 단순화되고 자동화된 프로세스를 통해 새로운 시스템을 구축하는 데 드는 비용과 수고를 거의 또는 전혀 최소화할 수 있습니다.

통합 후 [!DNL Amazon Seller Central] 계정, [!DNL Amazon Sales Channel] 확장을 사용하면 계정을 관리하고 다음 간 데이터를 동기화할 수 있습니다. [!DNL Commerce] 그리고 Amazon. 목록을 만들고, 프로모션을 관리하고, 가격을 설정하고, 인벤토리와 이행을 직접 관리할 수 있습니다. [!DNL Commerce] 관리자. 이러한 옵션에는 동일한 품목에 대한 Amazon 가격을 모니터링하고 가격을 자동으로 조정하여 보다 경쟁력있게 조정하는 가격 책정 규칙이 포함됩니다.

