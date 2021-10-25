---
title: 가격 규칙 조건
description: 가격 규칙 조건을 사용하여 목록 가격 규칙에 적합한 제품을 결정합니다.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# 가격 규칙 조건

조건은 가격 규칙에 적합한 제품을 결정합니다. Amazon 가격책정 규칙에 대한 조건을 정의하는 것은 [장바구니 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}의 [!DNL Commerce].

>[!IMPORTANT]
>
>가격 규칙이 [!DNL Commerce] 카탈로그, 이 섹션을 비워 둡니다.

굵게 표시된 조건에 있는 모든 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

## 예: 가격 규칙 조건 작성

이 프로세스는 카탈로그 구성에 따라 간단하거나 세부적일 수 있습니다. 다음과 같은 경우 `ALL` 또는 `ANY` 조건이 `TRUE` 또는 `FALSE` 제품의 경우, 해당 제품을 적용할 가격 규칙에 대한 자격이 있습니다.

조건은 [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 속성에 따라 조건을 정의하려면 **프로모션 규칙 조건에 사용** 의 경우 속성을 `Yes` 다음 위치에서 [Storefront 속성](https://docs.magento.com/user-guide/stores/attribute-product-create.html)특성에 대한 {target=&quot;_blank&quot;} 입니다.

![가격 규칙 조건 - 라인 1](assets/ob-price-rules-condition-1.png)

이 예는 `Books` 카테고리.

규칙 문에는 두 개의 굵은 링크가 있으며, 클릭하면 조건 문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하는 경우 규칙이 모든 제품에 적용됩니다.

- 클릭 **[!UICONTROL ALL]** 다음 중 하나를 선택합니다. `ALL` 또는 `ANY`.
- 클릭 **[!UICONTROL TRUE]**, 다음 중 하나를 선택합니다. `TRUE` 또는 `FALSE`.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 마십시오.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 조건이 적용되는 사용 가능한 속성을 표시하려면 추가(![추가 아이콘](assets/btn-add-grn.png))을 클릭하여 제품에서 사용할 수 있습니다.

   **[!UICONTROL Conditions Combination]** - 다른 일련의 `All/Any` 및 `True/False` 기존 조건 내의 조건.

   ![가격 규칙 조건 조합](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - 사용 가능한 제품 속성은 [속성 설정](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}. 목록에 속성을 표시하려면 *[!UICONTROL Use for Promo Rule Conditions]* 의 경우 속성을 `Yes` 다음 위치에서 [storefront 속성](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}.

   - 대상 **[!UICONTROL Product Attribute]**&#x200B;를 클릭하고 조건을 기준으로 정의할 속성을 선택합니다. 이 예제에서 선택한 조건은 다음과 같습니다 `Category`.

      ![가격 규칙 조건 - 라인 2, 부품 2](assets/ob-price-rule-condition-2.png)

      선택한 조건이 문에 나타나고 두 개의 굵은 링크가 표시됩니다. 옵션은 선택한 제품 속성에 따라 다릅니다.

      속성을 설정한 후에는 편집할 수 없습니다. 속성을 변경하려면 라인을 삭제하고 새 속성을 추가해야 합니다. 삭제(![삭제 아이콘](assets/btn-del-red.png) 아이콘 을 클릭하여 제품에서 사용할 수 있습니다.

   - 클릭 **[!UICONTROL is]** 을(를) 선택하고 충족될 제품에 대한 조건을 설명하는 비교 연산자를 선택합니다.

      이 예에서 비교 연산자는 `is`. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다르며 다른 비교 옵션을 포함할 수 있습니다. 옵션에는 하나 이상의 값을 포함하지 않거나 포함하지 않고, 둘 이상의 값, 같음 및 숫자보다 작은 값을 포함할 수 있습니다. 이 예에서 옵션은 다음과 같습니다 `is` 및 `is not`.

   - 클릭 **[!UICONTROL ...]** 및 조건이 기반으로 하는 속성 값을 선택합니다. 옵션은 속성의 설정에 따라 다릅니다.

      옵션을 선택하거나 조건에 대한 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서 필드는 공백으로 표시됩니다. 규칙의 카테고리를 선택하려면 선택기 아이콘(![선택기 아이콘](assets/btn-chooser.png))을 클릭하여 선택 옵션을 표시합니다. 이 규칙은 다음에 사용됩니다 _책_&#x200B;에서 을(를) 선택합니다. **[!UICONTROL Books]** 확인란을 선택합니다. 카테고리 번호가 채워집니다. 범주 선택을 수락하려면 녹색 확인 표시 아이콘(![확인 표시 아이콘](assets/btn-check-mark-green.png)).

      ![가격 규칙 조건 - 라인 2, 부품 3](assets/ob-price-rule-condition-3.png)

      조건을 완료하기 위해 선택한 항목이 문에 나타납니다.

      ![가격 규칙 조건 - 라인 2, 부품 4](assets/ob-price-rule-condition-4.png)

      이 예제 조건은 완료되었습니다. 명시된 대로, 이 조건은 [!DNL Commerce] 정의된 장부 범주를 갖는 카탈로그`4`)은 이 가격 규칙에 적합합니다. 조건 라인을 추가하여 적격 제품을 더 좁힐 수 있습니다.

1. 문에 다른 조건 라인을 추가하려면 1단계로 돌아가서 원하는 모든 조건이 완료될 때까지 프로세스를 반복합니다.

   Delete(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 제품에서 사용할 수 있습니다.
