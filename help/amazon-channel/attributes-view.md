---
title: 속성
description: Amazon Sales Channel은 [!UICONTROL Attributes] 탭을 제공하여 Amazon 및 상거래 속성 목록과 제품 일치를 위해 매핑되는 방법을 모니터링합니다.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 속성

_[!UICONTROL Attributes]_보기는 Amazon 목록과 [!DNL Commerce] 속성을 보여줍니다. 또한 이 목록에는 제품 일치를 위해 매핑된 특성이 표시됩니다. 자세한 내용은 [속성 관리](./managing-attributes.md)를 참조하십시오.

![속성 보기](assets/amazon-attributes-view.png)

_[!UICONTROL Attributes]_보기에서 테이블의 속성 설정을 검토하고 [속성을 만들거나 편집합니다.](./creating-attributes.md)

## 속성 목록 보기

1. _관리_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**로 이동합니다.

1. 왼쪽 메뉴에서 **[!UICONTROL Attributes]** 을 클릭하고 Amazon 속성을 찾은 다음 속성 목록을 검토합니다.

1. 필요에 따라 속성을 만들거나 편집합니다.

   - [을(를) 만들고](./creating-attributes.md#create-an-attribute) 속성에 대한 일치하는 속성 값을 정의하려면 **[!UICONTROL Create]**&#x200B;를 클릭합니다.

   - 속성에 대한 설정](./creating-attributes.md#edit-an-attribute) 또는 일치하는 속성 값을 비활성화하거나 **[!UICONTROL Edit]**&#x200B;편집하려면 [를 클릭합니다.

      속성을 편집하면 제품 일치를 위해 속성 매핑을 변경하는 작업이 포함됩니다.

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Country] | [스토어 통합](./store-integration.md)에서 **[!DNL Amazon Marketplace]국가**&#x200B;에 정의된 영업 활동의 국가입니다. |
| [!UICONTROL ID] | 속성을 만들 때 [!DNL Commerce]에 의해 생성된 일반 속성 값입니다. |
| [!UICONTROL Amazon Attribute Name] | Amazon에서 가져온 속성의 이름입니다. |
| [!UICONTROL Product Catalog Attribute Code] | 매핑된 경우 일치하는 카탈로그 및 제품 목록을 위해 _[!UICONTROL Amazon Attribute Name]_에 매핑하도록 지정된 [!DNL Commerce] 속성을 사용합니다. |
| [!UICONTROL Overwrite Magento Values] | 속성 설정에서 특성이 `Overwrite Existing Magento Values`으로 설정된 경우 테이블에 `Enabled`이 표시됩니다. 활성화됨 은 Amazon에서 속성에 대한 제품 정보를 업데이트하면 새 정보가 [!DNL Commerce] 카탈로그의 제품에 대한 해당 정보를 업데이트(덮어쓰기)함을 의미합니다. 또한 [!DNL Commerce] 스토어에 나열된 제품에도 영향을 줄 수 있습니다. |
| 상태 | 특성 값을 [!DNL Commerce](으)로 가져와 [!DNL Commerce] 속성에 매핑했는지 여부를 나타냅니다. 옵션: `Enabled` / `Disabled` |
| 작업 | 속성에 사용할 수 있는 작업 옵션을 나타냅니다. 옵션: `Create` / `Edit` |
