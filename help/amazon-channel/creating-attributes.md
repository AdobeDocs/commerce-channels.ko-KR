---
title: Amazon 판매 채널에 대한 속성 만들기 및 편집
description: Amazon Sales Channel은 현재 Amazon 속성 및 연결된 상거래 속성을 검토하는 데 도움이 되는 속성 보기를 제공합니다.
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# 속성 만들기 및 편집

만들기 또는 업데이트 [!DNL Commerce] 속성은 Amazon을 통해 판매하고 스토어를 업데이트할 때 사용됩니다. 현재 Amazon 속성 및 연결됨 검토 [!DNL Commerce] 속성을 통해 다음을 수행할 수 있습니다. [_[!UICONTROL Attributes]_보기](./attributes-view.md) / Amazon sales channel 홈 페이지 다음_[!UICONTROL Action]_ 열에는 속성에 사용할 수 있는 작업이 표시됩니다. 새 를 만들고 매핑할 수 있습니다 [!DNL Commerce] 연결되지 않은 Amazon 속성에 대한 속성 또는 기존 속성을 편집할 수 있는 경우 [!DNL Commerce] 속성 및 Amazon 속성에 대한 해당 매핑.

속성을 만들고 업데이트할 때 의 속성 값을 확인할 수 있습니다. [!DNL Commerce] 및 Amazon 제품. 이러한 값은 동기화하지 않고 Amazon에서 값을 가져오는 경우 다를 수 있습니다. 이러한 속성에 대한 Amazon 값을 검토하려면 다음을 참조하십시오 [Amazon 속성 매핑 검토](./amazon-matching-attributes-values.md). 이러한 값을 변경하려면 다음을 수행합니다. [매핑 편집 또는 만들기](./amazon-manually-update-incomplete-listing.md) Amazon과/와 사이 [!DNL Commerce].

## 속성 만들기 {#create-an-attribute}

다음 단계는 [!DNL Commerce] 속성을 지정하고 Amazon 속성에 매핑합니다. 구성에 따라 카탈로그 간 값 동기화가 시작될 수 있습니다.

1. 다음에서 _관리자_ 사이드바, 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾고 **[!UICONTROL Create Attribute]** 다음에서 _[!UICONTROL Action]_열.

1. 링크된 항목에 대한 Amazon 값 동기화를 활성화하려면 [!DNL Commerce] 속성, 설정 **[!UICONTROL Is Active]** 끝 `Yes`.

   로 설정된 경우 `Yes`, 값은 구성에 따라 동기화됩니다.

1. 선택 `Create New Magento Attribute` 대상 **[!UICONTROL Select Magento Product Attribute]**.

   속성은 다음에 대해 선택된 로 매핑됩니다. **[!UICONTROL Amazon Attribute Name]**.

1. 입력 **[!UICONTROL Magento Product Attribute Name]**.

1. 입력 **[!UICONTROL Magento Product Attribute Code]**.

   이 값은 모두 공백 없이 소문자여야 합니다.

1. 대상 **[!UICONTROL Attribute Set Ids]**&#x200B;을 클릭하고, 할당할 속성 세트를 선택합니다.

   일반적으로 속성은 파란색, 녹색, 노란색 및 빨간색 속성이 있는 색상에 대한 세트와 같은 속성 세트의 일부입니다.

1. 대상 **[!UICONTROL Type]**&#x200B;속성 값의 유형을 선택합니다(예: 텍스트 및 숫자).

   이 옵션은 속성에 대해 허용되는 값에 영향을 줍니다.

1. 대상 **[!UICONTROL Use for Promo Rule Conditions]**, 다음으로 설정 `Yes` 이관 조건 내에서 매개 변수에 속성을 사용할 수 있도록 허용하십시오.

1. 대상 **[!UICONTROL Used in Search]**, 다음으로 설정 `Yes` 속성 및 값을 제품 검색에 사용할 수 있는 경우.

1. 대상 **[!UICONTROL Comparable on Storefront]**, 다음으로 설정 `Yes` 속성 값을 Amazon의 &quot;비교 기준&quot; 기능에 사용할 수 있는 경우.

1. 다음을 선택합니다. [!DNL Commerce] [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) 을 누르고 하나 이상의 [보기 저장]을 선택하여 Amazon 값을으로 가져옵니다.

   범위가 로 설정된 경우 `Global`, _[!UICONTROL Store View]_특성을 만든 후에는 변경할 수 없습니다.

   다음을 선택하는 경우 `All Store Views (Global)`모든 Amazon 스토어 보기에 값을 동기화하고 저장합니다. 특정 스토어 보기에 값을 동기화할 수 있습니다.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save Attribute Settings]**.

저장한 후 속성을 편집하여 설정을 검토하고 Amazon 및 와(과) 일치하는 항목을 확인할 수 있습니다. [!DNL Commerce] 속성에 대한 값입니다. Amazon 값을 덮어쓸지 여부를 나타낼 수도 있습니다 [!DNL Commerce] 값.

