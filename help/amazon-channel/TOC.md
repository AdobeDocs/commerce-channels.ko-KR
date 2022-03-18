---
user-guide-title: Amazon Sales Channel 사용 안내서
user-guide-description: Adobe Commerce 또는 Magento Open Source을 와 통합하여 Amazon을 통해 판매 생성 [!DNL Amazon Seller Central] 계정이 필요합니다.
breadcrumb-title: Amazon Sales Channel
source-git-commit: e20e377fdef565ca526e6f67cca126c36b450e75
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 2%

---


# Amazon 영업 채널 - [!DNL channel manager] Adobe Commerce {#amazon}

- [안내서 개요](guide-overview.md)
- [Amazon 영업 채널 소개](overview.md)
- [릴리스 노트](release-notes.md)
- 시작하기 {#getting-started}
   - [Amazon 판매 채널 기본 정보](about-amazon-sales-channel.md)
   - [Amazon Marketplace에 대하여](about-amazon-marketplace.md)
   - [Amazon 및 전자 상거래 카탈로그 정보](about-listings-and-catalog.md)
   - [우수 사례 및 제한 사항](amazon-best-practices.md)
   - [확장 설치](install.md)
- 온보딩 {#onboarding}
   - [온보드 Amazon 영업 채널](amazon-onboarding-home.md)
   - [사전 설정 작업](amazon-pre-setup-tasks.md)
   - [만들기 [!DNL Commerce] Amazon 속성](ob-creating-magento-attributes.md)
   - [Amazon API 키 확인](amazon-verify-api-key.md)
   - [스토어 통합](store-integration.md)
   - [목록 규칙 만들기](ob-create-listing-rule.md)
   - [기본 저장소 설정](default-store-settings.md)
- 영업 채널 관리 {#manage}
   - [홈 페이지](amazon-sales-channel-home.md)
   - [Amazon 스토어](managing-stores.md)
   - [작업 공간 컨트롤](workspace-controls.md)
   - [학습 및 준비](learning-preparation.md)
   - 속성 {#attributes}
      - [속성 보기](attributes-view.md)
      - [속성 관리](managing-attributes.md)
      - [속성 만들기 및 편집](creating-attributes.md)
      - [속성 매핑 보기](amazon-matching-attributes-values.md)
   - [영업 채널 관리 설정](sales-channel-settings.md)
   - [Amazon 스토어 대시보드](amazon-store-dashboard.md)
   - [스토어 설정](ob-store-review.md)
- 목록 설정 {#listing-settings}
   - [목록 설정 보기](listing-settings.md)
   - [제품 목록 작업](product-listing-actions.md)
   - [타사 목록](third-party-listing-settings.md)
   - [목록 가격](listing-price.md)
   - [(B2B) 비즈니스 가격 책정](business-pricing.md)
   - [주식/수량](stock-quantity.md)
   - [다음 기간 동안 이행](fulfilled-by.md)
   - [카탈로그 검색](catalog-search.md)
   - [제품 목록 조건](product-listing-condition.md)
   - [갱신된 제품](renewed-products.md)
- [순서 설정](order-settings.md)
- [저장 통합 설정](store-integration-settings.md)
- 목록 및 가격책정 규칙 {#rules}
   - [목록 규칙](listing-rules.md)
   - 가격책정 규칙 {#pricing-rules}
      - [가격 관리](pricing-products.md)
      - [새 가격 규칙 추가](add-pricing-rule.md)
      - [가격 규칙 일반 설정](pricing-rule-general-settings.md)
      - [가격 규칙 조건](pricing-rule-conditions.md)
      - [가격 규칙 작업](pricing-rule-actions.md)
      - [표준 가격 규칙](standard-price-rules.md)
      - [지능형 가격 조정 규칙](intelligent-repricing-rules.md)
      - [경쟁업체 조건부 분산](competitor-conditional-variances.md)
      - [가격 조정](price-adjustment.md)
      - [가격](floor-price.md)
      - [가격(옵션)](optional-ceiling-price.md)
      - [가격 범위](price-scope.md)
      - [가격 우선순위 논리](price-priority-logic.md)
      - [Buy Box 경쟁업체 가격 책정](buy-box-competitor-pricing.md)
      - [가장 낮은 경쟁업체 가격](lowest-competitor-pricing.md)
   - 예 {#rules-examples}
      - [조건 정의](ob-define-condition-example.md)
      - [가격 규칙 예](price-rule-examples.md)
- 보고서 및 로그 {#reports-logs}
   - [보고서 로그 및 저장](amazon-logs-reports.md)
   - 보고서 저장 {#store-reports}
      - [경쟁력 분석](competitive-price-analysis.md)
      - [목록 개선 사항](listing-improvements.md)
   - 로그 {#logs}
      - [변경 내용 로그 나열](listing-changes-log.md)
      - [통신 오류 로그](communication-errors-log.md)
- 목록 관리 {#admin-listings}
   - [Amazon 목록 관리](managing-product-listings.md)
   - 상태/탭별 {#status-tab}
      - [상태/탭별 관리](managing-listings-by-tab.md)
      - [불완전한 목록](incomplete-listings.md)
      - [새 타사 목록](new-third-party-listings.md)
      - [목록 준비 완료](ready-to-list.md)
      - [비활성 목록](inactive-listings.md)
      - [활성 목록](active-listings.md)
      - [무시](overrides.md)
      - [부적격 목록](ineligible-listings.md)
      - [종료 목록](ended-listings.md)
   - 작업 기준 {#actions}
      - [작업별 관리](managing-listings-by-action.md)
      - [카탈로그 제품 만들기 및 할당](creating-assigning-catalog-products.md)
      - [무시 만들기 및 편집](creating-editing-overrides.md)
      - [별칭 판매자 SKU 만들기](create-alias-seller-sku.md)
      - [할당된 ASIN 편집](edit-assigned-asin.md)
      - [Amazon 목록 종료](end-listings-manually.md)
      - [Amazon 목록 게시](publish-listings-manually.md)
      - [업데이트 필수 정보](amazon-manually-update-incomplete-listing.md)
      - [세부 사항 보기](product-listing-details.md)
- 주문 관리 {#admin-orders}
   - [주문 관리](managing-orders.md)
   - [Amazon 주문 보기](amazon-orders-all.md)
   - [Amazon 주문 세부 사항 보기](amazon-order-details.md)
   - [일반적인 주문 처리 작업](common-order-processing.md)
   - [이행 워크플로우](fulfillment-workflows.md)
   - [미출하 주문 취소](cancel-unshipped-order.md)
