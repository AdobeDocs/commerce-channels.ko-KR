---
title: Amazon 판매 채널 - 제품 목록 작업
description: 제품 목록 작업 설정을 사용하여 상거래 카탈로그와 Amazon의 상호 작용 방식을 정의합니다.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 제품 목록 작업

제품 목록 작업 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 카탈로그와 Amazon의 상호 작용 방식을 정의합니다. 이러한 설정은 다음과 같습니다.

- 다음의 경우 표시 [!DNL Commerce] Amazon 자격 요구 사항을 충족하는 카탈로그 제품은 [!DNL Amazon Seller Central] 목록을 만들 계정입니다.

- 주문에 대한 기본 처리 시간을 설정합니다. 이 값은 주문을 처리하고 출하하는 데 필요한 일수를 정의합니다. 예를 들어 2일 배송을 선택하는 경우 처리가 완료되고 패키지가 운송업자에게 전달될 때까지 해당 배송 통과 시간이 시작되지 않습니다. 총 배달 시간은 (처리 시간 + 수송 시간 + 임의 휴일)입니다.

## 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 _[!UICONTROL Product Listing Actions]_섹션.

1. 대상 **[!UICONTROL Automatic List Action]** (필수) 다음 옵션을 선택합니다.

   - `Automatically List Eligible Products` - (기본값) 원하는 시간 선택 [!DNL Commerce] Amazon의 자격 요구 사항을 충족하는 카탈로그 제품을 사용하여 Amazon에 자동으로 게시하고 Amazon 목록을 만듭니다.

   - `Do Not Automatically List Eligible Products` - 적격한 항목을 수동으로 선택할 때 선택 [!DNL Commerce] 제품 카탈로그를 만들고 Amazon 목록을 만듭니다. 이 옵션을 선택하면 목록 기준을 충족하고 필요한 모든 정보를 포함하는 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) Amazon 수동 게시 탭.

1. 대상 **[!UICONTROL Default Handling Time]** (필수) 선적 전 리드타임에 필요한 일수를 입력합니다.

   기본값은 입니다. `2` 일.

   >[!NOTE]
   >
   >이 기본 전달 시간 값은 Amazon 판매 채널을 통해 생성된 Amazon 목록에만 적용됩니다. 에서 만들어진 모든 Amazon 목록 [!DNL Amazon Seller Central] 계정은 Amazon에 설정된 기본 처리 시간을 사용합니다.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![제품 목록 작업](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | 옵션:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (권장) 원하는 시간을 선택합니다. [!DNL Commerce] Amazon의 자격 요구 사항을 충족하는 카탈로그 제품을 사용하여 Amazon에 자동으로 게시하고 Amazon 목록을 만듭니다. 이 옵션을 선택하면 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭이 표시되지 않습니다. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - 적격 여부를 수동으로 선택하려면 선택 [!DNL Commerce] 제품 카탈로그를 만들고 Amazon 목록을 만듭니다. 이 옵션을 선택하면 목록 기준을 충족하고 필요한 모든 정보를 포함하는 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 수동 게시 탭</li></ul> |
| [!UICONTROL Default Handling Time] | 일반적으로 주문을 처리하고 배송하는 데 걸리는 일 수를 나타내는 숫자 값입니다. 기본값은 입니다. `2`. 이 값은에서 만든 Amazon 목록에 사용됩니다. [!DNL Commerce] Amazon에 게시됩니다. 와 통합하기 전 Amazon 목록의 기본 처리 시간 [!DNL Commerce] 은 이 설정의 영향을 받지 않습니다.<br><br>Amazon 판매 채널에 정의된 값이 기존 Amazon 목록에 정의된 기본 처리 시간을 대체하지 않습니다. 다음과 같은 경우 **[!UICONTROL Handling Time Override]** 이 활성화되고 나면 주문에 대한 처리 시간이 여기에 정의된 값으로 되돌아갑니다.<br><br>처리 시간이 다른 제품이 있는 경우 제품별 수준에서 처리 시간 재정의를 만들 수 있습니다. 에서 시간 재정의 처리를 관리할 수 있습니다. [_[!UICONTROL Overrides]_](./overrides.md) 탭 - 제품 이행을 유연하게 관리할 수 있습니다. 에 처리 시간 재정의가 없는 경우 [!DNL Commerce] 제품의 경우 처리 시간 기본값은 Amazon 목록에 정의된 값입니다.<br><br>처리 시간 은 지역 속성입니다. 목록에 대한 값이 변경되면 변경 사항은 를 공유하는 모든 목록에 영향을 줍니다 [!DNL Amazon Seller SKU] 동일한 지역(에 정의됨)에 대해 존재하는 모든 Amazon 스토어에서 [스토어 통합](./store-integration.md)). 하지만 공유 값 변경 [!DNL Amazon Seller SKU] 북미 지역은 다른 지역을 정의한 스토어에 나열된 동일한 제품에 영향을 주지 않습니다. 생성 날짜가 가장 오래된 영역의 저장소는 기본 처리 시간 설정의 우선 순위를 제어합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
