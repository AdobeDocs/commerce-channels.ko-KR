---
title: Amazon 목록에 대한 카탈로그 검색
description: 적격한 Commerce 카탈로그 제품을 Amazon 목록에 매핑하는 데 도움이 되는 속성 일치를 설정하려면 카탈로그 검색 설정을 업데이트합니다.
feature: Sales Channels, Search, Catalog Management, Products, Configuration
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Amazon 목록에 대한 카탈로그 검색

_카탈로그 검색_ 설정은 스토어 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정을 사용하면 적격 매핑에 도움이 되는 속성 일치를 설정할 수 있습니다 [!DNL Commerce] Amazon 목록이 포함된 제품 매핑되면 Amazon은 가격책정, 수량, 대체, 주문 및 제품 동기화와 관련된 작업을 활성화합니다.

이러한 매핑 값을 정의하면 정확한 일치의 가능성이 증가하므로 제품 목록을 수동으로 일치시킬 필요가 없습니다. 의 일부로 속성 추가 [사전 설정 작업](./amazon-pre-setup-tasks.md), Amazon sales channel 은 Amazon 와 간에 온보딩 및 제품 데이터 동기화 중에 제품이 자동으로 일치할 가능성이 더 높습니다 [!DNL Commerce].

제품당 ASIN 값을 추가하지 않고 Amazon ASIN 속성만 만드는 경우 [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하지 않을 수 있습니다. 다음을 수행할 수 있습니다. [수동으로 할당](./creating-assigning-catalog-products.md) 제품. 그러나 수동 일치는 제품 데이터를 공유하고 동기화하는 데 필요한 데이터 요소를 만들지 않습니다.

>[!IMPORTANT]
>
>제품을 수동으로 일치시키고 제품에 대한 ASIN, UPC 또는 기타 데이터 요소를 업데이트하려면 두 위치에서 데이터를 업데이트해야 합니다. 에서 업데이트 [!DNL Commerce] 카탈로그 및 의 Amazon 목록 [!DNL Amazon Seller Central] 계정입니다.

가능한 경우 이러한 속성과 값을 매핑하는 것이 좋습니다. 이 매핑을 완료할 필요는 없지만 제품 일치에 도움이 되며 Amazon과 간의 적절한 카탈로그 동기화에 필요합니다. [!DNL Commerce].

속성을 추가하려면 다음을 참조하십시오 [Amazon 일치를 위한 제품 속성 만들기](./ob-creating-magento-attributes.md).

## 구성 [!UICONTROL Catalog Search] 설정

1. 클릭 **[!UICONTROL Listing Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 확장 _[!UICONTROL Catalog Search]_섹션.

1. 대상 **[!UICONTROL ASIN]**, Amazon ASIN 값에 대해 만든 제품 속성을 선택합니다.

   ASIN([!DNL Amazon Standard Identification Number])는 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다.

1. 대상 **[!UICONTROL EAN]**&#x200B;에서 Amazon EAN 값에 대해 만든 제품 속성을 선택합니다.

   EAN(유럽 문서 번호)은 바코드 표준, 12자리 또는 13자리 제품 식별 코드입니다. 각 EAN은 제품, 제조업체 및 해당 속성을 고유하게 식별하며, 일반적으로 EAN은 제품 라벨 또는 포장재에 바코드로 인쇄됩니다. Amazon은 검색 결과의 품질과 카탈로그의 품질을 향상시키기 위해 EAN 코드가 필요합니다. 제조업체로부터 EAN을 구할 수 있습니다.

1. 대상 **[!UICONTROL GCID]**, Amazon GCIN 값에 대해 만든 제품 속성을 선택합니다.

   GCID(글로벌 카탈로그 식별자)는 UPC 코드나 ISBN이 없는 제품에 대한 ID입니다. Amazon의 Brand Registry를 사용하면 브랜드 소유자로 등록하고 제품에 대한 고유 ID를 만들 수 있습니다.

1. 대상 **[!UICONTROL ISBN]**&#x200B;에서 Amazon ISBN 값에 대해 만든 제품 속성을 선택합니다.

   국제 표준 도서 번호(ISBN)는 고유한 상업용 도서 식별자 바코드입니다. 각 ISBN 코드는 장부를 고유하게 식별합니다. ISBN은 10자리 또는 13자리입니다. 2007년 1월 1일 이후 할당된 모든 ISBN은 13자리 수를 가진다.

1. 대상 **[!UICONTROL UPC]**, Amazon UPC 값에 대해 만든 제품 속성을 선택합니다.

   범용 제품 코드(UPC)는 미국의 소매 포장에 광범위하게 사용되는 12자리 바코드입니다.

1. 대상 **[!UICONTROL General Search]**&#x200B;일반 검색 일치에 사용할 제품 속성을 선택합니다.

   이 속성은 일치하도록 선택할 수 있는 속성입니다. [!DNL Commerce] 제품을 적절한 Amazon 목록에 추가합니다. 일반 검색은 카탈로그의 키워드 검색을 사용합니다. 따라서 를 사용하는 것이 좋습니다 [!DNL Commerce] 제품 SKU 또는 제품 이름과 같이 관련 키워드를 전달하는 특성입니다. 일반 검색은 가능한 많은 일치 항목을 반환할 수 있으며, 이러한 경우 가능한 일치 항목에서 적절한 Amazon 목록을 선택할 수 있습니다. 이 필드에 대한 일반적인 선택 사항은 다음과 같습니다. `Product Name`.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save listing settings]**.

![카탈로그 검색](assets/amazon-catalog-search.png){width="500" zoomable="yes"}

| 필드 | 설명 |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL ASIN] | 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유 블록입니다.<br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다. |
| [!UICONTROL EAN (European Article Number)] | 12자리 또는 13자리 제품 식별 코드. EAN(유럽 문서 번호)은 바코드 표준, 12자리 또는 13자리 제품 식별 코드입니다. 각 EAN은 제품, 제조업체 및 해당 속성을 고유하게 식별하며, 일반적으로 EAN은 제품 라벨 또는 포장재에 바코드로 인쇄됩니다. Amazon은 검색 결과의 품질과 카탈로그의 품질을 향상시키기 위해 EAN 코드가 필요합니다. 제조업체로부터 EAN을 구할 수 있습니다. |
| [!UICONTROL GCID (Global Catalog Identifier)] | GCID(글로벌 카탈로그 식별자)는 UPC 코드나 ISBN이 없는 제품에 대한 ID입니다. Amazon의 Brand Registry를 사용하면 브랜드 소유자로 등록하고 UPC 또는 ISBN이 없을 수 있는 제품에 대한 고유 ID를 만들 수 있습니다. |
| [!UICONTROL ISBN (International Standard Book Number)] | 10자리 또는 13자리 고유 상업용 책 식별자 바코드. 국제 표준 도서 번호(ISBN)는 고유한 상업용 도서 식별자 바코드입니다. 각 ISBN 코드는 장부를 고유하게 식별합니다. ISBN은 10자리 또는 13자리입니다. 2007년 1월 1일 이후 할당된 모든 ISBN은 13자리 수를 가진다. |
| UPC(범용 제품 코드) | 12자리 바코드. 범용 제품 코드(UPC)는 미국의 소매 포장에 광범위하게 사용되는 12자리 바코드입니다. |
| [!UICONTROL General Search] | 속성을 선택합니다. 이 속성은 일치하도록 선택할 수 있는 속성입니다. [!DNL Commerce] 제품을 적절한 Amazon 목록에 추가합니다. 일반 검색은 카탈로그의 키워드 검색을 사용합니다. 따라서 를 사용하는 것이 좋습니다 [!DNL Commerce] 제품 SKU 또는 제품 이름과 같이 관련 키워드를 전달하는 특성입니다. 일반 검색은 가능한 많은 일치 항목을 반환할 수 있으며, 이러한 경우 가능한 일치 항목에서 적절한 Amazon 목록을 선택할 수 있습니다. 이 필드에 대한 일반적인 선택 사항은 다음과 같습니다. `Product Name`. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
