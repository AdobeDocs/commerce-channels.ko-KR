---
title: '지능형 가격 조정 규칙: 현장 가격'
description: 현장 가격 설정을 사용하여 지능형 가격 책정 규칙의 최저 가격을 결정하여 Amazon 목록을 관리할 수 있습니다.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 현장 가격

지능형 가격 조정 규칙의 섹션은 다음과 같습니다.

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

다음 [최저 가격](./floor-price.md) 설정은 지능형 가격 책정 규칙으로부터 최저 제품 가격을 자동으로 보호합니다. 이러한 설정을 사용하여 인텔리전트 가격 책정 규칙에 대한 최저 가격(최저 가격)을 설정하여 제품이 원하는 가격 이하로 목록에 표시되지 않도록 할 수 있습니다.

다음의 경우 웹 사이트 범위를 기반으로 최저 가격 속성 [!DNL Commerce] 스토어에서 웹 사이트 가격 범위를 사용하고 있습니다. 다음을 참조하십시오 [가격 범위](./price-scope.md).

가격은 다음과 같은 경우에만 사용됩니다. **[!UICONTROL Rule Type]** 이(가) (으)로 설정됨 `Intelligent repricing rule`.

## 현장 가격 구성

에서 최저 가격 설정 정의 _[!UICONTROL Floor Price]_섹션.

1. 대상 **[!UICONTROL Floor Price Source]**, 가격 소스 속성을 선택합니다.

   다음을 선택합니다. [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 그것은 당신의 상대적인 층 제한을 나타냅니다. 예를 들어, Amazon 목록 가격이 항목의 비용 아래로 내려가지 않도록 하려면 *비용* 특성.

1. 대상 **[!UICONTROL Floor Price Action]**&#x200B;옵션을 선택합니다.

   - `Decrease By` - 정의할 시기를 선택합니다. _[!UICONTROL Floor Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 낮은 수준의 가격을 만들어 조정해야 할 값입니다.

   - `Increase By` - 정의할 시기를 선택합니다. _[!UICONTROL Floor Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 만들어 조정할 값입니다.

   - `Match` - 정의된 가격보다 낮게 목록 가격을 변동시키지 않으려면 선택합니다. _[!UICONTROL Floor Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화되었습니다.

1. 나가기 **[!UICONTROL Apply]** 기본값: `Apply as percentage`.

1. 대상 **[!UICONTROL Floor Adjustment Price]**&#x200B;를 조정할 백분율에 대한 숫자 값을 입력합니다. _[!UICONTROL Floor Price Source]_값.

이 사례에서 바닥 가격은 물건의 원가보다 3% 높게 책정된다.

![지능형 가격 조정 규칙 예 - 현장 가격](assets/ob-intelligent-pricde-rule-floor-price.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Floor Price Source] | 다음을 선택합니다. [!DNL Commerce] 상대 층(최저 가격) 제한을 나타내는 속성입니다. 예를 들어, Amazon 목록 가격이 항목의 비용 아래로 내려가지 않도록 하려면 `Cost` 특성. |
| [!UICONTROL Floor Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시기를 선택합니다. _[!UICONTROL Floor Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 낮은 수준의 가격을 만들어 조정해야 할 값입니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시기를 선택합니다. _[!UICONTROL Floor Price Source]_Amazon에 나열하기 전에 규칙에 대해 더 높은 가격을 만들어 조정할 값입니다.</li><li>**[!UICONTROL Match]** - 정의된 가격보다 낮게 목록 가격을 변동시키지 않으려면 선택합니다. _[!UICONTROL Floor Price Source]_값. 이 옵션을 선택하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화되었습니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 다음을 기준으로 한 백분율 조정 _[!UICONTROL Floor Price Source]_값. |
| [!UICONTROL Floor Adjustment Amount] | 조정할 백분율에 대한 숫자 값을 입력합니다. _[!UICONTROL Floor Price Source]_값. |
