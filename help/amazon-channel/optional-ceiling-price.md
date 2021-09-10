---
title: '''지능형 가격 조정 규칙: 선택적 천정 가격'''
description: Amazon 목록을 관리하는 지능형 가격 규칙으로부터 최고 가격을 보호하려면 선택적 천정 가격 설정을 사용하십시오.
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
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

_[!UICONTROL Optional Ceiling Price]_섹션에서 선택적 최고가격 설정을 정의합니다.

1. **[!UICONTROL Ceiling Price Source]**&#x200B;에 대해 속성을 선택합니다.

   상대 천정 제한을 나타내는 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}을 선택합니다. 예를 들어 Amazon 목록 가격이 항목의 MSRP보다 높은 가격을 원하지 않는 경우 `Manufacturer's Suggested Retail Price` 속성을 선택합니다.

1. **[!UICONTROL Ceiling Price Action]**&#x200B;에 대해 옵션을 선택합니다.

   - `Decrease By` - Amazon에 나열하기 전 _[!UICONTROL Ceiling Price Source]_에 정의된 값을 조정하여 규칙의 천정 가격을 낮출려면 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 정의된 값 _[!UICONTROL Ceiling Price Source]_을 조정하여 규칙에 대한 천정 가격을 높인 시점을 선택합니다.

   - `Match` - 목록 가격이 정의된  _[!UICONTROL Ceiling Price Source]_값 이상으로 변동하지 않도록 할 시기를 선택합니다. `Match`으로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화됩니다.

1. **[!UICONTROL Apply]** 기본값을 `Apply as percentage`(으)로 둡니다.

1. **[!UICONTROL Ceiling Adjustment Price]**&#x200B;에 대해 백분율에 대한 숫자 값을 입력하여 _[!UICONTROL Ceiling Price Source]_값을 조정합니다.

이 예에서 천정 가격은 항목의 MSRP 보다 2% 낮게 설정됩니다.

![지능형 가격 책정 규칙 - 선택적 한도](assets/ob-intelligent-price-rule-ceiling.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 상대 천정 제한을 나타내는 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}을 선택합니다. 예를 들어 제품 목록 가격이 항목의 MSRP보다 높게 이동하지 않으려면 `Manufacturer's Suggested Retail Price` 속성을 선택합니다. |
| [!UICONTROL Ceiling Price Action] | 가격 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - Amazon에 나열하기 전 _[!UICONTROL Ceiling Price Source]_에 정의된 값을 조정하여 규칙의 천정 가격을 낮출려면 선택합니다.</li><li>**[!UICONTROL Increase By]** - Amazon에 나열하기 전에 정의된 값 _[!UICONTROL Ceiling Price Source]_을 조정하여 규칙에 대한 천정 가격을 높인 시점을 선택합니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된  _[!UICONTROL Ceiling Price Source]_값 이상으로 변동하지 않도록 할 시기를 선택합니다. `Match`으로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화됩니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 값에 대한 백분율  _[!UICONTROL Ceiling Price Source]_조정 |
| [!UICONTROL Ceiling Price Adjustment] | 백분율에 대한 숫자 값을 입력하여 _[!UICONTROL Ceiling Price Source]_값을 조정합니다. |
