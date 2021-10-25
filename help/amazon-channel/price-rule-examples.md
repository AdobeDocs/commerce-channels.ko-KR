---
title: 가격 규칙 예
description: Amazon 목록에 대한 가격 규칙을 디자인하는 데 도움이 되도록 일반적인 시나리오에 따라 이러한 예를 검토하십시오.
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# 가격 규칙 예

## 표준 가격 규칙 예

### 후속 규칙 삭제

후속 규칙을 취소할 수 있는 기능은 여러 가격책정 규칙이 스택되지 않도록 하고 의도하지 않은 추가 할인을 제공하는 가격 규칙 내의 탁월한 기능입니다. 후속 규칙을 삭제하려면 가격책정 규칙에서 _[!UICONTROL Priority]_섹션 [가격책정 규칙 일반 설정](./pricing-rule-general-settings.md).

If **[!UICONTROL Discard Subsequent Rules]** 가 로 설정되어 있습니다. `Yes`을 지정하는 경우 우선순위가 낮은 규칙(높은 숫자)은 해당 제품에 적용되지 않습니다.

예를 들어 다음과 같은 세 가지 가격 규칙이 있다고 가정합니다.

| 예 | 규칙 이름 | 우선순위 | 후속 규칙 삭제 |
|----------|----|----|----|
| 1 | 판매 제품 10% 할인 | 1 | 아니요 |
| 2개 | 판매 상품 2개 | 2개 | 예 |
| 3 | 모든 제품의 5% 할인 | 3 | 아니요 |

이 시나리오에서는 규칙 #1 및 #2가 적합한 제품에 적용됩니다. 규칙 #3는 예보다 우선 순위가 낮으므로 규칙 #2에 포함되지 않은 적합한 제품에만 #2 **[!UICONTROL Discard Subsequent Rules]** 가 로 설정되어 있습니다. `Yes`. 따라서, 판매 카테고리의 적격 제품은 Amazon의 정가에서 10% 할인 및 2달러를 받을 수 있습니다.

### 두 가지 표준 가격 규칙 적용

| 필드 | 설정 - 규칙 1 | 설정 - 규칙 2 |
|----------|----|----|
| [!UICONTROL Rule Name] | 규칙-1 | 규칙-2 |
| [!UICONTROL Priority] | 1 | 2개 |
| [!UICONTROL Rule Type] | 표준 가격 규칙 | 표준 가격 규칙 |
| [!UICONTROL Price action] | 감소 기준 | 감소 기준 |
| [!UICONTROL Apply] | 백분율로 적용 | 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### 제품 1

가격: US$45.49

적용된 규칙 1: $45.49 x (0.9) = $40.94

적용된 규칙 2: $40.94 - $10.00 = $30.94

규칙 1 및 규칙 2 이후의 최종 가격은 다음과 같이 적용됩니다. US$30.94

#### 제품 2

가격: US$47.76

적용된 규칙 1: $47.76 x (0.9) = $42.98

적용된 규칙 2: $42.98 - $10.00 = $32.98

규칙 1과 규칙 2 뒤의 최종 가격이 적용됩니다. US$32.98

## 지능형 가격 조정 규칙 예

### Buy Box 가격 및 가격 출처 = 가격

| 필드 | 설정 |
|----------|----|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot; 가격 사용 |
| [!UICONTROL Price Action] | 경쟁업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 일치 |

#### 제품 1

가격: 15달러

[Buy Box](./buy-box-competitor-pricing.md) Amazon 가격: 10달러

왜냐하면 [Buy Box](./buy-box-competitor-pricing.md) 가격은 원래 가격보다 저렴하고 원래 가격으로 진열되어 있습니다

규칙이 적용된 후의 최종 가격: 15달러

#### 제품 2

가격: 5달러

[Buy Box](./buy-box-competitor-pricing.md) Amazon 가격: 10달러

왜냐하면 [Buy Box](./buy-box-competitor-pricing.md) 가격이 원래 가격보다 크고, 제품이 다음 위치에 나열됩니다 [Buy Box](./buy-box-competitor-pricing.md) 가격.

규칙이 적용된 후의 최종 가격: 10달러

### Buy Box 가격 및 가격 출처 = 가격 및 20% 가격 감소

| 필드 | 설정 |
|----------|----|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot; 가격 사용 |
| [!UICONTROL Price Action] | 경쟁업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 감소 기준 |
| [!UICONTROL Apply] | 백분율로 적용 |
| [!UICONTROL Floor Adjustment Amount] | 20년 |

#### 제품 1

가격: 20달러

계산된 가격: 16달러

[Buy Box](./buy-box-competitor-pricing.md) Amazon 가격: 15달러

왜냐하면 [Buy Box](./buy-box-competitor-pricing.md) 가격은 계산된 값보다 작습니다. [가격](./floor-price.md)를 입력하면 Calculated에 제품이 나열됩니다 [가격](./floor-price.md).

규칙이 적용된 후의 최종 가격: 16달러

#### 제품 2

가격: 15달러

계산된 지표 [가격](./floor-price.md): 12달러

[Buy Box](./buy-box-competitor-pricing.md) Amazon 가격: 15달러

왜냐하면 [Buy Box](./buy-box-competitor-pricing.md) 가격이 계산된 값보다 큽니다. [가격](./floor-price.md)로 설정되면, 제품 목록은 [Buy Box](./buy-box-competitor-pricing.md) 가격.

규칙이 적용된 후의 최종 가격: 15달러

#### 제품 3

