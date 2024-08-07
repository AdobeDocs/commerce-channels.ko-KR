---
title: Amazon 판매 채널 - 가격 규칙 예
description: Amazon 목록의 가격 책정 규칙을 디자인하는 데 도움이 되도록 일반적인 시나리오를 기반으로 이러한 예제를 검토하십시오.
feature: Sales Channels, Price Rules
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# 가격 규칙 예

## 표준 가격 규칙 예

### 후속 규칙 버리기

후속 규칙을 폐기하는 기능은 여러 가격책정 규칙이 누적되어 의도하지 않은 추가 할인을 제공하는 것을 방지하는 가격책정 규칙 내의 큰 기능입니다. 후속 규칙을 삭제하려면 [가격 규칙 일반 설정](./pricing-rule-general-settings.md)의 _[!UICONTROL Priority]_섹션에 설정된 우선 순위를 가격 규칙에 사용해야 합니다.

**[!UICONTROL Discard Subsequent Rules]**&#x200B;이(가) `Yes`(으)로 설정된 경우 우선순위가 낮은(높은 숫자) 규칙이 적합한 제품에 적용되지 않습니다.

예를 들어 세 가지 가격 규칙이 있다고 가정해 보겠습니다.

| 예 | 규칙 이름 | 우선 순위 | 후속 규칙 버리기 |
|---------|-----------------------|----------|-------------------------|
| 1 | 10% 할인 판매 제품 | 1 | 아니요 |
| 2 | $2 할인 판매 제품 | 2 | 예 |
| 3 | 모든 제품 5% 할인 | 3 | 아니요 |

이 시나리오에서는 규칙 #1 및 #2가 적격 제품에 적용됩니다. 규칙 #3은 예제 #2보다 우선 순위가 낮고 **[!UICONTROL Discard Subsequent Rules]**&#x200B;이(가) `Yes`(으)로 설정되어 있으므로 규칙 #2 내에 포함되지 않은 적격 제품에만 적용됩니다. 따라서 판매 범주에 속하는 적격 제품은 Amazon 상장 가격에서 10% 할인 및 $2 할인됩니다.

### 두 가지 표준 가격 규칙 적용

| 필드 | 설정 - 규칙 1 | 설정 - 규칙 2 |
|--------------------------------|---------------------|-----------------------|
| [!UICONTROL Rule Name] | 규칙-1 | 규칙-2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | 표준 가격 규칙 | 표준 가격 규칙 |
| [!UICONTROL Price action] | 감소 기준 | 감소 기준 |
| [!UICONTROL Apply] | 백분율로 적용 | 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### 제품 1

가격: $45.49

규칙 1 적용됨: $45.49 x (0.9) = $40.94

규칙 2 적용됨: $40.94 - $10.00 = $30.94

규칙 1과 규칙 2가 적용된 후의 최종 가격: $30.94

#### 제품 2

가격: $47.76

규칙 1 적용됨: $47.76 x (0.9) = $42.98

규칙 2 적용됨: $42.98 - $10.00 = $32.98

규칙 1과 규칙 2가 적용된 최종 가격: $32.98

## 지능형 가격 조정 규칙 예

### Buy Box 가격(현장 가격 포함) Source = 가격

| 필드 | 설정 |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot; 가격 사용 |
| [!UICONTROL Price Action] | 경쟁 업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 일치 |

#### 제품 1

가격: $15

Amazon의 [Buy Box](./buy-box-competitor-pricing.md) 가격: $10

[Buy Box](./buy-box-competitor-pricing.md) 가격이 원래 가격보다 낮으므로 제품이 원래 가격으로 나열됩니다.

규칙이 적용된 후 최종 가격: $15

#### 제품 2

가격: $5

Amazon의 [Buy Box](./buy-box-competitor-pricing.md) 가격: $10

[Buy Box](./buy-box-competitor-pricing.md) 가격이 원래 가격보다 높으므로 제품이 [Buy Box](./buy-box-competitor-pricing.md) 가격으로 나열됩니다.

규칙이 적용된 후 최종 가격: $10

### Buy Box 가격(현장 가격) Source = 가격 및 20% 가격 인하

| 필드 | 설정 |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot; 가격 사용 |
| [!UICONTROL Price Action] | 경쟁 업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 감소 기준 |
| [!UICONTROL Apply] | 백분율로 적용 |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### 제품 1

가격: $20

계산된 현장 가격: $16

[Buy Box](./buy-box-competitor-pricing.md) 가격(Amazon 기준): $15

[Buy Box](./buy-box-competitor-pricing.md) 가격이 계산된 [최저가](./floor-price.md)보다 낮으므로 제품은 계산된 [최저가](./floor-price.md)에 나열됩니다.

규칙이 적용된 후 최종 가격: $16

#### 제품 2

가격: $15

계산된 [최저 가격](./floor-price.md): $12

[Buy Box](./buy-box-competitor-pricing.md) 가격(Amazon 기준): $15

[Buy Box](./buy-box-competitor-pricing.md) 가격이 계산된 [기본 가격](./floor-price.md)보다 크므로 제품이 [Buy Box](./buy-box-competitor-pricing.md) 가격으로 나열됩니다.

규칙이 적용된 후 최종 가격: $15

#### 제품 3

가격: $17

계산된 현장 가격: $13.60

[Buy Box](./buy-box-competitor-pricing.md) 가격(Amazon 기준): $15

