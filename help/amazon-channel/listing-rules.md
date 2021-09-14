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

[대시보드](./amazon-store-dashboard.md)에 저장할 목록 규칙에 액세스할 수 있습니다.

목록 규칙은 Amazon 판매 채널이 Amazon에 게시하는 제품을 결정하는 규칙을 정의합니다. 이러한 규칙은 제품을 목록으로 포함하거나 제외하도록 간단한 규칙으로 복잡한 규칙을 만드는 많은 옵션을 제공합니다. 각 규칙은 제품 목록 자격에 대한 요구 사항을 설정하는 조건으로 구성됩니다.

목록 규칙은 [!DNL Commerce] 카탈로그와 계속 동기화됩니다. 목록 규칙에서 설정한 자격 요구 사항을 충족하는 새 [!DNL Commerce] 제품을 추가하면 제품이 Amazon에서 목록을 위해 자동으로 처리됩니다.

- 모든 제품을 Amazon 목록에 게시하려면 목록 규칙에 조건을 정의하지 마십시오.

- Amazon에 게시되는 카탈로그 제품 중 하나를 제한하려면 목록 규칙 조건을 정의합니다. Amazon 목록 규칙에 대한 조건을 정의하는 것은 [장바구니 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}에 대한 조건을 정의하는 것과 동일한 논리 및 프로세스를 따릅니다.

- 목록 규칙에서 제품을 제외하는 경우 해당 제품의 자격 상태가 `Ineligible`으로 변경됩니다. 부적격 제품은 Amazon에 게시되지 않습니다.

- 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 [!DNL Commerce] 카탈로그 제품에 일치시키는 경우 Amazon 목록 수량이 `0` (으)로 변경되어 제품 판매를 방지할 수 있습니다. Amazon 목록은 [수동으로 제거](./end-listings-manually.md)할 수 있습니다.

수량 및 자격 상태 변경 사항은 [스토어 통합](./store-integration.md) 동안 _[!UICONTROL Amazon Marketplace Country]_에 정의된 대로 동일한 지역에 판매하기 위해 있는 시장에서 Amazon 판매자 SKU를 공유하는 모든 목록에 영향을 줍니다. 그러나 한 지역에서 공유된 [!DNL Amazon Seller SKU] 을 변경해도 다른 국가의 제품 Amazon 목록에 영향을 주지 않습니다.

![목록 규칙](assets/ob-listing-rules.png)

## 목록 규칙 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Rules]** 을 클릭합니다.

1. Amazon에 나열할 제품 자격에 대해 원하는 조건을 정의합니다.

[예제: 조건](./ob-define-condition-example.md)을 정의합니다.

| 필드 | 설명 |
|---|---|
| [!UICONTROL Websites] | 사용 가능한 옵션은 [!DNL Commerce] 구성에서 설정한 [웹 사이트](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}에 따라 다릅니다. Amazon에 나열된 적합한 제품에 대한 웹 사이트를 선택합니다. 각 웹 사이트에는 Amazon 판매 채널에서 만든 고유한 Amazon 스토어가 필요하므로 하나의 웹 사이트만 선택할 수 있습니다. |
| [!UICONTROL Conditions] | Amazon 지역 내에서 제품 자격에 대한 [!DNL Commerce] 속성을 정의하는 데 사용됩니다. [예제: 조건](./ob-define-condition-example.md)을 정의합니다. |

## 조건 작업 공간

굵게 표시된 조건에 있는 모든 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

- 선택한 웹 사이트 내의 모든 제품이 적합한 경우 조건을 추가하지 마십시오.
- Amazon 시스템과 직접 통신할 수 있는 복잡한 백엔드 프로세스 세트가 있습니다. 표시하려는 항목 수와 Amazon 시스템의 사용 가능 여부(예: 블랙 프라이데이)를 기준으로 항목을 Amazon에 나열하는 데 시간이 걸릴 수 있습니다.

조건에 대한 자세한 내용은 [조건 설명](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}을 참조하십시오.

## 목록 규칙 미리 보기

목록 규칙에 대한 조건 정의를 수정하는 경우 **[!UICONTROL Preview Changes]** 을 클릭하여 규칙 변경 사항을 적용하고 목록의 영향을 받는 방식을 볼 수 있습니다. 목록 규칙 변경 사항을 저장하기 전에 이 목록 미리 보기 기능에서 목록을 확인합니다.

Amazon 목록이 규칙 및 정의된 조건과 비교됩니다. 그런 다음 다음을 검토할 수 있습니다.

