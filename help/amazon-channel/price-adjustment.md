---
title: 가격 조정
description: Amazon 경쟁업체 가격 출처를 식별한 경우 가격 계산을 정의하기 위해 가격 조정을 구성합니다.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 가격 조정

>[!NOTE]
>
>가격 조정 섹션은 표준 및 지능형 가격 조정 규칙에 대해 약간 다릅니다. **[!UICONTROL Match Competitor Price]** 는 가 로 설정된  _[!UICONTROL Price Action]_경우에만&#x200B;**[!UICONTROL Rule Type]**사용할 수  `Intelligent repricing rule`있습니다.

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- 가격 조정
- [가격](./floor-price.md)
- [선택적 천정 가격](./optional-ceiling-price.md)

가격 조정은 경쟁사 가격 출처를 식별한 경우 가격 계산을 정의합니다.

## 가격 조정 구성

_[!UICONTROL Price Adjustment]_섹션에서 가격 조정을 정의합니다.

1. **[!UICONTROL Price Action]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - `Decrease By` - Amazon에 나열하기 전에 정의된 가격 출처 값을 조정하여 규칙의 가격을 낮출지를 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 정의된 가격 소스 값을 조정하여 규칙에 대한 더 높은 가격을 만들 시기를 선택합니다.

   - `Match Competitor Price` - (지능형 가격 책정 규칙만 해당) 경쟁업체 피드백 및 차이 매개 변수를 기반으로  [가장 ](./lowest-competitor-pricing.md) 낮은 경쟁 가격과 일치하도록 Amazon 목록 가격을 변경할 시기를 선택합니다. `Match Competitor Price`으로 설정하면 _[!UICONTROL Apply]_및_[!UICONTROL Adjustment Amount]_ 필드가 제거됩니다.

1. **[!UICONTROL Apply]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - `Apply as percentage` - 목록 가격 **[!UICONTROL Magento Price Source]** 에 정의된 값을 백분율로  [조정할 ](./listing-price.md) 시기를 선택합니다.

   - `Apply as fixed amount` - 목록 가격 **[!UICONTROL Magento Price Source]** 에 정의된 값을  [고정 ](./listing-price.md) 금액으로 조정할 시기를 선택합니다.

1. **[!UICONTROL Adjustment Amount]**(필수)에 가격 조정에 대한 숫자 값을 입력합니다.

   - **[!UICONTROL Apply]**&#x200B;이 `Apply as percentage`로 설정되면 백분율 값을 입력합니다(예: 25% 조정을 위해 `25` 입력).

   - **[!UICONTROL Apply]**&#x200B;이 `Apply as fixed amount`로 설정되면 고정 금액에 대한 숫자 값을 입력합니다(예: $25 고정 조정에 대해 `25`를 입력합니다.

![지능형 가격 조정 규칙 - 가격 조정](assets/amazon-price-adjustment.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Price Action] | 가격 조정 조치를 선택합니다. 옵션:<br>**[!UICONTROL Decrease By]**- [목록 가격](./listing-price.md)에 정의된 _[!UICONTROL Magento Price Source]_을(를) 조정하여 Amazon에 나열하기 전에 규칙에 대해 낮은 가격을 만들려면 선택합니다.<br>**[!UICONTROL Increase By]**- Amazon에 나열하기 전_[!UICONTROL Magento Price Source]_ 에 목록 [에 정의된 가격](./listing-price.md) 을 조정하여 규칙의 가격을 높인 후에 표시할 시기를 선택합니다.<br>**[!UICONTROL Match Competitor Price]**- (지능형 가격 책정 규칙만 해당) 경쟁업체 피드백 및 차이 매개 변수를 기반으로  [가장 ](./lowest-competitor-pricing.md) 낮은 경쟁 가격과 일치하도록 Amazon 목록 가격을 변경할 시기를 선택합니다. 선택한 경우 _적용_ 및 _조정 금액_ 필드가 제거됩니다. |
| [!UICONTROL Apply] | 옵션:<br>**[!UICONTROL Apply as percentage]**- [목록 가격](./listing-price.md)에 정의된 _[!UICONTROL Magento Price Source]_을 백분율로 조정할 시기를 선택합니다.<br>**[!UICONTROL Apply as fixed amount]**- 목록 가격_[!UICONTROL Magento Price Source]_ 에 정의된 값을  [고정 ](./listing-price.md) 금액으로 조정할 시기를 선택합니다. |
| [!UICONTROL Adjustment Amount] | 필수 여부.<br>에  `Apply as percentage` 대해 선택한  **[!UICONTROL Apply]**&#x200B;경우 퍼센트 값을 입력합니다(예: 25%  `25` 조정을 입력합니다.)<br>을( `Apply as fixed amount` 를)  **[!UICONTROL Apply]**&#x200B;선택한 경우 고정 금액에 대한 숫자 값을 입력합니다(예: $ `25` 25 고정 조정에 을(를) 입력합니다. |
