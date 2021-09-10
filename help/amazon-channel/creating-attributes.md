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

Amazon을 통해 판매하고 스토어를 업데이트할 때 [!DNL Commerce] 속성을 만들거나 업데이트합니다. Amazon 판매 채널 홈 페이지의 [_[!UICONTROL Attributes]_view](./attributes-view.md)를 통해 현재 Amazon 속성과 연결된 [!DNL Commerce] 속성을 검토합니다._[!UICONTROL Action]_ 열에는 속성에 사용할 수 있는 작업이 표시됩니다. 연결되지 않은 Amazon 속성에 대해 새 [!DNL Commerce] 속성을 만들고 매핑하거나 기존 [!DNL Commerce] 속성 및 Amazon 속성에 대한 매핑을 편집할 수 있습니다.

속성을 만들고 업데이트할 때 [!DNL Commerce] 및 Amazon 제품에 대한 속성 값을 확인할 수 있습니다. Amazon에서 값을 동기화하고 가져오지 않는 경우 이 값이 다를 수 있습니다. 이러한 특성에 대한 Amazon 값을 검토하려면 [Amazon 속성 매핑 검토](./amazon-matching-attributes-values.md)를 참조하십시오. 이러한 값을 변경하려면 [Amazon과 [!DNL Commerce] 간의 매핑](./amazon-manually-update-incomplete-listing.md)을 편집하거나 만들 수 있습니다.

## 속성 만들기 {#create-an-attribute}

이러한 단계에서는 [!DNL Commerce] 속성을 만들고 Amazon 속성에 매핑합니다. 구성에 따라 값이 카탈로그 간에 동기화를 시작할 수 있습니다.

1. _관리_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]** 을 클릭하고 Amazon 속성을 찾은 다음 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Create Attribute]**를 클릭합니다.

1. Amazon 값을 연결된 [!DNL Commerce] 속성에 동기화할 수 있도록 하려면 **[!UICONTROL Is Active]**&#x200B;을 `Yes`로 설정합니다.

   `Yes`로 설정하면 값이 구성에 따라 동기화됩니다.

1. **[!UICONTROL Select Magento Product Attribute]**&#x200B;에 대해 `Create New Magento Attribute`을 선택합니다.

   속성은 선택한 **[!UICONTROL Amazon Attribute Name]**&#x200B;에 대해 매핑됩니다.

1. **[!UICONTROL Magento Product Attribute Name]** 을 입력합니다.

1. **[!UICONTROL Magento Product Attribute Code]** 을 입력합니다.

   이 값은 공백 없이 모두 소문자여야 합니다.

1. **[!UICONTROL Attribute Set Ids]**&#x200B;에 대해 할당할 속성 세트를 선택합니다.

   일반적으로 속성은 파란색, 녹색, 노란색 및 빨간색에 대한 특성이 있는 색상 세트와 같이 속성 세트의 일부입니다.

1. **[!UICONTROL Type]**&#x200B;에 대해 텍스트 및 숫자와 같은 속성 값의 유형을 선택합니다.

   이 옵션은 속성에 대해 허용되는 값에 영향을 줍니다.

1. **[!UICONTROL Use for Promo Rule Conditions]**&#x200B;의 경우 판촉 조건 내의 매개 변수에 속성을 사용할 수 있도록 하려면 `Yes`로 설정하십시오.

1. **[!UICONTROL Used in Search]**&#x200B;의 경우 속성 및 값을 제품 검색에 사용할 수 있는 경우 `Yes` 로 설정합니다.

1. **[!UICONTROL Comparable on Storefront]**&#x200B;의 경우, 속성 값을 Amazon의 &quot;Compare By&quot; 기능에서 사용할 수 있으면 `Yes`로 설정하십시오.

