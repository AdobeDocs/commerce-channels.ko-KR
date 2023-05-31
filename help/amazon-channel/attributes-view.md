---
title: Amazon 목록 속성
description: Amazon Sales Channel은 [!UICONTROL Attributes] 탭에서는 Amazon 및 Commerce 특성 목록과 제품 일치를 위해 특성이 매핑되는 방법을 모니터링할 수 있습니다.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Amazon 목록 속성

다음 _[!UICONTROL Attributes]_보기는 Amazon 및 [!DNL Commerce] 속성. 이 목록은 제품 일치를 위해 매핑된 속성도 나타냅니다. 자세한 내용은 [속성 관리](./managing-attributes.md).

![속성 보기](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

다음에서 _[!UICONTROL Attributes]_테이블에서 속성 설정을 보고 검토합니다. [만들기 또는 편집](./creating-attributes.md) 속성.

## 속성 목록 보기

1. 다음에서 _관리자_ 사이드바, 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾아 속성 목록을 검토합니다.

1. 필요에 따라 속성을 만들거나 편집합니다.

   - 종료 [만들기](./creating-attributes.md#create-an-attribute) 속성에 대해 일치하는 속성 값을 정의하고 **[!UICONTROL Create]**.

   - 또는 비활성화 [설정 편집](./creating-attributes.md#edit-an-attribute) 또는 속성의 속성 값 일치에서 **[!UICONTROL Edit]**.

      속성 편집에는 제품 일치를 위한 속성 매핑 변경이 포함됩니다.

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Country] | 에 정의된 영업 활동 국가  **[!DNL Amazon Marketplace]국가** 다음 기간 동안 [스토어 통합](./store-integration.md). |
| [!UICONTROL ID] | 일반 속성 값 생성자 [!DNL Commerce] 속성이 만들어지는 경우. |
| [!UICONTROL Amazon Attribute Name] | Amazon에서 가져온 특성의 이름입니다. |
| [!UICONTROL Product Catalog Attribute Code] | 매핑된 경우 [!DNL Commerce] 에 매핑하기 위해 할당된 속성 _[!UICONTROL Amazon Attribute Name]_를 참조하십시오. |
| [!UICONTROL Overwrite Magento Values] | 속성이 로 설정된 경우 `Overwrite Existing Magento Values` 속성 설정에서 테이블은 `Enabled`. 활성화됨은 Amazon에서 속성에 대한 업데이트된 제품 정보를 받으면 새 정보가 의 제품에 대한 해당 정보를 업데이트(덮어쓰기)함을 의미합니다 [!DNL Commerce] 카탈로그. 또한 다음에 나열된 제품에도 영향을 줄 수 있습니다. [!DNL Commerce] 상점. |
| 상태 | 속성 값을 로 가져왔는지 여부를 나타냅니다. [!DNL Commerce] 및에 매핑됨 [!DNL Commerce] 특성. 옵션: `Enabled` / `Disabled` |
| 작업 | 속성에 사용할 수 있는 작업 옵션을 나타냅니다. 옵션: `Create` / `Edit` |
