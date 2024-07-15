---
title: Amazon 목록의 속성 관리
description: Commerce 제품 특성과 Amazon 특성 간의 매핑을 관리하여 시스템 간에 정확한 제품 정보를 얻을 수 있습니다.
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Amazon 목록의 속성 관리

Amazon과 [!DNL Commerce] 모두 제품을 정의하는 데 사용되는 제품 속성 시스템(특성)을 사용합니다. 속성은 제품에 대한 설명, 콘텐츠, 이미지, 가격 및 다양한 데이터를 정의합니다.

Commerce과 Amazon이 성공적으로 통신하려면 [!DNL Commerce] 특성을 해당 Amazon 특성에 올바르게 매핑(또는 일치)해야 합니다. Amazon과 통합할 때 이러한 속성을 Amazon 속성에 매핑합니다. 완료되면 [!DNL Commerce]은(는) [!DNL Commerce] 제품 카탈로그와 Amazon 목록을 동기화하고 유지 관리할 수 있습니다.

예를 들어 [!DNL Commerce] 카탈로그 및 Amazon 목록에 동일한 항목이 있다고 가정해 보겠습니다. 제품에 대한 속성 중 하나는 항목의 목록 가격일 수 있습니다. [!DNL Commerce]의 목록 가격 이름은 `Price`(으)로 지정될 수 있고 Amazon의 목록 가격 이름은 `ListingPrice`(으)로 지정될 수 있습니다. Amazon과 통신할 때 이름이 `Price`인 [!DNL Commerce] 특성이 이름이 `ListingPrice`인 Amazon 특성과 같음을 [!DNL Commerce]에 지시해야 합니다. 이 프로세스를 _특성 관리_&#x200B;라고 하며, 새 특성을 만들고 기존 특성을 편집하는 작업이 포함됩니다. 특성이 올바르게 일치하는지 확인하면 [!DNL Commerce]과(와) Amazon 간에 올바른 통신이 가능합니다.

특성 매핑이 설정되면 [!DNL Commerce]에서 Amazon과 제품 정보를 주고받을 수 있습니다. Amazon 제품 목록이 있는 경우 [!DNL Commerce]이(가) Amazon 제품 및 세부 정보를 [!DNL Commerce] 카탈로그로 가져와 중앙의 단일 제품 카탈로그에서 Amazon 목록을 관리할 수 있습니다.

Amazon 판매 채널을 사용하면 Amazon 판매 채널 홈 페이지의 [_[!UICONTROL Attributes]_보기](./attributes-view.md)에서 필요에 따라 속성에 액세스하고, 검토하고, 만들고, 관리할 수 있습니다. [!DNL Commerce] 카탈로그에 특성을 추가하는 경우 모든 제품에서 해당 값을 업데이트해야 할 수 있습니다.

[!DNL Commerce] 및 Amazon 특성 집합 및 값에 대한 자세한 내용은 다음을 참조하십시오.

- [특성 관리 기본 사항](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [속성 만들기](./creating-attributes.md#create-an-attribute)
- [기존 속성 편집](./creating-attributes.md#edit-an-attribute)
- [속성 매핑 보기](./amazon-matching-attributes-values.md)
- [속성 매핑 편집 또는 생성](./amazon-manually-update-incomplete-listing.md)