1. 특성에 대해 [!DNL Commerce] [범위](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}를 선택한 다음 하나 이상의 [보기 저장]을 선택하여 Amazon 값을 으로 가져옵니다.

   범위가 `Global`으로 설정된 경우 속성을 만든 후에는 _[!UICONTROL Store View]_을 변경할 수 없습니다.

   `All Store Views (Global)`을 선택하면 값이 동기화되고 모든 Amazon 저장소 보기에 저장됩니다. 값을 특정 저장소 보기에만 동기화할 수 있습니다.

1. 완료되면 **[!UICONTROL Save Attribute Settings]** 을 클릭합니다.

저장 후 속성을 편집하여 설정을 검토하고 해당 속성에 대해 일치하는 Amazon 및 [!DNL Commerce] 값을 검토할 수 있습니다. Amazon 값이 [!DNL Commerce] 값을 덮어쓰도록 지정할 수도 있습니다.

![속성 설정 만들기](assets/amazon-attribute-settings-create.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 특성이 라이브인지 여부를 나타내며 Amazon과 [!DNL Commerce] 간에 활발하게 동기화되는지를 나타냅니다. Amazon 및 [!DNL Commerce]의 속성 값이 선택한 속성에 대해 계속 동기화되도록 하려면 `Yes` 로 설정하십시오. |
| Magento 제품 속성 선택 | 나열된 Amazon 속성 이름에 연결할 선택한 속성을 나타냅니다. 속성을 만들 때 `Create New Magento Attribute` 을 선택합니다. |
| [!UICONTROL Amazon Attribute Name] | 선택한 Amazon 속성의 이름을 표시합니다. 선택한 속성이 이 Amazon 속성에 연결됩니다. [!DNL Commerce]을 통해 이 값을 편집할 수 없습니다. |
| [!UICONTROL Magento Product Attribute Name] | 속성 이름 또는 &quot;label&quot;을 나타냅니다. |
| [!UICONTROL Magento Product Attribute Code] | 특성 코드를 나타내며 공백 없이 모두 소문자로 표시됩니다. |
| [!UICONTROL Attribute Set Ids] | 속성을 지정할 속성 세트를 나타냅니다. 속성은 파란색, 녹색, 노란색 및 빨간색에 대한 특성이 있는 색상 세트와 같이 속성 세트의 일부인 경향이 있습니다. |
| [!UICONTROL Type] | 텍스트 및 숫자와 같은 속성 값의 값 유형을 나타냅니다. 선택 사항은 속성에 대해 허용되는 값에 영향을 줍니다. |
| [!UICONTROL Use for Promo Rule Conditions] | 프로모션 조건 내의 매개 변수에 속성을 사용할 수 있도록 하려면 `Yes` 을 전환합니다. |
| [!UICONTROL Used in Search] | 제품 검색에서 속성과 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Comparable on Storefront] | Amazon의 &quot;비교 기준&quot; 기능에서 속성 값을 사용할 수 있는지 여부를 나타냅니다. |
| [!UICONTROL Magento Product Attribute Scope] | 특성에 대한 [범위](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}를 나타냅니다. 옵션: 전역/저장소 보기<br>를 `Global`로 설정하면 속성을 만든 후에는 저장소 보기를 편집할 수 없습니다. |
| [!UICONTROL Store Views (to import values into to)] | 범위가 `Store View`으로 설정된 경우에만 나타납니다. Amazon 특성 값이 동기화되는 [저장소 보기](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}를 선택합니다. `All Store Views (Global)`을 선택하면 모든 [!DNL Commerce] 저장소 보기에서 값이 업데이트됩니다. |

## 속성 편집 {#edit-an-attribute}

1. _관리_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]** 을 클릭하고 Amazon 속성을 찾은 다음 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Edit]**를 클릭합니다.

1. 연결된 [!DNL Commerce] 속성에 Amazon 값의 동기화를 활성화하거나 비활성화하려면 **Is Active**&#x200B;를 `Yes` 또는 `No`로 설정하십시오.

   `Yes`로 설정하면 값이 구성에 따라 동기화됩니다.

