---
title: Amazon 판매 채널 - 표준 가격 규칙 작업
description: 표준 가격 규칙 작업을 사용하여 상거래 카탈로그 가격(또는 가격 출처)에 따라 Amazon 목록 가격을 높이거나 낮춥니다.
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 표준 가격 규칙 작업

표준 가격 규칙 작업을 사용하면 다음을 기준으로 Amazon 목록 가격을 특정 비율이나 고정 달러 금액만큼 증가 또는 감소시킬 수 있습니다. [!DNL Commerce] 카탈로그 가격(또는 가격 출처).

표준 가격 규칙 작업의 섹션에는 다음이 포함됩니다.

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 가격 규칙 작업 구성

1. 대상 **[!UICONTROL Rule Type]**, 선택 `Standard price rule`.

   이 옵션은 _[!UICONTROL Select Rule Type]_섹션.

1. 확장 _[!UICONTROL Price Adjustment]_섹션에 있는 마지막 항목이 될 필요가 없습니다.

1. 대상 **[!UICONTROL Price Action]**&#x200B;을(를) 클릭하고 변경할 방법을 결정합니다. *[!UICONTROL Magento Price Source]* (에 정의됨) [목록 가격](./listing-price.md)) 값을 반환합니다.

   - `Decrease By` - Amazon에 나열하기 전에 값을 줄일 시기를 선택하십시오.

   - `Increase By` - Amazon에 나열하기 전에 값을 늘릴 시기를 선택합니다.

1. 대상 **[!UICONTROL Apply]**&#x200B;옵션을 선택하여 정의할 방법을 결정합니다 *[!UICONTROL Magento Price Source]* 다음에 정의됨: [목록 가격](./listing-price.md) 조정할 값:

   - `Apply as percentage` - 정의할 시기를 선택합니다. *[!UICONTROL Magento Price Source]* 다음에 정의됨: [목록 가격](./listing-price.md) 백분율로 조정된 값

   - `Apply as fixed amount` - 정의할 시기를 선택합니다. *[!UICONTROL Magento Price Source]* 다음에 정의됨: [목록 가격](./listing-price.md) 고정 금액으로 조정된 값입니다.

1. 대상 **[!UICONTROL Adjustment Amount]** (필수) 가격 조정에 대한 숫자 값을 입력합니다.

   - 날짜 *[!UICONTROL Apply]* 이(가) (으)로 설정됨 `Apply as percentage`, 백분율 값을 입력합니다(예: enter `25` (25% 가격 조정).

   - 날짜 *[!UICONTROL Apply]* 이(가) (으)로 설정됨 `Apply as fixed amount`고정 금액에 대한 숫자 값을 입력합니다(예: enter `25` $25 고정 가격 조정).

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save pricing rule]**.

![표준 가격 규칙](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | 선택 `Standard price rule`. |
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시기를 선택합니다. [!DNL Commerce] Amazon에 상장하기 전에 감소할 가격 소스 값입니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시기를 선택합니다. [!DNL Commerce] Amazon에 나열하기 전에 인상할 가격 소스 값.</li></ul> |
| [!UICONTROL Apply] | 옵션:<ul><li>**[!UICONTROL Apply as percentage]** - 정의할 시기를 선택합니다. [!DNL Commerce] 가격 출처 값을 퍼센트로 조정합니다.</li><li>**[!UICONTROL Apply as fixed amount]** - 정의할 시기를 선택합니다. [!DNL Commerce] 고정 금액으로 조정된 가격 출처 값.</li></ul> |
| [!UICONTROL Adjustment Amount] | 필수.<br><br>다음을 선택하는 경우 `Apply as percentage` 대상 *[!UICONTROL Apply]*, 백분율 값을 입력합니다(예: enter `25` 25% 조정).<br><br>다음을 선택한 경우 `Apply as fixed amount` 대상 *[!UICONTROL Apply]*&#x200B;고정 금액에 대한 숫자 값을 입력합니다(예: enter `25` $25 고정 조정). |
