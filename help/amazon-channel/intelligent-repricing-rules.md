---
title: '''지능형 가격 조정 규칙: 규칙 유형 선택'''
description: 지능형 가격 조정 규칙을 만들어 경쟁업체의 가격에 따라 Amazon 목록 가격을 결정합니다.
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 규칙 유형 선택

>[!IMPORTANT]
>
>온보딩 중이어서 Amazon 지역이 `Inactive` 상태로 설정된 경우 지능형 가격 조정 규칙이 제대로 작동하지 않습니다. 가격 계산은 배송비에 따라 다르며, 배송료가 Amazon에서 동기화되려면 해당 지역이 `Active` 상태여야 합니다.<br><br>
>
>Amazon 계정에서 지역 상태를 업데이트하려면 설정 > 계정 정보 > 휴가 설정으로 이동합니다. [Amazon 를 참조하십시오. 휴가 상태 나열](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

지능형 가격 조정 규칙은 Amazon 경쟁 업체의 가격을 사용하여 목록 가격을 결정합니다. Amazon에 나와 같은 제품을 나열한 다른 판매업체들이다.

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- 규칙 유형 선택
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- [가격 조정](./price-adjustment.md)
- [가격](./floor-price.md)
- [선택적 천정 가격](./optional-ceiling-price.md)

## 규칙 유형 구성

_[!UICONTROL Select Rule Type]_섹션에서 규칙 유형을 정의합니다.

1. **[!UICONTROL Rule Type]**&#x200B;에 대해 `Intelligent repricing rule`을 선택합니다.

   이 설정을 사용하면 _[!UICONTROL Competitor Price Source]_필드와 [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md) 및 [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) 섹션이 활성화됩니다.

1. **[!UICONTROL Competitor Price Source]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - **[!UICONTROL Use "Buy Box" Price]** - Amazon 판매가를 기준으로 Amazon 가격을 조정할 시기를  [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 선택합니다. Amazon의 여러 판매자가 동일한 제품을 제공할 때 [!DNL Buy Box] 가격이 존재합니다. Amazon은 성능 요구 사항을 기반으로 [!DNL Buy Box] 판매자를 정의합니다. 상인들은 [!DNL Buy Box] 판매자 상태를 획득하고 제품 목록을 최대한 확인할 수 있도록 노력하고 있습니다.

   - **[!UICONTROL Use Lowest Competitor Price]** - 동일한 제품에 대한 경쟁사 가격 책정 비교 및 조정을 원하는 시점을 선택합니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화됩니다.

1. 활성화되면 **[!UICONTROL Minimum Positive Feedback]** 옵션을 선택합니다.

   - **[!UICONTROL All Competitor's Prices]** - 동일한 제품에 대한 모든 경쟁사 가격을 기준으로 가격 비교 및 조정을 원하는 시점을 선택합니다.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - 동일한 제품에 대한 가격 비교 대상을 제한하려는 시점을 선택합니다. 이 설정은 가장 낮은 가격 규칙을 적용하기 전에 목록에서 선택된 긍정적인 피드백의 최소 비율을 갖도록 요구함으로써 경쟁자를 더 좁힙니다.

1. 활성화되면 **[!UICONTROL Minimum Feedback Count]**&#x200B;에 대한 숫자 값을 입력합니다.

   이 선택적 수치로 인해 경쟁사 가격을 더 낮출 수 있습니다. 예를 들어, 상인에 95% 양의 피드백 등급이 있지만 피드백 카운트가 `20`인 경우 가격을 수정할 경쟁사가 아닐 수 있습니다. 그러나 `1000` 값을 입력하는 경우 상인에 95% 양의 피드백이 있고 최소 1000개의 머천트 리뷰가 있어야 합니다.

>[!NOTE]
>
>이러한 경쟁사 가격 책정 및 피드백 옵션을 사용하여 피드백이 좋지 않고 품질이 낮은 제품을 판매하는 경쟁사를 기준으로 가격을 책정하는 것을 방지할 수 있습니다.

![지능형 가격 조정 규칙 - 규칙 유형 선택](assets/ob-intelligent-price-rule-type.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Rule Type] | 규칙 유형을 선택합니다. 옵션:<ul><li>**[!UICONTROL Standard price rule]** - 이 규칙 유형을 사용하면 Amazon 목록 가격을 대/소문자를 기준으로 특정 백분율 또는 고정 달러 금액만큼 늘리거나 줄일 수 있습니다 _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - 이 규칙 유형을 사용하면 경쟁업체 가격에 따라 Amazon 목록 가격을 조정할 수 있습니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화됩니다.</li></ul> |
| [!UICONTROL Competitor Price Source] | 원하는 가격 출처를 선택합니다. 옵션:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Amazon 판매가를 기준으로 Amazon 가격을 조정하려는 경우 이 옵션을  [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 선택합니다. Amazon의 여러 판매자가 동일한 제품을 제공할 때 [!DNL Buy Box] 가격이 존재합니다. Amazon은 성능 요구 사항을 기반으로 [!DNL Buy Box] 판매자를 정의합니다. 상인들은 [!DNL Buy Box] 판매자 상태를 획득하고 제품 목록을 최대한 확인할 수 있도록 노력하고 있습니다.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - 동일한 제품에 대한 가장  [낮은 경쟁사 가격](./lowest-competitor-pricing.md) 과 목록 가격을 비교하고 조정하려는 경우 이 옵션을 선택합니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화됩니다.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | `Use Lowest Competitor Price`이 선택된 경우에만 활성화됩니다. 옵션:<ul><li>**[!UICONTROL All Competitor's Prices]** - 동일한 제품에 대한 모든 경쟁사 가격을 기준으로 가격 비교 및 조정을 원하는 시점을 선택합니다.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - 가격 비교 및 조정 대상 경쟁업체를 제한하려는 시점을 선택합니다. 이 설정은 해당 목록이 선택된 긍정적인 피드백 중 최소 비율을 갖도록 한 다음, 해당 경쟁사의 하위 집합에 대한 최저 가격을 사용하도록 함으로써 경쟁사의 수를 더 줄입니다.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | `Use Lowest Competitor Price`이 선택된 경우에만 활성화됩니다. 이 선택적 수치로 인해 가격 비교 범위를 더 좁힐 수 있습니다. 예를 들어, 상인에 95% 양의 피드백 등급이 있지만 피드백 카운트가 `20`인 경우 가격을 수정할 경쟁사가 아닐 수 있습니다. 그러나 `1000` 값을 입력하는 경우 상인에 95% 양의 피드백이 있고 최소 1000개의 머천트 리뷰가 있어야 합니다. |
