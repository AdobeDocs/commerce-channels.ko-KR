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
>Amazon 지역이 `Inactive` 상태, 온보딩 중임. 가격 계산은 배송비에 따라 다르며 해당 지역은 다음 위치에 있어야 합니다 `Active` Amazon에서 동기화할 배송 요금에 대한 상태입니다.<br><br>
>
>Amazon 계정에서 지역 상태를 업데이트하려면 설정 > 계정 정보 > 휴가 설정으로 이동합니다. 을(를) 참조하십시오. [Amazon: 휴가 상태 나열](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

지능형 가격 조정 규칙은 Amazon 경쟁 업체의 가격을 사용하여 목록 가격을 결정합니다. Amazon에 나와 같은 제품을 나열한 다른 판매업체들이다.

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- 규칙 유형 선택
- [경쟁업체 조건부 분산](./competitor-conditional-variances.md)
- [가격 조정](./price-adjustment.md)
- [가격](./floor-price.md)
- [선택적 천정 가격](./optional-ceiling-price.md)

## 규칙 유형 구성

에서 규칙 유형을 정의합니다 _[!UICONTROL Select Rule Type]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Rule Type]**, 선택 `Intelligent repricing rule`.

   이 설정은 _[!UICONTROL Competitor Price Source]_필드 및 [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md), 및 [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) 섹션에 자세히 설명되어 있습니다.

1. 대상 **[!UICONTROL Competitor Price Source]**&#x200B;다음 옵션을 선택합니다.

   - **[!UICONTROL Use "Buy Box" Price]** - Amazon을 기반으로 Amazon 가격을 조정할 시기를 선택합니다 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 판매가격입니다. A [!DNL Buy Box] 가격은 Amazon의 여러 판매자가 동일한 제품을 제공할 때 존재합니다. Amazon은 다음을 정의합니다 [!DNL Buy Box] 성능 요구 사항을 기반으로 판매자 상인들은 이기기 위해 노력한다 [!DNL Buy Box] 판매자 상태 및 해당 제품 목록을 최대 표시할 수 있습니다.

   - **[!UICONTROL Use Lowest Competitor Price]** - 동일한 제품에 대한 경쟁사 가격 책정 비교 및 조정을 원하는 시점을 선택합니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화되어 있습니다.

1. 활성화된 경우 다음 옵션을 선택합니다 **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]** - 동일한 제품에 대한 모든 경쟁사 가격을 기준으로 가격 비교 및 조정을 원하는 시점을 선택합니다.

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]** - 동일한 제품에 대한 가격 비교 대상을 제한하려는 시점을 선택합니다. 이 설정은 가장 낮은 가격 규칙을 적용하기 전에 목록에서 선택된 긍정적인 피드백의 최소 비율을 갖도록 요구함으로써 경쟁자를 더 좁힙니다.

1. 활성화한 경우 숫자 값을 입력합니다 **[!UICONTROL Minimum Feedback Count]**.

   이 선택적 수치로 인해 경쟁사 가격을 더 낮출 수 있습니다. 예를 들어 매장에 95% 양수 피드백 등급이 있지만 피드백 카운트만 있는 경우 `20`를 지정하는 경우 가격을 수정하려는 경쟁사가 아닐 수 있습니다. 그러나 값을 입력한 경우 `1000`상인은 95%의 긍정적인 의견을 가지고 있고 최소 1000개의 상인의 평가를 받아야 한다.

>[!NOTE]
>
>이러한 경쟁사 가격 책정 및 피드백 옵션을 사용하여 피드백이 좋지 않고 품질이 낮은 제품을 판매하는 경쟁사를 기준으로 가격을 책정하는 것을 방지할 수 있습니다.

![지능형 가격 조정 규칙 - 규칙 유형 선택](assets/ob-intelligent-price-rule-type.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Rule Type] | 규칙 유형을 선택합니다. 옵션:<ul><li>**[!UICONTROL Standard price rule]** - 이 규칙 유형을 사용하면 Amazon 목록 가격을 _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]** - 이 규칙 유형을 사용하면 경쟁업체 가격에 따라 Amazon 목록 가격을 조정할 수 있습니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화되어 있습니다.</li></ul> |
| [!UICONTROL Competitor Price Source] | 원하는 가격 출처를 선택합니다. 옵션:<ul><li>**[!UICONTROL Use "Buy Box" Price]** - Amazon을 기반으로 Amazon 가격을 조정하려는 경우 이 옵션을 선택합니다 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 판매가격입니다. A [!DNL Buy Box] 가격은 Amazon의 여러 판매자가 동일한 제품을 제공할 때 존재합니다. Amazon은 다음을 정의합니다 [!DNL Buy Box] 성능 요구 사항을 기반으로 판매자 상인들은 이기기 위해 노력한다 [!DNL Buy Box] 판매자 상태 및 해당 제품 목록을 최대 표시할 수 있습니다.</li><li>**[!UICONTROL Use Lowest Competitor Price]** - 목록 가격을 비교 및 조정하여 [최저 가격 가격](./lowest-competitor-pricing.md) 해당 항목이 없습니다. 선택한 경우 _[!UICONTROL Minimum Positive Feedback]_및_[!UICONTROL Minimum Feedback Count]_ 필드가 활성화되어 있습니다.</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | 활성 상태인 경우에만 `Use Lowest Competitor Price` 이(가) 선택되어 있습니다. 옵션:<ul><li>**[!UICONTROL All Competitor's Prices]** - 동일한 제품에 대한 모든 경쟁사 가격을 기준으로 가격 비교 및 조정을 원하는 시점을 선택합니다.</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]** - 가격 비교 및 조정 대상 경쟁업체를 제한하려는 시점을 선택합니다. 이 설정은 해당 목록이 선택된 긍정적인 피드백 중 최소 비율을 갖도록 한 다음, 해당 경쟁사의 하위 집합에 대한 최저 가격을 사용하도록 함으로써 경쟁사의 수를 더 줄입니다.</li></ul> |
| [!UICONTROL Minimum Feedback Count] | 활성 상태인 경우에만 `Use Lowest Competitor Price` 이(가) 선택되어 있습니다. 이 선택적 수치로 인해 가격 비교 범위를 더 좁힐 수 있습니다. 예를 들어 매상인 피드백 등급이 95%지만 피드백 카운트가 인 경우 `20`를 지정하는 경우 가격을 수정하려는 경쟁사가 아닐 수 있습니다. 그러나 값을 입력한 경우 `1000`상인은 95%의 긍정적인 의견을 가지고 있고 최소 1000개의 상인의 평가를 받아야 한다. |
