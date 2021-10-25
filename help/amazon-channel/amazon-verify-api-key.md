---
title: Amazon API 키 추가 또는 확인
description: 상거래 구성에서 확인된 Amazon API 키를 사용하면 스토어를 Amazon Seller 계정과 통합할 수 있습니다.
exl-id: 2257b64d-309d-4efd-ba79-6e0cdeed63cb
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Amazon API 키 추가 또는 확인

Amazon 판매 채널에 액세스할 때 [!DNL Commerce] 저장소 구성에 추가한 Amazon API 키를 자동으로 확인하고 확인합니다. 유효성이 확인되면 다음 단계로 이동할 수 있습니다. [스토어 통합](./store-integration.md).

Amazon API 키가 없거나, 잘못되었거나, 만료된 경우 키를 업데이트해야 합니다. API 키를 가져오고 이 키를 Amazon 판매 채널 구성에 추가하라는 메시지가 나타납니다.

## 메시지가 표시되면 Amazon API 키를 가져와 추가합니다

API 키는 Amazon 판매 채널에 액세스할 때마다 검증됩니다.

1. 에 로그인합니다. [!DNL Commerce] 관리자.

1. 설정 _[!UICONTROL Admin]_사이드바, 다음 위치로 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Amazon 판매 채널에 처음 액세스하거나 API 키를 업데이트해야 하는 경우 프로세스를 안내합니다.

   ![Amazon API 키 프롬프트 가져오기 및 추가](assets/amazon-api-verification-prompt.png)

1. 클릭 **[!UICONTROL Sign in]** 액세스 권한 [!DNL Commerce] 웹 계정.

   상거래 계정 페이지가 새 브라우저 탭에서 열립니다.

   - 로그인되어 있다면 [!DNL Commerce] 계정, _[!UICONTROL API Portal]_섹션_[!UICONTROL My Account]_ 페이지가 자동으로 나타납니다.

   - 로그인하지 않은 경우 을 입력하라는 메시지가 표시됩니다 [!DNL Commerce] 계정 사용자 이름 및 이전 암호 _[!UICONTROL API Portal]_탭이 나타납니다.

   - 계정이 없는 경우 를 방문합니다. [a [!DNL Commerce] 계정 페이지](https://account.magento.com/customer/account/login/){target=&quot;_blank&quot;} 및 등록합니다. 이 계정은 회사 또는 비즈니스의 일부여야 합니다.

1. 필요한 경우 _[!UICONTROL API Portal]_탭 [!DNL Commerce] 계정이 필요합니다.

   API 키를 만들려면 다음과 같은 설명을 입력합니다 `Amazon Sales Channel` 을(를) 클릭합니다. **[!UICONTROL Add New]**. 새 키가 생성되어 입력한 이름과 함께 표시됩니다. 클릭 **[!UICONTROL Copy]** 새 키를 복사하려면 다음을 수행하십시오.

   ![API 키 생성 또는 복사](assets/amazon-add-api-key.png)

1. 새 키가 생성되어 복사되면 _[!UICONTROL Amazon Sales Channel]_탭에서 사용할 수 있습니다.

1. 설정 _[!UICONTROL Welcome to Amazon Sales Channel]_페이지를 클릭한 다음&#x200B;**[!UICONTROL Add the key]**.

   브라우저가 Amazon 판매 채널을 종료하고 저장소 구성 페이지가 열립니다 _[!UICONTROL Api Keys]_페이지의 [!DNL Commerce] 관리자. 로 이동할 때 이 페이지를 수동으로 열 수 있습니다.**[!UICONTROL Stores]**>_[!UICONTROL Settings]_ > **[!UICONTROL Configuration]**, 확장 **[!UICONTROL Services]** 왼쪽 패널에서 **[!UICONTROL Magento Services]**.

1. 복사된 키 붙여넣기 **[!UICONTROL Production Api key]**.

1. 클릭 **[!UICONTROL Save Config]**. 이제 Amazon 판매 채널로 돌아갈 수 있습니다.

   ![저장소 구성에 API 키 추가](assets/config-magento-services-api-screen.png)

1. 설정 _[!UICONTROL Admin]_사이드바, 다음 위치로 이동&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

   Amazon 판매 채널 트리거 다시 액세스 [!DNL Commerce] api 키를 확인하고 유효성을 검사하여 계속할 수 있습니다.

   키를 다시 확인하라는 메시지가 표시되면 다음 단계를 반복합니다 _추가 및 확인_ 프로세스.

![다음 아이콘](assets/btn-next.png) [**계속 통합 저장**](./store-integration.md)
