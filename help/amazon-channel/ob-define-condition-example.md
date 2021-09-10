---
title: '''예: 조건 정의'''
description: 목록 규칙을 만들 때 Amazon Marketplace에 나열할 상거래 카탈로그 제품을 식별하는 조건을 정의합니다.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 예: 조건 정의

## 조건

굵게 표시된 조건에 있는 모든 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

**선택한 웹 사이트 내의 모든 제품이 적합한 경우 조건을 추가하지 마십시오.**

>[!NOTE]
>
>Amazon 시스템과 직접 통신할 수 있는 복잡한 백엔드 프로세스 세트가 있습니다. 표시하려는 항목 수와 Amazon 시스템의 사용 가능 여부(예: 블랙 프라이데이)를 기준으로 항목을 Amazon에 나열하는 데 시간이 걸릴 수 있습니다.

[장바구니 가격 규칙 만들기](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){:target=&quot;_blank&quot;}의 조건 섹션을 참조하십시오.

## 조건 정의

이 프로세스는 카탈로그 설정에 따라 간단하거나 세부적일 수 있습니다. 정의 조건의 `ALL` 또는 `ANY`이 제품에 대해 `TRUE` 또는 `FALSE`인 경우 해당 제품을 Amazon에 나열할 수 있도록 조건을 설정할 수 있습니다.

조건은 기존 제품 속성 값을 기준으로 합니다. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 속성에 따라 조건을 정의하려면 속성에 대한 **[!UICONTROL Use for Promo Rule Conditions]** 설정을 `Yes`으로 설정합니다. [Storefront 속성](https://docs.magento.com/user-guide/catalog/product-attributes-add.html){:target=&quot;_blank&quot;} 페이지에서 속성에 대한 이 설정에 액세스할 수 있습니다.

![조건 - 라인 1](assets/ob-listing-rule-conditions-start.png)

이 예제의 규칙은 _Amazon FBA_ 속성이 `Yes`로 설정된 모든 카탈로그 제품에 대한 Amazon 자격을 설정하는 규칙을 정의합니다.

규칙 명령문에는 두 개의 굵은 링크가 있으며, 클릭하면 명령문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하는 경우 규칙이 모든 제품에 적용됩니다.

- **[!UICONTROL ALL]** 을 클릭하고 `ALL` 또는 `ANY` 중 하나를 선택합니다.
- **[!UICONTROL TRUE]** 을 클릭하고 `TRUE` 또는 `FALSE` 중 하나를 선택합니다.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 마십시오.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 조건 라인의 시작 부분에 있는 추가(![추가 아이콘](assets/btn-add-grn.png)) 아이콘을 클릭하고 조건 조합이나 제품 속성과 같이 조건을 기준으로 할 속성을 선택합니다.

   - **[!UICONTROL Conditions Combination]** - 기존 세트 내에 다른  `All/Any` 및  `True/False` 조건 세트를 만들 수 있도록 선택합니다.

      ![조건 조합](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - 제품 속성은 속성 설정에 따라 다릅니다. 목록에 속성을 표시하려면 프로모션 규칙 조건에서 사용하도록 구성해야 합니다. [제품 속성](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}에서 _프로모션 규칙 조건 사용_&#x200B;을 참조하십시오.

      **[!UICONTROL Product Attribute]** 아래의 목록에서 조건을 기준으로 사용할 속성을 선택합니다. 이 예제에서 선택한 조건은 `Amazon FBA`입니다.

      ![조건 라인 2, 제2부](assets/ob-condition-attribute-dropdown.png)

      선택한 조건이 문에 나타나고 두 개의 굵은 링크가 표시됩니다. 옵션은 선택한 제품 속성에 따라 다릅니다.

      속성을 설정한 후에는 변경할 수 없습니다. 속성을 변경하려면 라인을 삭제하고 새 속성을 추가해야 합니다. 라인 끝에서 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건 라인을 삭제할 수 있습니다.

      1. **[!UICONTROL is]** 을 클릭하고 제품을 충족할 조건을 설명하는 비교 연산자를 선택하십시오.

         이 예에서 비교 연산자는 `is`입니다. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다릅니다. 옵션에는 일치 값(예: 값 중 하나 이상을 포함하지 않거나 포함하지 않음), 보다 큼, 같음 및 보다 작음 등의 다른 비교 옵션이 포함될 수 있습니다. 이 예에서 옵션은 `is` 및 `is not`입니다.

      1. **[!UICONTROL ...]** 을 클릭하고 조건이 기반으로 하는 속성 값을 선택합니다.

         옵션은 속성의 설정에 따라 다릅니다. 옵션을 선택하거나 조건에 대한 텍스트 또는 숫자 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서는 선택 항목이 `Yes`입니다.

         조건을 완료하기 위해 선택한 항목이 문에 나타납니다.

         ![조건 라인 2, 제3부](assets/ob-listing-rule-condition-is.png)
   이 조건은 완료되었습니다. 명시된 대로, 이 조건은 [!DNL Commerce] 카탈로그의 Amazon FBA 속성이 `Yes` 값으로 설정된 모든 제품이 지역 및 스토어에 대해 Amazon에 나열될 수 있음을 의미합니다. 조건 라인을 추가하여 적격 제품을 더 좁힐 수 있습니다.

1. 문에 다른 조건 라인을 추가하려면 1단계로 돌아가서 원하는 모든 조건이 완료될 때까지 프로세스를 반복합니다.

언제든지 라인 끝에서 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건 문의 줄을 삭제할 수 있습니다.
