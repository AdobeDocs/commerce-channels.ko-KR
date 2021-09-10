---
title: 가격책정 규칙 추가
description: 가격 규칙을 사용하여 전자 상거래 제품 카탈로그의 Amazon Marketplace에 대한 목록 가격을 관리합니다.
exl-id: 37ecf25a-7b47-4f6d-a4bb-2f306f7b5997
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 가격 규칙 추가

스토어를 통합한 후 언제든지 가격 책정 규칙을 구성하거나 수정할 수 있습니다. 가격 책정 규칙은 [목록 설정](./listing-settings.md)의 일부이며 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

## 표준 가격 규칙

표준 가격 규칙 작업을 사용하면 [목록 가격](./listing-price.md)에 정의된 **[!UICONTROL Magento Price Source*]*&#x200B;에 상대적인 특정 백분율 또는 고정 달러 금액만큼 Amazon 목록 가격을 늘리거나 줄일 수 있습니다.

### 표준 가격책정 규칙 추가

1. 저장소 대시보드에서 **[!UICONTROL Pricing rules]** 을 클릭합니다.

1. **[!UICONTROL Add new pricing rule]** 을 클릭합니다.

1. 규칙에 대한 **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)**&#x200B;을 완료합니다.

1. 규칙에 대한 **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)**&#x200B;을 완료합니다.

1. 규칙에 대한 **[[!UICONTROL Price Rule Actions]](./standard-price-rules.md)**&#x200B;을 완료합니다.

1. 완료되면 **[!UICONTROL Save pricing rule]** 을 클릭합니다.

## 지능형 가격 조정 규칙

지능형 가격 조정 규칙은 Amazon 경쟁 업체의 가격을 사용하여 목록 가격을 결정합니다. 경쟁 업체는 Amazon에서 나열하는 동일한 제품을 나열하는 다른 판매자입니다.

### 지능형 가격 조정 규칙 추가

1. 저장소 대시보드에서 **[!UICONTROL Pricing rules]** 을 클릭합니다.

1. **[!UICONTROL Add new pricing rule]** 을 클릭합니다.

1. 규칙에 대한 **[[!UICONTROL General Settings]](./pricing-rule-general-settings.md)**&#x200B;을 완료합니다.

1. 규칙에 대한 **[[!UICONTROL Price Rule Conditions]](./pricing-rule-conditions.md)**&#x200B;을 완료합니다.

1. 규칙에 대한 **[!UICONTROL Price Rule Actions]**&#x200B;을 완료합니다.

   - [[!UICONTROL Select Rule Typ]e](./intelligent-repricing-rules.md)

   - [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)

   - [[!UICONTROL Price Adjustment]](./price-adjustment.md)

   - [[!UICONTROL Floor Price]](./floor-price.md)

   - [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

1. 완료되면 **[!UICONTROL Save pricing rule]** 을 클릭합니다.
