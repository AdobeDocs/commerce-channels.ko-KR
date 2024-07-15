---
title: Amazon 속성 매핑 보기
description: 연결된 Commerce 속성의 값을 확인하여 Commerce과 Amazon 간에 올바르게 동기화합니다.
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Amazon 속성 매핑 보기

Amazon 특성을 [!DNL Commerce] 특성에 매핑하면 Amazon 판매 채널이 모든 Amazon 값을 추적하고 필터링 가능한 목록을 제공합니다. 연결된 [!DNL Commerce] 특성의 값이 [!DNL Commerce]과(와) Amazon 간에 올바르게 동기화되는지 확인하려면 이 페이지를 사용하십시오. [!DNL Commerce] 특성에 연결되거나 연결되지 않은 Amazon 특성에 대해 동기화된 값을 검토할 수 있습니다. Amazon 특성을 만들거나 편집하려면 [특성 만들기 및 편집](./creating-attributes.md)을 참조하세요.

_Amazon 값_&#x200B;은(는) 표시되는 특성 유형과 Amazon 특성에 따라 다릅니다. 예를 들어 `Label`에 대해 나열된 Amazon 값은 텍스트 값이지만 `AmazonListPrice`은(는) 숫자 값입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다.

## 속성 값 보기

1. _[!UICONTROL Admin]_사이드바에서&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]**&#x200B;을(를) 클릭하고 Amazon 특성을 찾은 다음 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Create]**또는&#x200B;**[!UICONTROL Edit]**을(를) 클릭합니다.

1. **[!UICONTROL Matching Attribute Values]** 탭을 클릭합니다.

   해당 [!DNL Commerce] 카탈로그 제품이 있는 목록의 _[!UICONTROL Magento Product SKU]_열에 연결된 값이 표시됩니다. 링크를 클릭하면 해당 카탈로그 제품 세부 사항 페이지가 열립니다. 제품 세부 사항 페이지의 Amazon 속성 변경 사항이 Amazon 판매 채널에 다시 동기화되지 않습니다.

>[!TIP]
>목록에 대한 매핑을 편집하거나 카탈로그 제품에 할당하려면 [필수 정보 업데이트](./amazon-manually-update-incomplete-listing.md)를 참조하세요.

![특성 값 보기](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | 저장소 통합 중에 **[!DNL Amazon Marketplace]국가**&#x200B;에 정의된 영업 활동의 지역입니다. |
| [!UICONTROL Magento Product SKU] | Amazon 스토어와 동기화된 [!DNL Commerce] 제품을 나타냅니다. 값은 [!DNL Commerce]이(가) 할당하여 카탈로그의 제품에 연결된 제품 ID입니다. [!DNL Commerce]에서 제품을 열려면 링크를 클릭하세요. |
| [!UICONTROL ASIN] | Amazon에서 제품 식별을 위해 제품에 할당한 10자의 영숫자 고유 식별자인 Amazon ASIN(표준 식별 번호)을 나타냅니다. |
| [!UICONTROL Amazon Value] | 선택한 속성에 대한 값을 나타냅니다. Amazon 값은 속성 유형 및 사용자가 보는 Amazon 속성에 따라 다릅니다. 예를 들어 `Label`에 대해 나열된 Amazon 값은 텍스트 값이지만 `AmazonListPrice`은(는) 숫자 값입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다. |
| [!UICONTROL Status] | 특성 값을 [!DNL Commerce](으)로 가져와서 [!DNL Commerce] 특성에 연결했는지 여부를 나타냅니다. 옵션: `Not Imported` / `Imported` |
