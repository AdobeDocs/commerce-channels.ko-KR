---
title: Amazon 판매 채널 - 가격 규칙 작업
description: 가격 규칙 작업을 사용하여 가격 출처에 적용되는 조정 계산을 정의하여 Amazon 목록 가격을 결정합니다.
feature: Sales Channels, Price Rules
exl-id: c46bd5c2-7994-45b4-ae0c-9e473372c73a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 가격 규칙 작업

가격 규칙 조치는 목록 가격을 결정하기 위해 가격 출처에 적용되는 조정 계산을 정의합니다.

## 표준 가격 규칙

[표준 가격 규칙](./standard-price-rules.md)을(를) 사용하면 [!DNL Commerce] 카탈로그 가격(또는 가격 원본)과 비교하여 특정 비율이나 고정 달러 금액만큼 Amazon 목록 가격을 늘리거나 줄일 수 있습니다.

| 섹션 | 설명 |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./standard-price-rules.md) | 규칙 유형을 `Standard price rule`(으)로 설정합니다. |
| [[!UICONTROL Price Adjustment]](./standard-price-rules.md) | 가격 출처에 적용되는 조정 계산을 정의하여 목록 가격을 결정합니다 |

## 지능형 가격 조정 규칙

[지능형 가격 조정 규칙](./intelligent-repricing-rules.md)은(는) Amazon 경쟁사의 가격을 사용하여 목록 가격을 결정합니다. 경쟁업체는 Amazon에 나열하는 것과 동일한 제품을 나열하는 다른 판매자입니다.

| 섹션 | 설명 |
|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md) | 경쟁업체 가격 Source 및 피드백 요구 사항과 함께 규칙 유형을 `Intelligent repricing rule`(으)로 설정하십시오. |
| [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md) | 경쟁업체가 판매한 동일한 제품의 조건에 대한 차이를 정의합니다. |
| [[!UICONTROL Price Adjustment]](./price-adjustment.md) | 가격 출처에 적용되는 조정 계산을 정의하여 목록 가격을 결정합니다 |
| [[!UICONTROL Floor Price]](./floor-price.md) | 여러 가격책정 규칙이 목록 가격을 너무 낮게 설정하지 못하도록 제품에 대한 최저 가격을 정의합니다. |
| [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md) | 제품의 최고 가격을 정의하여 가격 경쟁력을 유지할 수 있습니다. |
