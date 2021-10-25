---
title: 만들기 [!DNL Commerce] Amazon 속성
description: Amazon 판매 채널 온보딩 프로세스를 완료하기 전에 필요한 항목이 있는지 확인하십시오 [!UICONTROL Commerce] 제품 속성을 사용합니다.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# 만들기 [!DNL Commerce] Amazon 속성

온보딩하기 전에 [!DNL Amazon Seller Central] 계정을 추가하는 것이 가장 좋습니다 [!DNL Commerce] [제품 속성](https://docs.magento.com/user-guide/stores/attributes-product.html)제품 목록을 매핑하려면 {target=&quot;_blank&quot;}. 온보딩을 완료하면 다음을 통해 제품 속성을 관리할 수 있습니다. [속성](./managing-attributes.md) 의 탭 [Amazon 영업 채널 홈](./amazon-sales-channel-home.md) 페이지.

이러한 지침은 [!DNL Commerce] Amazon ASIN 및 Amazon 조건에 대한 속성입니다. Amazon EAN, Amazon ISBN 및 Amazon UPC를 포함한 추가 속성을 만드는 것이 좋습니다. Amazon 목록 가격을 가격책정 규칙의 가격 소스로 사용하려면 Amazon 가격 속성을 생성할 수도 있습니다. 이러한 속성은 온보딩 중에 목록 및 가격 설정을 구성할 때 사용됩니다. 또한 Amazon 목록을 만들고 업데이트하거나 동기화할 때 이러한 특성을 사용하십시오 [!DNL Commerce] 카탈로그 및 Amazon 목록.

카탈로그 검색 설정을 사용하면 적합한 검색 매개 변수를 매핑하는 데 도움이 되는 일치하는 검색 매개 변수를 설정할 수 있습니다 [!DNL Commerce] Amazon 목록이 있는 제품. 매핑되면 Amazon에서 가격 책정, 수량, 무시, 주문 및 제품 동기화와 관련된 작업을 활성화합니다.

이러한 값을 정의하면 정확한 일치 가능성이 높아지므로 나중에 수동으로 제품 목록을 일치시킬 필요가 최소화됩니다. 온보딩의 일부로 속성 추가 [사전 설정 작업](./amazon-pre-setup-tasks.md), Amazon 판매 채널은 Amazon과 간에 온보딩하고 제품 데이터를 동기화하는 동안 제품을 자동으로 일치시킬 가능성이 높습니다 [!DNL Commerce] 온보딩 후.

Amazon ASIN 속성만 만드는 경우(제품당 ASIN 값을 추가하지 않고) [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하지 않을 수 있습니다. 을 통해 제품을 수동으로 일치시킬 수 있습니다. _저장소 검토_. 그러나 수동 일치로는 제품 데이터를 공유 및 동기화하는 데 필요한 데이터 요소가 만들어지지 않습니다.

>[!IMPORTANT]
>
>수동으로 일치하는 제품에 대한 ASIN, UPC 또는 기타 데이터 요소를 업데이트하는 경우, 두 위치에서 데이터를 업데이트해야 합니다. your [!DNL Commerce] 카탈로그 및 목록의 [!DNL Amazon Seller Central] 계정이 필요합니다.

## Amazon ASIN 제품 속성 만들기

1. 에 로그인합니다. [!DNL Commerce] 관리자.

1. 클릭 **[!UICONTROL Stores]** 왼쪽 메뉴에 있습니다.

1. 에서 _[!UICONTROL Attributes]_섹션을 클릭합니다.**[!UICONTROL Product]**.

1. 속성 속성을 열려면 **[!UICONTROL Add New Attribute]**.

1. 대상 **[!UICONTROL Default Label]**, 입력 `Amazon ASIN` (속성의 이름)

1. 대상 **[!UICONTROL Catalog Input Type for Store Owner]**, 선택 `Text Field`.

1. 대상 **[!UICONTROL Values Required]**, 선택 `No`.

   Amazon에 제품을 나열하려면 Amazon ASIN이 필요하지만 일부 카탈로그 제품이 Amazon에 나열되지 않을 수 있습니다.

1. 를 확장합니다. _[!UICONTROL Advanced Attribute Properties]_섹션을 설정하고 옵션을 설정합니다.

   - 대상 **[!UICONTROL Attribute Code]**, 입력 `amazon_asin`.

   - 대상 **[!UICONTROL Scope]**, 선택 `Global`.

   - 대상 **[!UICONTROL Unique Value]**, 선택 `No`.

   - 대상 **[!UICONTROL Input Validation for Store Owner]**, 선택 `None`.

   - 대상 **[!UICONTROL Add to Column Options]**, 선택 `Yes`.

   - 대상 **[!UICONTROL Use in Filter Options]**, 선택 `Yes`.

1. 클릭 **[!UICONTROL Save Attribute]**.

![Amazon ASIN 특성](assets/creating-asin-attribute.png)

## Amazon 조건 제품 속성 만들기

1. 에 로그인합니다. [!DNL Commerce] 관리자.

1. 클릭 **[!UICONTROL Stores]** 왼쪽 메뉴에 있습니다.

1. 에서 _[!UICONTROL Attributes]_섹션을 클릭합니다.**[!UICONTROL Product]**.

1. 속성 속성을 열려면 **[!UICONTROL Add New Attribute]**.

1. 대상 **[!UICONTROL Default Label]**, 입력 `Amazon Condition` (속성의 이름)

1. 대상 **[!UICONTROL Catalog Input Type for Store Owner]**, 선택 `Dropdown`.

   다음 _[!UICONTROL Manage Options (Values of your Attribute)]_섹션이 나타납니다.

1. 대상 **[!UICONTROL Values Required]**, 선택 `No`.

1. 대상 **[!UICONTROL Manage Options (Values for your Attribute)]**, 각 조건 옵션을 추가합니다.

   표준 Amazon 조건은 다음과 같습니다.

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. 클릭 **[!UICONTROL Add Option]**.

1. 을(를) 선택합니다 **[!UICONTROL Is Default]** 기본 선택 항목으로 지정할 조건에 대한 옵션입니다.

1. 에서 _[!UICONTROL Admin]_열에서 추가할 조건 레이블(예: `New`, `Used`, 및 `Used-Like New`)

1. 클릭 **[!UICONTROL Add Option]** 필요에 따라 옵션을 더 추가합니다.

1. 확장 _[!UICONTROL Advanced Attribute Properties]_섹션을 설정하고 옵션을 설정합니다.

   - 대상 **[!UICONTROL Attribute Code]**, 입력 `amazon_condition`.

   - 대상 **[!UICONTROL Scope]**, 선택 `Global`.

   - 대상 **[!UICONTROL Unique Value]**, 선택 `No`.

   - 대상 **[!UICONTROL Input Validation for Store Owner]**, 선택 `None`.

   - 대상 **[!UICONTROL Add to Column Options]**, 선택 `Yes`.

   - 대상 **[!UICONTROL Use in Filter Options]**, 선택 `Yes`.

1. 클릭 **[!UICONTROL Save Attribute]**.

![Amazon 조건 속성](assets/creating-amazon-condition-attribute.png)

![다음 아이콘](assets/btn-next.png) [**API 키 추가 또는 확인 계속**](./amazon-verify-api-key.md)
