---
title: Amazon 속성 매핑 보기
description: 연결된 상거래 특성 값을 확인하여 상거래 및 Amazon 간에 올바르게 동기화하십시오.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Amazon 속성 매핑 보기

Amazon 속성을 [!DNL Commerce] 속성에 매핑하면 Amazon 영업 채널이 추적되고 모든 Amazon 값의 필터링 가능한 목록을 제공합니다. 이 페이지에서 연결된 [!DNL Commerce] 속성의 값이 [!DNL Commerce] 과 Amazon 간에 올바르게 동기화되는지 확인할 수 있습니다. [!DNL Commerce] 속성에 연결되거나 연결되지 않은 Amazon 속성에 대해 동기화된 값을 검토할 수 있습니다. Amazon 속성을 만들거나 편집하려면 [속성 만들기 및 편집](./creating-attributes.md)을 참조하십시오.

_Amazon 값_&#x200B;은 사용자가 보는 속성 유형과 Amazon 속성에 따라 다릅니다. 예를 들어 `Label`에 대해 나열된 Amazon 값은 텍스트 값이고 `AmazonListPrice`은 숫자 양입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다.

## 속성 값 보기

1. _[!UICONTROL Admin]_사이드바에서&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**&#x200B;로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]** 을 클릭하고 Amazon 속성을 찾은 다음 **[!UICONTROL Create]** 열에서 **[!UICONTROL Edit]** 또는 _[!UICONTROL Action]_를 클릭합니다.

1. **[!UICONTROL Matching Attribute Values]** 탭을 클릭합니다.

   해당 [!DNL Commerce] 카탈로그 제품이 있는 목록은 _Magento 제품 SKU_ 열에 연결된 값을 표시합니다. 링크를 클릭하면 해당 카탈로그 제품 세부 사항 페이지가 열립니다. 제품 세부 사항 페이지의 Amazon 속성에 대한 변경 사항이 Amazon 판매 채널에 다시 동기화되지 않습니다.

>[!TIP]
>목록을 편집하거나 카탈로그 제품에 지정하려면 [필수 정보 업데이트](./amazon-manually-update-incomplete-listing.md)를 참조하십시오.

![속성 값 보기](assets/amazon-managing-attribute-values.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Region] | 저장소 통합 중 **[!DNL Amazon Marketplace]국가**&#x200B;에 정의된 영업 활동의 영역입니다. |
| [!UICONTROL Magento Product SKU] | Amazon 스토어와 동기화된 [!DNL Commerce] 제품을 나타냅니다. 이 값은 [!DNL Commerce]에 의해 지정된 제품 ID이며 카탈로그의 제품에 연결됩니다. [!DNL Commerce]에서 제품을 열려면 링크를 클릭합니다. |
| [!UICONTROL ASIN] | 제품 식별을 위해 Amazon이 제품에 할당한 ASIN(Amazon Standard Identity Number) 10자의 영숫자 고유 식별자를 나타냅니다. |
| [!UICONTROL Amazon Value] | 선택한 속성에 대한 값을 나타냅니다. Amazon 값은 보는 속성 유형과 Amazon 속성에 따라 다릅니다. 예를 들어 `Label`에 대해 나열된 Amazon 값은 텍스트 값이고 `AmazonListPrice`은 숫자 양입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다. |
| [!UICONTROL Status] | 속성 값을 [!DNL Commerce] (으)로 가져와서 [!DNL Commerce] 속성에 연결했는지 여부를 나타냅니다. 옵션: `Not Imported` / `Imported` |
