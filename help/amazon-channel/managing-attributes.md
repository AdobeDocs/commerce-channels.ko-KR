---
title: Amazon 목록의 속성 관리
description: Amazon 속성에 대한 Commerce 제품 속성 매핑을 관리하여 시스템 간에 정확한 제품 정보를 제공할 수 있습니다.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Amazon 목록의 속성 관리

Amazon 및 [!DNL Commerce] 둘 다 제품을 정의하는 데 사용되는 제품 속성 시스템(속성)을 사용합니다. 속성은 제품에 대한 설명, 콘텐츠, 이미지, 가격 및 다양한 데이터를 정의합니다.

Commerce와 Amazon 간의 성공적인 커뮤니케이션을 위해서는 다음과 같은 작업이 필요합니다. [!DNL Commerce] 속성을 해당 Amazon 속성에 올바르게 매핑(또는 일치)할 수 있습니다. Amazon과 통합할 때 이러한 속성을 Amazon 속성에 매핑합니다. 완료되면, [!DNL Commerce] 을(를) 통해 Amazon 목록을 동기화하고 유지 관리할 수 있습니다. [!DNL Commerce] 제품 카탈로그.

예를 들어, 다음 항목에 동일한 항목이 있다고 가정해 보겠습니다. [!DNL Commerce] 카탈로그 및 Amazon 목록. 제품에 대한 속성 중 하나는 항목의 목록 가격일 수 있습니다. 의 가격 목록 이름 [!DNL Commerce] 이름이 지정될 수 있음 `Price`, 반면에 Amazon의 목록 가격은 이름이 지정될 수 있습니다 `ListingPrice`. 다음을 지시해야 합니다. [!DNL Commerce] Amazon과 통신할 때 [!DNL Commerce] 속성 이름: `Price` 은(는) 이라는 Amazon 속성과 동일합니다. `ListingPrice`. 이 프로세스를 호출합니다. _속성 관리_&#x200B;및 에는 새 속성 만들기 및 기존 속성 편집이 포함됩니다. 속성이 올바르게 일치하는지 확인하면 다음 사이에 올바른 통신이 이루어집니다 [!DNL Commerce] 그리고 Amazon.

속성 매핑이 설정되면 [!DNL Commerce] 는 Amazon과 제품 정보를 주고받을 수 있습니다. Amazon 제품 목록이 있는 경우 [!DNL Commerce] 에서 Amazon 제품 및 세부 사항을 로 가져올 수 있습니다. [!DNL Commerce] 카탈로그 를 사용하면 중앙의 단일 제품 카탈로그에서 Amazon 목록을 관리할 수 있습니다.

Amazon sales channel을 사용하면 필요에 따라 다음과 같이 속성에 액세스하고, 검토하고, 만들고, 관리할 수 있습니다 [_[!UICONTROL Attributes]_보기](./attributes-view.md) Amazon sales channel 홈 페이지에서 확인할 수 있습니다. 에 속성을 추가하는 경우 [!DNL Commerce] 카탈로그에서는 모든 제품에 대해 이러한 값을 업데이트해야 할 수 있습니다.

에 대한 자세한 내용 [!DNL Commerce] 및 Amazon 속성 세트와 값은 다음을 참조하십시오.

- [속성 관리 기본 사항](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [속성 만들기](./creating-attributes.md#create-an-attribute)
- [기존 속성 편집](./creating-attributes.md#edit-an-attribute)
- [속성 매핑 보기](./amazon-matching-attributes-values.md)
- [속성 매핑 편집 또는 생성](./amazon-manually-update-incomplete-listing.md)
