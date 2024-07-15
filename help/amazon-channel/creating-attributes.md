---
title: Amazon 판매 채널에 대한 속성 만들기 및 편집
description: Amazon Sales Channel은 현재 Amazon 속성 및 연결된 Commerce 속성을 검토하는 데 도움이 되는 속성 보기를 제공합니다.
feature: Sales Channels, Products, Configuration
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# 속성 만들기 및 편집

Amazon을 통해 판매하고 스토어를 업데이트할 때 [!DNL Commerce] 특성을 만들거나 업데이트합니다. Amazon 판매 채널 홈 페이지의 [_[!UICONTROL Attributes]_보기](./attributes-view.md)를 통해 현재 Amazon 특성 및 연결된 [!DNL Commerce] 특성을 검토하십시오._[!UICONTROL Action]_ 열에는 특성에 사용할 수 있는 작업이 표시됩니다. 링크되지 않은 Amazon 특성에 대해 새 [!DNL Commerce] 특성을 만들어 매핑하거나 기존 [!DNL Commerce] 특성과 Amazon 특성에 대한 매핑을 편집할 수 있습니다.

특성을 만들고 업데이트할 때 [!DNL Commerce] 및 Amazon 제품에 대한 특성 값을 확인할 수 있습니다. 이러한 값은 동기화하지 않고 Amazon에서 값을 가져오는 경우 다를 수 있습니다. 이러한 특성에 대한 Amazon 값을 검토하려면 [Amazon 특성 매핑 검토](./amazon-matching-attributes-values.md)를 참조하십시오. 이러한 값을 변경하려면 Amazon과 [!DNL Commerce] 간의 [매핑을 편집하거나 만들 수 있습니다](./amazon-manually-update-incomplete-listing.md).

## 속성 만들기 {#create-an-attribute}

다음 단계에서는 [!DNL Commerce] 특성을 만들어 Amazon 특성에 매핑합니다. 구성에 따라 카탈로그 간 값 동기화가 시작될 수 있습니다.

1. _관리자_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]**&#x200B;을(를) 클릭하고 Amazon 특성을 찾은 다음 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Create Attribute]**을(를) 클릭합니다.

1. Amazon 값을 연결된 [!DNL Commerce] 특성에 동기화하려면 **[!UICONTROL Is Active]**&#x200B;을(를) `Yes`(으)로 설정하십시오.

   `Yes`(으)로 설정하면 구성에 따라 값이 동기화됩니다.

1. **[!UICONTROL Select Magento Product Attribute]**&#x200B;에 대해 `Create New Magento Attribute`을(를) 선택하십시오.

   특성이 **[!UICONTROL Amazon Attribute Name]**&#x200B;에 대해 선택된 항목에 매핑됩니다.

1. **[!UICONTROL Magento Product Attribute Name]** 입력.

1. **[!UICONTROL Magento Product Attribute Code]** 입력.

   이 값은 모두 공백 없이 소문자여야 합니다.

1. **[!UICONTROL Attribute Set Ids]**&#x200B;에 대해 할당할 속성 집합을 선택하십시오.

   일반적으로 속성은 파란색, 녹색, 노란색 및 빨간색 속성이 있는 색상에 대한 세트와 같은 속성 세트의 일부입니다.

1. **[!UICONTROL Type]**&#x200B;의 경우 텍스트 및 숫자와 같은 특성 값의 유형을 선택합니다.

   이 옵션은 속성에 대해 허용되는 값에 영향을 줍니다.

1. **[!UICONTROL Use for Promo Rule Conditions]**&#x200B;의 경우 프로모션 조건 내에서 매개 변수에 특성을 사용할 수 있도록 하려면 `Yes`(으)로 설정하십시오.

1. 제품 검색에 특성과 값을 사용할 수 있는 경우 **[!UICONTROL Used in Search]**&#x200B;의 경우 `Yes`(으)로 설정하십시오.

