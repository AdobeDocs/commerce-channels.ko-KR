---
title: 속성 만들기 및 편집
description: Amazon Sales Channel은 현재 Amazon 속성 및 연결된 상거래 속성을 검토하는 데 도움이 되는 속성 보기를 제공합니다.
exl-id: 3cd5fb7e-68a3-45fd-8f50-72d3cc0244b5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# 속성 만들기 및 편집

만들기 또는 업데이트 [!DNL Commerce] Amazon을 통해 판매하고 스토어를 업데이트하는 경우의 특성입니다. 현재 Amazon 속성 및 연결 검토 [!DNL Commerce] 를 통해 속성 생성 [_[!UICONTROL Attributes]_보기](./attributes-view.md) Amazon 영업 채널 홈 페이지의 자산 다음_[!UICONTROL Action]_ 열에는 속성에 사용할 수 있는 작업이 표시됩니다. 새 템플릿을 만들고 매핑할 수 있습니다 [!DNL Commerce] 연결되지 않은 Amazon 속성에 대한 속성을 만들거나 기존 속성을 편집할 수 있습니다 [!DNL Commerce] 속성 및 Amazon 속성에 대한 매핑.

속성을 생성 및 업데이트할 때 [!DNL Commerce] 및 Amazon 제품. Amazon에서 값을 동기화하고 가져오지 않는 경우 이 값이 다를 수 있습니다. 이러한 속성에 대한 Amazon 값을 검토하려면 다음을 참조하십시오 [Amazon 속성 매핑 검토](./amazon-matching-attributes-values.md). 이러한 값을 변경하려는 경우 다음을 수행할 수 있습니다 [매핑 편집 또는 만들기](./amazon-manually-update-incomplete-listing.md) Amazon 및 [!DNL Commerce].

## 속성 만들기 {#create-an-attribute}

이러한 단계는 다음을 생성합니다 [!DNL Commerce] 속성을 만들고 Amazon 속성에 매핑합니다. 구성에 따라 값이 카탈로그 간에 동기화를 시작할 수 있습니다.

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾아 **[!UICONTROL Create Attribute]** 에서 _[!UICONTROL Action]_열.

1. 연결된 항목에 Amazon 값 동기화를 활성화하려면 [!DNL Commerce] 속성, 설정 **[!UICONTROL Is Active]** to `Yes`.

   로 설정된 경우 `Yes`로 설정되면 값은 구성에 따라 동기화됩니다.

1. 선택 `Create New Magento Attribute` 대상 **[!UICONTROL Select Magento Product Attribute]**.

   속성은 선택한 속성에 매핑됩니다 **[!UICONTROL Amazon Attribute Name]**.

1. 을(를) 입력합니다. **[!UICONTROL Magento Product Attribute Name]**.

1. 을(를) 입력합니다. **[!UICONTROL Magento Product Attribute Code]**.

   이 값은 공백 없이 모두 소문자여야 합니다.

1. 대상 **[!UICONTROL Attribute Set Ids]**&#x200B;을 눌러 지정할 속성 세트를 선택합니다.

   일반적으로 속성은 파란색, 녹색, 노란색 및 빨간색에 대한 특성이 있는 색상 세트와 같이 속성 세트의 일부입니다.

1. 대상 **[!UICONTROL Type]**&#x200B;텍스트 및 숫자와 같은 속성 값의 유형을 선택합니다.

   이 옵션은 속성에 대해 허용되는 값에 영향을 줍니다.

1. 대상 **[!UICONTROL Use for Promo Rule Conditions]**, 다음 으로 설정됨 `Yes` 프로모션 조건 내의 매개 변수에 속성을 사용할 수 있도록 합니다.

1. 대상 **[!UICONTROL Used in Search]**, 다음 으로 설정됨 `Yes` 제품 검색에 속성과 값을 사용할 수 있는 경우.

1. 대상 **[!UICONTROL Comparable on Storefront]**, 다음 으로 설정됨 `Yes` Amazon의 &quot;비교 기준&quot; 기능에서 속성 값을 사용할 수 있는 경우.

1. 을(를) 선택합니다 [!DNL Commerce] [범위](https://docs.magento.com/user-guide/configuration/scope.html)특성에 대해 {target=&quot;_blank&quot;} 를 선택한 다음 하나 이상의 [보기 저장]을 선택하여 Amazon 값을 으로 가져옵니다.

   범위가 `Global`, _[!UICONTROL Store View]_특성을 만든 후에는 변경할 수 없습니다.

   만약 `All Store Views (Global)`를 입력하면 모든 Amazon 저장소 보기에 값을 동기화하고 저장합니다. 값을 특정 저장소 보기에만 동기화할 수 있습니다.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save Attribute Settings]**.

저장한 후 속성을 편집하여 설정을 검토하고 Amazon과 일치하는 [!DNL Commerce] 속성에 대한 값. Amazon 값을 덮어쓰도록 지정할 수도 있습니다 [!DNL Commerce] 값.

