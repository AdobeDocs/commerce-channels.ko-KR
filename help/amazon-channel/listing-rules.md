---
title: 목록 규칙
description: 목록 사용 규칙에 따라 Amazon Marketplace 목록으로 게시되는 상거래 카탈로그 제품을 결정합니다.
redirect_from: /sales-channels/asc/ob-listing-rules.html/sales-channels/asc/ob-listing-preview.html/sales-channels/asc/listing-rule-preview.html
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 목록 규칙

에 저장할 목록 규칙에 액세스할 수 있습니다 [대시보드 저장](./amazon-store-dashboard.md).

목록 규칙은 Amazon 판매 채널이 Amazon에 게시하는 제품을 결정하는 규칙을 정의합니다. 이러한 규칙은 제품을 목록으로 포함하거나 제외하도록 간단한 규칙으로 복잡한 규칙을 만드는 많은 옵션을 제공합니다. 각 규칙은 제품 목록 자격에 대한 요구 사항을 설정하는 조건으로 구성됩니다.

목록 규칙은 계속 과 동기화됩니다 [!DNL Commerce] 카탈로그 새로 추가할 때 [!DNL Commerce] 목록 규칙에서 설정한 자격 요구 사항을 충족하는 제품은 Amazon에서 목록을 위해 자동으로 처리됩니다.

- 모든 제품을 Amazon 목록에 게시하려면 목록 규칙에 조건을 정의하지 마십시오.

- Amazon에 게시되는 카탈로그 제품 중 하나를 제한하려면 목록 규칙 조건을 정의합니다. Amazon 목록 규칙에 대한 조건을 정의하는 것은 조건을 정의하는 것과 동일한 논리 및 프로세스를 따릅니다 [장바구니 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

- 목록 규칙에서 제품을 제외하는 경우, 해당 제품의 자격 상태는 `Ineligible`. 부적격 제품은 Amazon에 게시되지 않습니다.

- 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 과 일치시키는 경우 [!DNL Commerce] 카탈로그 제품, 변경 사항이 나열된 Amazon의 수량 `0` 제품의 판매를 막기 위해. Amazon 목록 [수동으로 제거](./end-listings-manually.md).

수량 및 자격 상태 변경 사항은 동일한 지역(에 정의됨)에서 판매하기 위해 존재하는 시장에서 Amazon 판매자 SKU를 공유하는 모든 목록에 영향을 줍니다 _[!UICONTROL Amazon Marketplace Country]_기간 [스토어 통합](./store-integration.md)). 그러나 공유로 변경 [!DNL Amazon Seller SKU] 한 지역에서는 다른 국가의 제품 Amazon 목록에 영향을 주지 않습니다.

![목록 규칙](assets/ob-listing-rules.png)

## 목록 규칙 설정 구성

1. 클릭 **[!UICONTROL Listing Rules]** 저장 대시보드에서

1. Amazon에 나열할 제품 자격에 대해 원하는 조건을 정의합니다.

자세한 내용은 [예: 조건 정의](./ob-define-condition-example.md).

| 필드 | 설명 |
|---|---|
| [!UICONTROL Websites] | 사용 가능한 옵션은 [웹 사이트](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} 님이 [!DNL Commerce] 구성. Amazon에 나열된 적합한 제품에 대한 웹 사이트를 선택합니다. 각 웹 사이트에는 Amazon 판매 채널에서 만든 고유한 Amazon 스토어가 필요하므로 하나의 웹 사이트만 선택할 수 있습니다. |
| [!UICONTROL Conditions] | 을(를) 정의하는 데 사용됩니다. [!DNL Commerce] Amazon 지역 내의 제품 자격에 대한 속성입니다. 자세한 내용은 [예: 조건 정의](./ob-define-condition-example.md). |

## 조건 작업 공간

굵게 표시된 조건에 있는 모든 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

- 선택한 웹 사이트 내의 모든 제품이 적합한 경우 조건을 추가하지 마십시오.
- Amazon 시스템과 직접 통신할 수 있는 복잡한 백엔드 프로세스 세트가 있습니다. 표시하려는 항목 수와 Amazon 시스템의 사용 가능 여부(예: 블랙 프라이데이)를 기준으로 항목을 Amazon에 나열하는 데 시간이 걸릴 수 있습니다.

조건에 대한 자세한 내용은 [조건 설명](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}.

## 목록 규칙 미리 보기

