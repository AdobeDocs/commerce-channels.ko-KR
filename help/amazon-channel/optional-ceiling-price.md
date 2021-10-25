---
title: '''지능형 가격 조정 규칙: 선택적 천정 가격'''
description: Amazon 목록을 관리하는 지능형 가격 규칙으로부터 최고 가격을 보호하려면 선택적 천정 가격 설정을 사용하십시오.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 선택적 한도 가격

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- [규칙 유형 선택](./intelligent-repricing-rules.md)
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- [가격 조정](./price-adjustment.md)
- [가격](./floor-price.md)
- 선택적 천정 가격

자동 천정 가격 설정은 지능형 가격책정 규칙으로부터 최고 제품 가격을 자동으로 보호하므로 지능형 가격책정 규칙에 대해 최고 가격(최고 가격)을 설정할 수 있습니다.

## 선택적 천정 가격 구성

에서 선택 사항인 최고 가격 설정을 정의합니다 _[!UICONTROL Optional Ceiling Price]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Ceiling Price Source]**&#x200B;속성을 선택합니다.

   을(를) 선택합니다 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html)상대 천정 제한을 나타내는 {target=&quot;_blank&quot;}. 예를 들어 Amazon 목록 가격이 항목의 MSRP보다 높은 가격을 원하지 않는 경우, `Manufacturer's Suggested Retail Price` 속성을 사용합니다.

1. 대상 **[!UICONTROL Ceiling Price Action]**&#x200B;옵션을 선택합니다.

   - `Decrease By` - 정의할 시점을 선택합니다 _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 값을 조정하여 규칙에 대한 천정 가격을 낮춥니다.

   - `Increase By` - 정의할 시점을 선택합니다 _[!UICONTROL Ceiling Price Source]_값을 조정하여 Amazon에 나열하기 전에 규칙에 대한 천정 가격을 높입니다.

   - `Match` - 목록 가격이 정의된 것보다 크게 변동하지 않도록 할 때 선택합니다 _[!UICONTROL Ceiling Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화되어 있습니다.

1. 을(를) 종료하십시오. **[!UICONTROL Apply]** 기본값은 입니다. `Apply as percentage`.

1. 대상 **[!UICONTROL Ceiling Adjustment Price]**&#x200B;를 조정하려면 백분율에 대한 숫자 값을 입력합니다 _[!UICONTROL Ceiling Price Source]_값.

이 예에서 천정 가격은 항목의 MSRP 보다 2% 낮게 설정됩니다.

![지능형 가격 책정 규칙 - 선택적 한도](assets/ob-intelligent-price-rule-ceiling.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 을(를) 선택합니다 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html)상대 천정 제한을 나타내는 {target=&quot;_blank&quot;}. 예를 들어 제품 목록 가격이 항목의 MSRP보다 높은 가격을 원하지 않는 경우, `Manufacturer's Suggested Retail Price` 속성을 사용합니다. |
| [!UICONTROL Ceiling Price Action] | 가격 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시점을 선택합니다 _[!UICONTROL Ceiling Price Source]_Amazon에 나열하기 전에 값을 조정하여 규칙에 대한 천정 가격을 낮춥니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시점을 선택합니다 _[!UICONTROL Ceiling Price Source]_값을 조정하여 Amazon에 나열하기 전에 규칙에 대한 천정 가격을 높입니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된 것보다 크게 변동하지 않도록 할 때 선택합니다 _[!UICONTROL Ceiling Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화되어 있습니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 을 기준으로 백분율 조정 _[!UICONTROL Ceiling Price Source]_값. |
| [!UICONTROL Ceiling Price Adjustment] | 백분율에 대한 숫자 값을 입력하여 비율을 조정합니다 _[!UICONTROL Ceiling Price Source]_값. |