1. **[!UICONTROL Comparable on Storefront]**&#x200B;의 경우 Amazon의 &quot;비교 기준&quot; 기능에서 특성 값을 사용할 수 있는 경우 `Yes`(으)로 설정하십시오.

1. 특성에 대한 [!DNL Commerce] [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)를 선택한 다음 Amazon 값을 가져올 저장소 보기를 하나 이상 선택하십시오.

   범위를 `Global`(으)로 설정하면 특성을 만든 후에는 _[!UICONTROL Store View]_을(를) 변경할 수 없습니다.

   `All Store Views (Global)`을(를) 선택하면 동기화되어 모든 Amazon 스토어 보기에 값을 저장합니다. 특정 스토어 보기에 값을 동기화할 수 있습니다.

1. 완료되면 **[!UICONTROL Save Attribute Settings]**&#x200B;을(를) 클릭합니다.

저장한 후 속성을 편집하여 설정을 검토하고 속성에 대해 일치하는 Amazon 및 [!DNL Commerce] 값을 검토할 수 있습니다. Amazon 값이 [!DNL Commerce] 값을 덮어쓸지 여부도 나타낼 수 있습니다.

![특성 설정 만들기](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | 이 특성이 Amazon과 [!DNL Commerce] 간에 활성 상태로 동기화되는지 여부를 나타냅니다. Amazon 및 [!DNL Commerce]의 특성 값이 선택한 특성에 대해 동기화 상태를 유지하려면 `Yes`(으)로 설정하십시오. |
| Magento 제품 속성 선택 | 나열된 Amazon 속성 이름에 연결할 선택한 속성을 나타냅니다. 특성을 만들 때 `Create New Magento Attribute`을(를) 선택하십시오. |
| [!UICONTROL Amazon Attribute Name] | 선택한 Amazon 속성의 이름을 표시합니다. 선택한 속성은 이 Amazon 속성에 연결됩니다. [!DNL Commerce]을(를) 통해 이 값을 편집할 수 없습니다. |
| [!UICONTROL Magento Product Attribute Name] | 속성 이름 또는 &quot;label&quot;을 나타냅니다. |
| [!UICONTROL Magento Product Attribute Code] | 속성 코드를 나타냅니다. 모두 공백 없이 소문자로 표시됩니다. |
| [!UICONTROL Attribute Set Ids] | 속성을 지정할 속성 세트를 나타냅니다. 속성은 파란색, 녹색, 노란색 및 빨간색 속성이 있는 색상 집합과 같은 속성 집합의 일부인 경향이 있습니다. |
| [!UICONTROL Type] | 텍스트 및 숫자와 같은 속성 값의 값 유형을 나타냅니다. 선택 사항은 속성에 대해 허용되는 값에 영향을 줍니다. |
| [!UICONTROL Use for Promo Rule Conditions] | 프로모션 조건 내에서 매개 변수에 특성을 사용할 수 있도록 `Yes`(으)로 전환합니다. |
| [!UICONTROL Used in Search] | 제품 검색에 속성 및 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Comparable on Storefront] | Amazon의 &quot;비교 기준&quot; 기능에서 속성 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Magento Product Attribute Scope] | 특성에 대한 [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)을(를) 나타냅니다. 옵션: 전역/저장소 보기<br>이(가) `Global`(으)로 설정된 경우 특성을 만든 후에는 저장소 보기를 편집할 수 없습니다. |
| [!UICONTROL Store Views (to import values into to)] | 범위가 `Store View`(으)로 설정된 경우에만 나타납니다. Amazon 특성 값을 동기화할 [스토어 보기](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)를 선택하십시오. `All Store Views (Global)`을(를) 선택하면 모든 [!DNL Commerce] 스토어 보기에서 값이 업데이트됩니다. |

## 속성 편집 {#edit-an-attribute}

1. _관리자_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]**&#x200B;을(를) 클릭하고 Amazon 특성을 찾은 다음 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Edit]**을(를) 클릭합니다.