[Buy Box](./buy-box-competitor-pricing.md) 가격이 계산된 [기본 가격](./floor-price.md)보다 크므로 제품이 [Buy Box](./buy-box-competitor-pricing.md) 가격으로 나열됩니다.

규칙이 적용된 후 최종 가격: $15

### 모든 경쟁사의 가격과 모든 경쟁사의 제품 조건을 사용하는 최저 가격

| 필드 | 설정 |
|----------------------------------------|-----------------------------------------|
| [!UICONTROL Rule Name] | 규칙-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | 지능형 가격 조정 규칙 |
| [!UICONTROL Competitor Price Source] | 경쟁사 최저 가격 사용 |
| [!UICONTROL Minimum Positive Feedback] | 모든 경쟁사 가격 |
| [!UICONTROL Conditional Variance] | 모든 경쟁업체의 제품 조건 사용 |
| [!UICONTROL Price Action] | 경쟁 업체 가격 일치 |
| [!UICONTROL Floor Price Source] | 가격 |
| [!UICONTROL Floor Price Action] | 일치 |

| 가격 | 조건 |
|-------|-----------------|
| 17달러 | 신규 |
| 15달러 | 신규 |
| 14달러 | 사용됨, 매우 좋음 |
| 13달러 | 사용됨, 양호 |

#### 제품 1

가격: $10

조건: 새로 만들기

New 조건의 최저 경쟁자 가격이 $15이기 때문에 제품은 $15로 표시됩니다.

규칙이 적용된 후 최종 가격: $15

#### 제품 2

가격: $10

조건: 사용됨, 수락됨

사용된 조건에 대한 [경쟁사 최저 가격](./lowest-competitor-pricing.md)이(가) $13이므로 제품이 $13으로 표시됩니다.

규칙이 적용된 후 최종 가격: $13

### 천정 가격, 통화 전환 및 VAT를 결합한 지능형 가격 조정 규칙

| 필드 | 설정 |
|-----------------------------------|---------------|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | 10달러 |
| [!UICONTROL Currency conversion] | 1.25유로:1USD |

[유럽(VAT) 시장의 천정 가격](./optional-ceiling-price.md): $10 x 1.25 = $12.50

유럽(VAT) 시장의 [상한가](./optional-ceiling-price.md)에 도달하면 VAT가 계산되어 추가됩니다.

VAT 이후 최종 가격: $12.50 x (1.1) = $13.75

### 여러 가격책정 규칙, 한도 가격, 통화 변환 및 VAT 결합

#### 지능형 가격 규칙(이전 예)

| 필드 | 설정 |
|----------------------|---------------|
| 우선 순위 | 1 |
| VAT | 10% |
| 최고 가격 자료 | 10달러 |
| 통화 전환 | 1.25유로:1USD |

[유럽(VAT) 시장의 천정 가격](./optional-ceiling-price.md): $10 x 1.25 = $12.50

VAT 이후 최종 가격: $12.50 x (1.1) = $13.75

#### 표준 가격 규칙

| 필드 | 설정 |
|--------------------------------|-----------------------|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | 증가 기준 |
| [!UICONTROL Apply] | 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 5.00달러 |

[상한 가격](./optional-ceiling-price.md)이 적중되면 지능형 가격 책정 규칙 위에 표준 가격 책정 규칙이 적용됩니다.

표준 가격 규칙이 적용된 후의 최종 가격: $13.75 + $5.00 = $18.75

### 가격 조정

이 예에서 가장 경쟁력 있는 가격은 95%의 긍정적인 피드백과 1,000개의 판매자 후기의 최소 피드백 수로 Amazon [경쟁사의 최저 가격](./lowest-competitor-pricing.md)을(를) 고려하여 정의됩니다.

![가격 조정 예](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

이러한 매개변수를 기반으로 이 검색을 실행한 후 경쟁력 있는 가격은 $25로 돌아옵니다.

여기에서는 이 최저가를 기준으로 세 가지 다른 [가격 규칙 작업](./pricing-rule-actions.md) 선택 사항이 있습니다.

| 필드 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | 옵션:<ul><li>**[!UICONTROL Decrease By]** - 이 옵션은 [경쟁사 최저 가격](./lowest-competitor-pricing.md)에 비해 목록 가격을 낮춥니다.</li><li>**[!UICONTROL Increase By]** - 이 옵션은 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md)에 비해 목록 가격을 높입니다.</li><li>**[!UICONTROL Match Competitor Price]** - 이 옵션은 매개 변수를 기반으로 최저가와 일치하도록 Amazon 목록 가격을 변경합니다. 이 예제에서 Amazon 목록 가격은 $25입니다.</li></ul> |
| [!UICONTROL Apply] | 옵션: 백분율로 적용 / 고정 금액으로 적용 |
| [!UICONTROL Adjustment Amount] | 할인율을 적용할 퍼센트 또는 고정 금액을 정의하는 숫자 값입니다. <br>이 항목을 선택하면 최저가를 적용해서 $0.01 이하로 설정됩니다. |

### 최저 가격

| 필드 | 설정 |
|--------------------------------------|---------------------|
| [!UICONTROL Floor Price Source] | 비용 = $5 |
| [!UICONTROL Floor Price Action] | 증가 기준 |
| [!UICONTROL Apply] | 백분율로 적용 |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[최저 가격](./floor-price.md) 계산 = 최저 가격 Source `$5` x 최저 조정 금액 `5%` = $5.25

인텔리전트 가격 책정 규칙이 적용되면 비용이 $5일 때 이 특정 제품에 대해 상장 가격이 $5.25보다 낮아질 수 있도록 합니다.
