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

Amazon 속성을 [!DNL Commerce] Amazon 영업 채널은 속성을 추적하고 모든 Amazon 값에 대한 필터링 가능한 목록을 제공합니다. 이 페이지에서는 연결된 항목에 대한 값을 확인할 수 있습니다 [!DNL Commerce] 속성 간 올바르게 동기화 [!DNL Commerce] 및 Amazon. 에 연결되어 있거나 연결되어 있지 않은 Amazon 속성에 대해 동기화된 값을 검토할 수 있습니다 [!DNL Commerce] 속성을 사용합니다. Amazon 속성을 만들거나 편집하려면 다음을 참조하십시오 [속성 만들기 및 편집](./creating-attributes.md).

다음 _Amazon 가치_ 보는 속성 유형과 Amazon 속성에 따라 다릅니다. 예를 들어, 다음 기간 동안 나열된 Amazon 값 `Label` 는 `AmazonListPrice` 숫자일 수도 있습니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다.

## 속성 값 보기

1. 설정 _[!UICONTROL Admin]_사이드바, 다음 위치로 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾은 다음 **[!UICONTROL Create]** 또는 **[!UICONTROL Edit]** 에서 _[!UICONTROL Action]_열.

1. 을(를) 클릭합니다. **[!UICONTROL Matching Attribute Values]** 탭.

   해당 항목이 있는 목록 [!DNL Commerce] 카탈로그 제품에 연결된 값이 표시됩니다 _Magento 제품 SKU_ 열. 링크를 클릭하면 해당 카탈로그 제품 세부 사항 페이지가 열립니다. 제품 세부 사항 페이지의 Amazon 속성에 대한 변경 사항이 Amazon 판매 채널에 다시 동기화되지 않습니다.

>[!TIP]
>목록을 편집하거나 카탈로그 제품에 지정하려면 다음을 참조하십시오 [업데이트 필수 정보](./amazon-manually-update-incomplete-listing.md).

![속성 값 보기](assets/amazon-managing-attribute-values.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Region] | 에 정의된 영업 활동의 영역입니다. **[!DNL Amazon Marketplace]국가** 저장 통합 중에 |
| [!UICONTROL Magento Product SKU] | 를 나타냅니다 [!DNL Commerce] Amazon 스토어와 동기화된 제품. 값은 가 할당한 제품 ID입니다. [!DNL Commerce] 및 를 카탈로그에 있는 제품에 연결합니다. 에서 제품을 열려면 [!DNL Commerce]를 클릭하여 링크를 클릭합니다. |
| [!UICONTROL ASIN] | 제품 식별을 위해 Amazon이 제품에 할당한 ASIN(Amazon Standard Identity Number) 10자의 영숫자 고유 식별자를 나타냅니다. |
| [!UICONTROL Amazon Value] | 선택한 속성에 대한 값을 나타냅니다. Amazon 값은 보는 속성 유형과 Amazon 속성에 따라 다릅니다. 예를 들어, 다음 기간 동안 나열된 Amazon 값 `Label` 는 `AmazonListPrice` 숫자일 수도 있습니다. 상태는 Amazon 값을 가져왔는지 여부를 나타냅니다. |
| [!UICONTROL Status] | 속성 값을 로 가져왔는지 여부를 나타냅니다. [!DNL Commerce] 및 [!DNL Commerce] 속성을 사용합니다. 옵션: `Not Imported` / `Imported` |
