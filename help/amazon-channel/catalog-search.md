---
title: 카탈로그 검색
description: 적합한 상거래 카탈로그 제품을 Amazon 목록에 매핑하는 데 도움이 되는 속성 일치를 설정하려면 카탈로그 검색 설정을 업데이트하십시오.
redirect_from: /sales-channels/asc/ob-catalog-search.html: 
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 981
ht-degree: 0%

---

# 카탈로그 검색

_카탈로그_ 검색 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스합니다.

이러한 설정을 사용하면 자격이 있는 [!DNL Commerce] 제품을 Amazon 목록에 매핑하는 데 도움이 되는 속성 일치를 설정할 수 있습니다. 매핑되면 Amazon에서 가격 책정, 수량, 무시, 주문 및 제품 동기화와 관련된 작업을 활성화합니다.

이러한 매핑 값을 정의하면 정확한 일치 가능성이 높아지므로 제품 목록을 수동으로 일치시킬 필요가 최소화됩니다. [사전 설정 작업](./amazon-pre-setup-tasks.md)의 일부로 속성을 추가하면 Amazon 판매 채널이 Amazon과 [!DNL Commerce] 간에 제품 데이터를 온보딩하고 동기화하는 동안 제품을 자동으로 일치시킬 가능성이 높아집니다.

