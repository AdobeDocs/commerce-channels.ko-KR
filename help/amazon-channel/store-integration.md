---
title: ' [!DNL Amazon Seller Account]과(와) 스토어 통합'
description: 온보딩 프로세스를 시작하기 전에 Amazon Sales Channel 저장소를 생성(추가)하고 Amazon 판매자 계정에 연결해야 합니다.
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# [!DNL Amazon Seller Account]과(와) 스토어 통합

Amazon 판매 채널을 시작하려면 Amazon 판매 채널 스토어를 만들고(추가) [!DNL Amazon Seller Account]에 연결해야 합니다. 이 두 단계는 [!DNL Commerce] 및 Amazon 계정을 통합하여 데이터를 공유하고 제품을 동기화하는 등의 작업을 수행합니다.

_스토어에 연결하려면 [!DNL Amazon Seller Central] 계정(판매자 계정을 만드는 데 사용되는 전자 메일 또는 전화)에 대한 기본 로그인 자격 증명이 필요합니다._

>[!NOTE]
>
>첫 번째 스토어 통합 후에는 액세스 권한을 다시 부여하여 Amazon에 대한 Amazon 판매 채널 연결을 갱신하라는 메시지가 매년 표시됩니다. Seller Central 계정의 **설정** > **사용자 권한** 페이지의 _Amazon MWS 개발자 권한_ 섹션의 _현재 권한_ 테이블에서 이 권한을 갱신하거나 취소할 수 있습니다.

## Amazon 스토어 추가

1. _관리자_ 사이드바에서 **마케팅** > _채널_ > **Amazon Sales Channel**(으)로 이동합니다.

   첫 번째 Amazon 판매 채널 스토어를 추가하면 _사전 설정 작업_ 모달이 나타납니다. 첫 스토어가 추가되면 사전 설정 작업은 왼쪽 메뉴에서 _학습 및 준비_ 아래의 [Amazon 판매 채널 홈](./amazon-sales-channel-home.md) 페이지에서 액세스할 수 있습니다.

1. **[!UICONTROL Add Amazon Store]**&#x200B;을(를) 클릭합니다.

   _[!UICONTROL Add Amazon sales channel]_페이지가 열립니다.

   ![Amazon 판매 채널 스토어 추가](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. **[!UICONTROL Magento Website to use for Amazon Listing]**&#x200B;의 경우 이 Amazon 판매 채널 스토어에 연결할 [!DNL Commerce] 웹 사이트 중 하나를 선택하십시오.

   이 설정은 [Amazon 주문 가져오기](./order-settings.md)에 대한 기본 [!DNL Commerce] 저장소도 정의합니다.

1. **[!UICONTROL Email Address]**&#x200B;의 경우 선호하는 연락처 전자 메일 주소를 입력하십시오.

1. **[!UICONTROL New Store Name]**&#x200B;에 새 Amazon 판매 채널 스토어의 수사적 이름을 입력하십시오.

   >[!NOTE]
   >
   >이 이름은 [!DNL Commerce] 참조로만 사용되며 [Amazon 판매 채널 홈](./amazon-sales-channel-home.md) 페이지에서 스토어를 식별합니다. 팀이 쉽게 식별할 수 있는 항목으로 만들고 싶을 수 있습니다. 예를 들어 미국 지역에서 판매하는 Amazon 스토어의 이름은 `Amazon Store USA`일 수 있습니다.

1. **[!UICONTROL Amazon Marketplace Country]**&#x200B;의 경우 이 Amazon 판매 채널 스토어에서 제품을 판매하는 지역/국가를 선택하십시오. 옵션:

   - 미국
   - 캐나다
   - 멕시코
   - 영국

1. _[!UICONTROL Map your Magento attributes to Amazon]_섹션에서 다음을 수행합니다.

   - **[!UICONTROL Product ID on the Amazon market]**&#x200B;의 경우 아래에서 선택한 [!DNL Commerce] 특성에 매핑할 Amazon 특성을 선택하십시오.

     이 ID는 [!DNL Commerce] 카탈로그의 해당 제품을 올바르게 연결하는 데 도움이 됩니다.

   - **[!UICONTROL Map a Magento attribute]**&#x200B;의 경우 위에서 선택한 Amazon 특성에 매핑할 [!DNL Commerce] 제품 특성을 선택하십시오.

     [특성 매핑](./ob-creating-magento-attributes.md)을 통해 Amazon 목록이 [!DNL Commerce] 카탈로그의 해당 제품과 올바르게 일치하는지 확인할 수 있습니다.

1. **[!UICONTROL Connect]**&#x200B;을(를) 클릭합니다.

   대화 상자가 닫히고 새 저장소가 [Amazon 판매 채널 홈](./amazon-sales-channel-home.md) 페이지에 확인 메시지와 함께 나타납니다.

## 스토어를 [!DNL Amazon Seller Central]에 연결

1. 스토어 대시보드에서 스토어 카드의 **[!UICONTROL Connect store]**&#x200B;을(를) 클릭하여 새 탭에서 [!DNL Amazon Seller Central]을(를) 시작합니다.

1. [!DNL Amazon Seller Central] 계정 자격 증명을 입력하고 **[!UICONTROL Sign in]**&#x200B;을(를) 클릭합니다.

   이 연결을 완료하려면 기본 사용자의 로그인 자격 증명(판매자 계정을 만드는 데 사용되는 전자 메일 또는 전화)을 사용하여 [!DNL Amazon Seller Central] 계정에 로그인해야 합니다.

1. 메시지가 표시되면 Amazon에서 받은 코드를 입력하여 Amazon 2단계 인증(2FA)을 완료한 다음 **[!UICONTROL Sign in]**&#x200B;을(를) 클릭합니다.

1. _[!UICONTROL Amazon Marketplace Web Service]_확인 페이지에서 &quot;[!UICONTROL I understand...]&quot; 확인란을 선택하고&#x200B;**[!UICONTROL Next]**을(를) 클릭합니다.

1. _[!UICONTROL You are almost done]_메시지에서&#x200B;**[!UICONTROL Continue]**을(를) 클릭합니다.

   [!DNL Amazon Seller Central] 계정과 데이터에 액세스하고 공유할 수 있는 Amazon 판매 채널 권한을 부여했습니다. Amazon 페이지가 닫히고 확인 메시지가 나타납니다.

   Amazon 스토어 카드를 표시하는 [Amazon 판매 채널 홈](./amazon-sales-channel-home.md) 페이지가 열립니다.

   스토어 대시보드를 보려면 스토어 카드에서 **[!UICONTROL View Store]**&#x200B;을(를) 클릭하십시오.

새 스토어 카드가 있는 ![Amazon 판매 채널 홈](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

새 Amazon 판매 채널 저장소가 이제 [!DNL Amazon Seller Central] 계정에 연결되었습니다.

![다음 아이콘](assets/btn-next.png) [**목록 규칙을 계속 만듭니다**](./ob-create-listing-rule.md)