- 현재 [!DNL Amazon Seller Central] 계정을 기반으로 부적격 상태로 이동하는 제품
- 부적격 상태에서 다시 적격 상태로 이동하는 제품
- 자격 조건을 갖춘 [!DNL Commerce] 제품에서 Amazon 목록에 추가된 새로운 Amazon 목록 제품

목록 미리 보기를 사용하면 잠재적인 Amazon 목록을 미리 보고 목록 규칙에 필요한 조정을 수행할 수 있습니다.

잠재적인 Amazon 목록이 다음 세 개의 탭 중 하나에 있는 _[!UICONTROL Listing Preview]_페이지에 채워집니다.

- **[!UICONTROL Ineligible Listings]** - 나열된 제품은 현재 목록 규칙 및 조건을 기준으로 Amazon 목록에 사용할 수 없습니다.

   부적격 제품은 Amazon에 게시되지 않습니다. 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 [!DNL Commerce] 카탈로그 제품에 일치시키는 경우 Amazon 목록 수량이 `0` (으)로 변경되어 제품 판매를 방지할 수 있습니다. 목록을 수동으로 제거하려면 [Amazon 목록 종료](./end-listings-manually.md)를 참조하십시오. Amazon 요구 사항에 맞지 않는 제품은 여기에 나열되어 있지 않습니다. 이러한 제품은 [비활성 목록 탭](./inactive-listings.md)에 나열되어 있습니다.

- **[!UICONTROL Eligible Listings]** - 나열된 제품은 현재 목록 규칙 및 조건을 기반으로 Amazon 목록에 포함될 수 있으며 Amazon 요구 사항도 적용할 수 있습니다. 이 목록에는 가져오는 기존 Amazon 목록이 포함되어 있습니다(**타사 목록 가져오기**&#x200B;가 [목록 설정](./third-party-listing-settings.md)에 `Import Listing`로 설정된 경우).

- **[!UICONTROL New Listings]** - 나열된 제품에는  [!DNL Commerce] 현재 목록 규칙 및 조건에 따라 Amazon 목록에 새로 적합한 카탈로그 제품이 포함되며 새 Amazon 목록을 만들고 게시합니다.

### 목록 미리 보기 보기 보기

1. 저장소 대시보드에서 **[!UICONTROL Listing Rules]** 을 클릭합니다.

1. [목록 규칙](./listing-rules.md)을 보거나 추가합니다.

1. [목록 규칙 조건](./ob-define-condition-example.md)을 수정합니다.

1. **[!UICONTROL Preview Changes]** 을 클릭합니다.

1. _[!UICONTROL Ineligible Listings]_,_[!UICONTROL Eligible Listings]_ 및 _[!UICONTROL New Listings]_탭에서 목록을 검토하고 확인합니다.

1. 목록이 예상과 일치하는 경우 **[!UICONTROL Save and close]** 을 클릭합니다.

   목록이 예상대로 표시되지 않으면 **[!UICONTROL Back]** 을 클릭하고 목록이 기대에 부합될 때까지 규칙과 조건을 수정하십시오.

![목록 규칙 미리 보기](assets/amazon-listing-rule-preview.png)

### 미리 보기 레코드 나열

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Product ID] | 추가된 [!DNL Commerce] 카탈로그 제품에 할당된 고유한 순차적 번호입니다. |
| [!UICONTROL Thumbnail] | 기본 제품 이미지의 축소판을 표시합니다. |
| [!UICONTROL Name] | [!DNL Commerce] [products 표](https://docs.magento.com/user-guide/catalog/products.html){target=&quot;_blank&quot;}에서 관리되는 제품의 이름입니다. |
| [!UICONTROL Type] | [!DNL Commerce] 제품 그리드에서 관리되는 제품 유형입니다. |
| [!UICONTROL Attribute Set] | [!DNL Commerce] 제품 그리드에서 관리되는 제품의 템플릿으로 사용되는 속성 세트의 이름입니다. |
| [!UICONTROL SKU] | [!DNL Commerce] 제품 그리드에서 관리되는 제품에 할당된 고유한 재고 유지 단위입니다. |
| [!UICONTROL Visibility] | [!DNL Commerce] 제품 그리드에서 관리되는 제품이 표시되는 위치를 나타냅니다. 옵션:<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| 상태 | [!DNL Commerce] 제품 그리드에서 관리되는 제품의 상태를 나타냅니다. 옵션: `Enabled` / `Disabled` |

![미리 보기 워크플로우 나열](assets/listing-preview-flowchart.png)