![속성 설정 만들기](assets/amazon-attribute-settings-create.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 특성이 라이브인지 여부를 나타내며 Amazon과 [!DNL Commerce]. 을 로 설정합니다. `Yes` Amazon 및 [!DNL Commerce] 선택한 속성에 대해 동기화 상태를 유지합니다. |
| Magento 제품 속성 선택 | 나열된 Amazon 속성 이름에 연결할 선택한 속성을 나타냅니다. 속성을 만들 때 `Create New Magento Attribute`. |
| [!UICONTROL Amazon Attribute Name] | 선택한 Amazon 속성의 이름을 표시합니다. 선택한 속성이 이 Amazon 속성에 연결됩니다. 이 값은 [!DNL Commerce]. |
| [!UICONTROL Magento Product Attribute Name] | 속성 이름 또는 &quot;label&quot;을 나타냅니다. |
| [!UICONTROL Magento Product Attribute Code] | 특성 코드를 나타내며 공백 없이 모두 소문자로 표시됩니다. |
| [!UICONTROL Attribute Set Ids] | 속성을 지정할 속성 세트를 나타냅니다. 속성은 파란색, 녹색, 노란색 및 빨간색에 대한 특성이 있는 색상 세트와 같이 속성 세트의 일부인 경향이 있습니다. |
| [!UICONTROL Type] | 텍스트 및 숫자와 같은 속성 값의 값 유형을 나타냅니다. 선택 사항은 속성에 대해 허용되는 값에 영향을 줍니다. |
| [!UICONTROL Use for Promo Rule Conditions] | 전환 `Yes` 프로모션 조건 내의 매개 변수에 속성을 사용할 수 있도록 합니다. |
| [!UICONTROL Used in Search] | 제품 검색에서 속성과 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Comparable on Storefront] | Amazon의 &quot;비교 기준&quot; 기능에서 속성 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Magento Product Attribute Scope] | 를 나타냅니다 [범위](https://docs.magento.com/user-guide/configuration/scope.html)특성에 대한 {target=&quot;_blank&quot;} 입니다. 옵션: 전역/저장소 보기<br>로 설정된 경우 `Global`를 지정하는 경우, 속성을 만든 후에는 저장소 보기를 편집할 수 없습니다. |
| [!UICONTROL Store Views (to import values into to)] | 범위가 로 설정된 경우에만 나타납니다 `Store View`. 을(를) 선택합니다 [저장소 보기](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Amazon 속성 값이 동기화되는 {target=&quot;_blank&quot;}. 선택 `All Store Views (Global)` 는 모든 위치에서 값을 업데이트합니다 [!DNL Commerce] 보기를 저장합니다. |

## 속성 편집 {#edit-an-attribute}

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾아 **[!UICONTROL Edit]** 에서 _[!UICONTROL Action]_열.

1. 연결된 항목에 Amazon 값 동기화를 활성화하거나 비활성화하려면 [!DNL Commerce] 속성, 설정 **활성 상태** to `Yes` 또는 `No`.

   로 설정된 경우 `Yes`로 설정되면 값은 구성에 따라 동기화됩니다.

1. 대상 **[!UICONTROL Select Magento Product Attribute]**, 선택한 속성에 매핑할 속성을 확인하거나 업데이트합니다 **[!UICONTROL Amazon Attribute Name]**.

1. 들어오는 Amazon 속성 값을 기존 속성 값을 덮어쓸지 여부를 나타냅니다.

   예를 들어 Amazon의 가격을 [!DNL Commerce].

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - 값을 유지하고 다른 값을 유지합니다 [!DNL Commerce] 그리고 Amazon 스토어도 있습니다.

   - **[!UICONTROL Overwrite Existing Magento Values]** - 의 값을 덮어씁니다. [!DNL Commerce] 수신 Amazon 값이 있는 제품 카탈로그.

1. 편집할 수 있는 경우 하나 이상을 선택합니다 **[!UICONTROL Store Views (to import Amazon values into)]**.

   속성을 `Global` 범위, _저장소 보기_ 특성을 만든 후에는 변경할 수 없습니다.

   만약 `All Store Views (Global)`값을 동기화하고 모든 저장소 보기에 저장합니다. 값을 특정 저장소 보기에만 동기화할 수 있습니다.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save Attribute Settings]**.

![속성 설정 편집](assets/amazon-attribute-settings-edit.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 특성이 라이브인지 여부를 나타내며 Amazon과 [!DNL Commerce]. 을 로 설정합니다. `Yes` Amazon 및 [!DNL Commerce] 선택한 속성에 대해 동기화 상태를 유지합니다. |
| [!UICONTROL Select Magento Product Attribute] | 선택한 항목을 나타냅니다 [!DNL Commerce] 나열된 Amazon 속성 이름에 연결할 속성입니다. 연결된 항목을 변경하려면 [!DNL Commerce] 속성을 만들려면 드롭다운 목록에서 다른 속성을 선택합니다. 값은 구성에 따라 동기화됩니다. |
| [!UICONTROL Amazon Attribute Name] | 에 정의된 대로 Amazon 속성의 이름을 표시합니다. [!DNL Amazon Seller Central]. 선택한 항목 [!DNL Commerce] 이 Amazon 속성에 대한 특성 링크. 이 값은 [!DNL Commerce]. |
| [!UICONTROL Overwrite Existing Value] | Amazon 속성 값이 기존 값을 덮어쓸지 여부를 나타냅니다 [!DNL Commerce] 값, 이 값을 사용하여 모든 제품에 영향 [!DNL Commerce] 속성을 사용합니다.<ul><li>**기존 Magento 값을 덮어쓰지 않음** - (기본값) [!DNL Commerce] 값, 다른 값 유지 [!DNL Commerce] 그리고 Amazon 스토어도 있습니다.</li><li>**기존 Magento 값 덮어쓰기** - Amazon 값을 [!DNL Commerce] 값에서 [!DNL Commerce] 제품 카탈로그</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 속성을 `Global` 범위. 를 나타냅니다 [!DNL Commerce] [범위](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}이(가) 생성되어 `Store View`. |
| [!UICONTROL Store Views (to import values into to)] | 선택 [!DNL Commerce] [저장소 보기](https://docs.magento.com/user-guide/stores/websites-stores-views.html)Amazon 속성 값을 동기화할 {target=&quot;_blank&quot;}. 선택 `All Store Views (Global)` 모든 저장소 보기에서 값을 업데이트합니다. |
