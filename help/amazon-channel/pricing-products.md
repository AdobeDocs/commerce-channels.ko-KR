---
title: Amazon 가격 관리
description: 가격책정 규칙을 사용하여 Amazon 목록의 가격을 Commerce 스토어와 다르게 설정할 수 있습니다.
feature: Sales Channels, Price Rules
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Amazon 가격 관리

Amazon 판매 채널을 사용하면 가격 규칙을 설정할 수 있으므로 [가격 목록](./listing-price.md)에서 정의된 **[!UICONTROL Magento Price Source]**&#x200B;과(와) 다른 Amazon 목록 가격을 설정할 수 있습니다. 여러 규칙을 스택하고 지능형 가격 책정을 사용하여 경쟁업체의 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [경쟁업체 최저 가격](./lowest-competitor-pricing.md)을 기준으로 Amazon 목록 가격을 조정할 수도 있습니다.

가격책정 규칙에는 두 가지 유형이 있습니다.

- [표준 가격 규칙](./standard-price-rules.md)
- [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)

  >[!IMPORTANT]
  >
  >Amazon 지역이 온보딩 중이므로 `Inactive` 상태로 설정된 경우 지능형 가격 조정 규칙이 제대로 작동하지 않습니다. 가격 계산은 배송 요금에 따라 다르며, 배송 요금을 Amazon에서 동기화하려면 해당 지역이 `Active` 상태여야 합니다.
  >
  >Amazon 계정에서 지역 상태를 업데이트하려면 설정 > 계정 정보 > 휴가 설정으로 이동합니다. [Amazon: 휴가 목록 상태](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620)를 참조하세요(판매자 중앙 로그인 필요).

이 기능을 사용하면 [!DNL Commerce] [카탈로그 가격 규칙](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html)과 유사한 방식으로 Amazon 가격을 조작할 수 있습니다. 특정 제품, 특정 카테고리 내의 제품 또는 특정 속성이 있는 제품의 가격을 변경할 수 있는 복잡한 규칙을 만들 수 있습니다.

Amazon 목록에 대한 가격 책정 규칙을 추가할 수 있습니다. 가격 규칙을 사용하여 정의된 조건 세트를 기준으로 목록 가격을 자동으로 조정할 수 있습니다. 가격 규칙은 트리거되어 제품이 Amazon에 나열되기 전에 조정된 가격을 계산합니다.

>[!NOTE]
>
>Amazon 목록의 가격 원본이 [목록 가격](./listing-price.md) 설정에서 **[!UICONTROL Magento Price Source]**&#x200B;에 대해 정의되어 있습니다. 가격책정 규칙에 정의된 모든 조정 계산은 가격 출처를 시작 값으로 사용합니다.

가격 규칙을 사용하면 [가격 표시](./listing-price.md) 설정에서 **[!UICONTROL Magento Price Source]**&#x200B;과(와) 다른 Amazon 목록 가격을 설정할 수 있습니다. 가격을 조정하기 위해 함께 작동하는 여러 규칙을 스택할 수도 있습니다.

가격책정/가격 조정 규칙을 설정하려면 설정하는 동안 세 가지 정보 세트가 필요합니다.

- [일반 설정](./pricing-rule-general-settings.md): 규칙의 이름, 설명, 활성 날짜, 우선 순위를 정의하고 우선 순위 설정을 기반으로 후속 규칙의 동작을 설정합니다.
- [조건](./pricing-rule-conditions.md): 가격 규칙에 적합한 제품을 결정하십시오.
- [작업](./pricing-rule-actions.md): 가격 원본에 적용되는 조정 계산을 정의하여 목록 가격을 결정합니다.

