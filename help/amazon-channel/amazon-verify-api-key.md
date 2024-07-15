---
title: Amazon API 키 추가 또는 확인
description: Commerce 구성에서 검증된 Amazon API 키를 사용하면 스토어를 Amazon 판매자 계정과 통합할 수 있습니다.
role: Admin, Developer
feature: Sales Channels, Integration, Tools and External Services
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Amazon API 키 추가 또는 확인

Amazon 판매 채널에 액세스할 때 [!DNL Commerce]은(는) 스토어 구성에 추가한 Amazon API 키를 자동으로 확인하고 유효성을 검사합니다. 유효성을 검사한 경우 다음 단계인 [스토어 통합](./store-integration.md)(으)로 이동할 수 있습니다.

Amazon API 키가 없거나, 잘못되었거나, 만료된 경우 키를 업데이트해야 합니다. API 키를 가져오고 해당 키를 Amazon 판매 채널 구성에 추가하라는 메시지가 표시됩니다.

## 메시지가 표시되면 Amazon API 키 가져오기 및 추가

Amazon 판매 채널에 액세스할 때마다 API 키의 유효성을 검사합니다.

1. [!DNL Commerce] 관리자에 로그인합니다.

1. _[!UICONTROL Admin]_사이드바에서&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

   Amazon 판매 채널에 처음 액세스하거나 API 키를 업데이트해야 하는 경우 프로세스를 안내하는 메시지가 표시됩니다.

   ![Amazon API 키 프롬프트 가져오기 및 추가](assets/amazon-api-verification-prompt.png){width="500"}

1. [!DNL Commerce] 웹 계정에 액세스하려면 **[!UICONTROL Sign in]**&#x200B;을(를) 클릭하십시오.

   Commerce 계정 페이지가 새 브라우저 탭에서 열립니다.

   - [!DNL Commerce] 계정에 로그인하면 _[!UICONTROL My Account]_페이지의_[!UICONTROL API Portal]_ 섹션이 자동으로 나타납니다.

   - 로그인하지 않은 경우 _[!UICONTROL API Portal]_탭이 나타나기 전에 [!DNL Commerce] 계정 사용자 이름과 암호를 입력하라는 메시지가 표시됩니다.

   - 계정이 없는 경우 [계정 페이지 [!DNL Commerce] 2}{target="_blank"}를 방문하여 등록하세요. ](https://account.magento.com/customer/account/login/) 이 계정은 회사 또는 비즈니스의 일부여야 합니다.

1. 필요한 경우 [!DNL Commerce] 계정의 _[!UICONTROL API Portal]_탭에서 API 키를 보고 생성할 수 있습니다.

   API 키를 만들려면 `Amazon Sales Channel`과(와) 같은 설명을 입력하고 **[!UICONTROL Add New]**&#x200B;을(를) 클릭합니다. 새 키가 생성되고 입력한 이름으로 표시됩니다. **[!UICONTROL Copy]**&#x200B;을(를) 클릭하여 새 키를 복사합니다.

   ![API 키 생성 또는 복사](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. 새 키를 생성하고 복사한 후 브라우저의 _[!UICONTROL Amazon Sales Channel]_탭으로 돌아갑니다.

1. _[!UICONTROL Welcome to Amazon Sales Channel]_페이지에서&#x200B;**[!UICONTROL Add the key]**을(를) 클릭합니다.

   브라우저가 Amazon 판매 채널을 종료하고 저장소 구성 페이지에서 [!DNL Commerce] 관리자의 _[!UICONTROL Api Keys]_페이지가 열립니다.**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**(으)로 이동하여 왼쪽 패널에서 **[!UICONTROL Services]**&#x200B;을(를) 확장하고 **[!UICONTROL Magento Services]**&#x200B;을(를) 선택하면 이 페이지를 수동으로 열 수 있습니다.

1. **[!UICONTROL Production Api key]**&#x200B;에 대해 복사한 키를 붙여넣습니다.

1. **[!UICONTROL Save Config]**&#x200B;을(를) 클릭합니다. 이제 Amazon 판매 채널로 돌아갈 수 있습니다.

   ![저장소 구성에 API 키 추가](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. _[!UICONTROL Admin]_사이드바에서&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

   Amazon 판매 채널 트리거 [!DNL Commerce]에 다시 액세스하여 API 키를 확인하고 검증하여 계속할 수 있도록 합니다.

   키를 다시 확인하라는 메시지가 표시되면 이 _추가 및 확인_ 프로세스를 반복합니다.

![다음 아이콘](assets/btn-next.png) [**통합 저장 계속**](./store-integration.md)
