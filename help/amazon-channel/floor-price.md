---
title: '''지능형 가격 조정 규칙: 가격'
description: 가격 설정을 사용하여 지능형 가격 규칙에 대한 가장 낮은 가격을 결정하여 Amazon 목록을 관리합니다.
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 가격

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

다음 [가격](./floor-price.md) 설정은 지능형 가격 책정 규칙으로부터 가장 낮은 제품 가격을 자동으로 보호합니다. 이 설정을 사용하여 지능형 가격 규칙에 대한 최저 가격(최저 가격)을 설정하여 제품이 원하는 가격 이하로 나열되지 않도록 합니다.

가격 속성은 [!DNL Commerce] 저장소는 웹 사이트 가격 범위를 사용하고 있습니다. 자세한 내용은 [가격 범위](./price-scope.md).

가격은 **[!UICONTROL Rule Type]** 가 로 설정되어 있습니다. `Intelligent repricing rule`.

## 가격 구성

에서 가장 낮은 가격 설정을 정의합니다. _[!UICONTROL Floor Price]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Floor Price Source]**&#x200B;가격 출처 속성을 선택합니다.

   을(를) 선택합니다 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html)상대 용적률을 나타내는 {target=&quot;_blank&quot;}. 예를 들어 Amazon 목록 가격이 항목의 비용보다 낮게 유지되지 않게 하려면 *비용* 속성을 사용합니다.

1. 대상 **[!UICONTROL Floor Price Action]**&#x200B;옵션을 선택합니다.

   - `Decrease By` - 정의할 시점을 선택합니다 _[!UICONTROL Floor Price Source]_조정할 값으로, Amazon에 나열하기 전에 규칙에 대한 낮은 가격을 만듭니다.

   - `Increase By` - 정의할 시점을 선택합니다 _[!UICONTROL Floor Price Source]_조정할 값으로, Amazon에 나열하기 전에 규칙에 대한 높은 최저가를 만듭니다.

   - `Match` - 목록 가격이 정의된 값 이하로 변동하지 않을 경우를 선택합니다 _[!UICONTROL Floor Price Source]_값. 로 설정된 경우 `Match`,_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화되어 있습니다.

1. 을(를) 종료하십시오. **[!UICONTROL Apply]** 기본값은 입니다. `Apply as percentage`.

1. 대상 **[!UICONTROL Floor Adjustment Price]**&#x200B;를 조정하려면 백분율에 대한 숫자 값을 입력합니다 _[!UICONTROL Floor Price Source]_값.

이 예에서 가격 은 품목 원가보다 3% 높게 설정됩니다.

![지능형 가격 조정 규칙 예 - 가격](assets/ob-intelligent-pricde-rule-floor-price.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Floor Price Source] | 을(를) 선택합니다 [!DNL Commerce] 상대 바닥(최저 가격) 제한을 나타내는 속성입니다. 예를 들어 Amazon 목록 가격이 항목의 비용보다 낮게 유지되지 않게 하려면 `Cost` 속성을 사용합니다. |
| [!UICONTROL Floor Price Action] | 가격 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의할 시점을 선택합니다 _[!UICONTROL Floor Price Source]_조정할 값으로, Amazon에 나열하기 전에 규칙에 대한 낮은 가격을 만듭니다.</li><li>**[!UICONTROL Increase By]** - 정의할 시점을 선택합니다 _[!UICONTROL Floor Price Source]_조정할 값으로, Amazon에 나열하기 전에 규칙에 대한 높은 최저가를 만듭니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된 값 이하로 변동하지 않을 경우를 선택합니다 _[!UICONTROL Floor Price Source]_값. 선택한 경우_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화되어 있습니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 을 기준으로 백분율 조정 _[!UICONTROL Floor Price Source]_값. |
| [!UICONTROL Floor Adjustment Amount] | 백분율에 대한 숫자 값을 입력하여 비율을 조정합니다 _[!UICONTROL Floor Price Source]_값. |
