---
title: 가격 규칙 조건
description: 가격 규칙 조건을 사용하여 목록 가격 규칙에 적합한 제품을 결정합니다.
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html: 
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 757
ht-degree: 0%

---

# 가격 규칙 조건

조건은 가격 규칙에 적합한 제품을 결정합니다. Amazon 가격 규칙에 대한 조건을 정의하는 것은 [!DNL Commerce]장바구니 가격 규칙](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){:target=&quot;_blank&quot;}에 대한 조건을 정의하는 것과 동일한 논리 및 프로세스를 따릅니다.[

>[!IMPORTANT]
>
>가격 규칙이 [!DNL Commerce] 카탈로그의 모든 제품에 적용되는 경우 이 섹션을 비워 둡니다.

굵게 표시된 조건에 있는 모든 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

## 예: 가격 규칙 조건 작성

이 프로세스는 카탈로그 구성에 따라 간단하거나 세부적일 수 있습니다. 조건 중 `ALL` 또는 `ANY`이 제품에 대해 `TRUE` 또는 `FALSE`인 경우 해당 제품이 가격 규칙을 적용할 수 있도록 조건을 정의할 수 있습니다.

조건은 [제품 속성](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}을 기반으로 합니다. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 속성에 따라 조건을 정의하려면 **Use for Promo Rule Conditions** 속성에 대해 [Storefront Properties](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}에서 `Yes`로 설정해야 합니다.

![가격 규칙 조건 - 라인 1](assets/ob-price-rules-condition-1.png)

이 예는 `Books` 카테고리에 정의된 모든 제품에 25% 할인을 적용하는 규칙을 정의합니다.

규칙 문에는 두 개의 굵은 링크가 있으며, 클릭하면 조건 문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하는 경우 규칙이 모든 제품에 적용됩니다.

- **[!UICONTROL ALL]** 을 클릭하고 `ALL` 또는 `ANY` 중 하나를 선택합니다.
- **[!UICONTROL TRUE]** 을 클릭하고 `TRUE` 또는 `FALSE` 중 하나를 선택합니다.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 마십시오.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 조건이 적용되는 사용 가능한 속성을 표시하려면 조건 라인의 시작 부분에서 추가(![추가 아이콘](assets/btn-add-grn.png)) 아이콘을 클릭하고 조건을 기준으로 할 속성을 선택합니다.

   **[!UICONTROL Conditions Combination]** - 기존 조건 내에 다른  `All/Any` 및  `True/False` 조건 세트를 만들도록 선택합니다.

   ![가격 규칙 조건 조합](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]** - 사용 가능한 제품 속성은 속성  [설정](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}에 따라 다릅니다. 목록에 표시할 속성의 경우 [storefront 속성](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}에서 속성에 대한 *[!UICONTROL Use for Promo Rule Conditions]*&#x200B;을 `Yes`로 설정해야 합니다.

   - **[!UICONTROL Product Attribute]**&#x200B;에 대해 조건의 기본으로 정의할 속성을 선택합니다. 이 예제에서 선택한 조건은 `Category`입니다.

      ![가격 규칙 조건 - 라인 2, 부품 2](assets/ob-price-rule-condition-2.png)

      선택한 조건이 문에 나타나고 두 개의 굵은 링크가 표시됩니다. 옵션은 선택한 제품 속성에 따라 다릅니다.

      속성을 설정한 후에는 편집할 수 없습니다. 속성을 변경하려면 라인을 삭제하고 새 속성을 추가해야 합니다. 라인 끝에서 삭제(![삭제 아이콘](assets/btn-del-red.png) 아이콘을 클릭하여 조건 라인을 삭제할 수 있습니다.

   - **[!UICONTROL is]** 을 클릭하고 제품을 충족할 조건을 설명하는 비교 연산자를 선택하십시오.

      이 예에서 비교 연산자는 `is`입니다. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다르며 다른 비교 옵션을 포함할 수 있습니다. 옵션에는 하나 이상의 값을 포함하지 않거나 포함하지 않고, 둘 이상의 값, 같음 및 숫자보다 작은 값을 포함할 수 있습니다. 이 예에서 옵션은 `is` 및 `is not`입니다.

   - **[!UICONTROL ...]** 을 클릭하고 조건이 기반으로 하는 속성 값을 선택합니다. 옵션은 속성의 설정에 따라 다릅니다.

      옵션을 선택하거나 조건에 대한 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서 필드는 공백으로 표시됩니다. 규칙의 카테고리를 선택하려면 선택기 아이콘(![선택 아이콘](assets/btn-chooser.png))을 클릭하여 선택 옵션을 표시합니다. 이 규칙은 _책_&#x200B;에 대한 것입니다. **[!UICONTROL Books]** 확인란을 선택하십시오. 카테고리 번호가 채워집니다. 카테고리 선택을 수락하려면 녹색 확인 표시 아이콘(![확인 표시 아이콘](assets/btn-check-mark-green.png))을 클릭합니다.

      ![가격 규칙 조건 - 라인 2, 부품 3](assets/ob-price-rule-condition-3.png)

      조건을 완료하기 위해 선택한 항목이 문에 나타납니다.

      ![가격 규칙 조건 - 라인 2, 부품 4](assets/ob-price-rule-condition-4.png)

      이 예제 조건은 완료되었습니다. 명시된 대로, 이 조건은 [!DNL Commerce] 카탈로그의 정의된 장부 범주(`4`)가 있는 모든 제품이 이 가격책정 규칙에 적합함을 의미합니다. 조건 라인을 추가하여 적격 제품을 더 좁힐 수 있습니다.

1. 문에 다른 조건 라인을 추가하려면 1단계로 돌아가서 원하는 모든 조건이 완료될 때까지 프로세스를 반복합니다.

   언제든지 라인 끝에서 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건 문의 줄을 삭제할 수 있습니다.
