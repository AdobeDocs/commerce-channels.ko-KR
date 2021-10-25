---
title: Amazon 가격 관리
description: 가격 규칙을 사용하여 Amazon 목록과 COmbox 스토어에 대한 가격을 설정할 수 있습니다.
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Amazon 가격 관리

Amazon 판매 채널을 사용하면 정의된 가격과 다른 Amazon 목록 가격을 설정할 수 있는 가격 규칙을 설정할 수 있습니다 **[!UICONTROL Magento Price Source]** 다음 위치에서 [가격 목록](./listing-price.md). 또한 여러 규칙을 스택하고 지능형 가격 책정 기능을 사용하여 경쟁업체의 경쟁 제품에 따라 Amazon 목록 가격을 조정할 수도 있습니다 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [최저 경쟁사 가격](./lowest-competitor-pricing.md).

가격책정 규칙에는 두 가지 유형이 있습니다.

- [표준 가격책정 규칙](./standard-price-rules.md)
- [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >Amazon 지역이 `Inactive` 상태, 온보딩 중임. 가격 계산은 배송비에 따라 다르며 해당 지역은 다음 위치에 있어야 합니다 `Active` Amazon에서 동기화할 배송 요금에 대한 상태입니다.
   >
   >Amazon 계정에서 지역 상태를 업데이트하려면 설정 > 계정 정보 > 휴가 설정으로 이동합니다. 을(를) 참조하십시오. [Amazon: 휴가 상태 나열](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){target=&quot;_blank&quot;}(판매자 중앙 로그인 필요).

이 기능을 사용하면 Amazon 가격을 과 유사한 방식으로 조작할 수 있습니다 [!DNL Commerce] [카탈로그 가격 규칙](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}. 특정 제품, 특정 카테고리 내의 제품 또는 특정 속성에 대한 제품 가격을 변경할 수 있는 복잡한 규칙을 만들 수 있습니다.

Amazon 목록에 대한 가격 규칙을 추가할 수 있습니다. 가격 규칙을 사용하여 정의된 조건 세트에 따라 목록 가격을 자동으로 조정할 수 있습니다. 가격 규칙이 트리거되고 제품이 Amazon에 나열되기 전에 조정된 가격을 계산합니다.

>[!NOTE]
>
>Amazon 목록의 가격 소스는 다음에 정의되어 있습니다 **[!UICONTROL Magento Price Source]** 다음 위치에서 [가격 목록](./listing-price.md) 설정. 가격책정 규칙에 정의된 모든 조정 계산은 가격 출처를 시작 값으로 사용합니다.

가격 규칙을 사용하면 Amazon 목록 가격이 **[!UICONTROL Magento Price Source]** 다음 위치에서 [가격 목록](./listing-price.md) 설정. 함께 작동하는 여러 규칙을 스택하여 가격을 조정할 수도 있습니다.

가격책정/가격 조정 규칙은 설정 중에 세 세트의 정보를 필요로 합니다.

- [일반 설정](./pricing-rule-general-settings.md): 규칙의 이름, 설명, 활성 날짜, 우선 순위를 정의하고 해당 우선 순위 설정을 기반으로 후속 규칙의 동작을 설정합니다.
- [조건](./pricing-rule-conditions.md): 가격 규칙에 적합한 제품을 결정합니다.
- [작업](./pricing-rule-actions.md): 가격 출처에 적용되는 조정 계산을 정의하여 목록 가격을 결정합니다.

다음을 만들 수 있습니다 [표준 가격 규칙](./standard-price-rules.md) 선택한 항목에 따라 Amazon 목록 가격이 자동으로 조정됩니다 **[!UICONTROL Magento Price Source]** 다음 위치에서 [가격 목록](./listing-price.md) 설정. 이 기능을 사용하면 Amazon 가격을 과 유사한 방식으로 조작할 수 있습니다 [!DNL Commerce] [카탈로그 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;}. 특정 제품, 특정 카테고리 내의 제품 또는 특정 속성을 갖는 제품에 대한 가격을 자동으로 변경하는 복잡한 규칙을 만들 수 있습니다. 기존 설정을 완료하고 고정 금액 또는 백분율에 따라 제품 가격을 인상하거나 내릴 수 있습니다.

또 다른 강력한 도구는 [지능형 가격 조정](./intelligent-repricing-rules.md) 경쟁사를 기반으로 Amazon 목록 가격을 조정하는 기능 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md). 와 비슷합니다 [!DNL Commerce] [카탈로그 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} 이 고급 기능을 사용하면 복잡한 규칙을 만들어 Amazon 가격을 조작할 수 있습니다. 규칙은 특정 제품, 특정 카테고리 내의 제품 또는 특정 제품 속성에 대한 가격 변경의 범위를 정의할 수 있습니다.

지능형 가격 조정 기능을 사용하여 경쟁업체의 가격에 따라 Amazon 목록 가격을 조정합니다. Amazon 판매 채널에는 마진을 보호하거나 낮은 피드백이 있는 상인의 가격과 일치하지 않도록 구성할 수 있는 보호 장치가 내장되어 있습니다. 사용 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md), Amazon 목록 가격은 고정 또는 비율(상향 또는 하향) 또는 과 동기화되어 자동으로 조작할 수 있습니다 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 가격 또는 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md) 품목별로. 규칙을 스택하여 무제한 유연성을 제공할 수도 있습니다.

활성/비활성 상태, 웹 사이트 자격, 선택적 날짜 범위 및 선택적 우선순위 수준(규칙 스택에 사용됨)과 같은 규칙의 중요한 측면을 제어할 수 있습니다.

예를 들어, 조건이 충족될 경우 Amazon으로 전송되기 전에 목록 가격을 자동으로 조정하는 가격 규칙에 대한 조건을 정의하고 설정할 수 있습니다.

다른 가격 옵션은 다음과 같습니다 [가격 대체](./overrides.md): 개별 목록 수준에서 설정됩니다. A [가격 대체](./overrides.md) 를 설정할 수 있고, 무시는 다른 모든 기본값, 설정 및 규칙보다 우선 순위가 높습니다. An [재정의](./overrides.md) 가격, 처리 시간, 조건 및 판매자 노트에 대해 설정할 수 있습니다(몇 가지 예외 포함).

![가격 규칙](assets/amazon-pricing-rules.png)

## 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Name] | 에 설정된 대로 가격책정 규칙의 이름입니다. [가격책정 규칙 일반 설정](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | 에 설정된 대로 규칙 유형 [가격책정 규칙 조치](./pricing-rule-actions.md) (표준 가격 규칙 또는 지능형 가격 규칙) |
| [!UICONTROL Is Active] | 에 설정된 대로 규칙이 활성 상태인지 여부 [가격책정 규칙 일반 설정](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | 에 설정된 다른 가격 조건보다 우선합니다. [가격책정 규칙 일반 설정](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | 에 설정된 대로 이 규칙에 적합한 제품에서 추가 가격 규칙이 처리되는지 여부를 나타냅니다. [가격 규칙 일반 설정](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | 규칙이 활성화된 기간의 시작 |
| [!UICONTROL To Date] | 규칙이 활성화된 기간의 종료 |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 모든 작업을 나열합니다. 작업을 적용하려면 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열. 옵션: `Edit Price Rule` / `Delete Price Rule` |
