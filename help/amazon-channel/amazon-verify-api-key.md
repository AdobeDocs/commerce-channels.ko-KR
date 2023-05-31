---
title: Amazon API 키 추가 또는 확인
description: 상거래 구성에서 검증된 Amazon API 키를 사용하면 스토어를 Amazon 판매자 계정과 통합할 수 있습니다.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 077d680da3c98ef9a48958eb548a9d5c1612f74e
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Amazon API 키 추가 또는 확인

Amazon 판매 채널에 액세스할 때 [!DNL Commerce] 스토어 구성에 추가한 Amazon API 키를 자동으로 확인하고 확인합니다. 유효성이 확인되면 다음 단계로 이동할 수 있습니다. [스토어 통합](./store-integration.md).

Amazon API 키가 없거나, 잘못되었거나, 만료된 경우 키를 업데이트해야 합니다. API 키를 가져오고 해당 키를 Amazon 판매 채널 구성에 추가하라는 메시지가 표시됩니다.

## 메시지가 표시되면 Amazon API 키 가져오기 및 추가

Amazon 판매 채널에 액세스할 때마다 API 키의 유효성을 검사합니다.

1. 에 로그인합니다 [!DNL Commerce] 관리자.

1. 다음에서 _[!UICONTROL Admin]_사이드바, 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Amazon 판매 채널에 처음 액세스하거나 API 키를 업데이트해야 하는 경우 프로세스를 안내하는 메시지가 표시됩니다.

   ![Amazon API 키 프롬프트 가져오기 및 추가](assets/amazon-api-verification-prompt.png){width="500"}

1. 클릭 **[!UICONTROL Sign in]** 에 액세스 [!DNL Commerce] 웹 계정입니다.

   새 브라우저 탭에서 상거래 계정 페이지가 열립니다.

   - 에 로그인한 경우 [!DNL Commerce] 계정, _[!UICONTROL API Portal]_의 섹션_[!UICONTROL My Account]_ 페이지가 자동으로 나타납니다.

   - 로그인하지 않은 경우 다음을 입력하라는 메시지가 표시됩니다. [!DNL Commerce] 계정 사용자 이름 및 암호 _[!UICONTROL API Portal]_탭이 나타납니다.

   - 계정이 없는 경우 다음을 방문하십시오. [다음 [!DNL Commerce] 계정 페이지](https://account.magento.com/customer/account/login/){target="_blank"} 등록합니다. 이 계정은 회사 또는 비즈니스의 일부여야 합니다.

1. 필요한 경우 의 API 키를 보고 생성할 수 있습니다. _[!UICONTROL API Portal]_의 탭 [!DNL Commerce] 계정입니다.

   API 키를 만들려면 다음과 같은 설명을 입력합니다 `Amazon Sales Channel` 및 클릭 **[!UICONTROL Add New]**. 새 키가 생성되고 입력한 이름으로 표시됩니다. 클릭 **[!UICONTROL Copy]** 새 키를 복사합니다.

   ![API 키 생성 또는 복사](assets/amazon-add-api-key.png){width="500" zoomable="yes"}

1. 생성 및 복사된 새 키를 사용하여 _[!UICONTROL Amazon Sales Channel]_브라우저의 탭입니다.

1. 다음에서 _[!UICONTROL Welcome to Amazon Sales Channel]_페이지, 클릭&#x200B;**[!UICONTROL Add the key]**.

   브라우저가 Amazon 판매 채널을 종료하고 스토어 구성 페이지가 _[!UICONTROL Api Keys]_페이지의 [!DNL Commerce] 관리자. 로 이동하면 이 페이지를 수동으로 열 수 있습니다.**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, 확장 **[!UICONTROL Services]** 왼쪽 패널에서 을 선택하고 **[!UICONTROL Magento Services]**.

1. 복사한 키 붙여넣기 **[!UICONTROL Production Api key]**.

1. 클릭 **[!UICONTROL Save Config]**. 이제 Amazon 판매 채널로 돌아갈 수 있습니다.

   ![스토어 구성에서 API 키 추가](assets/config-magento-services-api-screen.png){width="600" zoomable="yes"}

1. 다음에서 _[!UICONTROL Admin]_사이드바, 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Amazon 판매 채널 트리거 재액세스 [!DNL Commerce] api 키를 확인하고 유효성을 검사하면 계속할 수 있습니다.

   키를 다시 확인하라는 메시지가 표시되면 이 작업을 반복합니다 _추가 및 확인_ 프로세스.

![다음 아이콘](assets/btn-next.png) [**통합 저장 계속**](./store-integration.md)
