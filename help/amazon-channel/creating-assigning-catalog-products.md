---
title: Amazon 판매 채널을 위한 제품 만들기 및 할당
description: Amazon Sales Channel은 [!UICONTROL New Third Party] 탭에서 Amazon 목록이 있는 일치하는 상거래 카탈로그 제품을 만들고 할당할 수 있습니다.
feature: Sales Channels, Products, Configuration
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 0%

---

# 제품 만들기 및 할당

볼 때 _[!UICONTROL New Third Party]_탭, 다음과 일치시킬 수 있습니다. [!DNL Commerce] 기존 Amazon 목록에 제품 카탈로그 추가. 이 일치에는 두 가지 옵션이 있습니다. 기존 카탈로그 제품에 목록을 지정하거나 목록의 정보를 사용하여 카탈로그 제품을 만들 수 있습니다. 이러한 옵션은 Amazon 목록이 자동으로 일치하지 않을 때 유용합니다 [!DNL Commerce] 카탈로그.

Amazon 판매 채널의 전체 기능 세트를 사용하려면 Amazon 목록에 제품을 일치(또는 할당)해야 합니다.

Amazon 목록에서 카탈로그 제품을 만들 때:

- 다음 **아신** 이(가) [!DNL Commerce] SKU
- 다음 **제품 목록 이름** 이 카탈로그 목록 이름이 됩니다.
- 다음 **가격** 및 **수량** Amazon 목록에서 가져옵니다.

필요한 나머지 설정은 [!DNL Commerce] 만드는 동안 선택하는 제품 설정입니다.

이 목록을 만들고 일치시키면에서 목록이 제거됩니다. _[!UICONTROL New Third Party]_탭을에 표시하고_[!UICONTROL Active]_ 탭.

## Amazon 목록에 단일 카탈로그 제품 할당

1. 에서 제품 목록 보기 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 목록에서 지정하려는 목록을 찾은 다음 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_열 및 클릭&#x200B;**[!UICONTROL Assign Catalog Product]**.

   이 작업을 수행하면 _[!UICONTROL Assign Magento Catalog Product]_페이지를 가리키도록 업데이트하는 중입니다.

1. 다음을 사용하여 목록 찾아보기 또는 필터링 [작업 영역 컨트롤](./workspace-controls.md) 목록에 일치하는 적절한 카탈로그 제품을 찾습니다.

1. 목록에 올바른 제품이 나타나면 **[!UICONTROL Assign Catalog Product]** 다음에서 _[!UICONTROL Action]_열.

이제 제품과 목록이 일치합니다. 이제 Amazon 판매 채널은 Amazon과 제품 및 상장 데이터를 공유하고 상장 가격, 배송 가격, 재고/수량, 주문 정보 및 상태 등을 포함하여 상장 및 해당 정보를 관리할 수 있습니다.

## Amazon 목록 정보를 사용하여 단일 카탈로그 제품 만들기

1. 에서 제품 목록 보기 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 에서 만들려는 목록을 찾습니다. [!DNL Commerce] 카탈로그, 클릭 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_열 및 클릭&#x200B;**[!UICONTROL Create New Catalog Product]**.

   이 작업을 수행하면 _[!UICONTROL Create Magento Catalog Product]_페이지를 가리키도록 업데이트하는 중입니다.

1. 제품에 대한 카탈로그 설정을 완료합니다.

   - 설정 **[!UICONTROL Enable Product(s)]** 전환 대상 `Yes` 또는 `No` (필수).

     |예|제품을 사용할 수 있도록 하려면 선택합니다. [!DNL Commerce] 상점 판매.| |아니요|제품을 사용할 수 없게 하려면 선택합니다. [!DNL Commerce] 상점 판매.|

   - 대상 **[!UICONTROL Categories]**, 제품에 대한 카테고리를 할당합니다(선택 사항).

     제품의 카테고리를 선택하려면 아래쪽 화살표를 클릭하고 카테고리 확인란을 선택합니다. 클릭 **[!UICONTROL Done]** 완료 시.

   - 대상 **[!UICONTROL Website Ids]**&#x200B;을(를) 통해 제품과 연결할 웹 사이트(상점)를 선택합니다.

     이 목록의 옵션은 다음에 따라 다릅니다. [!DNL Commerce] [구성 저장](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) 설정.

   - 대상 **[!UICONTROL Attribute Set Id]** (필수) 옵션을 선택합니다.

     `Default` 는 기본 선택 항목입니다. 이 목록의 옵션은 다음에 따라 다릅니다. [!DNL Commerce] [속성 집합](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) 을(를) 구성했습니다.

   - 대상 **[!UICONTROL Visibility]**, 새 제품에 대한 옵션을 선택합니다.

     |**[!UICONTROL Not Visible Individually]** (기본값)|다른 제품의 변형으로 사용할 수 있는 제품이지만 해당 제품은 상점 목록에 포함되어 있지 않습니다.| |**[!UICONTROL Catalog]**|제품이 카탈로그 목록에 표시됩니다.| |**[!UICONTROL Search]**|제품을 검색 작업에 사용할 수 있습니다.| |**[!UICONTROL Catalog and Search]**|제품이 카탈로그 목록에 포함되어 있으며 검색 작업에 사용할 수 있습니다.|

   - 대상 **[!UICONTROL Assign Tax Class]**&#x200B;제품에 대한 옵션을 선택합니다.

     이 목록에 표시되는 옵션은 [세금 등급](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) 을(를) 구성했습니다.

   - 완료되면 다음을 클릭하십시오. **[!UICONTROL Create Catalog Products]**.

