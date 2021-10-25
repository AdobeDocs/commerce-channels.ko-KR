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
>가격 조정 섹션은 표준 및 지능형 가격 조정 규칙에 대해 약간 다릅니다. **[!UICONTROL Match Competitor Price]** 다음에서만 사용할 수 있습니다. _[!UICONTROL Price Action]_when **[!UICONTROL Rule Type]**가 로 설정되어 있습니다. `Intelligent repricing rule`.

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- 가격 조정
- [가격](./floor-price.md)
- [선택적 천정 가격](./optional-ceiling-price.md)

가격 조정은 경쟁사 가격 출처를 식별한 경우 가격 계산을 정의합니다.

## 가격 조정 구성

에서 가격 조정을 정의합니다. _[!UICONTROL Price Adjustment]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Price Action]**&#x200B;다음 옵션을 선택합니다.

   - `Decrease By` - Amazon에 나열하기 전에 정의된 가격 출처 값을 조정하여 규칙의 가격을 낮출지를 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 정의된 가격 소스 값을 조정하여 규칙에 대한 더 높은 가격을 만들 시기를 선택합니다.

   - `Match Competitor Price` - (Intelligent pricing 규칙만 해당) Amazon 목록 가격을 와 일치하도록 변경할 시기를 선택합니다 [최저 경쟁사](./lowest-competitor-pricing.md) 가격(경쟁업체 피드백 및 분산 매개 변수 기준) 로 설정된 경우 `Match Competitor Price`, _[!UICONTROL Apply]_및_[!UICONTROL Adjustment Amount]_ 필드가 제거됩니다.

1. 대상 **[!UICONTROL Apply]**&#x200B;다음 옵션을 선택합니다.

   - `Apply as percentage` - 정의할 시점을 선택합니다 **[!UICONTROL Magento Price Source]** 에 정의됨 [목록 가격](./listing-price.md) 백분율로 조정됨.

   - `Apply as fixed amount` - 정의할 시점을 선택합니다 **[!UICONTROL Magento Price Source]** 에 정의됨 [목록 가격](./listing-price.md) 고정 금액으로 조정됩니다.

1. 대상 **[!UICONTROL Adjustment Amount]** (필수) 가격 조정에 대한 숫자 값을 입력합니다.

   - When **[!UICONTROL Apply]** 가 로 설정되어 있습니다. `Apply as percentage`퍼센트 값을 입력합니다(예: enter `25` 25% 조정).

   - When **[!UICONTROL Apply]** 가 로 설정되어 있습니다. `Apply as fixed amount`고정된 금액에 대한 숫자 값을 입력합니다(예: enter `25` (25달러 고정 조정).

![지능형 가격 조정 규칙 - 가격 조정](assets/amazon-price-adjustment.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Price Action] | 가격 조정 조치를 선택합니다. 옵션:<br>**[!UICONTROL Decrease By]**- 정의할 시점을 선택합니다 _[!UICONTROL Magento Price Source]_에 정의됨 [목록 가격](./listing-price.md) 조정하여 Amazon에 게시하기 전에 규칙에 대한 낮은 가격을 만듭니다.<br>**[!UICONTROL Increase By]**- 정의할 시점을 선택합니다_[!UICONTROL Magento Price Source]_ 에 정의됨 [목록 가격](./listing-price.md) 조정할 수 있도록 Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 만듭니다.<br>**[!UICONTROL Match Competitor Price]**- (Intelligent pricing 규칙만 해당) Amazon 목록 가격을 와 일치하도록 변경할 시기를 선택합니다 [최저 경쟁사](./lowest-competitor-pricing.md) 가격(경쟁업체 피드백 및 분산 매개 변수 기준) 선택한 경우 _적용_ 및 _조정 금액_ 필드가 제거됩니다. |
| [!UICONTROL Apply] | 옵션:<br>**[!UICONTROL Apply as percentage]**- 정의할 시점을 선택합니다 _[!UICONTROL Magento Price Source]_에 정의됨 [목록 가격](./listing-price.md) 백분율로 조정됨.<br>**[!UICONTROL Apply as fixed amount]**- 정의할 시점을 선택합니다_[!UICONTROL Magento Price Source]_ 에 정의됨 [목록 가격](./listing-price.md) 고정 금액으로 조정됩니다. |
| [!UICONTROL Adjustment Amount] | 필수 여부.<br>선택한 경우 `Apply as percentage` 대상 **[!UICONTROL Apply]**&#x200B;퍼센트 값을 입력합니다(예: enter `25` 25% 조정).<br>선택한 경우 `Apply as fixed amount` 대상 **[!UICONTROL Apply]**&#x200B;고정된 금액에 대한 숫자 값을 입력합니다(예: enter `25` (25달러 고정 조정). |