![속성 설정 만들기](assets/amazon-attribute-settings-create.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 속성이 라이브 상태이고 Amazon과 간에 활성 동기화되는지 여부를 나타냅니다. [!DNL Commerce]. 다음으로 설정 `Yes` Amazon 및 [!DNL Commerce] 선택한 속성에 대해 동기화 상태를 유지합니다. |
| Magento 제품 속성 선택 | 나열된 Amazon 속성 이름에 연결할 선택한 속성을 나타냅니다. 속성을 만들 때 다음을 선택합니다. `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | 선택한 Amazon 속성의 이름을 표시합니다. 선택한 속성은 이 Amazon 속성에 연결됩니다. 다음을 통해 이 값을 편집할 수 없음 [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | 속성 이름 또는 &quot;label&quot;을 나타냅니다. |
| [!UICONTROL Magento Product Attribute Code] | 속성 코드를 나타냅니다. 모두 공백 없이 소문자로 표시됩니다. |
| [!UICONTROL Attribute Set Ids] | 속성을 지정할 속성 세트를 나타냅니다. 속성은 파란색, 녹색, 노란색 및 빨간색 속성이 있는 색상 집합과 같은 속성 집합의 일부인 경향이 있습니다. |
| [!UICONTROL Type] | 텍스트 및 숫자와 같은 속성 값의 값 유형을 나타냅니다. 선택 사항은 속성에 대해 허용되는 값에 영향을 줍니다. |
| [!UICONTROL Use for Promo Rule Conditions] | 전환 대상 `Yes` 이관 조건 내에서 매개 변수에 속성을 사용할 수 있도록 허용하십시오. |
| [!UICONTROL Used in Search] | 제품 검색에 속성 및 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Comparable on Storefront] | Amazon의 &quot;비교 기준&quot; 기능에서 속성 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Magento Product Attribute Scope] | 다음을 나타냅니다. [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) 속성용. 옵션: 글로벌/스토어 보기<br>로 설정된 경우 `Global`속성을 만든 후에는 저장소 보기를 편집할 수 없습니다. |
| [!UICONTROL Store Views (to import values into to)] | 범위가 로 설정된 경우에만 표시됩니다. `Store View`. 다음을 선택합니다. [스토어 뷰](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) Amazon 속성 값이 동기화되는 대상. 선택 중 `All Store Views (Global)` 모든 항목의 값을 업데이트합니다. [!DNL Commerce] 보기를 저장합니다. |

## 속성 편집 {#edit-an-attribute}

1. 다음에서 _관리자_ 사이드바, 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾고 **[!UICONTROL Edit]** 다음에서 _[!UICONTROL Action]_열.

1. 연결된 항목에 대한 Amazon 값 동기화를 활성화 또는 비활성화하려면 [!DNL Commerce] 속성, 설정 **활성화됨** 끝 `Yes` 또는 `No`.

   로 설정된 경우 `Yes`, 값은 구성에 따라 동기화됩니다.

1. 대상 **[!UICONTROL Select Magento Product Attribute]**, 선택한 로 매핑할 속성 확인 또는 업데이트 **[!UICONTROL Amazon Attribute Name]**.

1. 들어오는 Amazon 속성 값이 기존 속성 값을 덮어쓸지 여부를 나타냅니다.

   예를 들어 Amazon의 가격을 로 덮어쓰지 않으려고 할 수 있습니다 [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - 값을 유지하며 [!DNL Commerce] 및 Amazon 스토어.

   - **[!UICONTROL Overwrite Existing Magento Values]** - 의 값을 덮어씁니다. [!DNL Commerce] 들어오는 Amazon 값이 있는 제품 카탈로그.

1. 편집할 수 있는 경우 하나 이상을 선택합니다 **[!UICONTROL Store Views (to import Amazon values into)]**.

   속성이 `Global` 범위, _스토어 뷰_ 특성을 만든 후에는 변경할 수 없습니다.

   다음을 선택하는 경우 `All Store Views (Global)`를 입력하면 모든 스토어 보기에 값이 동기화되고 저장됩니다. 특정 스토어 보기에 값을 동기화할 수 있습니다.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save Attribute Settings]**.

![속성 설정 편집](assets/amazon-attribute-settings-edit.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 속성이 라이브 상태이고 Amazon과 간에 활성 동기화되는지 여부를 나타냅니다. [!DNL Commerce]. 다음으로 설정 `Yes` Amazon 및 [!DNL Commerce] 선택한 속성에 대해 동기화 상태를 유지합니다. |
| [!UICONTROL Select Magento Product Attribute] | 선택한 항목을 나타냅니다. [!DNL Commerce] 나열된 Amazon 속성 이름에 연결할 속성입니다. 연결된 [!DNL Commerce] 속성, 드롭다운 목록에서 다른 속성을 선택합니다. 값은 구성에 따라 동기화됩니다. |
| [!UICONTROL Amazon Attribute Name] | 에 정의된 대로 Amazon 속성의 이름을 표시합니다. [!DNL Amazon Seller Central]. 선택한 항목 [!DNL Commerce] 이 Amazon 속성에 대한 속성 링크입니다. 다음을 통해 이 값을 편집할 수 없음 [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Amazon 속성 값이 기존 값을 덮어쓰는지 여부를 나타냅니다. [!DNL Commerce] 값, 이 값을 가진 모든 제품에 영향 [!DNL Commerce] 특성.<ul><li>**기존 Magento 값을 덮어쓰지 않음** - (기본값) 다음을 유지합니다. [!DNL Commerce] 값, 다른 값 유지 [!DNL Commerce] 및 Amazon 스토어.</li><li>**기존 Magento 값 덮어쓰기** - 다음을 통해 Amazon 값을 저장합니다. [!DNL Commerce] 의 값 [!DNL Commerce] 제품 카탈로그.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 속성을 로 만든 경우 속성을 편집할 때 나타나지 않습니다. `Global` 범위. 다음을 나타냅니다. [!DNL Commerce] [범위](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html#scope-settings) 이(가) 을(를) 만들고 (으)로 설정됨 `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | 다음 항목 선택 [!DNL Commerce] [스토어 뷰](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html) Amazon 속성 값을 동기화할 대상. 선택 중 `All Store Views (Global)` 는 모든 스토어 조회수에 걸쳐 값을 업데이트합니다. |
