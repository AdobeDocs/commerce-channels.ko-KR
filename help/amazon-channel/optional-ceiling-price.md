---
title: '지능형 가격 조정 규칙: 선택적 한도 가격'
description: 선택적인 최고 가격 설정을 사용하여 Amazon 목록을 관리하는 지능적인 가격 책정 규칙으로부터 가장 높은 제품 가격을 보호합니다.
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '376'
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

_[!UICONTROL Optional Ceiling Price]_섹션에서 선택적 최고 가격 설정을 정의합니다.

1. **[!UICONTROL Ceiling Price Source]**&#x200B;의 경우 특성을 선택하십시오.

   상대 한도 제한을 나타내는 [!DNL Commerce] [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을 선택하세요. 예를 들어 Amazon 목록 가격이 항목의 MSRP를 넘지 않도록 하려면 `Manufacturer's Suggested Retail Price` 특성을 선택합니다.

1. **[!UICONTROL Ceiling Price Action]**&#x200B;에 대해 옵션을 선택하십시오.

   - `Decrease By` - 정의된 _[!UICONTROL Ceiling Price Source]_값을 아래로 조정하려면 선택한 후 Amazon에 나열하기 전에 규칙에 대해 더 낮은 천장 가격을 만듭니다.

   - `Increase By` - 정의된 _[!UICONTROL Ceiling Price Source]_값을 조정하여 Amazon에 나열하기 전에 규칙에 대한 더 높은 상한 가격을 만들 시기를 선택합니다.

   - `Match` - 목록 가격이 정의된 _[!UICONTROL Ceiling Price Source]_값 이상으로 변동하지 않도록 하려면 선택합니다. `Match`(으)로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화됩니다.

1. **[!UICONTROL Apply]** 기본값을 `Apply as percentage`(으)로 둡니다.

1. **[!UICONTROL Ceiling Adjustment Price]**&#x200B;의 경우 _[!UICONTROL Ceiling Price Source]_값을 조정하려면 백분율에 대한 숫자 값을 입력하십시오.

이 예에서, 상한가는 품목의 MSRP보다 2% 낮게 설정된다.

![지능형 가격 조정 규칙 - 선택적 상한 가격](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | 상대 한도 제한을 나타내는 [!DNL Commerce] [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을(를) 선택하십시오. 예를 들어 제품 목록 가격이 항목의 MSRP를 넘지 않도록 하려면 `Manufacturer's Suggested Retail Price` 특성을 선택합니다. |
| [!UICONTROL Ceiling Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의된 _[!UICONTROL Ceiling Price Source]_값을 아래로 조정하려면 선택한 후 Amazon에 나열하기 전에 규칙에 대해 더 낮은 천장 가격을 만듭니다.</li><li>**[!UICONTROL Increase By]** - 정의된 _[!UICONTROL Ceiling Price Source]_값을 조정하여 Amazon에 나열하기 전에 규칙에 대한 더 높은 상한 가격을 만들 시기를 선택합니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된 _[!UICONTROL Ceiling Price Source]_값 이상으로 변동하지 않도록 하려면 선택합니다. `Match`(으)로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Ceiling Adjustment Amount]_필드가 비활성화됩니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - _[!UICONTROL Ceiling Price Source]_값을 기준으로 한 백분율 조정입니다. |
| [!UICONTROL Ceiling Price Adjustment] | _[!UICONTROL Ceiling Price Source]_값을 조정하려면 백분율에 대한 숫자 값을 입력하십시오. |
