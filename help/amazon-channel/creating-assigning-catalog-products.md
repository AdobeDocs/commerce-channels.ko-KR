---
title: 제품 만들기 및 할당
description: Amazon Sales Channel은 [!UICONTROL New Third Party] Amazon 목록을 사용하여 일치하는 상거래 카탈로그 제품을 만들고 할당하는 데 도움이 되는 탭입니다.
exl-id: de000e80-7546-44d2-905e-28664b24f028
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# 제품 만들기 및 할당

볼 때 _[!UICONTROL New Third Party]_탭에서 [!DNL Commerce] 기존 Amazon 목록에 제품을 카탈로그로 추가합니다. 이 일치에는 두 가지 옵션이 있습니다. 목록을 기존 카탈로그 제품에 지정하거나 목록의 정보를 사용하여 카탈로그 제품을 만들 수 있습니다. 이러한 옵션은 Amazon 목록이 과 자동으로 일치하지 않을 때 유용합니다 [!DNL Commerce] 카탈로그

Amazon 판매 채널의 전체 기능을 사용하려면 제품을 Amazon 목록에 일치(또는 할당)해야 합니다.

Amazon 목록에서 카탈로그 제품을 만드는 경우:

- 다음 **ASIN** 다음과 같이 [!DNL Commerce] SKU
- 다음 **제품 목록 이름** 카탈로그 목록 이름이 됨
- 다음 **가격** 및 **수량** Amazon 목록에서 가져옵니다

필요한 나머지 설정은 [!DNL Commerce] 만드는 동안 선택하는 제품 설정입니다.

만들고 일치하면 목록이 _[!UICONTROL New Third Party]_탭하고_[!UICONTROL Active]_ 탭.

## Amazon 목록에 단일 카탈로그 제품 할당

