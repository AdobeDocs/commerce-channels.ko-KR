---
title: 표준 가격 규칙 조치
description: 표준 가격 규칙 작업을 사용하여 상거래 카탈로그 가격(또는 가격 출처)과 관련하여 Amazon 목록 가격을 늘리거나 줄일 수 있습니다.
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 표준 가격 규칙 작업

표준 가격 규칙 작업을 사용하면 [!DNL Commerce] 카탈로그 가격(또는 가격 출처)

표준 가격 규칙 작업의 섹션은 다음과 같습니다.

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 가격 규칙 작업 구성

1. 대상 **[!UICONTROL Rule Type]**, 선택 `Standard price rule`.

   이 옵션은 _[!UICONTROL Select Rule Type]_섹션을 참조하십시오.

1. 를 확장합니다. _[!UICONTROL Price Adjustment]_섹션에 문의하십시오.

1. 대상 **[!UICONTROL Price Action]**&#x200B;를 선택하는 경우 옵션을 선택하여 *[!UICONTROL Magento Price Source]* (에 정의됨) [목록 가격](./listing-price.md)) 내의 아무 곳에나 삽입할 수 있습니다.

   - `Decrease By` - Amazon에 나열하기 전에 값을 줄이려면 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 값을 늘릴 시점을 선택합니다.

1. 대상 **[!UICONTROL Apply]**&#x200B;을(를) 선택하고 옵션을 선택하여 정의할 방법을 결정합니다 *[!UICONTROL Magento Price Source]* 에 정의됨 [목록 가격](./listing-price.md) 조정할 값:

   - `Apply as percentage` - 정의할 시점을 선택합니다 *[!UICONTROL Magento Price Source]* 에 정의됨 [목록 가격](./listing-price.md) 백분율로 조정된 값

   - `Apply as fixed amount` - 정의할 시점을 선택합니다 *[!UICONTROL Magento Price Source]* 에 정의됨 [목록 가격](./listing-price.md) 고정 금액으로 조정된 값입니다.

1. 대상 **[!UICONTROL Adjustment Amount]** (필수) 가격 조정에 대한 숫자 값을 입력합니다.

   - When *[!UICONTROL Apply]* 가 로 설정되어 있습니다. `Apply as percentage`퍼센트 값을 입력합니다(예: enter `25` 25% 가격 조정).

   - When *[!UICONTROL Apply]* 가 로 설정되어 있습니다. `Apply as fixed amount`고정된 금액에 대한 숫자 값을 입력합니다(예: enter `25` (25달러의 고정 가격 조정).

1. 완료되면 를 클릭합니다. **[!UICONTROL Save pricing rule]**.

![표준 가격 규칙](assets/ob-price-rule-action-standard-example.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Rule Type] | 선택 `Standard price rule`. |
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시점을 선택합니다 [!DNL Commerce] Amazon에 나열하기 전에 가격 소스 값을 줄일 수 있습니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시점을 선택합니다 [!DNL Commerce] Amazon에 나열하기 전에 높일 가격 소스 값입니다.</li></ul> |
| [!UICONTROL Apply] | 옵션:<ul><li>**[!UICONTROL Apply as percentage]** - 정의할 시점을 선택합니다 [!DNL Commerce] 가격 출처 값을 백분율로 조정.</li><li>**[!UICONTROL Apply as fixed amount]** - 정의할 시점을 선택합니다 [!DNL Commerce] 고정 금액으로 조정된 가격 출처 값입니다.</li></ul> |
| [!UICONTROL Adjustment Amount] | 필수 여부.<br><br>만약 `Apply as percentage` 대상 *[!UICONTROL Apply]*&#x200B;퍼센트 값을 입력합니다(예: enter `25` 25% 조정).<br><br>선택한 경우 `Apply as fixed amount` 대상 *[!UICONTROL Apply]*&#x200B;고정된 금액에 대한 숫자 값을 입력합니다(예: enter `25` (25달러 고정 조정). |
