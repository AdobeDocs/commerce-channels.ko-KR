---
title: 별칭 Amazon 판매자 SKU 만들기
description: 별칭 Amazon 판매자 SKU를 사용하여 Commerce 카탈로그 제품에서 여러 지역 Amazon 목록을 만들 수 있습니다.
feature: Sales Channels, Products
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# 별칭 Amazon 판매자 SKU 만들기

[!DNL Alias Amazon Seller SKU]은(는) [!DNL Commerce] 카탈로그의 동일한 제품에서 Amazon 목록을 만드는 데 사용됩니다. 숙련된 Amazon 판매자인 경우 인벤토리 및 배송에 대한 [Amazon 글로벌 SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"} 및 마켓플레이스별 SKU에 익숙할 수 있습니다. Amazon 판매 채널에 대한 유사한 원칙에 따라 Amazon 판매자 SKU는 다중 지역 수준에서 제품 목록 정보를 제어하며 [!DNL Alias Amazon Seller SKU]을(를) 사용하여 지역별 수준에서 제품 목록 정보를 제어할 수 있습니다.

이 함수는 다음 두 가지 기능을 수행하는 데 사용할 수 있습니다.

- [!DNL Commerce] 카탈로그 제품 중 하나에 대한 [!DNL Alias Amazon Seller SKU]을(를) 만들어 지역별 목록 정보를 제어합니다.

  **예**: 미국과 캐나다 지역에서 판매자입니다. Amazon 판매 채널 스토어는 설정 중에 하나의 Amazon 영역만 할당할 수 있습니다. 따라서 미국 지역이 정의된 Amazon 판매 채널 스토어와 캐나다 지역이 정의된 다른 스토어가 있습니다. 두 매장은 [!DNL Commerce] 카탈로그를 공유하여 Amazon 판매자 SKU 및 ASIN 제품 특성을 포함한 두 지역의 정보를 나열합니다. 따라서 가격 책정, 재고/수량 및 기타 제품 속성을 공유하는 카탈로그 제품의 목록은 두 스토어에서 동일합니다. 그러나 캐나다 스토어의 재고는 캐나다 지역에서 배송되고 미국 스토어의 재고는 미국 지역에서 배송됩니다. 따라서 상장에 대한 상장 수량을 점포별로 구분하여 통제해야 한다. 이러한 유형의 지역별 제어를 수행하기 위해 별칭 Amazon 판매자 SKU를 만들 수 있습니다.

  기본적으로 동일한 카탈로그 제품에 연결되어 있고 해당 지역에서 동일한 목록을 다시 게시하는 데 사용할 수 있는 별칭 Amazon 판매자 SKU를 만들 수 있습니다.

- [!DNL Alias Amazon Seller SKU]을(를) 만들고 [!DNL Commerce] 카탈로그 제품 중 하나를 두 개의 Amazon 목록에 일치시키십시오.

  **예**: Amazon 목록과 일치하는 카탈로그 제품이 있습니다. Amazon에는 동일한 제품을 나타내는 여러 개의 목록이 자주 있으므로 동일한 제품에 대해 다른 Amazon 목록을 검색하지만 Amazon은 목록에 다른 ASIN을 할당했습니다. 을 포함하도록 제품 가시성을 높이려면 카탈로그 제품을 다른 ASIN에 일치시키고 두 ASIN 값 모두에 대한 목록을 만들어야 합니다. 이를 위해 별칭 Amazon 판매자 SKU를 만들 수 있습니다.

  기본적으로 단일 카탈로그 제품을 두 번째 Amazon 목록에 연결하는 데 사용할 수 있는 [!DNL Alias Amazon Seller SKU]을(를) 만들고 새로 일치하는 ASIN에 대한 목록을 만들 수 있습니다. 이 시나리오에서는 동일한 카탈로그 제품에 대한 Amazon 목록이 두 개 있습니다.

  별칭 Amazon 판매자 SKU를 만든 후에는 목록 설정, 규칙 및 재정의를 사용하여 해당 지역의 목록 정보를 제어할 수 있습니다. 목록화를 위해 지역별로 정의할 수 있는 제품 속성에는 수량/재고, 이행 방법, 조건, 제품 적격성 및 처리 시간이 포함됩니다.

## 지역별 목적에 사용 {#region-specific}

_[!UICONTROL Product Listings]_페이지(_[!UICONTROL Inactive]_, _활성_, _부적격_ 또는 _종료_ 탭)에서 목록을 봅니다.

1. _[!UICONTROL Actions]_에서&#x200B;**[!UICONTROL Create Alias Seller SKU]**을(를) 클릭합니다.

1. **[!UICONTROL Assign New Seller SKU]**&#x200B;에 대해 고유한 영숫자 값을 입력하십시오.

   이 값은 고유해야 합니다(카탈로그의 다른 제품 또는 별칭에 사용되지 않음).

1. **[!UICONTROL Assign New ASIN]**&#x200B;의 경우 변경하지 마십시오.

   이 값은 카탈로그 제품에 일치하는 제품 ASIN으로 자동으로 채워집니다. 이 값을 변경하면 카탈로그 제품이 ASIN을 기반으로 하는 두 개의 Amazon 목록에 일치합니다.

1. 필요에 따라 **[!UICONTROL Remove Existing Seller SKU]** 옵션을 전환합니다.

   - `Yes` - 목록을 삭제하고 제공된 새 정보를 사용하여 목록을 만들 수 있습니다.

   - `No` - 목록을 만들고 이전 목록을 변경되지 않은 상태로 유지하도록 선택합니다.

1. **[!UICONTROL Save Listing Update]**&#x200B;을(를) 클릭합니다.

## 단일 카탈로그 제품을 두 개의 Amazon 목록에 일치시키는 데 사용

1. _[!UICONTROL Product Listings]_페이지(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ 또는 _[!UICONTROL Ended]_탭)에서 목록을 봅니다.

1. _[!UICONTROL Actions]_에서&#x200B;**[!UICONTROL Create Alias Seller SKU]**을(를) 클릭합니다.

1. **[!UICONTROL Assign New Seller SKU]**&#x200B;에 대해 고유한 영숫자 값을 입력하십시오.

   이 값은 고유해야 합니다(카탈로그의 다른 제품 또는 별칭에 사용되지 않음).

1. **[!UICONTROL Assign New ASIN]**&#x200B;에 대해 고유한 영숫자 값을 입력하십시오.

   이 값은 카탈로그 제품에 일치하는 제품 ASIN으로 자동으로 채워집니다. 이 값을 변경하면 카탈로그 제품이 ASIN을 기반으로 하는 두 개의 Amazon 목록에 일치합니다.

1. 필요에 따라 **[!UICONTROL Remove Existing Seller SKU]** 옵션을 전환합니다.

   - `Yes` - 목록을 삭제하고 제공된 새 정보를 사용하여 목록을 만들 수 있습니다.

   - `No` - 다른 목록을 만들고 이전 목록을 변경되지 않은 상태로 유지하도록 선택합니다.

1. **[!UICONTROL Save Listing Update]**&#x200B;을(를) 클릭합니다.

![별칭 Amazon 판매자 SKU 만들기](assets/amazon-alias-sku-create.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Assign New Seller SKU] | 원래 Amazon 판매자 SKU에 연결할 고유한 새 영숫자 값을 입력합니다. 이 번호는 Amazon 판매 채널에서만 카탈로그 제품과 일치시키는 데 사용됩니다. 모든 SKU 값을 사용할 수 있지만 값은 카탈로그에서 한 번만 사용할 수 있습니다. |
| [!UICONTROL Assign New ASIN] | 카탈로그 제품과 일치시킬 목록에 대한 ASIN 값을 입력합니다. 동일한 제품에 대한 다른 목록에 대해 단일 카탈로그 제품을 ASIN에 일치시킬 때만 이 필드를 수정합니다. 이 값은 Amazon에서 할당한 ASIN과 일치해야 합니다. 그렇지 않으면 Amazon에서 목록을 거부하지 않습니다. |
| [!UICONTROL Remove Existing Seller SKU] | 옵션:<ul><li>**[!UICONTROL Yes]** - 목록을 삭제하고 제공된 새 정보를 사용하여 목록을 만들 수 있습니다. 새 목록이 _[!UICONTROL Active]_탭에 나타나고 이전 목록이_&#x200B;종료&#x200B;_탭으로 이동합니다.</li><li>**[!UICONTROL No]** - 다른 목록을 만들고 이전 목록을 변경되지 않은 상태로 유지하도록 선택합니다. 새 목록이 만들어지면 두 목록이 활성 탭에 나타납니다.</li></ul> |