1. 에서 제품 목록을 봅니다. [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 목록에서 할당할 목록을 찾아 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고&#x200B;**[!UICONTROL Assign Catalog Product]**.

   이 작업을 수행하면 _[!UICONTROL Assign Magento Catalog Product]_페이지.

1. 목록을 탐색하거나 [작업 영역 컨트롤](./workspace-controls.md) 및 목록에 일치하는 적절한 카탈로그 제품을 찾습니다.

1. 목록에 올바른 제품이 나타나면 **[!UICONTROL Assign Catalog Product]** 에서 _[!UICONTROL Action]_열.

이제 제품 및 목록이 일치합니다. 이제 Amazon 판매 채널은 제품 및 목록 데이터를 Amazon과 공유하고 목록 및 정보(목록 가격, 배송가격, 재고/수량, 주문 정보 및 상태 등)를 관리할 수 있습니다.

## Amazon 목록 정보를 사용하여 단일 카탈로그 제품 만들기

1. 에서 제품 목록을 봅니다. [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 에서 만들 목록을 찾습니다 [!DNL Commerce] 카탈로그, **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열을 선택하고&#x200B;**[!UICONTROL Create New Catalog Product]**.

   이 작업을 수행하면 _[!UICONTROL Create Magento Catalog Product]_페이지.

1. 제품에 대한 카탈로그 설정을 완료합니다.

   - 설정 **[!UICONTROL Enable Product(s)]** 전환 `Yes` 또는 `No` (필수).

      |예|제품을 귀하의 [!DNL Commerce] 상점 판매.| |아니요|제품이 [!DNL Commerce] 상점 판매|

   - 대상 **[!UICONTROL Categories]**&#x200B;를 채울 때 제품에 대한 카테고리를 지정합니다(선택 사항).

      제품 카테고리를 선택하려면 아래쪽 화살표를 클릭하고 카테고리 확인란을 선택합니다. 클릭 **[!UICONTROL Done]** 완료됨.

   - 대상 **[!UICONTROL Website Ids]**&#x200B;을(를) 선택하고 제품을 연결할 웹 사이트(storefront)를 선택합니다.

      이 목록의 옵션은 [!DNL Commerce] [저장 구성](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} 설정.

   - 대상 **[!UICONTROL Attribute Set Id]** (필수) 옵션을 선택합니다.

      `Default` 는 기본 선택 항목입니다. 이 목록의 옵션은 [!DNL Commerce] [속성 세트](https://docs.magento.com/user-guide/stores/attribute-sets.html)구성한 {target=&quot;_blank&quot;}.

   - 대상 **[!UICONTROL Visibility]**&#x200B;새 제품에 대한 옵션을 선택합니다.

      |**[!UICONTROL Not Visible Individually]** (기본값)|이 제품은 다른 제품의 변형으로 사용할 수 있지만 스토어프론트 목록에 포함되지 않습니다.| |**[!UICONTROL Catalog]**|제품이 카탈로그 목록에 나타납니다.| |**[!UICONTROL Search]**|제품을 검색 작업에 사용할 수 있습니다.| |**[!UICONTROL Catalog and Search]**|제품이 카탈로그 목록에 포함되어 있으며 검색 작업에 사용할 수 있습니다.|

   - 대상 **[!UICONTROL Assign Tax Class]**&#x200B;에서 제품에 대한 옵션을 선택합니다.

      이 목록에 표시되는 옵션은 [세금 분류](https://docs.magento.com/user-guide/tax/tax-class.html)구성한 {target=&quot;_blank&quot;}.

   - 완료되면 를 클릭합니다. **[!UICONTROL Create Catalog Products]**.

카탈로그 제품은 [!DNL Commerce] 카탈로그로 지정하고 작성된 Amazon 목록에 지정합니다. 이제 목록이 기존 Amazon 목록과 일치하면 목록이 _[!UICONTROL New Third Party]_탭하고_[!UICONTROL Active]_ 탭.

## Amazon 목록 정보를 사용하여 여러 카탈로그 제품 만들기

1. 에서 제품 목록을 봅니다. [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭.

1. 카탈로그 제품을 만들 목록을 선택합니다.

   왼쪽 열에서 개별 확인란을 선택하거나 왼쪽 상단 열의 아래쪽 화살표를 클릭하고 을 선택할 수 있습니다 **[!UICONTROL Select All]** 또는 **[!UICONTROL Select All on this Page]**.

1. 아래 _[!UICONTROL Actions]_를 클릭합니다.**[!UICONTROL Create New Catalog Product(s)]**.

1. 확인 메시지를 수락하고 _[!UICONTROL Create Magento Catalog Product]_페이지를 클릭한 다음&#x200B;**[!UICONTROL OK]**.

1. 제품에 대한 카탈로그 설정을 완료합니다.

   >[!NOTE]
   >선택한 여러 목록에 대한 카탈로그 제품을 만들 때 입력한 제품 설정이 모든 목록에 적용됩니다.

   - 설정 **[!UICONTROL Enable Product(s)]** 전환 `Yes` 또는 `No` (필수).

      |예|제품을 귀하의 [!DNL Commerce] 상점 판매.| |아니요|제품이 [!DNL Commerce] 상점 판매|

   - 대상 **[!UICONTROL Categories]**&#x200B;를 채울 때 제품에 대한 카테고리를 지정합니다(선택 사항).

      제품 카테고리를 선택하려면 아래쪽 화살표를 클릭하고 카테고리 확인란을 선택합니다. 클릭 **완료** 완료됨.

   - 대상 **[!UICONTROL Website Ids]**&#x200B;을(를) 선택하고 제품을 연결할 웹 사이트(storefront)를 선택합니다.

      이 목록의 옵션은 [!DNL Commerce] [저장 구성](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} 설정.

   - 대상 **[!UICONTROL Attribute Set Id]** (필수) 옵션을 선택합니다.

      `Default` 는 기본 선택 항목입니다. 이 목록의 옵션은 [!DNL Commerce] [속성 세트](https://docs.magento.com/user-guide/stores/attribute-sets.html)구성한 {target=&quot;_blank&quot;}.

   - 대상 **[!UICONTROL Visibility]**&#x200B;새 제품에 대한 옵션을 선택합니다.

      |**[!UICONTROL Not Visible Individually]** (기본값)|이 제품은 다른 제품의 변형으로 사용할 수 있지만 스토어프론트 목록에 포함되지 않습니다.| |**[!UICONTROL Catalog]**|제품이 카탈로그 목록에 나타납니다.| |**[!UICONTROL Search]**|제품을 검색 작업에 사용할 수 있습니다.| |**[!UICONTROL Catalog and Search]**|제품이 카탈로그 목록에 포함되어 있으며 검색 작업에 사용할 수 있습니다.|

   - 대상 **[!UICONTROL Assign Tax Class]**&#x200B;에서 제품에 대한 옵션을 선택합니다.

      이 목록에 표시되는 옵션은 [세금 분류](https://docs.magento.com/user-guide/tax/tax-class.html)구성한 {target=&quot;_blank&quot;}.

   - 완료되면 를 클릭합니다. **[!UICONTROL Create Catalog Products]**.

카탈로그 제품은 [!DNL Commerce] 카탈로그로 지정하고 작성된 Amazon 목록에 지정합니다. 이제 목록이 각 Amazon 목록에 일치하면 목록에서 제거됩니다 [_[!UICONTROL New Third Party]_](./new-third-party-listings.md) 탭하고 [_[!UICONTROL Active]_](./active-listings.md) 탭.

![전자 상거래 카탈로그 제품 만들기](assets/amazon-magento-catalog-product.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Enable Product(s)] | (필수) 활성화되어 있으면 제품이 [!DNL Commerce] 상점. 비활성화된 경우 제품이 [!DNL Commerce] 상점. |
| [!UICONTROL Categories] | 새 제품의 카테고리 이름을 입력하거나 아래쪽 화살표를 클릭하여 선택 사항을 선택하여 카테고리를 선택할 수 있습니다. 옵션은 [카테고리](https://docs.magento.com/user-guide/catalog/category-create.html){target=&quot;_blank&quot;} 구성입니다. |
| [!UICONTROL Website Ids] | (필수) 제품을 연결할 웹 사이트(storefront)를 선택합니다. 옵션은 [!DNL Commerce] [저장 구성](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;} 설정 |
| 속성 세트 Id | 속성 세트를 선택합니다. 옵션은 구성된 항목에 따라 다릅니다 [!DNL Commerce] [속성 세트](https://docs.magento.com/user-guide/stores/attribute-sets.html){target=&quot;_blank&quot;}. |
| [!UICONTROL Visibility] | 옵션:<ul><li>**[!UICONTROL Not Visible Individually]** - 제품이 [!DNL Commerce] storefront(변형 제품에 가장 일반적으로 사용됨)</li><li>**[!UICONTROL Catalog]** - 웹 사이트 내에서 연결된 카테고리를 통해 제품에 액세스할 수 있습니다.</li><li>**검색** - 검색 도구를 통해서만 제품을 찾을 수 있습니다.</li><li>**[!UICONTROL Catalog and Search]** - 카테고리 구조와 검색 도구를 통해 제품에 액세스할 수 있습니다.</li></ul> |
| [!UICONTROL Assign Tax Class] | 신규 제품에 세금 분류를 지정합니다. 옵션은 구성된 항목에 따라 다릅니다 [세금 분류](https://docs.magento.com/user-guide/tax/tax-class.html){target=&quot;_blank&quot;}. |
