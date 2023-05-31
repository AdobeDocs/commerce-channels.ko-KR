---
title: Amazon 속성 매핑 보기
description: Commerce와 Amazon 간에 올바르게 동기화하려면 연결된 Commerce 특성의 값을 확인하십시오.
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Amazon 속성 매핑 보기

Amazon 속성을 매핑할 때 [!DNL Commerce] Amazon 판매 채널이 모든 Amazon 값을 추적하고 필터링 가능한 목록을 제공합니다. 이 페이지를 사용하여 링크된 값을 확인합니다. [!DNL Commerce] 다음 사이에 속성이 올바르게 동기화됨 [!DNL Commerce] 그리고 Amazon. 에 연결되거나 연결되지 않은 Amazon 속성에 대한 동기화된 값을 검토할 수 있습니다. [!DNL Commerce] 특성. Amazon 속성을 만들거나 편집하려면 다음을 참조하십시오. [속성 만들기 및 편집](./creating-attributes.md).

다음 _Amazon 값_ 는 속성 유형 및 사용자가 보는 Amazon 속성에 따라 다릅니다. 예를 들어 나열된 Amazon 값 `Label` 이(가) 다음 기간 동안 텍스트 값이 됩니다. `AmazonListPrice` 숫자로 된 양입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다.

## 속성 값 보기

1. 다음에서 _[!UICONTROL Admin]_사이드바, 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾고 다음 중 하나를 클릭합니다 **[!UICONTROL Create]** 또는 **[!UICONTROL Edit]** 다음에서 _[!UICONTROL Action]_열.

1. 다음을 클릭합니다. **[!UICONTROL Matching Attribute Values]** 탭.

   해당하는 항목이 있는 목록 [!DNL Commerce] 카탈로그 제품에 연결된 값이 표시됨 _[!UICONTROL Magento Product SKU]_열. 링크를 클릭하면 해당 카탈로그 제품 세부 사항 페이지가 열립니다. 제품 세부 사항 페이지의 Amazon 속성 변경 사항이 Amazon 판매 채널에 다시 동기화되지 않습니다.

>[!TIP]
>목록 매핑을 편집하거나 카탈로그 제품에 할당하려면 다음을 참조하십시오. [필수 정보 업데이트](./amazon-manually-update-incomplete-listing.md).

![속성 값 보기](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Region] | 에 정의된 영업 활동의 지역 **[!DNL Amazon Marketplace]국가** 스토어 통합 도중. |
| [!UICONTROL Magento Product SKU] | 다음을 나타냅니다. [!DNL Commerce] Amazon 스토어와 동기화된 제품. 값은 이 할당한 제품 ID입니다. [!DNL Commerce] 카탈로그의 제품에 연결됩니다. 에서 제품을 열려면 [!DNL Commerce]링크를 클릭합니다. |
| [!UICONTROL ASIN] | Amazon에서 제품 식별을 위해 제품에 할당한 10자의 영숫자 고유 식별자인 Amazon ASIN(표준 식별 번호)을 나타냅니다. |
| [!UICONTROL Amazon Value] | 선택한 속성에 대한 값을 나타냅니다. Amazon 값은 속성 유형 및 사용자가 보는 Amazon 속성에 따라 다릅니다. 예를 들어 나열된 Amazon 값 `Label` 이(가) 다음 기간 동안 텍스트 값이 됩니다. `AmazonListPrice` 숫자로 된 양입니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다. |
| [!UICONTROL Status] | 속성 값을 로 가져왔는지 여부를 나타냅니다. [!DNL Commerce] 에 연결됨 [!DNL Commerce] 특성. 옵션: `Not Imported` / `Imported` |
