---
title: Amazon 판매 채널 - 제품 목록 작업
description: 제품 목록 작업 설정을 사용하여 Commerce 카탈로그와 Amazon의 상호 작용 방식을 정의합니다.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 제품 목록 작업

제품 목록 작업 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

이러한 설정은 카탈로그와 Amazon의 상호 작용 방식을 정의합니다. 이러한 설정은 다음과 같습니다.

- 목록을 만들기 위해 Amazon 자격 요구 사항을 충족하는 [!DNL Commerce] 카탈로그 제품을 [!DNL Amazon Seller Central] 계정에 자동으로 전송할지 여부를 지정하십시오.

- 주문에 대한 기본 처리 시간을 설정합니다. 이 값은 주문을 처리하고 출하하는 데 필요한 일수를 정의합니다. 예를 들어 2일 배송을 선택하는 경우 처리가 완료되고 패키지가 운송업자에게 전달될 때까지 해당 배송 통과 시간이 시작되지 않습니다. 총 배달 시간은 (처리 시간 + 수송 시간 + 임의 휴일)입니다.

## 설정 구성

1. 스토어 대시보드에서 **[!UICONTROL Listing Settings]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Product Listing Actions]_섹션을 확장합니다.

1. **[!UICONTROL Automatic List Action]**(필수)에 대해 다음 옵션을 선택하십시오.

   - `Automatically List Eligible Products` - (기본값) [!DNL Commerce] 카탈로그 제품(Amazon의 자격 요구 사항을 충족)을 Amazon에 자동으로 게시하고 Amazon 목록을 만들 때 선택합니다.

   - `Do Not Automatically List Eligible Products` - 적격한 [!DNL Commerce] 카탈로그 제품을 수동으로 선택하고 Amazon 목록을 만들 때 선택합니다. 선택하면 목록 기준을 충족하고 모든 필수 정보를 포함하는 카탈로그 제품이 Amazon에 수동으로 게시하기 위한 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭에 표시됩니다.

1. **[!UICONTROL Default Handling Time]**(필수)의 경우 선적 전 리드 타임에 필요한 일 수를 입력합니다.

   기본값은 `2`일입니다.

   >[!NOTE]
   >
   >이 기본 전달 시간 값은 Amazon 판매 채널을 통해 생성된 Amazon 목록에만 적용됩니다. [!DNL Amazon Seller Central] 계정에서 만든 모든 Amazon 목록은 Amazon에 설정된 기본 처리 시간을 사용합니다.

1. 완료되면 **[!UICONTROL Save listing settings]**&#x200B;을(를) 클릭합니다.

![제품 목록 작업](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | 옵션:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (권장) [!DNL Commerce] 카탈로그 제품(Amazon의 자격 요구 사항을 충족)을 Amazon에 자동으로 게시하고 Amazon 목록을 만들 때 선택합니다. 선택한 경우 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭이 표시되지 않습니다. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - 적격한 [!DNL Commerce] 카탈로그 제품을 수동으로 선택하고 Amazon 목록을 만들 때 선택합니다. 선택하면 목록 기준을 충족하고 필요한 모든 정보를 포함하는 카탈로그 제품이 수동 게시를 위해 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭에 표시됩니다.</li></ul> |
| [!UICONTROL Default Handling Time] | 일반적으로 주문을 처리하고 배송하는 데 걸리는 일 수를 나타내는 숫자 값입니다. 기본값은 `2`입니다. 이 값은 [!DNL Commerce]에서 만들어 Amazon에 게시한 Amazon 목록에 사용됩니다. [!DNL Commerce]과(와) 통합하기 전의 Amazon 목록에 대한 기본 처리 시간은 이 설정의 영향을 받지 않습니다.<br><br>Amazon 판매 채널에 정의된 값이 기존 Amazon 목록에 정의된 기본 처리 시간을 대체하지 않습니다. **[!UICONTROL Handling Time Override]**&#x200B;을(를) 사용하도록 설정한 후 제거하면 주문에 대한 처리 시간이 여기에 정의된 값으로 되돌아갑니다.<br><br>처리 시간이 다른 제품이 있는 경우 제품별 수준에서 처리 시간 재정의를 만들 수 있습니다. [_[!UICONTROL Overrides]_](./overrides.md) 탭에서 시간 재정의 처리를 관리할 수 있으므로 제품 이행을 유연하게 관리할 수 있습니다. 제품에 대한 [!DNL Commerce]에 처리 시간 재정의가 없는 경우 처리 시간 기본값은 Amazon 목록에 정의된 값입니다.<br><br>처리 시간은 지역 특성입니다. 목록에 대한 값이 변경되면 변경 사항은 동일한 지역([스토어 통합](./store-integration.md)에 정의됨)에 대해 존재하는 모든 Amazon 스토어에서 [!DNL Amazon Seller SKU]을(를) 공유하는 모든 목록에 영향을 줍니다. 그러나 북미 지역에서 공유 [!DNL Amazon Seller SKU]의 값을 변경해도 다른 정의된 지역이 있는 스토어에 나열된 동일한 제품에는 영향을 주지 않습니다. 생성 날짜가 가장 오래된 영역의 저장소는 기본 처리 시간 설정의 우선 순위를 제어합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
