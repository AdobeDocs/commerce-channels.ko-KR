---
title: Amazon 판매 채널 - [!UICONTROL Price Adjustment]
description: Amazon 경쟁업체 가격 출처를 식별한 경우 가격 조정을 구성하여 가격 계산을 정의합니다.
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>가격 조정 섹션은 표준 및 지능형 가격 조정 규칙에 대해 약간 다릅니다. **[!UICONTROL Rule Type]**&#x200B;이(가) `Intelligent repricing rule`(으)로 설정된 경우 **[!UICONTROL Match Competitor Price]**&#x200B;은(는) _[!UICONTROL Price Action]_에서만 사용할 수 있습니다.

지능형 가격 조정 규칙의 섹션은 다음과 같습니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- 가격 조정
- [최저 가격](./floor-price.md)
- [선택적 최고 가격](./optional-ceiling-price.md)

가격 조정은 경쟁업체 가격 출처를 식별한 경우 가격 계산을 정의합니다.

## 가격 조정 구성

_[!UICONTROL Price Adjustment]_섹션에서 가격 조정을 정의합니다.

1. **[!UICONTROL Price Action]**&#x200B;에 대해 다음 옵션을 선택하십시오.

   - `Decrease By` - 정의된 가격 원본 값을 하향 조정하여 규칙의 가격을 낮춘 후 Amazon에 나열할 시기를 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 만들어 정의된 가격 원본 값을 조정할 시기를 선택합니다.

   - `Match Competitor Price` - (지능형 가격 조정 규칙만 해당) 경쟁업체 피드백 및 차이 매개 변수를 기반으로 Amazon 목록 가격을 [가장 낮은 경쟁업체](./lowest-competitor-pricing.md) 가격과 일치하도록 변경할 시기를 선택합니다. `Match Competitor Price`(으)로 설정하면 _[!UICONTROL Apply]_및_[!UICONTROL Adjustment Amount]_ 필드가 제거됩니다.

1. **[!UICONTROL Apply]**&#x200B;에 대해 다음 옵션을 선택하십시오.

   - `Apply as percentage` - [가격 표시](./listing-price.md)에서 정의된 **[!UICONTROL Magento Price Source]**&#x200B;을(를) 백분율로 조정하려는 경우 선택합니다.

   - `Apply as fixed amount` - [가격 목록](./listing-price.md)에서 정의된 **[!UICONTROL Magento Price Source]**&#x200B;을(를) 고정 금액으로 조정하려는 경우 선택합니다.

1. **[!UICONTROL Adjustment Amount]**(필수)의 경우 가격 조정에 대한 숫자 값을 입력합니다.

   - **[!UICONTROL Apply]**&#x200B;이(가) `Apply as percentage`(으)로 설정된 경우 백분율 값을 입력합니다(예: 25% 비율 조정에 대한 `25` 입력).

   - **[!UICONTROL Apply]**&#x200B;이(가) `Apply as fixed amount`(으)로 설정된 경우 고정 금액에 대한 숫자 값을 입력합니다(예: $25 고정 조정에 대한 `25` 입력).

![지능형 가격 조정 규칙 - 가격 조정](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<br>**[!UICONTROL Decrease By]**- [목록 가격](./listing-price.md)에 정의된 _[!UICONTROL Magento Price Source]_을(를) 하향 조정하여 규칙의 가격을 낮춘 후 Amazon으로 나열할 시기를 선택합니다.<br>**[!UICONTROL Increase By]**- [가격 표시](./listing-price.md)에 정의된_[!UICONTROL Magento Price Source]_&#x200B;을(를) 조정할 시기를 선택하여 Amazon으로 나열하기 전에 규칙에 대해 더 높은 가격을 만듭니다.<br>**[!UICONTROL Match Competitor Price]**- (지능형 가격 조정 규칙만 해당) 경쟁업체 피드백 및 차이 매개 변수를 기반으로 Amazon 목록 가격을 [가장 낮은 경쟁업체](./lowest-competitor-pricing.md) 가격과 일치하도록 변경할 시기를 선택합니다. 선택하면 _적용_ 및 _조정 금액_ 필드가 제거됩니다. |
| [!UICONTROL Apply] | 옵션:<br>**[!UICONTROL Apply as percentage]**- [목록 가격](./listing-price.md)에 정의된 _[!UICONTROL Magento Price Source]_을(를) 백분율로 조정하려는 경우 선택합니다.<br>**[!UICONTROL Apply as fixed amount]**- [가격 목록](./listing-price.md)에서 정의된_[!UICONTROL Magento Price Source]_&#x200B;을(를) 고정 금액으로 조정하려는 경우 선택합니다. |
| [!UICONTROL Adjustment Amount] | 필수.<br>**[!UICONTROL Apply]**&#x200B;에 대해 `Apply as percentage`을(를) 선택한 경우 백분율 값을 입력하십시오(예: 25% 조정 시 `25` 입력).<br>**[!UICONTROL Apply]**&#x200B;에 대해 `Apply as fixed amount`을(를) 선택한 경우 고정 금액에 대한 숫자 값을 입력하십시오(예: $25 고정 조정에 대해 `25`을(를) 입력하십시오). |
