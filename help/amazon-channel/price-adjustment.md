---
title: 가격 조정
description: Amazon 경쟁업체 가격 출처를 식별한 경우 가격 조정을 구성하여 가격 계산을 정의합니다.
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 가격 조정

>[!NOTE]
>
>가격 조정 섹션은 표준 및 지능형 가격 조정 규칙에 대해 약간 다릅니다. **[!UICONTROL Match Competitor Price]** 은(는) 다음에서만 사용할 수 있습니다. _[!UICONTROL Price Action]_조건&#x200B;**[!UICONTROL Rule Type]**이(가) (으)로 설정됨 `Intelligent repricing rule`.

지능형 가격 조정 규칙의 섹션은 다음과 같습니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- 가격 조정
- [최저 가격](./floor-price.md)
- [선택적 최고 가격](./optional-ceiling-price.md)

가격 조정은 경쟁업체 가격 출처를 식별한 경우 가격 계산을 정의합니다.

## 가격 조정 구성

에서 가격책정 조정을 정의합니다. _[!UICONTROL Price Adjustment]_섹션.

1. 대상 **[!UICONTROL Price Action]**&#x200B;옵션을 선택합니다.

   - `Decrease By` - 정의된 가격 출처 값을 하향 조정하여 규칙의 가격을 낮춘 후 Amazon에 나열할 시기를 선택합니다.

   - `Increase By` - 정의된 가격 출처 값을 조정하여 Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 생성하는 시점을 선택합니다.

   - `Match Competitor Price` - (지능형 가격 조정 규칙만 해당) Amazon 목록 가격을 다음과 일치하도록 변경할 시기를 선택합니다. [가장 낮은 경쟁자](./lowest-competitor-pricing.md) 가격, 경쟁업체 피드백 및 차이 매개 변수를 기반으로 합니다. 로 설정된 경우 `Match Competitor Price`, _[!UICONTROL Apply]_및_[!UICONTROL Adjustment Amount]_ 필드가 제거됩니다.

1. 대상 **[!UICONTROL Apply]**&#x200B;옵션을 선택합니다.

   - `Apply as percentage` - 정의할 시기를 선택합니다. **[!UICONTROL Magento Price Source]** 다음에 정의됨: [목록 가격](./listing-price.md) 백분율로 조정되었습니다.

   - `Apply as fixed amount` - 정의할 시기를 선택합니다. **[!UICONTROL Magento Price Source]** 다음에 정의됨: [목록 가격](./listing-price.md) 고정 금액으로 조정됩니다.

1. 대상 **[!UICONTROL Adjustment Amount]** (필수) 가격 조정에 대한 숫자 값을 입력합니다.

   - 날짜 **[!UICONTROL Apply]** 이(가) (으)로 설정됨 `Apply as percentage`, 백분율 값을 입력합니다(예: enter `25` 25% 조정).

   - 날짜 **[!UICONTROL Apply]** 이(가) (으)로 설정됨 `Apply as fixed amount`고정 금액에 대한 숫자 값을 입력합니다(예: enter `25` $25 고정 조정).

![지능형 가격 조정 규칙 - 가격 조정](assets/amazon-price-adjustment.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<br>**[!UICONTROL Decrease By]**- 정의할 시기를 선택합니다. _[!UICONTROL Magento Price Source]_다음에 정의됨: [목록 가격](./listing-price.md) Amazon에 등록하기 전에 규칙의 가격을 낮추어 조정해야 합니다.<br>**[!UICONTROL Increase By]**- 정의할 시기를 선택합니다._[!UICONTROL Magento Price Source]_ 다음에 정의됨: [목록 가격](./listing-price.md) Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 만들어 조정을 해야 합니다.<br>**[!UICONTROL Match Competitor Price]**- (지능형 가격 조정 규칙만 해당) Amazon 목록 가격을 다음과 일치하도록 변경할 시기를 선택합니다. [가장 낮은 경쟁자](./lowest-competitor-pricing.md) 가격, 경쟁업체 피드백 및 차이 매개 변수를 기반으로 합니다. 이 옵션을 선택하면 _적용_ 및 _조정 금액_ 필드가 제거됩니다. |
| [!UICONTROL Apply] | 옵션:<br>**[!UICONTROL Apply as percentage]**- 정의할 시기를 선택합니다. _[!UICONTROL Magento Price Source]_다음에 정의됨: [목록 가격](./listing-price.md) 백분율로 조정되었습니다.<br>**[!UICONTROL Apply as fixed amount]**- 정의할 시기를 선택합니다._[!UICONTROL Magento Price Source]_ 다음에 정의됨: [목록 가격](./listing-price.md) 고정 금액으로 조정됩니다. |
| [!UICONTROL Adjustment Amount] | 필수.<br>다음을 선택한 경우 `Apply as percentage` 대상 **[!UICONTROL Apply]**, 백분율 값을 입력합니다(예: enter `25` 25% 조정).<br>다음을 선택한 경우 `Apply as fixed amount` 대상 **[!UICONTROL Apply]**&#x200B;고정 금액에 대한 숫자 값을 입력합니다(예: enter `25` $25 고정 조정). |
