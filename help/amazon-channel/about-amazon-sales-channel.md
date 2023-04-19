---
title: Amazon Sales Channel
description: Amazon 판매 채널 확장을 사용하여 Adobe Commerce 또는 Magento Open Source을 Amazon Seller Central 계정과 원활하게 통합합니다.
exl-id: 11752491-d0da-4ff7-a0a7-d17d4fa1bfc9
source-git-commit: f9ef1b031a1a8a8a4b6c2453d431a6f35155c4ac
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# 정보 [!DNL Amazon Sales Channel]

[!DNL Amazon Sales Channel] 은 Amazon 영업 채널 확장을 제공하여 [!DNL Commerce] 관리자 [!DNL Amazon Seller Central] 계정이 필요합니다. 후 [온보딩](./amazon-onboarding-home.md), [!DNL Commerce] Amazon 스토어에 대한 Amazon 목록, 주문 및 인벤토리, 가격 등을 관리 및 제어할 수 있는 &quot;중앙 관리 센터&quot;가 됩니다.

[스토어 통합](./store-integration.md) 연결 [!DNL Commerce] 두 플랫폼 간에 데이터를 동기화할 인스턴스와 Amazon 입니다. Amazon 영업 채널을 통해 다음을 수행할 수 있습니다.

- [온보드](./amazon-onboarding-home.md) 하나 이상 통합 [!DNL Amazon Seller Central] Adobe Commerce 또는 Magento Open Source을 사용하는 계정.

- 기존 Amazon 목록을 가져와 동기화하고 의 제품에 일치시킵니다 [!DNL Commerce] 카탈로그, 중앙 집중식 제품 카탈로그를 만듭니다.

- 의 제품에 대한 Amazon 목록을 만들고 관리합니다 [!DNL Commerce] 카탈로그

- 주문 조회 및 이행(출하) [!DNL Commerce] 및 Amazon, 주문 상태, 결제 및 환불 정보 동기화

- 분석 및 오류에 대한 로그 보기 [경쟁력 있는 가격](./competitive-price-analysis.md), [변경 사항 나열](./listing-changes-log.md), 및 [통신 문제](./communication-errors-log.md).

Amazon 스토어에 액세스하여 Amazon 판매 채널에서 이러한 모든 기능, 계정 정보, 목록, 주문 등을 보고 관리할 수 있습니다 [홈 페이지](./amazon-sales-channel-home.md).

## 프로모션 및 가격

사용 [!DNL Amazon Sales Channel] 확장을 사용할 수 있는 방법은 다음과 같습니다.

- Amazon 목록 가격표 동기화 [!DNL Commerce] 카탈로그 가격(또는 대체 가격 속성)

