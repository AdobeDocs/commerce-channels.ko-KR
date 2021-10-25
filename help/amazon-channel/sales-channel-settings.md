---
title: Sales Channel 설정
description: Amazon 영업 채널 기능에 대한 로깅, 로그온 소스 및 동기화를 관리하려면 상거래 구성을 업데이트하십시오.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel 설정

이 [!DNL Amazon Sales Channel] 확장이 설치되면 Amazon 판매 채널에 대한 Admin에서 기본값이 설정됩니다. 이러한 설정은 Amazon 저장소의 구성 설정에서 수정할 수 있습니다. 이러한 설정은 다음과 같습니다.

- 활동 로그 기록을 지우는 간격
- 소스 선택
- 로그 동기화 옵션

## 상거래 채널 설정 수정

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. 왼쪽 패널에서 를 확장합니다. **[!UICONTROL Sales Channels]** 및 **[!UICONTROL Global Settings]**.

1. 대상 **[!UICONTROL Clear Log History]**&#x200B;다음 옵션을 선택합니다.

   - `Once Daily` - 매일 한 번 스토어 활동 내역을 지우도록 선택합니다.

   - `Once Weekly` - 일주일에 한 번 스토어 활동 내역을 지우도록 선택합니다.

   - `Once Monthly` - (기본값) 한 달에 한 번 스토어 활동 내역을 지우도록 선택합니다.

1. 대상 **[!UICONTROL Background Tasks (CRON) Source]**, 선택 `Magento CRON`.

   이 옵션을 사용하면 Amazon 영업 채널에서 [!DNL Commerce] [크론](https://docs.magento.com/user-guide/system/cron.html) 통신 및 데이터 동기화 간격을 [!DNL Amazon Seller Central].

1. 대상 **[!UICONTROL Enable Debug Logging]**, 선택 `Enabled` 문제 해결 시 추가 동기화 데이터를 수집하려면

   Amazon 영업 채널 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 파일 및에서 볼 수 있습니다. [개발자 모드](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}. 로깅은 `Enabled` 문제 해결 중 및에 대해 `Disabled` 문제 해결이 완료되면

1. 클릭 **[!UICONTROL Save Config]**.

![Sales Channel 구성 설정](assets/config-sales-channel-global-settings.png)
