---
title: '지능형 가격 조정 규칙: 선택적 한도 가격'
description: 선택적인 최고 가격 설정을 사용하여 Amazon 목록을 관리하는 지능적인 가격 책정 규칙으로부터 가장 높은 제품 가격을 보호합니다.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 선택적 한도 가격

지능형 가격 조정 규칙의 섹션은 다음과 같습니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- [가격 조정](./price-adjustment.md)
- [최저 가격](./floor-price.md)
- 선택적 최고 가격

자동화된 상한 가격 설정은 지능형 가격 책정 규칙에 대해 가장 높은 제품 가격을 자동으로 보호하므로 지능형 가격 책정 규칙에 대한 한도(가장 높은 가격)를 설정할 수 있습니다.

## 선택적 최고 가격 구성

다음에서 선택적 최고 가격 설정을 정의합니다. _[!UICONTROL Optional Ceiling Price]_섹션.

1. 대상 **[!UICONTROL Ceiling Price Source]**&#x200B;속성을 선택합니다.

   다음 항목 선택 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 이는 사용자의 상대적 한도 제한을 나타냅니다. 예를 들어 Amazon 목록 가격이 항목의 MSRP를 넘지 않도록 하려면 다음을 선택합니다. `Manufacturer's Suggested Retail Price` 특성.

1. 대상 **[!UICONTROL Ceiling Price Action]**&#x200B;옵션을 선택합니다.

   - `Decrease By` - 정의할 시기를 선택합니다. _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 낮은 상한 가격을 만들어 하향 조정할 값입니다.

   - `Increase By` - 정의할 시기를 선택합니다. _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 높은 상한 가격을 만들어 상향 조정될 값입니다.

   - `Match` - 정의된 가격보다 높게 목록 가격을 변동시키지 않으려면 선택합니다. _[!UICONTROL Ceiling Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화되었습니다.

1. 나가기 **[!UICONTROL Apply]** 기본값: `Apply as percentage`.

1. 대상 **[!UICONTROL Ceiling Adjustment Price]**&#x200B;를 조정할 백분율에 대한 숫자 값을 입력합니다. _[!UICONTROL Ceiling Price Source]_값.

이 예에서, 상한가는 품목의 MSRP보다 2% 낮게 설정된다.

![지능형 가격 조정 규칙 - 선택적 한도 가격](assets/ob-intelligent-price-rule-ceiling.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 다음을 선택합니다. [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 이는 사용자의 상대적 한도 제한을 나타냅니다. 예를 들어 제품 목록 가격이 항목의 MSRP를 넘지 않도록 하려면 `Manufacturer's Suggested Retail Price` 특성. |
| [!UICONTROL Ceiling Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시기를 선택합니다. _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 낮은 상한 가격을 만들어 하향 조정할 값입니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시기를 선택합니다. _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 높은 상한 가격을 만들어 상향 조정될 값입니다.</li><li>**[!UICONTROL Match]** - 정의된 가격보다 높게 목록 가격을 변동시키지 않으려면 선택합니다. _[!UICONTROL Ceiling Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화되었습니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 다음을 기준으로 한 백분율 조정 _[!UICONTROL Ceiling Price Source]_값. |
| [!UICONTROL Ceiling Price Adjustment] | 조정할 백분율에 대한 숫자 값을 입력합니다. _[!UICONTROL Ceiling Price Source]_값. |