1. **[!UICONTROL Select Magento Product Attribute]**&#x200B;에 대해 선택한 **[!UICONTROL Amazon Attribute Name]**&#x200B;에 매핑할 특성을 확인하거나 업데이트하십시오.

1. 들어오는 Amazon 속성 값을 기존 속성 값을 덮어쓸지 여부를 나타냅니다.

   예를 들어 Amazon의 가격을 [!DNL Commerce]으로 덮어쓰지 않을 수 있습니다.

   - **[!UICONTROL Do Not Overwrite Existing Magento Values]** - 값을 유지하고  [!DNL Commerce] 및 Amazon 저장소에 대해 다른 값을 유지합니다.

   - **[!UICONTROL Overwrite Existing Magento Values]** -  [!DNL Commerce] 제품 카탈로그의 값을 들어오는 Amazon 값으로 덮어씁니다.

1. 편집할 수 있는 경우 **[!UICONTROL Store Views (to import Amazon values into)]** 이상을 선택하십시오.

   특성이 `Global` 범위로 생성된 경우 속성을 만든 후 _Store View_&#x200B;를 변경할 수 없습니다.

   `All Store Views (Global)`을 선택하면 값을 동기화하고 모든 저장소 보기에 저장합니다. 값을 특정 저장소 보기에만 동기화할 수 있습니다.

1. 완료되면 **[!UICONTROL Save Attribute Settings]** 을 클릭합니다.

![속성 설정 편집](assets/amazon-attribute-settings-edit.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Is Active] | 이 특성이 라이브인지 여부를 나타내며 Amazon과 [!DNL Commerce] 간에 활발하게 동기화되는지를 나타냅니다. Amazon 및 [!DNL Commerce]의 속성 값이 선택한 속성에 대해 계속 동기화되도록 하려면 `Yes` 로 설정하십시오. |
| [!UICONTROL Select Magento Product Attribute] | 나열된 Amazon 속성 이름에 연결할 선택한 [!DNL Commerce] 속성을 나타냅니다. 연결된 [!DNL Commerce] 속성을 변경하려면 드롭다운 목록에서 다른 속성을 선택합니다. 값은 구성에 따라 동기화됩니다. |
| [!UICONTROL Amazon Attribute Name] | [!DNL Amazon Seller Central]에 정의된 대로 Amazon 속성의 이름을 표시합니다. 선택한 [!DNL Commerce] 속성이 이 Amazon 속성에 연결됩니다. [!DNL Commerce]을 통해 이 값을 편집할 수 없습니다. |
| [!UICONTROL Overwrite Existing Value] | Amazon 속성 값이 기존 [!DNL Commerce] 값을 덮어쓰는지 여부를 나타내며 이 [!DNL Commerce] 특성으로 모든 제품에 영향을 줍니다.<ul><li>**기존 Magento 값을 덮어쓰지 않음**  - (기본값)  [!DNL Commerce] 값을 유지하여  [!DNL Commerce] 및 Amazon 저장소에 대해 다른 값을 유지합니다.</li><li>**기존 Magento 값 덮어쓰기**  -  [!DNL Commerce] 제품 카탈로그의 값 위에 Amazon  [!DNL Commerce] 값을 저장합니다.</li></ul> |
| [!UICONTROL Magento Product Attribute Scope] | 특성이 `Global` 범위로 생성된 경우 속성을 편집할 때 나타나지 않습니다. [!DNL Commerce] [scope](https://docs.magento.com/user-guide/configuration/scope.html){target=&quot;_blank&quot;}이 생성되어 `Store View`로 설정되었음을 나타냅니다. |
| [!UICONTROL Store Views (to import values into to)] | Amazon 특성 값을 동기화할 [!DNL Commerce] [보기](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target=&quot;_blank&quot;}를 선택합니다. `All Store Views (Global)`을 선택하면 모든 저장소 보기에서 값이 업데이트됩니다. |
