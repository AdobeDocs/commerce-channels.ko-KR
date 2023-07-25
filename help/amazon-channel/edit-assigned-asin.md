---
title: 할당된 ASIN 편집
description: Amazon 목록 중 하나와 일치하지 않는 경우 Commerce 제품에 대한 ASIN 값을 변경합니다.
feature: Sales Channels, Products, Configuration
exl-id: 2aaeb700-96ac-4a15-9379-f74728d2dcbe
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 할당된 ASIN 편집

의 제품에 할당된 Amazon ASIN 값을 편집할 수 있습니다. [!DNL Commerce] 카탈로그. 이 기능은 카탈로그 제품이 Amazon 목록 중 하나와 잘못 일치하는 경우 유용합니다. 목록에 할당된 ASIN을 변경해도 Amazon에서 제품에 할당한 ASIN은 변경되지 않습니다. 카탈로그 제품이 일치하는 Amazon 목록만 변경합니다.

할당된 ASIN이 변경되면:

- [!DNL Commerce] 이전 ASIN에 첨부된 Amazon 목록을 종료합니다.
- Amazon을 사용하여 ASIN의 유효성을 검사합니다.
- 업데이트된 ASIN에 대한 목록을 만듭니다.
- Amazon 판매 채널의 목록 정보 업데이트

**_지정된 ASIN을 편집하려면_**

1. 다음에서 목록 보기: _[!UICONTROL Product Listings]_페이지 (_[!UICONTROL Inactive]_, _[!UICONTROL Active]_, 또는_[!UICONTROL Ineligible]_ 탭).

1. 아래 _[!UICONTROL Actions]_, 클릭&#x200B;**[!UICONTROL Edit Assigned ASIN]**.

   이 작업을 수행하면 _[!UICONTROL Product Listing Update]_페이지를 가리키도록 업데이트하는 중입니다.

1. 대상 **[!UICONTROL Assign ASIN]**&#x200B;새 ASIN 값을 입력합니다.

1. 변경 사항을 저장하려면 를 클릭합니다. **[!UICONTROL Save Listing Update]**.

![할당된 ASIN 편집](assets/amazon-assigned-asin-edit.png){width="600" zoomable="yes"}
