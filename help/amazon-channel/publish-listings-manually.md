---
title: Amazon 목록 수동 게시
description: 필요한 경우 Commerce 관리자로부터 종료된 Amazon 목록을 수동으로 게시할 수 있습니다.
feature: Sales Channels, Products, Merchandising
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Amazon 목록 수동 게시

종료된 하나 이상의 Amazon 목록을 수동으로 게시할 수 있습니다.

1. [제품 목록](./managing-product-listings.md) 페이지의 _[!UICONTROL Ended]_탭에서 하나 이상의 목록을 봅니다(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_또는_[!UICONTROL Ineligible]_ 탭).

1. 왼쪽 열에서 다시 게시할 각 목록을 클릭하여 선택합니다.

1. _[!UICONTROL Actions]_에서&#x200B;**[!UICONTROL Publish Product to Amazon]**을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

   선택한 목록이 Amazon에 게시하기 위해 처리되고 있음을 확인하는 메시지가 표시됩니다.

   목록 정보는 cron 설정에 따라 Amazon에 게시됩니다. 목록 정보는 다음 데이터 동기화 시 Amazon으로 전송됩니다. Amazon이 목록 확인에 회신할 때까지 수동으로 게시한 목록은 _목록 준비_ 탭에 `List in Progress` 상태로 유지됩니다. Amazon에서 목록 확인 메시지를 받으면 목록이 `Active` 상태로 _활성_ 탭으로 이동합니다.