1. 연결된 [!DNL Commerce] 특성에 대한 Amazon 값의 동기화를 활성화하거나 비활성화하려면 **활성 상태임**&#x200B;을(를) `Yes` 또는 `No`(으)로 설정하십시오.

   `Yes`(으)로 설정하면 구성에 따라 값이 동기화됩니다.

1. **[!UICONTROL Select Magento Product Attribute]**&#x200B;의 경우 선택한 **[!UICONTROL Amazon Attribute Name]**&#x200B;에 매핑할 특성을 확인하거나 업데이트하십시오.

1. 들어오는 Amazon 속성 값이 기존 속성 값을 덮어쓸지 여부를 나타냅니다.

   예를 들어 Amazon의 가격을 [!DNL Commerce](으)로 덮어쓰지 않을 수 있습니다.

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - 값을 유지하고 [!DNL Commerce] 및 Amazon 스토어에 대해 다른 값을 유지합니다.

   - **[!UICONTROL Overwrite Existing Magento Values]** - [!DNL Commerce] 제품 카탈로그의 값을 들어오는 Amazon 값으로 덮어씁니다.

1. 편집할 수 있는 경우 **[!UICONTROL Store Views (to import Amazon values into)]**&#x200B;을(를) 하나 이상 선택하십시오.

   특성이 `Global` 범위로 만들어진 경우 특성을 만든 후에는 _스토어 보기_&#x200B;를 변경할 수 없습니다.

   `All Store Views (Global)`을(를) 선택하면 동기화되어 모든 저장소 보기에 값을 저장합니다. 특정 스토어 보기에 값을 동기화할 수 있습니다.

1. 완료되면 **[!UICONTROL Save Attribute Settings]**&#x200B;을(를) 클릭합니다.

![특성 설정 편집](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Is Active] | 이 특성이 Amazon과 [!DNL Commerce] 간에 활성 상태로 동기화되는지 여부를 나타냅니다. Amazon 및 [!DNL Commerce]의 특성 값이 선택한 특성에 대해 동기화 상태를 유지하려면 `Yes`(으)로 설정하십시오. |
| [!UICONTROL Select Magento Product Attribute] | 나열된 Amazon 특성 이름에 연결할 선택한 [!DNL Commerce] 특성을 나타냅니다. 연결된 [!DNL Commerce] 특성을 변경하려면 드롭다운 목록에서 다른 특성을 선택하십시오. 값은 구성에 따라 동기화됩니다. |
| [!UICONTROL Amazon Attribute Name] | [!DNL Amazon Seller Central]에 정의된 대로 Amazon 특성의 이름을 표시합니다. 선택한 [!DNL Commerce] 특성은 이 Amazon 특성에 연결됩니다. [!DNL Commerce]을(를) 통해 이 값을 편집할 수 없습니다. |
| [!UICONTROL Overwrite Existing Value] | Amazon 특성 값이 기존 [!DNL Commerce] 값을 덮어쓰는지 여부를 나타내며, 이 [!DNL Commerce] 특성을 사용하는 모든 제품에 영향을 줍니다.<ul><li>**기존 Magento 값을 덮어쓰지 않음** - (기본값) [!DNL Commerce] 및 Amazon 스토어에 대해 다른 값을 유지하면서 [!DNL Commerce] 값을 유지합니다.</li><li>**기존 Magento 값 덮어쓰기** - [!DNL Commerce] 제품 카탈로그의 [!DNL Commerce] 값 위에 Amazon 값을 저장합니다.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 특성이 `Global` 범위로 만들어진 경우 특성을 편집할 때 나타나지 않습니다. [!DNL Commerce] [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings)이(가) 만들어지고 `Store View`(으)로 설정되었음을 나타냅니다. |
| [!UICONTROL Store Views (to import values into to)] | Amazon 특성 값을 동기화할 [!DNL Commerce] [스토어 보기](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)를 선택하십시오. `All Store Views (Global)`을(를) 선택하면 모든 스토어 보기에서 값이 업데이트됩니다. |