Amazon ASIN 속성만 만드는 경우(제품당 ASIN 값을 추가하지 않고) [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하지 않을 수 있습니다. [수동으로](./creating-assigning-catalog-products.md)제품을 할당할 수 있습니다. 그러나 수동 일치로는 제품 데이터를 공유 및 동기화하는 데 필요한 데이터 요소가 만들어지지 않습니다.

>[!IMPORTANT]
>
>제품을 수동으로 일치시키고 제품에 대한 ASIN, UPC 또는 기타 데이터 요소를 업데이트하려면 두 위치에서 데이터를 업데이트해야 합니다. [!DNL Commerce] 카탈로그와 [!DNL Amazon Seller Central] 계정의 Amazon 목록에서 업데이트합니다.

가능한 경우 이러한 속성과 값을 매핑하는 것이 좋습니다. 이 매핑을 완료할 필요는 없지만 제품 일치에 유용하며 Amazon과 [!DNL Commerce] 간의 적절한 카탈로그 동기화에 필요합니다.

속성을 추가하려면 [Amazon Matching](./ob-creating-magento-attributes.md)에 대한 제품 속성 만들기를 참조하십시오.

## [!UICONTROL Catalog Search] 설정 구성

1. 저장소 대시보드에서 **[!UICONTROL Listing Settings]** 을 클릭합니다.

1. _[!UICONTROL Catalog Search]_섹션을 확장합니다.

1. **[!UICONTROL ASIN]**&#x200B;에 대해 Amazon ASIN 값에 대해 만든 제품 속성을 선택합니다.

   ASIN([!DNL Amazon Standard Identification Number])은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다.

1. **[!UICONTROL EAN]**&#x200B;에 대해 Amazon EAN 값에 대해 만든 제품 속성을 선택합니다.

   EAN(European Article Number)은 바코드 표준으로, 12 또는 13자리 제품 식별 코드입니다. 각 EAN은 제품, 제조업체 및 해당 속성을 고유하게 식별합니다. 일반적으로 EAN은 제품 레이블이나 패키징에 바코드 형태로 인쇄됩니다. Amazon에서는 검색 결과의 품질과 카탈로그의 품질을 향상시키기 위해 EAN 코드가 필요합니다. 제조업체에서 EAN을 얻을 수 있습니다.

1. **[!UICONTROL GCID]**&#x200B;에 대해 Amazon GCIN 값에 대해 만든 제품 속성을 선택합니다.

   GCID(Global Catalog Identifier)는 UPC 코드 또는 ISBN이 없는 제품의 ID입니다. Amazon의 Brand Registry를 통해 브랜드 소유자로 등록하고 제품에 대한 고유 ID를 만들 수 있습니다.

1. **[!UICONTROL ISBN]**&#x200B;에 대해 Amazon ISBN 값에 대해 만든 제품 속성을 선택합니다.

   ISBN(International Standard Book Number)은 고유한 상업책 식별자 바코드입니다. 각 ISBN 코드는 책을 고유하게 식별합니다. ISBN은 10자리나 13자리입니다. 2007년 1월 1일 이후에 지정된 모든 ISBN은 13자리 숫자를 갖습니다.

1. **[!UICONTROL UPC]**&#x200B;에 대해 Amazon UPC 값에 대해 만든 제품 속성을 선택합니다.

   UPC(Universal Product Code)는 미국에서 소매 패키징에 광범위하게 사용되는 12자리 바코드 입니다.

1. **[!UICONTROL General Search]**&#x200B;에 대해 일반 검색 일치에 사용할 제품 속성을 선택합니다.

   이 속성은 [!DNL Commerce] 제품을 적절한 Amazon 목록에 일치시키도록 선택할 수 있는 속성입니다. 일반 검색은 카탈로그의 키워드 검색을 사용합니다. 따라서 제품 SKU 또는 제품 이름과 같이 관련 키워드를 전달하는 [!DNL Commerce] 속성을 사용하는 것이 좋습니다. 일반 검색은 가능한 여러 일치 항목을 반환할 수 있으며, 이 경우 가능한 일치 항목 중에서 적절한 Amazon 목록을 선택할 수 있습니다. 이 필드의 일반적인 선택 항목은 `Product Name`입니다.

1. 완료되면 **[!UICONTROL Save listing settings]** 을 클릭합니다.

![카탈로그 검색](assets/amazon-catalog-search.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 을  [!DNL Amazon Standard Identification Number]의미합니다. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL EAN (European Article Number)] | 12자리 또는 13자리 제품 식별 코드입니다. EAN(European Article Number)은 바코드 표준으로, 12 또는 13자리 제품 식별 코드입니다. 각 EAN은 제품, 제조업체 및 해당 속성을 고유하게 식별합니다. 일반적으로 EAN은 제품 레이블이나 패키징에 바코드 형태로 인쇄됩니다. Amazon에서는 검색 결과의 품질과 카탈로그의 품질을 향상시키기 위해 EAN 코드가 필요합니다. 제조업체에서 EAN을 얻을 수 있습니다. |
| [!UICONTROL GCID (Global Catalog Identifier)] | GCID(Global Catalog Identifier)는 UPC 코드 또는 ISBN이 없는 제품의 ID입니다. Amazon의 Brand Registry를 통해 브랜드 소유자로 등록하고 UPC 또는 ISBN이 없을 수 있는 제품에 대한 고유 ID를 만들 수 있습니다. |
| [!UICONTROL ISBN (International Standard Book Number)] | 10자리 또는 13자리 고유한 상용 도서 식별자 바코드. ISBN(International Standard Book Number)은 고유한 상업책 식별자 바코드입니다. 각 ISBN 코드는 책을 고유하게 식별합니다. ISBN은 10자리나 13자리입니다. 2007년 1월 1일 이후에 지정된 모든 ISBN은 13자리 숫자를 갖습니다. |
| UPC(범용 제품 코드) | 12자리 막대 코드입니다. UPC(Universal Product Code)는 미국에서 소매 패키징에 광범위하게 사용되는 12자리 바코드 입니다. |
| [!UICONTROL General Search] | 속성을 선택합니다. 이 속성은 [!DNL Commerce] 제품을 적절한 Amazon 목록에 일치시키도록 선택할 수 있는 속성입니다. 일반 검색은 카탈로그의 키워드 검색을 사용합니다. 따라서 제품 SKU 또는 제품 이름과 같이 관련 키워드를 전달하는 [!DNL Commerce] 속성을 사용하는 것이 좋습니다. 일반 검색은 가능한 여러 일치 항목을 반환할 수 있으며, 이 경우 가능한 일치 항목 중에서 적절한 Amazon 목록을 선택할 수 있습니다. 이 필드의 일반적인 선택 항목은 `Product Name`입니다. |

**빠른 액세스**  -  [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
