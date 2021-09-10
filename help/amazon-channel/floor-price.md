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

[floor price](./floor-price.md) 설정은 지능형 가격 책정 규칙으로부터 가장 낮은 제품 가격을 자동으로 보호합니다. 이 설정을 사용하여 지능형 가격 규칙에 대한 최저 가격(최저 가격)을 설정하여 제품이 원하는 가격 이하로 나열되지 않도록 합니다.

가격 속성은 [!DNL Commerce] 스토어가 웹 사이트 가격 범위를 사용하는 경우 웹 사이트 범위를 기반으로 합니다. [가격 범위](./price-scope.md)를 참조하십시오.

가격은 **[!UICONTROL Rule Type]**&#x200B;이 `Intelligent repricing rule`로 설정된 경우에만 사용됩니다.

## 가격 구성

_[!UICONTROL Floor Price]_섹션에서 가장 낮은 가격 설정을 정의합니다.

1. **[!UICONTROL Floor Price Source]**&#x200B;에 대해 가격 출처 속성을 선택합니다.

   상대 바닥 제한을 나타내는 [!DNL Commerce] [제품 특성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}을 선택합니다. 예를 들어, Amazon 목록 가격이 항목의 비용보다 낮게 유지되지 않게 하려면 *Cost* 속성을 선택합니다.

1. **[!UICONTROL Floor Price Action]**&#x200B;에 대해 옵션을 선택합니다.

   - `Decrease By` - Amazon에 나열하기 전 _[!UICONTROL Floor Price Source]_에 정의된 값을 조정하여 규칙의 낮은 가격을 만들 시기를 선택합니다.

   - `Increase By` - Amazon에 나열하기 전에 정의된 값 _[!UICONTROL Floor Price Source]_을 조정하여 규칙의 높은 가격을 만들 시기를 선택합니다.

   - `Match` - 목록 가격이 정의된  _[!UICONTROL Floor Price Source]_값 아래에서 변동하지 않도록 할 시기를 선택합니다. `Match`으로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화됩니다.

1. **[!UICONTROL Apply]** 기본값을 `Apply as percentage`(으)로 둡니다.

1. **[!UICONTROL Floor Adjustment Price]**&#x200B;에 대해 백분율에 대한 숫자 값을 입력하여 _[!UICONTROL Floor Price Source]_값을 조정합니다.

이 예에서 가격 은 품목 원가보다 3% 높게 설정됩니다.

![지능형 가격 조정 규칙 예 - 가격](assets/ob-intelligent-pricde-rule-floor-price.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Floor Price Source] | 상대 바닥(최저 가격) 제한을 나타내는 [!DNL Commerce] 속성을 선택합니다. 예를 들어 Amazon 목록 가격이 항목의 비용보다 낮게 유지되지 않게 하려면 `Cost` 속성을 선택합니다. |
| [!UICONTROL Floor Price Action] | 가격 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - Amazon에 나열하기 전 _[!UICONTROL Floor Price Source]_에 정의된 값을 조정하여 규칙의 낮은 가격을 만들 시기를 선택합니다.</li><li>**[!UICONTROL Increase By]** - Amazon에 나열하기 전에 정의된 값 _[!UICONTROL Floor Price Source]_을 조정하여 규칙의 높은 가격을 만들 시기를 선택합니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된  _[!UICONTROL Floor Price Source]_값 아래에서 변동하지 않도록 할 시기를 선택합니다. 선택한 경우_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화됩니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - 값에 대한 백분율  _[!UICONTROL Floor Price Source]_조정 |
| [!UICONTROL Floor Adjustment Amount] | 백분율에 대한 숫자 값을 입력하여 _[!UICONTROL Floor Price Source]_값을 조정합니다. |