[가격 나열](./listing-price.md) 설정에서 선택한 **[!UICONTROL Magento Price Source]**&#x200B;에 대해 Amazon 목록 가격을 자동으로 조정하는 [표준 가격 규칙](./standard-price-rules.md)을 만들 수 있습니다. 이 기능을 사용하면 [!DNL Commerce] [카탈로그 가격 규칙](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html)과 유사한 방식으로 Amazon 가격을 조작할 수 있습니다. 특정 제품, 특정 카테고리 내의 제품 또는 특정 속성을 가진 제품의 가격을 자동으로 변경하는 복잡한 규칙을 만들 수 있습니다. 기존 설정을 완료하고 고정 금액 또는 백분율에 따라 제품의 가격을 높이거나 낮출 수 있습니다.

다른 강력한 도구는 경쟁업체 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [경쟁업체 최저 가격](./lowest-competitor-pricing.md)에 따라 Amazon 목록 가격을 조정하는 [지능형 가격 조정](./intelligent-repricing-rules.md) 기능입니다. [!DNL Commerce] [카탈로그 가격 규칙](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html)과(와) 유사한 이 고급 기능을 사용하면 복잡한 규칙을 만들어 Amazon 가격을 조작할 수 있습니다. 규칙은 특정 제품, 특정 카테고리 내의 제품 또는 특정 제품 속성이 있는 제품에 대한 가격 변경 범위를 정의할 수 있습니다.

지능형 가격 조정을 사용하여 경쟁업체의 가격을 기준으로 Amazon 목록 가격을 조정합니다. Amazon sales channel에는 마진을 보호하거나 낮은 피드백으로 판매자의 가격을 일치시키지 않도록 구성할 수 있는 보호 장치가 내장되어 있습니다. [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)을 사용하면 Amazon 목록 가격을 고정 금액 또는 백분율 금액(상향 또는 하향)로 자동으로 조작하거나 항목별로 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md)과 동기화할 수 있습니다. 규칙을 스택하여 무제한 유연성을 제공할 수도 있습니다.

활성/비활성 상태, 웹 사이트 자격, 선택적 날짜 범위 및 선택적 우선 순위 수준(규칙 스택에 사용됨)과 같은 규칙의 중요한 측면을 제어할 수 있습니다.

예를 들어 조건이 충족될 때 목록 가격이 Amazon으로 전송되기 전에 자동으로 조정되는 가격 규칙에 대한 조건을 정의하고 설정할 수 있습니다.

다른 가격 옵션은 개별 목록 수준에서 설정되는 [가격 재정의](./overrides.md)입니다. [가격 재정의](./overrides.md)을(를) 설정할 수 있으며 재정의는 다른 모든 기본값, 설정 및 규칙보다 우선 순위를 무시/가져옵니다. 가격, 처리 시간, 조건 및 판매자 노트에 대해 [override](./overrides.md)을(를) 설정할 수 있습니다(몇 가지 예외).

![가격 규칙](assets/amazon-pricing-rules.png){width="600" zoomable="yes"}

## 기본 열

| 열 | 설명 |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Name] | [가격 규칙 일반 설정](./pricing-rule-general-settings.md)에 설정된 가격 규칙 이름 |
| [!UICONTROL Rule Type] | [가격 규칙 작업](./pricing-rule-actions.md)에 설정된 규칙 유형(표준 가격 규칙 또는 지능형 가격 조정 규칙) |
| [!UICONTROL Is Active] | [가격 규칙 일반 설정](./pricing-rule-general-settings.md)에 설정된 대로 규칙이 활성 상태인지 여부 |
| [!UICONTROL Priority] | [가격 규칙 일반 설정](./pricing-rule-general-settings.md)에 설정된 다른 가격 조건보다 우선 순위 |
| [!UICONTROL Stop Further Rules Processing] | [가격 규칙 일반 설정](./pricing-rule-general-settings.md)에 설정된 대로 이 규칙에 적합한 제품에 대해 추가 가격 규칙이 처리되는지 여부를 나타냅니다. |
| [!UICONTROL From Date] | 규칙이 활성화된 기간의 시작 |
| [!UICONTROL To Date] | 규칙이 활성화된 기간의 끝 |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 모든 작업을 나열합니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을(를) 클릭합니다. 옵션: `Edit Price Rule` / `Delete Price Rule` |
