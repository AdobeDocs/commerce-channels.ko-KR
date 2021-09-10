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

표준 가격 규칙 작업을 사용하면 [!DNL Commerce] 카탈로그 가격(또는 가격 소스)에 대해 특정 백분율 또는 고정 달러 금액만큼 Amazon 목록 가격을 증가 또는 줄일 수 있습니다.

표준 가격 규칙 작업의 섹션은 다음과 같습니다.

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 가격 규칙 작업 구성

1. **[!UICONTROL Rule Type]**&#x200B;에 대해 `Standard price rule`을 선택합니다.

   이 옵션은 _[!UICONTROL Select Rule Type]_섹션의 다른 필드를 비활성화합니다.

1. 필요한 경우 _[!UICONTROL Price Adjustment]_섹션을 확장합니다.

1. **[!UICONTROL Price Action]**&#x200B;에 대해 *[!UICONTROL Magento Price Source]*([목록 가격](./listing-price.md)에 정의됨) 값을 변경하는 방법을 결정하는 옵션을 선택합니다.

   - `Decrease By` - Amazon에 나열하기 전에 값을 줄이려면 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 값을 늘릴 시점을 선택합니다.

1. **[!UICONTROL Apply]**&#x200B;에 대해 [목록 가격](./listing-price.md) 값에 정의된 *[!UICONTROL Magento Price Source]* 값을 조정할 방법을 결정하는 옵션을 선택합니다.

   - `Apply as percentage` - 목록 가격에 정의된 값 *[!UICONTROL Magento Price Source]* 을 백분율로  [조정할 ](./listing-price.md) 시기를 선택합니다

   - `Apply as fixed amount` - 목록 가격표에 정의된 값 *[!UICONTROL Magento Price Source]* 을  [고정 ](./listing-price.md) 금액으로 조정할 시기를 선택합니다.

1. **[!UICONTROL Adjustment Amount]**(필수)에 가격 조정에 대한 숫자 값을 입력합니다.

   - *[!UICONTROL Apply]*&#x200B;이 `Apply as percentage`로 설정되면 백분율 값을 입력합니다(예: 25% 가격 조정을 위해 `25`를 입력합니다.

   - *[!UICONTROL Apply]*&#x200B;이 `Apply as fixed amount`로 설정되면 고정 금액에 대한 숫자 값을 입력합니다(예: $25 고정 가격 조정에 대해 `25`를 입력합니다.

1. 완료되면 **[!UICONTROL Save pricing rule]** 을 클릭합니다.

![표준 가격 규칙](assets/ob-price-rule-action-standard-example.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Rule Type] | `Standard price rule` 을 선택합니다. |
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - Amazon으로 나열하기 전에 정의된  [!DNL Commerce] 가격 출처 값을 줄이려면 선택합니다.</li><li>**[!UICONTROL Increase By]** - Amazon에 나열하기 전에 정의된  [!DNL Commerce] 가격 출처 값을 늘릴 시점을 선택합니다.</li></ul> |
| [!UICONTROL Apply] | 옵션:<ul><li>**[!UICONTROL Apply as percentage]** - 정의된  [!DNL Commerce] 가격 출처 값을 백분율로 조정할 시기를 선택합니다.</li><li>**[!UICONTROL Apply as fixed amount]** - 정의된  [!DNL Commerce] 가격 출처 값을 고정 금액으로 조정할 시기를 선택합니다.</li></ul> |
| [!UICONTROL Adjustment Amount] | 필수 여부.<br><br>에 대해 `Apply as percentage` 를 선택하는  *[!UICONTROL Apply]*&#x200B;경우 퍼센트 값을 입력합니다(예: 25%  `25` 조정을 입력합니다.)<br><br>을( `Apply as fixed amount` 를)  *[!UICONTROL Apply]*&#x200B;선택한 경우 고정 금액에 대한 숫자 값을 입력합니다(예: $ `25` 25 고정 조정에 을(를) 입력합니다. |