가격: 17달러

계산된 가격: 13.60달러

[Buy Box](./buy-box-competitor-pricing.md) Amazon 가격: 15달러

왜냐하면 [Buy Box](./buy-box-competitor-pricing.md) 가격이 계산된 값보다 큽니다. [가격](./floor-price.md)로 설정되면, 제품 목록은 [Buy Box](./buy-box-competitor-pricing.md) 가격.

규칙이 적용된 후의 최종 가격: 15달러

### 모든 경쟁사의 가격에서 가장 낮은 가격 및 모든 경쟁사의 제품 조건 사용

| 필드 | 설정 |
|----------|-----|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | 가장 낮은 경쟁업체 가격 사용 |
| [!UICONTROL Minimum Positive Feedback] | 모든 경쟁업체 가격 |
| [!UICONTROL Conditional Variance] | 모든 경쟁사의 제품 조건 사용 |
| [!UICONTROL Price Action] | 경쟁업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 일치 |

| 가격 | 조건 |
|----------|----|
| 17달러 | 새로 만들기 |
| 15달러 | 새로 만들기 |
| 14달러 | 사용됨; 아주 좋아요 |
| 13달러 | 사용됨; 좋아요 |

#### 제품 1

가격: 10달러

조건: 새로 만들기

새 조건에 대한 가장 낮은 경쟁사 가격은 15달러이므로, 이 제품은 15달러로 나열되어 있습니다.

규칙이 적용된 후의 최종 가격: 15달러

#### 제품 2

가격: 10달러

조건: 사용됨; 허용 가능

왜냐하면 [최저 경쟁사 가격](./lowest-competitor-pricing.md) 사용됨 조건의 경우 $13이고, 이 제품은 $13로 나열됩니다.

규칙이 적용된 후의 최종 가격: 13달러

### 천장 가격, 통화 변환 및 VAT를 결합한 지능형 가격 조정 규칙

| 필드 | 설정 |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | 10달러 |
| [!UICONTROL Currency conversion] | 1.25유로:1USD |

[천정 가격](./optional-ceiling-price.md) 유럽(VAT) 시장에서 다음을 수행합니다. $10 x 1.25 = $12.50

이 [상한가격](./optional-ceiling-price.md) 유럽(VAT) 시장에서 VAT가 계산되고 추가됩니다.

VAT 이후의 최종 가격: $12.50 x (1.1) = $13.75

### 복수 가격책정 규칙, 한도 가격, 통화 변환 및 VAT 결합

#### 지능형 가격책정 규칙(이전 예제의 경우)

| 필드 | 설정 |
|----------|----|
| 우선순위 | 1 |
| 부가세 | 10% |
| 천정 가격 출처 | 10달러 |
| 통화 전환 | 1.25유로:1USD |

[천정 가격](./optional-ceiling-price.md) 유럽(VAT) 시장에서 다음을 수행합니다. $10 x 1.25 = $12.50

VAT 이후의 최종 가격: $12.50 x (1.1) = $13.75

#### 표준 가격책정 규칙

| 필드 | 설정 |
|----------|-----|
| [!UICONTROL Priority] | 2개 |
| [!UICONTROL Price Action] | 증가 기준 |
| [!UICONTROL Apply] | 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 5달러 |

이 [상한가격](./optional-ceiling-price.md) 이 히트이면 지능형 가격책정 규칙 맨 위에 표준 가격책정 규칙이 적용됩니다.

표준 가격책정 규칙이 적용된 후의 최종 가격: $13.75 + $5.00 = $18.75

### 가격 조정

이 예제에서 가장 경쟁력 있는 가격은 Amazon을 보고 정의됩니다 [경쟁사의 최저 가격](./lowest-competitor-pricing.md) 95%의 긍정적인 피드백과 1,000개의 머천트 리뷰에 대한 최소 피드백 카운트가 있습니다.

![가격 조정 예](assets/amazon-price-adjustment-example.png)

이러한 매개 변수를 기반으로 이 검색을 실행한 후 경쟁 가격은 $25로 돌아옵니다.

여기에서는 세 가지가 있습니다 [가격 규칙 작업](./pricing-rule-actions.md) 가장 낮은 가격에 기반을 둔 선택.

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - 이 옵션은 [최저 경쟁사 가격](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - 이 옵션은 [최저 경쟁사 가격](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - 이 옵션은 매개 변수를 기반으로 한 가장 낮은 가격과 일치하도록 Amazon 목록 가격을 변경합니다. 이 예에서 Amazon의 가격은 $25입니다.</li></ul> |
| [!UICONTROL Apply] | 옵션: 백분율로 적용 / 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 적용할 할인에 대한 백분율 또는 고정 금액을 정의하는 숫자 값입니다. <br>이러한 선택 사항은 가장 낮은 가격을 취하여 $0.01로 설정하게 됩니다. |

### 가격

| 필드 | 설정 |
|----------|----|
| [!UICONTROL Floor Price Source] | 비용 = 5달러 |
| [!UICONTROL Floor Price Action] | 증가 기준 |
| [!UICONTROL Apply] | 백분율로 적용 |
| [!UICONTROL Floor Adjustment Amount] | 5개 |

[가격](./floor-price.md) 계산 = 현장 가격 출처 `$5` x 바닥 조정 금액 `5%` = $5.25

지능형 가격책정 규칙이 적용되면 비용이 5달러인 경우 이 특정 제품에 대해 목록 가격이 $5.25보다 낮아질 수 있습니다.