카탈로그 제품이 [!DNL Commerce] 카탈로그와 이 카탈로그가 생성된 Amazon 목록에 지정됩니다. 이제 목록이 기존 Amazon 목록과 일치하면 목록에서 제거됩니다. _[!UICONTROL New Third Party]_탭을에 표시_[!UICONTROL Active]_ 탭.

## Amazon 목록 정보를 사용하여 여러 카탈로그 제품 만들기

1. 에서 제품 목록 보기 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 카탈로그 제품을 만들 목록을 선택하십시오.

   왼쪽 열에서 개별 확인란을 선택하거나 왼쪽 상단 열의 아래쪽 화살표를 클릭하고 을 선택할 수 있습니다 **[!UICONTROL Select All]** 또는 **[!UICONTROL Select All on this Page]**.

1. 아래 _[!UICONTROL Actions]_, 클릭&#x200B;**[!UICONTROL Create New Catalog Product(s)]**.

1. 확인 메시지를 수락하고 _[!UICONTROL Create Magento Catalog Product]_페이지, 클릭&#x200B;**[!UICONTROL OK]**.

1. 제품에 대한 카탈로그 설정을 완료합니다.

   >[!NOTE]
   >선택한 여러 목록의 카탈로그 제품을 만들 때 입력한 제품 설정이 모든 목록에 적용됩니다.

   - 설정 **[!UICONTROL Enable Product(s)]** 전환 대상 `Yes` 또는 `No` (필수).

     |예|제품을 사용할 수 있도록 하려면 선택합니다. [!DNL Commerce] 상점 판매.| |아니요|제품을 사용할 수 없게 하려면 선택합니다. [!DNL Commerce] 상점 판매.|

   - 대상 **[!UICONTROL Categories]**, 제품에 대한 카테고리를 할당합니다(선택 사항).

     제품의 카테고리를 선택하려면 아래쪽 화살표를 클릭하고 카테고리 확인란을 선택합니다. 클릭 **완료** 완료 시.

   - 대상 **[!UICONTROL Website Ids]**&#x200B;을(를) 통해 제품과 연결할 웹 사이트(상점)를 선택합니다.

     이 목록의 옵션은 다음에 따라 다릅니다. [!DNL Commerce] [구성 저장](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) 설정.

   - 대상 **[!UICONTROL Attribute Set Id]** (필수) 옵션을 선택합니다.

     `Default` 는 기본 선택 항목입니다. 이 목록의 옵션은 다음에 따라 다릅니다. [!DNL Commerce] [속성 집합](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html) 을(를) 구성했습니다.

   - 대상 **[!UICONTROL Visibility]**, 새 제품에 대한 옵션을 선택합니다.

     |**[!UICONTROL Not Visible Individually]** (기본값)|다른 제품의 변형으로 사용할 수 있는 제품이지만 해당 제품은 상점 목록에 포함되어 있지 않습니다.| |**[!UICONTROL Catalog]**|제품이 카탈로그 목록에 표시됩니다.| |**[!UICONTROL Search]**|제품을 검색 작업에 사용할 수 있습니다.| |**[!UICONTROL Catalog and Search]**|제품이 카탈로그 목록에 포함되어 있으며 검색 작업에 사용할 수 있습니다.|

   - 대상 **[!UICONTROL Assign Tax Class]**&#x200B;제품에 대한 옵션을 선택합니다.

     이 목록에 표시되는 옵션은 [세금 등급](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html) 을(를) 구성했습니다.

   - 완료되면 다음을 클릭하십시오. **[!UICONTROL Create Catalog Products]**.

카탈로그 제품이 [!DNL Commerce] 카탈로그와 이 카탈로그가 생성된 Amazon 목록에 지정됩니다. 이제 목록이 해당 Amazon 목록과 일치하면 목록에서 제거됩니다. [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭을에 표시 [_[!UICONTROL Active]_](./active-listings.md) 탭.

![상거래 카탈로그 제품 만들기](assets/amazon-magento-catalog-product.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Product(s)] | (필수) 활성화된 경우 제품이 [!DNL Commerce] 가게 앞이야 비활성화된 경우 제품이에 표시되지 않습니다. [!DNL Commerce] 가게 앞이야 |
| [!UICONTROL Categories] | 새 제품에 대한 범주 이름을 입력하거나 아래쪽 화살표를 클릭하여 선택 사항을 표시하는 범주를 선택할 수 있습니다. 옵션은 다음에 따라 다릅니다. [카테고리](https://experienceleague.adobe.com/docs/commerce-admin/catalog/categories/create/category-create.html) 구성. |
| [!UICONTROL Website Ids] | (필수) 제품을 연결할 웹 사이트(상점)를 선택합니다. 옵션은 다음에 따라 다릅니다. [!DNL Commerce] [구성 저장](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) 설정 |
| 속성 집합 Id | 속성 세트를 선택합니다. 옵션은 구성된 항목에 따라 다릅니다 [!DNL Commerce] [속성 집합](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-sets.html). |
| [!UICONTROL Visibility] | 옵션:<ul><li>**[!UICONTROL Not Visible Individually]** - 제품이 다음에 표시되지 않음 [!DNL Commerce] storefront(변형 제품에 가장 일반적으로 사용됨).</li><li>**[!UICONTROL Catalog]** - 웹 사이트 내에서 연결된 카테고리를 통해 제품에 액세스할 수 있습니다.</li><li>**검색** - 검색 도구를 통해서만 제품을 찾을 수 있습니다.</li><li>**[!UICONTROL Catalog and Search]** - 범주 구조를 통해 검색 도구를 사용하여 제품에 액세스할 수 있습니다.</li></ul> |
| [!UICONTROL Assign Tax Class] | 신규 제품에 세금 분류를 지정합니다. 옵션은 구성된 항목에 따라 다릅니다 [세금 등급](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/taxes/tax-class.html). |
