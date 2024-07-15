---
title: '예: Amazon 목록 규칙 조건 정의'
description: 목록 규칙을 만들 때 Amazon Marketplace에 나열할 Commerce 카탈로그 제품을 식별하는 조건을 정의합니다.
feature: Sales Channels, Products, Configuration
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# 예: 조건 정의

## 조건

조건의 굵게 표시된 영역을 클릭하여 다양한 옵션을 볼 수 있습니다.

**선택한 웹 사이트에 있는 모든 제품이 적합한 경우 조건을 추가하지 마십시오.**

>[!NOTE]
>
>Amazon 시스템과 직접 통신하는 복잡한 백엔드 프로세스 세트가 있습니다. 나열하려는 항목의 수와 Amazon 시스템의 사용 빈도에 따라(예: 블랙 프라이데이) Amazon에 항목이 나열되는 데 시간이 걸릴 수 있습니다.

[장바구니 가격 규칙 만들기](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog-create.html)의 조건 섹션을 참조하십시오.

## 조건 정의

이 프로세스는 카탈로그 설정에 따라 간단하거나 자세히 지정할 수 있습니다. 정의된 조건 중 `ALL` 또는 `ANY`이(가) 제품에 대한 `TRUE` 또는 `FALSE`인 경우 제품이 Amazon에 나열될 수 있도록 조건을 설정할 수 있습니다.

조건은 기존 제품 속성 값을 기반으로 합니다. 모든 제품에 규칙을 적용하려면 조건 섹션을 비워 둡니다.

>[!NOTE]
>
>특정 제품 특성을 기반으로 조건을 정의하려면 특성에 대한 **[!UICONTROL Use for Promo Rule Conditions]** 설정을 `Yes`(으)로 설정합니다. 특성의 [Storefront 속성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes-add.html) 페이지에서 이 설정에 액세스할 수 있습니다.

![조건 - 줄 1](assets/ob-listing-rule-conditions-start.png){width="500"}

이 예제의 규칙은 _Amazon FBA_ 특성이 `Yes`(으)로 설정된 모든 카탈로그 제품에 대해 Amazon 자격 조건을 설정하는 규칙을 정의합니다.

규칙 명령문에는 두 개의 굵은 링크가 있으며, 이 링크를 클릭하면 명령문의 해당 부분에 대한 옵션이 표시됩니다. 굵게 옵션을 변경하지 않고 조건을 저장하면 규칙이 모든 제품에 적용됩니다.

- **[!UICONTROL ALL]**&#x200B;을(를) 클릭하고 `ALL` 또는 `ANY`을(를) 선택합니다.
- **[!UICONTROL TRUE]**&#x200B;을(를) 클릭하고 `TRUE` 또는 `FALSE`을(를) 선택합니다.
- 모든 제품에 규칙을 적용하려면 조건을 변경하지 않고 둡니다.

이러한 값의 조합을 변경하여 다른 조건을 만들 수 있습니다. 이 예에서는 다음 조건이 사용됩니다.

`If ALL of these conditions are TRUE:`

1. 조건 라인의 시작 부분에 있는 추가(![추가 아이콘](assets/btn-add-grn.png)) 아이콘을 클릭하고 조건 조합이나 제품 특성과 같이 조건을 기반으로 할 특성을 선택합니다.

   - **[!UICONTROL Conditions Combination]** - 기존 집합 내에 다른 `All/Any` 및 `True/False` 조건 집합을 만들 수 있도록 선택합니다.

     ![조건 조합](assets/ob-conditions-combinations.png){width="500"}

   - **[!UICONTROL Product Attribute]** - 제품 특성은 특성의 설정에 따라 다릅니다. 속성이 목록에 나타나도록 하려면 이관 규칙 조건에서 사용되도록 구성해야 합니다. [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)에서 _프로모션 규칙 조건에 사용_&#x200B;을 참조하세요.

     **[!UICONTROL Product Attribute]** 아래 목록에서 조건의 기준으로 사용할 특성을 선택합니다. 이 예제에서 선택한 조건은 `Amazon FBA`입니다.

     ![조건 줄 2, 부분 2](assets/ob-condition-attribute-dropdown.png){width="350"}

     선택한 조건이 문에 나타나고 그 뒤에 굵은 링크가 두 개 더 나타납니다. 옵션은 선택하는 제품 속성에 따라 다릅니다.

     속성을 설정한 후에는 변경할 수 없습니다. 속성을 변경하려면 줄을 삭제하고 새 속성을 추가해야 합니다. 줄 끝에 있는 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건 줄을 삭제할 수 있습니다.

      1. **[!UICONTROL is]**&#x200B;을(를) 클릭하고 제품을 충족하기 위한 조건을 설명하는 비교 연산자를 선택합니다.

         이 예제에서 비교 연산자는 `is`입니다. 사용 가능한 옵션은 이전 단계에서 선택한 속성에 따라 다릅니다. 옵션은 수치 이상, 같음 및 보다 작은 값 중 적어도 하나를 포함하거나 포함하지 않는 일치 값과 같은 다른 비교 옵션을 포함할 수 있습니다. 이 예제에서 옵션은 `is` 및 `is not`입니다.

      1. **[!UICONTROL ...]**&#x200B;을(를) 클릭하고 조건의 기반이 되는 특성 값을 선택합니다.

         옵션은 속성의 설정에 따라 다릅니다. 옵션을 선택하거나 조건에 대한 텍스트 또는 숫자 값을 입력하라는 메시지가 표시될 수 있습니다. 이 예제에서 선택 항목은 `Yes`입니다.

         선택한 항목이 문에 표시되어 조건을 완료합니다.

         ![조건 줄 2, 파트3](assets/ob-listing-rule-condition-is.png){width="500"}

   이 조건은 완료되었습니다. 명시된 바와 같이, 이 조건은 Amazon FBA 특성이 `Yes` 값으로 설정된 [!DNL Commerce] 카탈로그의 모든 제품을 지역 및 스토어의 Amazon에 나열할 수 있음을 의미합니다. 조건 라인을 더 추가하여 적격 제품의 범위를 더 좁힐 수 있습니다.

1. 문에 다른 조건 라인을 추가하려면 1단계로 돌아가서 원하는 조건이 모두 완료될 때까지 프로세스를 반복합니다.

언제든지 줄 끝에 있는 삭제(![삭제 아이콘](assets/btn-del-red.png)) 아이콘을 클릭하여 조건문의 줄을 삭제할 수 있습니다.
