---
title: '지능형 가격 조정 규칙: 현장 가격'
description: 현장 가격 설정을 사용하여 지능형 가격 책정 규칙의 최저 가격을 결정하여 Amazon 목록을 관리할 수 있습니다.
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 현장 가격

지능형 가격 조정 규칙의 섹션은 다음과 같습니다.

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

[최저 가격](./floor-price.md) 설정은 지능형 가격 책정 규칙과 비교하여 최저 제품 가격을 자동으로 보호합니다. 이러한 설정을 사용하여 인텔리전트 가격 책정 규칙에 대한 최저 가격(최저 가격)을 설정하여 제품이 원하는 가격 이하로 목록에 표시되지 않도록 할 수 있습니다.

[!DNL Commerce] 스토어에서 웹 사이트 가격 범위를 사용하는 경우 최저 가격 특성은 웹 사이트 범위를 기반으로 합니다. [가격 범위](./price-scope.md)를 참조하세요.

가격은 **[!UICONTROL Rule Type]**&#x200B;이(가) `Intelligent repricing rule`(으)로 설정된 경우에만 사용됩니다.

## 현장 가격 구성

_[!UICONTROL Floor Price]_섹션에서 최저가 설정을 정의합니다.

1. **[!UICONTROL Floor Price Source]**&#x200B;의 경우 가격 원본 특성을 선택하십시오.

   상대 층 한도를 나타내는 [!DNL Commerce] [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을(를) 선택하십시오. 예를 들어, Amazon 목록 가격이 항목의 비용 아래로 떨어지지 않도록 하려면 *Cost* 특성을 선택합니다.

1. **[!UICONTROL Floor Price Action]**&#x200B;에 대해 옵션을 선택하십시오.

   - `Decrease By` - 정의된 _[!UICONTROL Floor Price Source]_값을 하향 조정하여 더 낮은 수준의 규칙을 만든 후 Amazon에 나열하려면 선택하십시오.

   - `Increase By` - 정의된 _[!UICONTROL Floor Price Source]_값을 조정하여 더 높은 수준의 규칙을 만든 후 Amazon에 나열하려는 경우 선택합니다.

   - `Match` - 목록 가격이 정의된 _[!UICONTROL Floor Price Source]_값 미만으로 변동되지 않도록 하려면 선택합니다. `Match`(으)로 설정하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화됩니다.

1. **[!UICONTROL Apply]** 기본값을 `Apply as percentage`(으)로 둡니다.

1. **[!UICONTROL Floor Adjustment Price]**&#x200B;의 경우 _[!UICONTROL Floor Price Source]_값을 조정하려면 백분율에 대한 숫자 값을 입력하십시오.

이 사례에서 바닥 가격은 물건의 원가보다 3% 높게 책정된다.

![지능형 가격 조정 규칙 예 - 최저 가격](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source] | 상대 기간(최저 가격) 제한을 나타내는 [!DNL Commerce] 특성을 선택하십시오. 예를 들어, Amazon 목록 가격이 항목의 비용 아래로 떨어지지 않도록 하려면 `Cost` 특성을 선택합니다. |
| [!UICONTROL Floor Price Action] | 가격책정 조정 조치를 선택합니다. 옵션:<ul><li>**[!UICONTROL Decrease By]** - 정의된 _[!UICONTROL Floor Price Source]_값을 하향 조정하여 더 낮은 수준의 규칙을 만든 후 Amazon에 나열하려면 선택하십시오.</li><li>**[!UICONTROL Increase By]** - 정의된 _[!UICONTROL Floor Price Source]_값을 조정하여 더 높은 수준의 규칙을 만든 후 Amazon에 나열하려는 경우 선택합니다.</li><li>**[!UICONTROL Match]** - 목록 가격이 정의된 _[!UICONTROL Floor Price Source]_값 미만으로 변동되지 않도록 하려면 선택합니다. 선택하면_[!UICONTROL Apply]_ 및 _[!UICONTROL Floor Adjustment Amount]_필드가 비활성화됩니다.</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** - _[!UICONTROL Floor Price Source]_값을 기준으로 한 백분율 조정입니다. |
| [!UICONTROL Floor Adjustment Amount] | _[!UICONTROL Floor Price Source]_값을 조정하려면 백분율에 대한 숫자 값을 입력하십시오. |
