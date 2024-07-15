---
title: Amazon 판매 채널 - 표준 가격 규칙 작업
description: 표준 가격 규칙 작업을 사용하여 Commerce 카탈로그 가격(또는 가격 출처)에 비례하여 Amazon 목록 가격을 높이거나 낮춥니다.
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 표준 가격 규칙 작업

표준 가격 규칙 작업을 사용하면 [!DNL Commerce] 카탈로그 가격(또는 가격 원본)과 관련하여 특정 비율이나 고정 달러 금액만큼 Amazon 목록 가격을 늘리거나 줄일 수 있습니다.

표준 가격 규칙 작업의 섹션에는 다음이 포함됩니다.

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 가격 규칙 작업 구성

1. **[!UICONTROL Rule Type]**&#x200B;의 경우 `Standard price rule`을(를) 선택하십시오.

   이 옵션을 사용하면 _[!UICONTROL Select Rule Type]_섹션의 다른 필드가 비활성화됩니다.

1. 필요한 경우 _[!UICONTROL Price Adjustment]_섹션을 확장합니다.

1. **[!UICONTROL Price Action]**&#x200B;의 경우 *[!UICONTROL Magento Price Source]*(목록 가격](./listing-price.md)에 정의됨) 값을 변경할 방법을 결정하는 옵션을 선택하십시오.[

   - `Decrease By` - Amazon에 나열하기 전에 값을 줄이려면 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 값을 늘릴지 여부를 선택합니다.

1. **[!UICONTROL Apply]**&#x200B;에 대해 [가격 목록](./listing-price.md) 값에 정의된 *[!UICONTROL Magento Price Source]*&#x200B;을(를) 조정하는 방법을 결정하는 옵션을 선택하십시오.

   - `Apply as percentage` - [가격 표시](./listing-price.md) 값에 정의된 *[!UICONTROL Magento Price Source]*&#x200B;을(를) 정의할 시기를 백분율로 조정합니다.

   - `Apply as fixed amount` - [가격 표시](./listing-price.md) 값에 정의된 *[!UICONTROL Magento Price Source]*&#x200B;을(를) 고정 금액으로 조정하려는 경우 선택합니다.

1. **[!UICONTROL Adjustment Amount]**(필수)의 경우 가격 조정에 대한 숫자 값을 입력합니다.

   - *[!UICONTROL Apply]*&#x200B;이(가) `Apply as percentage`(으)로 설정된 경우 퍼센트 값을 입력합니다(예: 25% 퍼센트 가격 조정에 대한 `25` 입력).

   - *[!UICONTROL Apply]*&#x200B;이(가) `Apply as fixed amount`(으)로 설정된 경우 고정 금액에 대한 숫자 값을 입력하십시오(예: $25 고정 가격 조정에 대한 `25` 입력).

1. 완료되면 **[!UICONTROL Save pricing rule]**&#x200B;을(를) 클릭합니다.

![표준 가격 규칙](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | `Standard price rule`을(를) 선택합니다. |
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - Amazon에 나열하기 전에 정의된 [!DNL Commerce] 가격 원본 값을 줄이려면 선택하십시오.</li><li>**[!UICONTROL Increase By]** - Amazon에 나열하기 전에 정의된 [!DNL Commerce] 가격 원본 값을 늘릴지 선택합니다.</li></ul> |
| [!UICONTROL Apply] | 옵션:<ul><li>**[!UICONTROL Apply as percentage]** - 정의된 [!DNL Commerce] 가격 원본 값을 백분율로 조정하려는 경우 선택합니다.</li><li>**[!UICONTROL Apply as fixed amount]** - 정의된 [!DNL Commerce] 가격 원본 값을 고정 금액으로 조정하려는 경우 선택합니다.</li></ul> |
| [!UICONTROL Adjustment Amount] | 필수.<br><br>*[!UICONTROL Apply]*&#x200B;에 대해 `Apply as percentage`을(를) 선택하는 경우 백분율 값을 입력하십시오(예: 25% 조정을 하려면 `25`을(를) 입력하십시오).<br><br>*[!UICONTROL Apply]*&#x200B;에 대해 `Apply as fixed amount`을(를) 선택한 경우 고정 금액에 대한 숫자 값을 입력하십시오(예: $25 고정 조정에 대해 `25`을(를) 입력하십시오). |
