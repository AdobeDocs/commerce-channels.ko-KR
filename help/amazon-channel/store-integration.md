---
title: 와(과) 통합 저장 [!DNL Amazon Seller Account]
description: 온보딩 프로세스를 시작하기 전에 Amazon Sales Channel 저장소를 생성(추가)하고 Amazon 판매자 계정에 연결해야 합니다.
role: Admin, Developer
feature: Sales Channels, Configuration, Integration, Tools and External Services
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 와(과) 통합 저장 [!DNL Amazon Seller Account]

Amazon 판매 채널을 시작하려면 Amazon 판매 채널 스토어를 생성(추가)하고 여기에 연결해야 합니다. [!DNL Amazon Seller Account]. 이 두 단계는 [!DNL Commerce] 및 Amazon 계정을 사용하여 데이터를 공유하고 제품을 동기화하는 등의 작업을 수행할 수 있습니다.

_에 대한 기본 로그인 자격 증명이 필요합니다. [!DNL Amazon Seller Central] 계정(판매자 계정을 만드는 데 사용되는 이메일 또는 전화)을 사용하여 스토어를 연결합니다._

>[!NOTE]
>
>첫 번째 스토어 통합 후에는 액세스 권한을 다시 부여하여 Amazon에 대한 Amazon 판매 채널 연결을 갱신하라는 메시지가 매년 표시됩니다. 에서 이 인증을 갱신하거나 취소할 수 있습니다. _현재 권한_ 테이블의 _Amazon MWS 개발자 권한_ 의 섹션 **설정** > **사용자 권한** 판매자 중앙 계정 페이지.

## Amazon 스토어 추가

1. 다음에서 _관리자_ 사이드바, 이동 **마케팅** > _채널_ > **Amazon Sales Channel**.

   첫 번째 Amazon 판매 채널 스토어를 추가할 때 _사전 설정 작업_ 모달이 나타납니다. 첫 번째 저장소가 추가되면에서 사전 설정 작업에 액세스할 수 있습니다. [Amazon sales channel 홈](./amazon-sales-channel-home.md) 아래 페이지 _학습 및 준비_ 왼쪽 메뉴에 있는 을 참조하십시오.

1. 클릭 **[!UICONTROL Add Amazon Store]**.

   다음 _[!UICONTROL Add Amazon sales channel]_페이지가 열립니다.

   ![Amazon 판매 채널 스토어 추가](assets/amazon-store-integration.png){width="500" zoomable="yes"}

1. 대상 **[!UICONTROL Magento Website to use for Amazon Listing]**, 중에서 선택 [!DNL Commerce] 이 Amazon sales channel 스토어에 연결할 웹 사이트입니다.

   이 설정은 기본값도 정의합니다 [!DNL Commerce] 다음에 대한 저장 [Amazon 주문 가져오기](./order-settings.md).

1. 대상 **[!UICONTROL Email Address]**&#x200B;선호하는 연락처 이메일 주소를 입력합니다.

1. 대상 **[!UICONTROL New Store Name]**&#x200B;새 Amazon 판매 채널 스토어를 설명하는 이름을 입력합니다.

   >[!NOTE]
   >
   >이 이름은 다음으로 사용됩니다. [!DNL Commerce] 참조만 하고 [Amazon sales channel 홈](./amazon-sales-channel-home.md) 페이지를 가리키도록 업데이트하는 중입니다. 팀이 쉽게 식별할 수 있는 항목으로 만들고 싶을 수 있습니다. 예를 들어 미국 지역에서 판매되는 Amazon 스토어의 이름을 로 지정할 수 있습니다 `Amazon Store USA`.

1. 대상 **[!UICONTROL Amazon Marketplace Country]**&#x200B;에서 이 Amazon 판매 채널 스토어에서 제품을 판매하는 지역/국가를 선택합니다. 옵션:

   - 미국
   - 캐나다
   - 멕시코
   - 영국

1. 다음에서 _[!UICONTROL Map your Magento attributes to Amazon]_섹션에서 다음을 수행합니다.

   - 대상 **[!UICONTROL Product ID on the Amazon market]**&#x200B;에 매핑할 Amazon 속성을 선택합니다. [!DNL Commerce] 속성이 아래에서 선택되었습니다.

     이 ID는 의 해당 제품을 올바르게 일치시키는 데 도움이 됩니다. [!DNL Commerce] 카탈로그.

   - 대상 **[!UICONTROL Map a Magento attribute]**, 을(를) 선택합니다. [!DNL Commerce] 위에서 선택한 Amazon 속성에 매핑할 제품 속성

     [속성 매핑](./ob-creating-magento-attributes.md) 는 Amazon 목록이 의 해당 제품과 올바르게 일치하는지 확인하는 데 도움이 됩니다. [!DNL Commerce] 카탈로그.

1. 클릭 **[!UICONTROL Connect]**.

   대화 상자가 닫히고 새 저장소가 [Amazon sales channel 홈](./amazon-sales-channel-home.md) 확인 메시지가 표시된 페이지입니다.

## 저장소 연결 대상 [!DNL Amazon Seller Central]

1. 스토어 대시보드에서 을(를) 클릭합니다 **[!UICONTROL Connect store]** 실행할 스토어 카드에서 [!DNL Amazon Seller Central] 새 탭에서.

1. 다음을 입력하십시오. [!DNL Amazon Seller Central] 계정 자격 증명 및 클릭 **[!UICONTROL Sign in]**.

   이 연결을 완료하려면 [!DNL Amazon Seller Central] 기본 사용자의 로그인 자격 증명을 사용하는 계정(판매자 계정을 만드는 데 사용되는 이메일 또는 전화).

1. 메시지가 표시되면 Amazon에서 받은 코드를 입력하여 Amazon 2단계 인증(2FA)을 완료한 다음 을 클릭합니다. **[!UICONTROL Sign in]**.

1. 다음에서 _[!UICONTROL Amazon Marketplace Web Service]_확인 페이지에서 &quot;[!UICONTROL I understand...]&quot;확인란 및 클릭&#x200B;**[!UICONTROL Next]**.

1. 다음에서 _[!UICONTROL You are almost done]_메시지, 클릭&#x200B;**[!UICONTROL Continue]**.

   에 액세스하고 와 데이터를 공유할 수 있는 Amazon 판매 채널 권한을 부여했습니다. [!DNL Amazon Seller Central] 계정입니다. Amazon 페이지가 닫히고 확인 메시지가 나타납니다.

   다음 [Amazon sales channel 홈](./amazon-sales-channel-home.md) Amazon 스토어 카드가 표시된 페이지가 열립니다.

   스토어 대시보드를 보려면 **[!UICONTROL View Store]** 가게 카드에서요.

![새로운 스토어 카드가 있는 Amazon sales channel home](assets/asc-dashboard-after-2fa.png){width="600" zoomable="yes"}

이제 새 Amazon 판매 채널 스토어가 [!DNL Amazon Seller Central] 계정입니다.

![다음 아이콘](assets/btn-next.png) [**목록 규칙 만들기 계속**](./ob-create-listing-rule.md)
