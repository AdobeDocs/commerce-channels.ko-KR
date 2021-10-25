---
title: 속성
description: Amazon Sales Channel은 [!UICONTROL Attributes] 탭하여 Amazon 및 Commerce 속성 목록과 제품 매칭을 위해 매핑되는 방법을 모니터링합니다.
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 속성

다음 _[!UICONTROL Attributes]_보기 는 Amazon 및 [!DNL Commerce] 속성을 사용합니다. 또한 이 목록에는 제품 일치를 위해 매핑된 특성이 표시됩니다. 자세한 내용은 [속성 관리](./managing-attributes.md).

![속성 보기](assets/amazon-attributes-view.png)

에서 _[!UICONTROL Attributes]_를 보고, 테이블에서 속성 설정을 검토하고, [만들기 또는 편집](./creating-attributes.md) 속성을 사용합니다.

## 속성 목록 보기

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL Attributes]** 왼쪽 메뉴에서 Amazon 속성을 찾아 속성 목록을 검토합니다.

1. 필요에 따라 속성을 만들거나 편집합니다.

   - 종료 [만들기](./creating-attributes.md#create-an-attribute) 속성에 대한 일치 속성 값을 정의한 다음 **[!UICONTROL Create]**.

   - 또는 를 비활성화하려면 [설정 편집](./creating-attributes.md#edit-an-attribute) 또는 속성에 대한 속성 값 일치 **[!UICONTROL Edit]**.

      속성을 편집하면 제품 일치를 위해 속성 매핑을 변경하는 작업이 포함됩니다.

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Country] | 에 정의된 판매 활동의 국가  **[!DNL Amazon Marketplace]국가** 기간 [스토어 통합](./store-integration.md). |
| [!UICONTROL ID] | 에 의해 생성된 일반 속성 값 [!DNL Commerce] 속성을 만들 때. |
| [!UICONTROL Amazon Attribute Name] | Amazon에서 가져온 속성의 이름입니다. |
| [!UICONTROL Product Catalog Attribute Code] | 매핑된 경우 [!DNL Commerce] 맵에 지정된 속성 _[!UICONTROL Amazon Attribute Name]_일치하는 카탈로그 및 목록 제품에 대해 설명합니다. |
| [!UICONTROL Overwrite Magento Values] | 속성이 `Overwrite Existing Magento Values` 속성 설정에서 이 표는 `Enabled`. 활성화됨 은 속성에 대한 제품 정보가 Amazon에서 수신되면 새로운 정보가 의 제품에 대한 해당 정보를 업데이트(덮어쓰기)함을 의미합니다 [!DNL Commerce] 카탈로그 또한 [!DNL Commerce] 상점들. |
| 상태 | 속성 값을 로 가져왔는지 여부를 나타냅니다. [!DNL Commerce] 및 [!DNL Commerce] 속성을 사용합니다. 옵션: `Enabled` / `Disabled` |
| 작업 | 속성에 사용할 수 있는 작업 옵션을 나타냅니다. 옵션: `Create` / `Edit` |
