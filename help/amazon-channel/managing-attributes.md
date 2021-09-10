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

Amazon과 [!DNL Commerce] 모두 제품을 정의하는 데 사용되는 속성 시스템인 제품 속성 시스템을 사용합니다. 속성은 제품에 대한 설명, 콘텐츠, 이미지, 가격 및 다양한 데이터를 정의합니다.

Commerce와 Amazon 간의 성공적인 통신에서는 [!DNL Commerce] 속성이 해당 Amazon 속성에 올바르게 매핑되거나 일치되어야 합니다. Amazon과 통합할 때 이러한 속성을 Amazon 속성에 매핑합니다. 완료되면 [!DNL Commerce]이(가) Amazon 목록을 [!DNL Commerce] 제품 카탈로그와 동기화하고 유지 관리할 수 있습니다.

예를 들어 [!DNL Commerce] 카탈로그 및 Amazon 목록에 동일한 항목이 있다고 가정해 보십시오. 제품에 대한 하나의 속성은 항목의 목록 가격일 수 있습니다. [!DNL Commerce]의 목록 가격 이름은 `Price`로 지정될 수 있고, Amazon의 목록 가격은 `ListingPrice`로 지정될 수 있습니다. [!DNL Commerce]을(를) Amazon과 통신할 때 [!DNL Commerce] 속성 `Price`이(가) `ListingPrice`이라는 Amazon 속성과 동일하도록 지시해야 합니다. 이 프로세스를 _속성 관리_&#x200B;라고 하며, 새 속성을 만들고 기존 속성을 편집하는 것을 포함합니다. 특성이 올바르게 일치하는지 확인하면 [!DNL Commerce] 과 Amazon 간의 올바른 통신이 보장됩니다.

속성 매핑이 설정되면 [!DNL Commerce]은(는) Amazon과 제품 정보를 주고 받을 수 있습니다. Amazon 제품 목록이 있는 경우 [!DNL Commerce]에서 Amazon 제품 및 세부 사항을 [!DNL Commerce] 카탈로그로 가져와 중앙 단일 제품 카탈로그에서 관리할 수 있습니다.

Amazon 판매 채널을 사용하면 Amazon 판매 채널 홈 페이지의 [_[!UICONTROL Attributes]_보기](./attributes-view.md)에서 필요에 따라 속성에 액세스, 검토, 생성 및 관리할 수 있습니다. [!DNL Commerce] 카탈로그에 속성을 추가하는 경우 모든 제품에서 해당 값을 업데이트해야 할 수 있습니다.

[!DNL Commerce] 및 Amazon 속성 세트 및 값에 대한 자세한 내용은 다음을 참조하십시오.

- [특성 기본 사항](https://docs.magento.com/user-guide/catalog/product-attributes.html) 관리{target=&quot;_blank&quot;}
- [속성 만들기](./creating-attributes.md#create-an-attribute)
- [기존 속성 편집](./creating-attributes.md#edit-an-attribute)
- [속성 매핑 보기](./amazon-matching-attributes-values.md)
- [속성 매핑 편집 또는 생성](./amazon-manually-update-incomplete-listing.md)