목록 규칙에 대한 조건 정의를 수정하는 경우 **[!UICONTROL Preview Changes]** 규칙 변경 사항을 적용하고 목록의 영향을 받는 방법을 확인하십시오. 목록 규칙 변경 사항을 저장하기 전에 이 목록 미리 보기 기능에서 목록을 확인합니다.

Amazon 목록이 규칙 및 정의된 조건과 비교됩니다. 그런 다음 다음을 검토할 수 있습니다.

- 현재 상태에 따라 부적격 상태로 이동하는 제품 [!DNL Amazon Seller Central] account
- 부적격 상태에서 다시 적격 상태로 이동하는 제품
- 자격 조건을 갖춘 Amazon 목록에서 새 Amazon 목록에 추가되는 제품은 무엇입니까? [!DNL Commerce] products

목록 미리 보기를 사용하면 잠재적인 Amazon 목록을 미리 보고 목록 규칙에 필요한 조정을 수행할 수 있습니다.

잠재적인 Amazon 목록이 _[!UICONTROL Listing Preview]_세 개의 탭 중 하나에 있는 페이지:

- **[!UICONTROL Ineligible Listings]** - 나열된 제품은 현재 목록 규칙 및 조건을 기준으로 Amazon 목록에 사용할 수 없습니다.

   부적격 제품은 Amazon에 게시되지 않습니다. 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 과 일치시키는 경우 [!DNL Commerce] 카탈로그 제품, 변경 사항이 나열된 Amazon의 수량 `0` 제품의 판매를 막기 위해. 목록을 수동으로 제거하려면 다음을 참조하십시오 [Amazon 목록 종료](./end-listings-manually.md). Amazon 요구 사항에 맞지 않는 제품은 여기에 나열되어 있지 않습니다. 이러한 제품들은 [비활성 목록 탭](./inactive-listings.md).

- **[!UICONTROL Eligible Listings]** - 나열된 제품은 현재 목록 규칙 및 조건을 기반으로 Amazon 목록에 포함될 수 있으며 Amazon 요구 사항도 적용할 수 있습니다. 이 목록에는 가져오는 기존 Amazon 목록이 포함되어 있습니다(있는 경우) **타사 목록 가져오기** 설정 `Import Listing` in [목록 설정](./third-party-listing-settings.md)).

- **[!UICONTROL New Listings]** - 나열된 제품에는 [!DNL Commerce] 현재 목록 규칙 및 조건을 기반으로 Amazon 목록에 새로 적합한 카탈로그 제품을 만들고 새 Amazon 목록을 만들고 게시합니다.

### 목록 미리 보기 보기 보기

1. 클릭 **[!UICONTROL Listing Rules]** 저장 대시보드에서

1. 보기 또는 추가 [목록 규칙](./listing-rules.md).

1. 수정 [규칙 조건 나열](./ob-define-condition-example.md).

1. 클릭 **[!UICONTROL Preview Changes]**.

1. 에서 목록을 검토하고 확인합니다. _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_, 및 _[!UICONTROL New Listings]_탭.

1. 목록이 예상과 일치하는 경우 **[!UICONTROL Save and close]**.

   목록이 예상대로 표시되지 않으면 **[!UICONTROL Back]** 목록이 기대에 부합될 때까지 규칙과 조건을 수정합니다.

![목록 규칙 미리 보기](assets/amazon-listing-rule-preview.png)

### 미리 보기 레코드 나열

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Product ID] | 에 할당된 고유한 순차적 번호 [!DNL Commerce] 카탈로그 제품을 추가할 때 사용합니다. |
| [!UICONTROL Thumbnail] | 기본 제품 이미지의 축소판을 표시합니다. |
| [!UICONTROL Name] | 에서 관리되는 제품의 이름 [!DNL Commerce] [제품 표](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Type] | 에서 관리되는 제품 유형입니다. [!DNL Commerce] products 표. |
| [!UICONTROL Attribute Set] | 제품의 템플릿으로 사용되는 속성 집합에서 관리되는 이름입니다. [!DNL Commerce] products 표. |
| [!UICONTROL SKU] | 제품에서 관리되는 제품에 할당된 고유한 재고 유지 단위입니다. [!DNL Commerce] products 표. |
| [!UICONTROL Visibility] | 제품에서 표시되는 위치를 나타내며, [!DNL Commerce] products 표. 옵션:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| 상태 | 제품의 상태를 나타내며, [!DNL Commerce] products 표. 옵션: `Enabled` / `Disabled` |

![미리 보기 워크플로우 나열](assets/listing-preview-flowchart.png)