- MSRP 활성화 [클릭스루 가격](./listing-price.md#configure-listing-price-settings) Amazon 목록에서 고객 가치 제안을 늘릴 수 있습니다.

- 활성화 및 관리 [최소 광고 가격(MAP)](./listing-price.md#configure-listing-price-settings) 참조하십시오.

- 추가 구성 [부가세](./listing-price.md#configure-listing-price-settings) ( Amazon 가격 책정).

- 에서 &quot;사용 가능한 수량&quot;에 대한 사용자 지정 값을 설정합니다. [스톡/수량 설정](./stock-quantity.md#configure-stock--quantity-settings) 구매자의 긴급성을 높이기 위해 Amazon 목록을 표시합니다.

## 가격 규칙

사용 [!DNL Amazon Sales Channel] 확장을 사용할 수 있는 방법은 다음과 같습니다.

- 스택할 수 있고 유연하며 복잡한 컨텐츠 생성 [가격 규칙](./pricing-products.md) 매일 판매 또는 계절별 판촉에 대한 Amazon 가격을 관리합니다.

- 만들기 [바닥](./floor-price.md) 및 [천장](./optional-ceiling-price.md) 가장 낮은 가격과 가장 높은 가격을 보호하기 위한 가격.

- 만들기 및 관리 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md) 다른 Amazon 경쟁업체와 비교하여 제품 가격을 자동으로 조정합니다([최저 경쟁사](./lowest-competitor-pricing.md) 및 [Buy Box](./buy-box-competitor-pricing.md) 가격).

## 카탈로그 피드 관리

사용 [!DNL Amazon Sales Channel] 확장을 사용할 수 있는 방법은 다음과 같습니다.

- 기존 Amazon 목록(제품)을 가져와서 기존 와 일치시키거나 [!DNL Commerce] 카탈로그

- 게시 [!DNL Commerce] Amazon 목록을 만들기 위한 Amazon 제품 .

- 만들기 [무시](./creating-editing-overrides.md) 개별 가격, 처리 시간, 조건 및 판매자 노트 메시지를 설정하려면

- 제품 가져오기 및 매핑 [속성](./attributes-view.md) Amazon 목록 을 통해 [!DNL Commerce] 카탈로그

- Amazon 목록과 일치하도록 여러 검색 매개 변수를 설정합니다. [!DNL Commerce] 카탈로그

- 정의 [목록 규칙](./listing-rules.md) 어떤 [!DNL Commerce] 제품은 Amazon에 나열될 수 있습니다.

- 기본값 설정 [처리 시간](./product-listing-actions.md) 새 Amazon 목록에 대해 자세히 알아보십시오.

- 조건을 기준으로 목록 조건 일치 [!DNL Commerce] 속성을 사용합니다.

- 각 조건 유형에 대해 판매자 노트를 추가합니다(선택 사항).

- Amazon 목록을 으로 가져올 때 수량 임계값 구현 [!DNL Commerce] 카탈로그

- 권장 보기 [목록 개선 사항](./listing-improvements.md).

## 주문 관리 및 고객 서비스

사용 [!DNL Amazon Sales Channel] 확장을 사용할 수 있는 방법은 다음과 같습니다.

- Amazon 및 의 주문 지원 및 처리 [!DNL Commerce].

- [가져오기](./order-settings.md#configure-order-settings) Amazon이 [!DNL Commerce] 또는 Amazon에 둡니다.

- 원하는 항목을 정의합니다 [!DNL Commerce] 웹 사이트에서는 주문을 가져오고 관리하기 위해 Amazon 주문과 연결하도록 저장합니다.

- 주문 조회, 취소 및 출하 [!DNL Commerce] 및/또는 Amazon에 따라 [이행 설정](./fulfilled-by.md).

- 내에서 Amazon 주문 상태를 사용자 지정 상태에 매핑 [!DNL Commerce] (선택 사항).

- 주문 오류를 보고 관리하여 문제를 해결하고 고객과 연결할 수 있습니다.

- 주문 추적 데이터를 [!DNL Amazon Seller Central] 계정이 필요합니다.

- [주문 취소](./cancel-unshipped-order.md) 및 원인 응답을 선택합니다.

- 보기 [최근 주문](./amazon-store-dashboard.md) Amazon 주문에 대한 정보입니다.

## 보고

사용 [!DNL Amazon Sales Channel] 확장에서는 다음에 대한 보고서 정보를 검토할 수 있습니다.

- 활성, 비활성, 적격 및 불완전 상태의 상태별 목록

- 선적을 기다리는 주문.

- 가장 최근 주문입니다.

- Amazon [변경 사항 로그 나열](./listing-changes-log.md) 피드 변경 사항(예: 가격 및 수량)을 검토하려면

- 제품 [Buy Box](./buy-box-competitor-pricing.md) 경쟁업체 가격 정보.

- 제품 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md) 데이터.

## 글로벌 영업 지원

사용 [!DNL Amazon Sales Channel] 확장을 사용할 수 있는 방법은 다음과 같습니다.

- 여러 관리 [!DNL Amazon Marketplace] 지역(국가).

- 을 사용하여 여러 통화 지원 [[!DNL Commerce] 통화 변환 도구](https://docs.magento.com/user-guide/stores/currency-configuration.html){target="_blank"}.

- 제품 위치 및 Amazon 이행 센터에서 출하를 관리합니다.

## 고객 관리

빌드 [!DNL Commerce] 고객 데이터베이스 [고객 데이터 가져오기](./order-settings.md#configure-order-settings) 을 Amazon 주문과 연관시켰습니다. 다음을 통해 확장된 고객 목록을 통해 마케팅 가능성을 높일 수 있습니다. [!DNL Amazon Marketplace] 목록 [!DNL Commerce] 상점.
