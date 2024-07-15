---
title: Amazon용 Commerce 속성 만들기
description: Amazon 판매 채널 온보딩 프로세스를 완료하기 전에 필요한 [!UICONTROL Commerce] 제품 특성이 있는지 확인하십시오.
role: Admin
feature: Sales Channels, Products, Configuration
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Amazon용 Commerce 속성 만들기

[!DNL Amazon Seller Central] 계정을 온보딩하기 전에 [!DNL Commerce] [제품 특성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)을 추가하여 제품 목록을 매핑하는 것이 좋습니다. 온보딩을 완료한 후 [Amazon 판매 채널 홈](./amazon-sales-channel-home.md) 페이지의 [특성](./managing-attributes.md) 탭을 통해 제품 특성을 관리할 수 있습니다.

이 지침에서는 Amazon ASIN 및 Amazon 조건에 대한 [!DNL Commerce] 특성을 만드는 방법에 대해 자세히 설명합니다. Amazon EAN, Amazon ISBN 및 Amazon UPC를 비롯한 추가 속성을 만드는 것이 좋습니다. Amazon 목록 가격을 가격책정 규칙의 가격 출처로 사용하려면 Amazon 가격 속성을 생성할 수도 있습니다. 이러한 속성은 온보딩 중에 목록 및 가격 설정을 구성할 때 사용됩니다. 또한 Amazon 목록을 만들고 [!DNL Commerce] 카탈로그를 업데이트하고 Amazon 목록과 동기화할 때도 이러한 특성을 사용합니다.

카탈로그 검색 설정을 사용하면 적격한 [!DNL Commerce] 제품을 Amazon 목록에 매핑하는 데 도움이 되는 일치하는 검색 매개 변수를 설정할 수 있습니다. 매핑되면 Amazon은 가격책정, 수량, 대체, 주문 및 제품 동기화와 관련된 작업을 활성화합니다.

이러한 값을 정의하면 정확한 일치가 발생할 가능성이 높아져 나중에 수동으로 제품 목록을 일치시킬 필요가 최소화됩니다. 속성을 온보딩 [사전 설정 작업](./amazon-pre-setup-tasks.md)의 일부로 추가하면 Amazon 판매 채널에서는 온보딩 중에 제품과 자동으로 일치하고 온보딩 후 Amazon과 [!DNL Commerce] 간에 제품 데이터를 동기화할 수 있습니다.

제품당 ASIN 값을 추가하지 않고 Amazon ASIN 특성만 만드는 경우 [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하지 않을 수 있습니다. _스토어 검토_&#x200B;를 통해 제품을 수동으로 일치시킬 수 있습니다. 그러나 수동 일치는 제품 데이터를 공유하고 동기화하는 데 필요한 데이터 요소를 만들지 않습니다.

>[!IMPORTANT]
>
>수동으로 일치하는 제품에 대한 ASIN, UPC 또는 기타 데이터 요소를 업데이트하는 경우 [!DNL Commerce] 카탈로그와 [!DNL Amazon Seller Central] 계정의 목록을 비롯한 두 위치에서 데이터를 업데이트해야 합니다.

## Amazon ASIN 제품 속성 만들기

1. [!DNL Commerce] 관리자에 로그인합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Stores]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Attributes]_섹션에서&#x200B;**[!UICONTROL Product]**을(를) 클릭합니다.

1. 특성 속성을 열려면 **[!UICONTROL Add New Attribute]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Default Label]**&#x200B;에 `Amazon ASIN`(특성 이름)을 입력하십시오.

1. **[!UICONTROL Catalog Input Type for Store Owner]**&#x200B;의 경우 `Text Field`을(를) 선택하십시오.

1. **[!UICONTROL Values Required]**&#x200B;의 경우 `No`을(를) 선택하십시오.

   Amazon ASIN이 Amazon에 제품을 나열해야 하지만, 일부 카탈로그 제품이 Amazon에 나열되지 않을 수 있습니다.

1. _[!UICONTROL Advanced Attribute Properties]_섹션을 확장하고 옵션을 설정합니다.

   - **[!UICONTROL Attribute Code]**&#x200B;에 대해 `amazon_asin`을(를) 입력하십시오.

   - **[!UICONTROL Scope]**&#x200B;의 경우 `Global`을(를) 선택하십시오.

   - **[!UICONTROL Unique Value]**&#x200B;의 경우 `No`을(를) 선택하십시오.

   - **[!UICONTROL Input Validation for Store Owner]**&#x200B;의 경우 `None`을(를) 선택하십시오.

   - **[!UICONTROL Add to Column Options]**&#x200B;의 경우 `Yes`을(를) 선택하십시오.

   - **[!UICONTROL Use in Filter Options]**&#x200B;의 경우 `Yes`을(를) 선택하십시오.

1. **[!UICONTROL Save Attribute]**&#x200B;을(를) 클릭합니다.

![Amazon ASIN 특성](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Amazon Condition 제품 속성 만들기

1. [!DNL Commerce] 관리자에 로그인합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Stores]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Attributes]_섹션에서&#x200B;**[!UICONTROL Product]**을(를) 클릭합니다.

1. 특성 속성을 열려면 **[!UICONTROL Add New Attribute]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Default Label]**&#x200B;에 `Amazon Condition`(특성 이름)을 입력하십시오.

1. **[!UICONTROL Catalog Input Type for Store Owner]**&#x200B;의 경우 `Dropdown`을(를) 선택하십시오.

   _[!UICONTROL Manage Options (Values of your Attribute)]_섹션이 나타납니다.

1. **[!UICONTROL Values Required]**&#x200B;의 경우 `No`을(를) 선택하십시오.

1. **[!UICONTROL Manage Options (Values for your Attribute)]**&#x200B;의 경우 각 조건 옵션을 추가하십시오.

   표준 Amazon 조건은 다음과 같습니다.

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. **[!UICONTROL Add Option]**&#x200B;을(를) 클릭합니다.

1. 기본 선택으로 사용할 조건에 대한 **[!UICONTROL Is Default]** 옵션을 선택하십시오.

1. _[!UICONTROL Admin]_열에 추가할 조건 레이블에 대한 텍스트를 입력하십시오(예: `New`, `Used` 및 `Used-Like New`).

1. 필요에 따라 옵션을 추가하려면 **[!UICONTROL Add Option]**&#x200B;을(를) 클릭하십시오.

1. _[!UICONTROL Advanced Attribute Properties]_섹션을 확장하고 옵션을 설정합니다.

   - **[!UICONTROL Attribute Code]**&#x200B;에 대해 `amazon_condition`을(를) 입력하십시오.

   - **[!UICONTROL Scope]**&#x200B;의 경우 `Global`을(를) 선택하십시오.

   - **[!UICONTROL Unique Value]**&#x200B;의 경우 `No`을(를) 선택하십시오.

   - **[!UICONTROL Input Validation for Store Owner]**&#x200B;의 경우 `None`을(를) 선택하십시오.

   - **[!UICONTROL Add to Column Options]**&#x200B;의 경우 `Yes`을(를) 선택하십시오.

   - **[!UICONTROL Use in Filter Options]**&#x200B;의 경우 `Yes`을(를) 선택하십시오.

1. **[!UICONTROL Save Attribute]**&#x200B;을(를) 클릭합니다.

![Amazon 조건 특성](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![다음 아이콘](assets/btn-next.png) [**API 키를 계속 추가하거나 확인**](./amazon-verify-api-key.md)
