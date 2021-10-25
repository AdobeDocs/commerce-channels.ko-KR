---
title: '''예: 조건 정의'''
description: 목록 규칙을 만들 때 Amazon Marketplace에 나열할 상거래 카탈로그 제품을 식별하는 조건을 정의합니다.
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
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

의 조건 섹션을 참조하십시오. [장바구니 가격 규칙 만들기](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){target=&quot;_blank&quot;}.

## 조건 정의

이 프로세스는 카탈로그 설정에 따라 간단하거나 세부적일 수 있습니다. 다음과 같은 경우 `ALL` 또는 `ANY` 정의 조건 중 하나는 `TRUE` 또는 `FALSE` 제품의 경우 Amazon에 해당 제품을 나열할 수 있습니다.

조건은 기존 제품 속성 값을 기준으로 합니다. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 속성에 따라 조건을 정의하려면 **[!UICONTROL Use for Promo Rule Conditions]** 속성을으로 설정 `Yes`. 이 설정은 [Storefront 속성](https://docs.magento.com/user-guide/catalog/product-attributes-add.html)특성에 대한 {target=&quot;_blank&quot;} 페이지입니다.

![조건 - 라인 1](assets/ob-listing-rule-conditions-start.png)

이 예제의 규칙은 _Amazon FBA_ 속성 설정 `Yes`.

규칙 명령문에는 두 개의 굵은 링크가 있으며, 클릭하면 명령문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하는 경우 규칙이 모든 제품에 적용됩니다.

- 클릭 **[!UICONTROL ALL]** 다음 중 하나를 선택합니다. `ALL` 또는 `ANY`.
- 클릭 **[!UICONTROL TRUE]** 다음 중 하나를 선택합니다. `TRUE` 또는 `FALSE`.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 마십시오.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 추가 (![추가 아이콘](assets/btn-add-grn.png)) 아이콘을 클릭하고 조건 조합 또는 제품 속성과 같이 조건을 기반으로 할 속성을 선택합니다.

   - **[!UICONTROL Conditions Combination]** - 다른 일련의 `All/Any` 및 `True/False` 기존 집합 내의 조건.

      ![조건 조합](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]** - 제품 속성은 속성 설정에 따라 다릅니다. 목록에 속성을 표시하려면 프로모션 규칙 조건에서 사용하도록 구성해야 합니다. 자세한 내용은 _프로모션 규칙 조건에 사용_ in [제품 속성](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}.

      아래의 목록에서 **[!UICONTROL Product Attribute]**&#x200B;를 클릭하고 조건을 기준으로 사용할 속성을 선택합니다. 이 예제에서 선택한 조건은 다음과 같습니다 `Amazon FBA`.

      ![조건 라인 2, 제2부](assets/ob-condition-attribute-dropdown.png)

      선택한 조건이 문에 나타나고 두 개의 굵은 링크가 표시됩니다. 옵션은 선택한 제품 속성에 따라 다릅니다.

      속성을 설정한 후에는 변경할 수 없습니다. 속성을 변경하려면 라인을 삭제하고 새 속성을 추가해야 합니다. 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 제품에서 사용할 수 있습니다.

      1. 클릭 **[!UICONTROL is]** 을(를) 선택하고 충족될 제품에 대한 조건을 설명하는 비교 연산자를 선택합니다.

         이 예에서 비교 연산자는 `is`. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다릅니다. 옵션에는 일치 값(예: 값 중 하나 이상을 포함하지 않거나 포함하지 않음), 보다 큼, 같음 및 보다 작음 등의 다른 비교 옵션이 포함될 수 있습니다. 이 예에서 옵션은 다음과 같습니다 `is` 및 `is not`.

      1. 클릭 **[!UICONTROL ...]** 및 조건이 기반으로 하는 속성 값을 선택합니다.

         옵션은 속성의 설정에 따라 다릅니다. 옵션을 선택하거나 조건에 대한 텍스트 또는 숫자 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서는 선택 항목이 `Yes`.

         조건을 완료하기 위해 선택한 항목이 문에 나타납니다.

         ![조건 라인 2, 제3부](assets/ob-listing-rule-condition-is.png)
   이 조건은 완료되었습니다. 명시된 대로, 이 조건은 [!DNL Commerce] Amazon FBA 속성이 값으로 설정된 카탈로그 `Yes` 은 지역 및 스토어의 Amazon에 나열할 수 있습니다. 조건 라인을 추가하여 적격 제품을 더 좁힐 수 있습니다.

1. 문에 다른 조건 라인을 추가하려면 1단계로 돌아가서 원하는 모든 조건이 완료될 때까지 프로세스를 반복합니다.

Delete(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 제품에서 사용할 수 있습니다.
