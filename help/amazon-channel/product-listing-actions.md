---
title: 제품 목록 작업
description: 제품 목록 작업 설정을 사용하여 상거래 카탈로그가 Amazon과 상호 작용하는 방법을 정의합니다.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# 제품 목록 작업

제품 목록 작업 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스합니다.

이러한 설정은 카탈로그가 Amazon과 상호 작용하는 방식을 정의합니다. 다음 설정:

- Amazon 자격 조건을 충족하는 [!DNL Commerce] 카탈로그 제품이 자동으로 [!DNL Amazon Seller Central] 계정으로 전송되어 목록을 작성하는지 여부를 나타냅니다.

- 주문에 대한 기본 처리 시간을 설정합니다. 이 값은 주문을 처리하고 출하하는 데 필요한 일수를 정의합니다. 예를 들어, 2일 배송을 선택하면 처리가 완료되고 패키지가 운송업체에 전달될 때까지 해당 배송 시간이 시작되지 않습니다. 총 배달 시간은 (처리 시간 + 전송 시간 + 휴일)입니다.

## 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. _[!UICONTROL Product Listing Actions]_섹션을 확장합니다.

1. **[!UICONTROL Automatic List Action]**(필수)에 대해 다음 옵션을 선택합니다.

   - `Automatically List Eligible Products` - (기본값)  [!DNL Commerce] 카탈로그 제품(Amazon의 자격 조건을 충족하는)이 자동으로 Amazon에 게시하고 Amazon 목록을 만들 시기를 선택합니다.

   - `Do Not Automatically List Eligible Products` - 적합한  [!DNL Commerce] 카탈로그 제품을 수동으로 선택하고 Amazon 목록을 만들 시기를 선택합니다. 선택한 경우, 목록 기준을 충족하고 모든 필수 정보가 포함된 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭에 표시되어 Amazon에 수동으로 게시합니다.

1. **[!UICONTROL Default Handling Time]**&#x200B;에 대해 선적 전 리드 타임에 필요한 일수를 입력합니다(필수).

   기본값은 `2`일입니다.

   >[!NOTE]
   >
   >이 기본 처리 시간 값은 Amazon 판매 채널을 통해 작성된 Amazon 목록에만 적용됩니다. [!DNL Amazon Seller Central] 계정에서 만든 모든 Amazon 목록은 Amazon에 설정된 기본 처리 시간을 사용합니다.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![제품 목록 작업](assets/amazon-product-listing-actions.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Automatic List Action] | 옵션:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (권장)  [!DNL Commerce] 카탈로그 제품(Amazon의 자격 조건을 충족하는)이 자동으로 Amazon에 게시되고 Amazon 목록을 만들 시기를 선택합니다. 선택한 경우 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭이 표시되지 않습니다. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - 적합한  [!DNL Commerce] 카탈로그 제품을 수동으로 선택하고 Amazon 목록을 만들 시기를 선택합니다. 이 옵션을 선택하면 목록 기준을 충족하고 모든 필수 정보가 포함된 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭에 표시되어 수동 게시합니다.</li></ul> |
| [!UICONTROL Default Handling Time] | 일반적으로 주문을 처리하고 출하하는 데 걸리는 일 수를 나타내는 숫자 값입니다. 기본값은 `2`입니다. 이 값은 [!DNL Commerce]에서 만들어지고 Amazon에 게시된 Amazon 목록에 사용됩니다. [!DNL Commerce]과 통합하기 전에 Amazon 목록에 대한 기본 처리 시간은 이 설정의 영향을 받지 않습니다.<br><br>Amazon 판매 채널에 정의된 값이 기존 Amazon 목록에 정의된 기본 처리 시간을 대체하지 않습니다. **[!UICONTROL Handling Time Override]**&#x200B;이 활성화되고 제거되면 주문에 대한 처리 시간은 여기에 정의된 값으로 되돌아갑니다.<br><br>처리 시간이 다른 제품이 있는 경우 제품별 수준에서 처리 시간 무시 를 만들 수 있습니다. [_[!UICONTROL Overrides]_](./overrides.md) 탭에서 처리 시간 변경을 관리할 수 있으므로 제품 완료를 관리할 수 있는 유연성을 제공합니다. 제품에 대한 [!DNL Commerce]에 처리 시간 재정의가 없는 경우 처리 시간 기본값은 Amazon 목록에 정의된 값입니다.<br><br>처리 시간은 지역 특성입니다. 목록에 대해 값이 변경되면 변경 사항은 동일한 지역( [스토어 통합](./store-integration.md)에 정의됨)에 대해 존재하는 모든 Amazon 저장소에서 [!DNL Amazon Seller SKU]을 공유하는 모든 목록에 영향을 줍니다. 그러나 북미 지역에서 공유 [!DNL Amazon Seller SKU] 값을 변경해도 정의된 다른 영역이 있는 저장소에 나열된 동일한 제품에 영향을 주지 않습니다. 생성 날짜가 가장 오래된 영역의 저장소는 기본 처리 시간 설정의 우선 순위를 제어합니다. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
