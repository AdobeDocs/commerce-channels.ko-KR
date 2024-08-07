---
user-guide-title: Amazon Sales Channel 사용 안내서
user-guide-description: Adobe Commerce 또는 Magento Open Source을  [!DNL Amazon Seller Central]  계정과 통합하여 Amazon을 통해 매출을 생성합니다.
breadcrumb-title: Amazon Sales Channel
role: Admin, User
feature: Sales Channels
recommendations: noDisplay
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 4%

---


# Amazon 판매 채널 - Adobe Commerce용 [!DNL channel manager] {#amazon}

- [Amazon Sales Channel 사용 안내서](guide-overview.md)
- [Amazon 판매 채널 소개](overview.md)
- {#getting-started} 시작
   - [Amazon Marketplace 정보](about-amazon-marketplace.md)
   - [Amazon 및 Commerce 카탈로그](about-listings-and-catalog.md)
   - [우수 사례 및 제한 사항](amazon-best-practices.md)
   - [확장 설치](install.md)
- {#onboarding} 온보딩
   - [Amazon 판매 채널 온보드](amazon-onboarding-home.md)
   - [사전 설정 작업](amazon-pre-setup-tasks.md)
   - [Amazon용  [!DNL Commerce] 특성 만들기](ob-creating-magento-attributes.md)
   - [Amazon API 키 확인](amazon-verify-api-key.md)
   - [스토어 통합](store-integration.md)
   - [목록 규칙 만들기](ob-create-listing-rule.md)
   - [기본 저장소 설정](default-store-settings.md)
- 영업 채널 {#manage} 관리
   - [홈 페이지](amazon-sales-channel-home.md)
   - [Amazon 스토어](managing-stores.md)
   - [Workspace 컨트롤](workspace-controls.md)
   - [학습 및 준비](learning-preparation.md)
   - 특성 {#attributes}
      - [속성 보기](attributes-view.md)
      - [속성 관리](managing-attributes.md)
      - [속성 만들기 및 편집](creating-attributes.md)
      - [속성 매핑 보기](amazon-matching-attributes-values.md)
   - [판매 채널 관리자 설정](sales-channel-settings.md)
   - [Amazon 스토어 대시보드](amazon-store-dashboard.md)
   - [스토어 설정](ob-store-review.md)
- 설정 {#listing-settings} 나열 중
   - [목록 설정 보기](listing-settings.md)
   - [제품 목록 작업](product-listing-actions.md)
   - [서드파티 목록](third-party-listing-settings.md)
   - [목록 가격](listing-price.md)
   - [(B2B) 비즈니스 가격 책정](business-pricing.md)
   - [재고/수량](stock-quantity.md)
   - [이행한 사람](fulfilled-by.md)
   - [카탈로그 검색](catalog-search.md)
   - [제품 목록 조건](product-listing-condition.md)
   - [갱신한 제품](renewed-products.md)
- [주문 설정](order-settings.md)
- [통합 설정 저장](store-integration-settings.md)
- 목록 및 가격 규칙 {#rules}
   - [규칙 나열](listing-rules.md)
   - 가격 규칙 {#pricing-rules}
      - [가격 관리](pricing-products.md)
      - [새 가격 규칙 추가](add-pricing-rule.md)
      - [가격 규칙 일반 설정](pricing-rule-general-settings.md)
      - [가격 규칙 조건](pricing-rule-conditions.md)
      - [가격 규칙 작업](pricing-rule-actions.md)
      - [표준 가격 규칙](standard-price-rules.md)
      - [지능형 가격 조정 규칙](intelligent-repricing-rules.md)
      - [경쟁업체 조건부 분산](competitor-conditional-variances.md)
      - [가격 조정](price-adjustment.md)
      - [최저 가격](floor-price.md)
      - [선택적 최고 가격](optional-ceiling-price.md)
      - [가격 범위](price-scope.md)
      - [가격 우선 순위 논리](price-priority-logic.md)
      - [Buy Box 경쟁업체 가격](buy-box-competitor-pricing.md)
      - [경쟁사 최저 가격](lowest-competitor-pricing.md)
   - 예제 {#rules-examples}
      - [조건 정의](ob-define-condition-example.md)
      - [가격 규칙 예](price-rule-examples.md)
- 보고서 및 로그 {#reports-logs}
   - [로그 및 저장소 보고서](amazon-logs-reports.md)
   - 보고서 {#store-reports} 저장
      - [경쟁 제품 가격 분석](competitive-price-analysis.md)
      - [목록 개선 사항](listing-improvements.md)
   - 로그 {#logs}
      - [변경 로그 나열](listing-changes-log.md)
      - [통신 오류 로그](communication-errors-log.md)
- {#admin-listings} 목록 관리
   - [Amazon 목록 관리](managing-product-listings.md)
   - 상태/탭 {#status-tab}별
      - [상태/탭별 관리](managing-listings-by-tab.md)
      - [불완전한 목록](incomplete-listings.md)
      - [새 타사 목록](new-third-party-listings.md)
      - [나열 준비 완료](ready-to-list.md)
      - [비활성 목록](inactive-listings.md)
      - [활성 목록](active-listings.md)
      - [재정의](overrides.md)
      - [부적격 목록](ineligible-listings.md)
      - [종료된 목록](ended-listings.md)
   - 작업 {#actions}에서
      - [작업으로 관리](managing-listings-by-action.md)
      - [카탈로그 제품 만들기 및 할당](creating-assigning-catalog-products.md)
      - [재정의 만들기 및 편집](creating-editing-overrides.md)
      - [별칭 판매자 SKU 만들기](create-alias-seller-sku.md)
      - [할당된 ASIN 편집](edit-assigned-asin.md)
      - [Amazon 목록 종료](end-listings-manually.md)
      - [Publish 및 Amazon 목록](publish-listings-manually.md)
      - [필수 정보 업데이트](amazon-manually-update-incomplete-listing.md)
      - [세부 정보 보기](product-listing-details.md)
- {#admin-orders} 주문 관리
   - [주문 관리](managing-orders.md)
   - [Amazon 주문 보기](amazon-orders-all.md)
   - [Amazon 주문 세부 사항 보기](amazon-order-details.md)
   - [일반적인 주문 처리 작업](common-order-processing.md)
   - [이행 워크플로우](fulfillment-workflows.md)
   - [미출하 주문 취소](cancel-unshipped-order.md)
- [릴리스 정보](release-notes.md)
