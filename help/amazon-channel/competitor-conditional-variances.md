---
title: '''지능형 가격 조정 규칙: 경쟁업체 조건부 분산'''
description: 지능형 가격 조정 규칙을 만들어 경쟁업체의 가격 책정 및 제품 조건을 기준으로 Amazon 목록 가격을 결정합니다.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# 지능형 가격 조정 규칙: 경쟁업체 조건부 분산

지능형 가격 조정 규칙 섹션에는 다음이 포함됩니다.

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

지능형 가격 조정 규칙은 Amazon 경쟁 업체의 가격을 사용하여 목록 가격을 결정합니다. 경쟁 업체는 Amazon에서 나열하는 동일한 제품을 나열하는 다른 판매자입니다.

동일한 조건을 가진 제품이 있는 경우 기본 일치 가격은 동일한 조건을 가진 [가장 낮은 경쟁업체](./lowest-competitor-pricing.md) 가격입니다. 고객의 조건에 맞는 경쟁사 제품이 없을 경우 기본 대응 가격은 신규, 재설계부터 시작하여 사용 가능한 조건을 통해 계속 다운될 수 있는 기타 경쟁사 조건을 거칩니다. 조건이 발견되면 기본 일치 가격이 해당 조건 내에서 가장 낮은 가격이 됩니다.

조건 `Used; Good` 과 기본 일치 가격이 표시된 제품이 있고, 경쟁업체가 동일한 조건을 더 낮은 가격으로 가지고 있는 경우 경쟁 업체 가격이 사용됩니다. 동일한 조건을 가진 경쟁사가 없는 경우 시스템은 다음 조건( `New`)이 있는 경쟁사를 확인합니다. 해당 조건이 있는 경쟁자가 발견되면 가장 낮은 가격이 사용됩니다.

## 경쟁업체 조건부 분산 구성

_[!UICONTROL Competitor Conditional Variances]_섹션에서 조건 차이를 정의합니다.

**[!UICONTROL Conditional Variance]**&#x200B;에 대해 다음 옵션을 선택합니다.

- `Use all competitor's product conditions` - (기본값) 제품을 사용 가능한 조건과 비교할 시점을 선택합니다(나열하는 조건에 대한 일치가 없는 경우).

- `Use Only Matching Competitor's Product Condition` - 제품이 동일한 조건에 있는 경쟁사의 제품에만 비교되도록 하려면 선택합니다. 일치하는 항목이 없으면 제품의 가격은 [목록 가격](./listing-price.md)에 정의된 _Magento 가격 소스_&#x200B;에 있습니다.

- `Apply Variance (if competitor's product condition differs)` - 일치하는 제품 조건과 먼저 비교하도록 선택합니다. 일치하는 조건이 없으면 제품 조건 및 가장 낮은 경쟁업체 조건에 대해 차이(백분율)가 적용됩니다.

   _[!UICONTROL Apply Variance]_기능을 선택하면 각 Amazon 조건에 대한 추가 분산 필드가 표시됩니다. 이 기능을 사용하면 경쟁업체와 다른 조건을 가진 제품을 제공할 때 지능형 가격 조정 규칙을 사용할 수 있습니다. 조건부 차이 뒤에 있는 계산을 이해하려면 먼저 모든 차이가 기본 일치 가격에서 결정됨을 이해해야 합니다.

   표시되는 조건부 분산 옵션은 [!DNL Commerce] [제품 특성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}을 사용하여 조건 값에 매핑되는 `Condition`에 대한 목록 설정을 기반으로 합니다. 모든 매핑된 조건에 대해 1-100의 분산 백분율을 정의할 수 있습니다. 예외 사항은 컬렉션이며, 이 경우 100보다 큰 백분율을 적용할 수 있습니다.

![지능형 가격 조정 규칙 - 경쟁업체 조건부 분산](assets/amazon-competitor-cond-variances.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | 옵션: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - 제품을 나열하는 조건에 대해 일치하는 항목이 없으면 이 옵션은 사용 가능한 조건과 일치합니다. 이 메서드는 먼저 조건에 일치하려고 한 다음 `New` 조건에서 `Used; Acceptable`로 작동합니다.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - 이 옵션은 제품 조건과 일치합니다. 일치하는 항목이 없으면 _[!UICONTROL Magento Price Source]_의 제품 가격이 표시됩니다.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - 이 옵션은 먼저 제품 조건과 일치하려고 합니다. 일치하는 조건이 없으면 제품 조건과 가장 낮은 경쟁업체 조건에 대한 차이(백분율)가 적용됩니다.</li></ul><br><br> [!DNL Commerce] [제품 특성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}을 사용하여 조건 값에 매핑되는 조건에 대한 목록 설정을 기반으로 표시되는 조건부 분산 옵션입니다. 매핑된 모든 조건에 대해 분산 백분율을 1-100으로 표시할 수 있습니다. 예외 사항은 컬렉션이며, 이 경우 100보다 큰 백분율을 적용할 수 있습니다.<br><br>이 기능을 사용하면 경쟁업체와 다른 조건을 가진 제품을 제공할 때 지능형 가격 조정 규칙을 사용할 수 있습니다. 조건부 차이 뒤에 있는 계산을 이해하려면 먼저 모든 차이가 기본 일치 가격에서 결정됨을 이해해야 합니다. |

## 조건부 분산 기준 계산

- 기본 일치 조건 차이(BMC) = 기본 일치 가격 경쟁사의 조건에 대한 변수입니다. 이전 예를 사용하면 BMC가 `New` 조건에 대한 변수입니다.
- 머천트 조건 차이(MCV) = 제품 조건에 대한 변수입니다. 이전 예를 사용하면 MCV = `Used; Good` 조건에 대한 변수입니다.
- 기본 일치 가격(BMP) = $7.99(위에 설명)

조건부 분산 기준을 계산하는 공식은 다음과 같습니다.

![조건부 분산 기준 계산 공식](assets/amazon-cond-variance-calc-1.png)

## 예

조건부 분산 설정은 다음과 같습니다.

![조건부 분산 설정 예](assets/amazon-cond-variances.png)

- BMC = 100(경쟁업체 조건 = 신규)
- MCV = 80(머천트 조건 = 사용됨; 좋아요)
- BMP = $7.99 (기본 일치 가격 = 일치하는 경쟁업체 조건의 최저 가격)

![조건부 분산 기준 계산 예](assets/amazon-cond-variance-calc-2.png)

위에서 조건부 차이 기준 계산을 사용하면 조건부 차이 기준 = $6.39. 이 계산은 [가격 조정](./price-adjustment.md)에 더 설명된 가격 규칙 작업에 사용되는 경쟁업체 가격 출처입니다.
