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

제품 목록 작업 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 카탈로그가 Amazon과 상호 작용하는 방식을 정의합니다. 다음 설정:

- 다음 중 [!DNL Commerce] Amazon 자격 요구 사항을 충족하는 카탈로그 제품은 자동으로 [!DNL Amazon Seller Central] 목록을 만들 계정입니다.

- 주문에 대한 기본 처리 시간을 설정합니다. 이 값은 주문을 처리하고 출하하는 데 필요한 일수를 정의합니다. 예를 들어, 2일 배송을 선택하면 처리가 완료되고 패키지가 운송업체에 전달될 때까지 해당 배송 시간이 시작되지 않습니다. 총 배달 시간은 (처리 시간 + 전송 시간 + 휴일)입니다.

## 설정 구성

1. 클릭 **[!UICONTROL Listing Settings]** 저장 대시보드에서

1. 를 확장합니다. _[!UICONTROL Product Listing Actions]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Automatic List Action]** (필수) 옵션을 선택합니다.

   - `Automatically List Eligible Products` - (기본값) 원하는 시점을 선택합니다 [!DNL Commerce] Amazon에 자동으로 게시하고 Amazon 목록을 만들 수 있는 카탈로그 제품(Amazon의 자격 조건을 충족하는 제품)입니다.

   - `Do Not Automatically List Eligible Products` - 자격 조건을 수동으로 선택하려면 선택합니다 [!DNL Commerce] 카탈로그 제품 및 Amazon 목록 만들기 선택한 경우, 목록 기준을 충족하고 모든 필수 정보를 포함하는 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) Amazon에 수동으로 게시하기 위한 탭입니다.

1. 대상 **[!UICONTROL Default Handling Time]** (필수) 선적 전 리드 타임에 필요한 일수를 입력합니다.

   기본값은 입니다. `2` 일 수.

   >[!NOTE]
   >
   >이 기본 처리 시간 값은 Amazon 판매 채널을 통해 작성된 Amazon 목록에만 적용됩니다. 에서 만든 모든 Amazon 목록 [!DNL Amazon Seller Central] 계정은 Amazon에 설정된 기본 처리 시간을 사용합니다.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save listing settings]**.

![제품 목록 작업](assets/amazon-product-listing-actions.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Automatic List Action] | 옵션:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (권장) 원하는 시기를 선택합니다 [!DNL Commerce] Amazon에 자동으로 게시하고 Amazon 목록을 만들 수 있는 카탈로그 제품(Amazon의 자격 조건을 충족하는 제품)입니다. 선택한 경우 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 탭이 표시되지 않습니다. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - 수동으로 적격 항목을 선택할 시점을 선택합니다 [!DNL Commerce] 카탈로그 제품을 만들고 Amazon 목록을 만듭니다. 선택한 경우, 목록 기준을 충족하고 모든 필수 정보를 포함하는 카탈로그 제품이 [_[!UICONTROL Ready to List]_](./ready-to-list.md) 수동 게시용 탭입니다.</li></ul> |
| [!UICONTROL Default Handling Time] | 일반적으로 주문을 처리하고 출하하는 데 걸리는 일 수를 나타내는 숫자 값입니다. 기본값은 입니다. `2`. 이 값은 에서 만든 Amazon 목록에 사용됩니다 [!DNL Commerce] Amazon에 게시했습니다. 와 통합하기 전에 Amazon 목록에 대한 기본 처리 시간입니다 [!DNL Commerce] 은 이 설정의 영향을 받지 않습니다.<br><br>Amazon 판매 채널에 정의된 값이 기존 Amazon 목록에 정의된 기본 처리 시간을 대체하지 않습니다. 다음의 경우 **[!UICONTROL Handling Time Override]** 이 활성화되고 제거되면 주문에 대한 처리 시간이 여기에 정의된 값으로 되돌아갑니다.<br><br>처리 시간이 다른 제품이 있는 경우 제품별 수준에서 처리 시간 무시 를 만들 수 있습니다. 에서 시간 무시 처리를 관리할 수 있습니다 [_[!UICONTROL Overrides]_](./overrides.md) 탭, 제품 이행 관리를 위한 유연성을 제공합니다. 에서 처리 시간 재정의가 없는 경우 [!DNL Commerce] 제품의 경우 처리 시간 기본값은 Amazon 목록에 정의된 값입니다.<br><br>처리 시간은 지역 특성입니다. 목록에 대해 값을 변경하면 변경 사항은 [!DNL Amazon Seller SKU] 동일한 영역( [스토어 통합](./store-integration.md)). 그러나 공유 값에 대한 값 변경 [!DNL Amazon Seller SKU] 북미 지역에서는 정의된 지역이 다른 스토어에 나열된 동일한 제품에 영향을 주지 않습니다. 생성 날짜가 가장 오래된 영역의 저장소는 기본 처리 시간 설정의 우선 순위를 제어합니다. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
