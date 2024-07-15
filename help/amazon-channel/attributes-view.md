---
title: Amazon 목록 속성
description: Amazon Sales Channel은 Amazon 및 Commerce 특성 목록과 제품 일치를 위해 매핑되는 방법을 모니터링하는 [!UICONTROL Attributes] 탭을 제공합니다.
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Amazon 목록 속성

_[!UICONTROL Attributes]_보기에는 Amazon 및 [!DNL Commerce] 특성 목록이 표시됩니다. 이 목록은 제품 일치를 위해 매핑된 속성도 나타냅니다. 자세한 내용은 [특성 관리](./managing-attributes.md)를 참조하십시오.

![특성 보기](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

_[!UICONTROL Attributes]_보기에서 테이블의 특성 설정을 검토하고 특성을 [만들거나 편집](./creating-attributes.md)합니다.

## 속성 목록 보기

1. _관리자_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]**&#x200B;을(를) 클릭하고 Amazon 특성을 찾은 다음 특성 목록을 검토합니다.

1. 필요에 따라 속성을 만들거나 편집합니다.

   - [만들기](./creating-attributes.md#create-an-attribute)를 만들고 특성에 대해 일치하는 특성 값을 정의하려면 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

   - 속성에 대한 설정 ](./creating-attributes.md#edit-an-attribute) 또는 일치하는 특성 값을 비활성화하거나 [편집하려면 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

     속성 편집에는 제품 일치를 위한 속성 매핑 변경이 포함됩니다.

| 필드 | 설명 |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | [스토어 통합](./store-integration.md) 동안 **[!DNL Amazon Marketplace]국가**&#x200B;에 정의된 영업 활동의 국가입니다. |
| [!UICONTROL ID] | 특성을 만들 때 [!DNL Commerce]에서 생성한 일반 특성 값입니다. |
| [!UICONTROL Amazon Attribute Name] | Amazon에서 가져온 특성의 이름입니다. |
| [!UICONTROL Product Catalog Attribute Code] | 매핑되는 경우 일치하는 카탈로그와 제품을 나열하기 위해 _[!UICONTROL Amazon Attribute Name]_에 매핑하도록 [!DNL Commerce] 특성이 할당됩니다. |
| [!UICONTROL Overwrite Magento Values] | 특성 설정에서 특성이 `Overwrite Existing Magento Values`(으)로 설정되어 있으면 테이블에 `Enabled`이(가) 표시됩니다. Enabled는 Amazon에서 특성에 대한 업데이트된 제품 정보를 받으면 새 정보가 [!DNL Commerce] 카탈로그의 제품에 대한 해당 정보를 업데이트(덮어쓰기)하는 것을 의미합니다. [!DNL Commerce] 스토어에 나열된 제품에도 영향을 줄 수 있습니다. |
| 상태 | 특성 값을 [!DNL Commerce](으)로 가져와서 [!DNL Commerce] 특성에 매핑했는지 여부를 나타냅니다. 옵션: `Enabled` / `Disabled` |
| 작업 | 속성에 사용할 수 있는 작업 옵션을 나타냅니다. 옵션: `Create` / `Edit` |
