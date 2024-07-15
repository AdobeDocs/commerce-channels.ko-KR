---
title: Amazon 판매 채널 - 가격 규칙 조건
description: 가격 규칙 조건을 사용하여 목록 가격 규칙에 적합한 제품을 결정합니다.
feature: Sales Channels, Price Rules
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 가격 규칙 조건

조건은 가격 규칙에 적합한 제품을 결정합니다. Amazon 가격 규칙에 대한 조건을 정의하는 것은 [!DNL Commerce]의 [장바구니 가격 규칙](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html)에 대한 조건을 정의하는 것과 동일한 논리 및 프로세스를 따릅니다.

>[!IMPORTANT]
>
>가격 규칙이 [!DNL Commerce] 카탈로그의 모든 제품에 적용되는 경우 이 섹션을 비워 둡니다.

조건의 굵게 표시된 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

## 예: 가격 규칙 조건 작성

이 프로세스는 카탈로그 구성에 따라 간단하거나 자세할 수 있습니다. `ALL` 또는 `ANY` 조건의 `TRUE` 또는 `FALSE`이(가) 제품인 경우 적용할 가격 책정 규칙에 해당 제품을 사용할 수 있도록 조건을 정의할 수 있습니다.

조건은 [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을 기반으로 합니다. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 특성을 기반으로 조건을 정의하려면 특성에 대한 [Storefront 속성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html)에서 특성에 대한 **프로모션 규칙 조건에 사용**&#x200B;을(를) `Yes`(으)로 설정해야 합니다.

![가격 규칙 조건 - 줄 1](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

이 예제는 `Books` 범주에 정의된 모든 제품에 25% 할인을 적용하는 규칙을 정의합니다.

규칙 명령문에는 두 개의 굵은 링크가 있으며, 이 링크를 클릭하면 조건 명령문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하면 규칙이 모든 제품에 적용됩니다.

- **[!UICONTROL ALL]**&#x200B;을(를) 클릭하고 `ALL` 또는 `ANY`을(를) 선택합니다.
- **[!UICONTROL TRUE]**&#x200B;을(를) 클릭하고 `TRUE` 또는 `FALSE`을(를) 선택합니다.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 않고 둡니다.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 조건이 적용되는 사용 가능한 특성을 표시하려면 조건 줄의 맨 앞에 있는 추가(![추가 아이콘](assets/btn-add-grn.png)) 아이콘을 클릭하고 조건을 기준으로 할 특성을 선택하십시오.

   **[!UICONTROL Conditions Combination]** - 기존 조건 내에 다른 `All/Any` 및 `True/False` 조건 집합을 만들도록 선택합니다.

   ![가격 규칙 조건 조합](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** - 사용 가능한 제품 특성은 [특성의 설정](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html)에 따라 다릅니다. 목록에 표시할 특성을 표시하려면 특성의 *[!UICONTROL Use for Promo Rule Conditions]*&#x200B;을(를) 상점 속성에서 `Yes`(으)로 설정해야 합니다.

   - **[!UICONTROL Product Attribute]**&#x200B;에 대해 조건의 기준으로 정의할 특성을 선택합니다. 이 예제에서 선택한 조건은 `Category`입니다.

     ![가격 규칙 조건 - 2행, 2부](assets/ob-price-rule-condition-2.png){width="500"}

     선택한 조건이 문에 나타나고 그 뒤에 굵은 링크가 두 개 더 나타납니다. 옵션은 선택하는 제품 속성에 따라 다릅니다.

     속성을 설정한 후에는 편집할 수 없습니다. 속성을 변경하려면 줄을 삭제하고 새 속성을 추가해야 합니다. 줄 끝에 있는 삭제(![삭제 아이콘](assets/btn-del-red.png))를 클릭하여 조건 줄을 삭제할 수 있습니다.

   - **[!UICONTROL is]**&#x200B;을(를) 클릭하고 제품을 충족하기 위한 조건을 설명하는 비교 연산자를 선택합니다.

     이 예제에서 비교 연산자는 `is`입니다. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다르며 다른 비교 옵션을 포함할 수 있습니다. 옵션은 수치 이상, 같음 및 보다 작은 값 중 적어도 하나를 포함하지 않거나 포함하지 않는 매칭 값을 포함할 수 있다. 이 예제에서 옵션은 `is` 및 `is not`입니다.

   - **[!UICONTROL ...]**&#x200B;을(를) 클릭하고 조건의 기반이 되는 특성 값을 선택합니다. 옵션은 속성의 설정에 따라 다릅니다.

     옵션을 선택하거나 조건 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서는 필드가 비어 있습니다. 규칙에 대한 범주를 선택하려면 선택 아이콘(![선택 아이콘](assets/btn-chooser.png))을 클릭하여 선택 옵션을 표시합니다. 이 규칙은 _책_&#x200B;용입니다. **[!UICONTROL Books]** 확인란을 선택하세요. 범주 번호가 채워집니다. 범주 선택을 수락하려면 녹색 확인 표시 아이콘(![확인 표시 아이콘](assets/btn-check-mark-green.png))을 클릭합니다.

     ![가격 규칙 조건 - 2행, 3부](assets/ob-price-rule-condition-3.png){width="500"}

     선택한 항목이 문에 표시되어 조건을 완료합니다.

     ![가격 규칙 조건 - 라인 2, 파트 4](assets/ob-price-rule-condition-4.png){width="500"}

     이 예제 조건은 완료되었습니다. 명시된 대로, 이 조건은 장부의 범주(`4`)가 정의된 [!DNL Commerce] 카탈로그의 모든 제품이 이 가격 책정 규칙에 해당됨을 의미합니다. 조건 라인을 더 추가하여 적격 제품의 범위를 더 좁힐 수 있습니다.

1. 문에 다른 조건 행을 추가하려면 1단계로 돌아가서 원하는 조건이 모두 완료될 때까지 프로세스를 반복합니다.

   언제든지 줄 끝에 있는 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건문의 줄을 삭제할 수 있습니다.
