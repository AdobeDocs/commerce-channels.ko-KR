---
title: 속성 관리
description: Amazon 속성에 상거래 제품 속성의 매핑을 관리하여 시스템 간의 제품 정보를 정확하게 제공할 수 있습니다.
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 속성 관리

Amazon 및 [!DNL Commerce] 둘 다 제품을 정의하는 데 사용되는 속성 이라고 하는 제품 속성 시스템을 사용합니다. 속성은 제품에 대한 설명, 콘텐츠, 이미지, 가격 및 다양한 데이터를 정의합니다.

Commerce와 Amazon 간의 성공적인 커뮤니케이션에는 다음이 필요합니다 [!DNL Commerce] 속성이 해당 Amazon 속성에 올바르게 매핑되거나 일치되어야 합니다. Amazon과 통합할 때 이러한 속성을 Amazon 속성에 매핑합니다. 완료되면, [!DNL Commerce] Amazon 목록을 사용자의 [!DNL Commerce] 제품 카탈로그

예를 들어, [!DNL Commerce] 카탈로그 및 Amazon 목록 제품에 대한 하나의 속성은 항목의 목록 가격일 수 있습니다. 의 목록 가격 이름 [!DNL Commerce] 이름이 지정되었을 수 있습니다. `Price`로 설정되지만 Amazon의 목록 가격은 `ListingPrice`. 다음 사항을 지시해야 합니다. [!DNL Commerce] Amazon과 통신할 때 [!DNL Commerce] 명명된 속성 `Price` 는 이름이 인 Amazon 속성과 동일합니다 `ListingPrice`. 이 프로세스를 라고 합니다 _속성 관리_, 에는 새 속성 만들기 및 기존 속성 편집이 포함됩니다. 속성이 제대로 일치하는지 확인하면 두 속성 간에 올바른 통신이 보장됩니다 [!DNL Commerce] 및 Amazon.

속성 매핑이 설정되면, [!DNL Commerce] Amazon과 제품 정보를 주고 받을 수 있습니다. Amazon 제품 목록이 있는 경우, [!DNL Commerce] Amazon 제품 및 세부 사항을 [!DNL Commerce] 카탈로그 - 중앙 단일 제품 카탈로그에서 Amazon 목록을 관리할 수 있습니다.

Amazon 영업 채널을 사용하면 필요에 따라 [_[!UICONTROL Attributes]_보기](./attributes-view.md) Amazon 영업 채널 홈 페이지에서 확인할 수 있습니다. 속성을 [!DNL Commerce] catalog, it could required a update of that values from all products.

에 대한 자세한 정보 [!DNL Commerce] 및 Amazon 속성 세트와 값을 참조하십시오.

- [속성 관리 기본 사항](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}
- [속성 만들기](./creating-attributes.md#create-an-attribute)
- [기존 속성 편집](./creating-attributes.md#edit-an-attribute)
- [속성 매핑 보기](./amazon-matching-attributes-values.md)
- [속성 매핑 편집 또는 생성](./amazon-manually-update-incomplete-listing.md)
