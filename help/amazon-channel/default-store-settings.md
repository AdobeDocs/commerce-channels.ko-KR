---
title: 기본 저장소 설정
description: 기본 상거래 설정을 수정하여 스토어에 대한 Amazon Sales Channel을 사용자 지정합니다.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 기본 저장소 설정

스토어가 연결되고 첫 번째 목록 규칙, Amazon과 간의 데이터 동기화를 설정한 후 [!DNL Commerce] 시작. 필요에 따라 스토어를 사용자 정의할 수 있는 몇 가지 유형의 스토어 설정이 있습니다. 스토어 설정은 스토어에서 액세스됩니다 [대시보드](./amazon-store-dashboard.md).

저장소 설정에는 다음이 포함됩니다.

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - 제품 카탈로그와 [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Amazon 주문 관리 방법을 제어합니다.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Amazon에 나열할 수 있는 카탈로그 제품을 정의합니다.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - 적격 목록에 대해 Amazon 정가가 변경되는 방법을 정의합니다.

- **[!UICONTROL Store reports]** - [경쟁 제품 가격 분석](./competitive-price-analysis.md) 및 [목록 개선 사항](./listing-improvements.md).

- **[!UICONTROL Logs]** - [변경 내용 나열](./listing-changes-log.md) 및 [통신 오류](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - 에서 이메일 및 Amazon 판매 채널 스토어 이름 설정을 검토합니다. [!DNL Commerce] 관리자.

## 몇 가지 중요한 기본 설정

| 설정 | 기본값 | 설명 | 위치 |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | 해당 항목 만들기 [!DNL Commerce] Amazon에서 새 주문을 받을 때 주문하기 때문에 [[!DNL Commerce] 주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 워크플로입니다. 날짜 `Disabled`, Amazon orders는 검토를 위해 주문 정보를 가져오지만 주문은 [!DNL Amazon Seller Central] 계정입니다. | [주문 설정](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Amazon 주문의 고객 데이터를 [!DNL Commerce] 데이터베이스. 가져온 Amazon 주문은 게스트 체크아웃으로 처리됩니다. 을(를) 빌드하려면 [!DNL Commerce] 고객 데이터베이스입니다. 이 설정을 다음으로 변경해야 합니다. `Build New Customer Account`. | [주문 설정](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] Amazon의 자격 요구 사항을 충족하는 카탈로그 제품을 사용하여 Amazon에 자동으로 게시하고 Amazon 목록을 만듭니다. 제품을 수동으로 검토하고 게시하려면 이 설정을 로 변경해야 합니다. `Do Not Automatically List Eligible Products`. 수동 게시를 기다리는 제품이 [_나열 준비 완료_](./ready-to-list.md) 탭. | [제품 목록 작업](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Amazon 목록의 기반으로 사용되는 가격 소스 속성을 정의합니다. 를 사용하지 않으려면 [!DNL Commerce] `Price` 속성 가격책정 규칙의 기준이 되는 기준 가격으로서 이 설정을 다른 속성으로 변경해야 합니다. | [목록 가격](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | 상인은 모든 명령을 이행한다. Amazon에서 이행하는 방법을 사용하거나 이행 방법을 혼합하여 사용하는 경우 이 설정을 변경해야 합니다. | [이행한 사람](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | 모든 제품이 동일한 조건인 경우 Amazon 조건 옵션 중 하나를 선택하여 모든 제품을 표시할 수 있습니다. 카탈로그에 다른 조건(예: 신규, 사용 및 재생)의 제품이 포함되어 있는 경우 이 설정을 다음으로 변경해야 합니다. `Assign Condition Using Product Attribute` 및 매핑 [!DNL Commerce] Amazon 목록 조건에 대한 조건 속성. | [제품 목록 조건](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | 없음 | Amazon 판매 채널이 Amazon에 게시하는 제품을 결정하는 데 사용되는 규칙을 정의합니다. 이러한 규칙은 제품을 목록으로 포함하거나 제외하기 위한 간단하거나 복잡한 규칙을 만드는 많은 옵션을 제공합니다. | [목록 규칙](./listing-rules.md) |
| 가격책정 규칙 | 없음 | 정의된 가격과 다른 Amazon 목록 가격 속성 정의 _[!UICONTROL Magento Price Source]_(으)로 [목록 가격](./listing-price.md). 다음에 대해 목록 가격을 조정하려면 (상향 또는 하향)_[!UICONTROL Magento Price Source]_ 설정, 규칙 만들기. | [가격책정 규칙](./pricing-products.md) |

자세한 내용은 [스토어 설정](./ob-store-review.md).
