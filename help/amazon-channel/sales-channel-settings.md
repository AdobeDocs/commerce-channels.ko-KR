---
title: Sales Channel 설정
description: Amazon 영업 채널 기능에 대한 로깅, 로그온 소스 및 동기화를 관리하려면 상거래 구성을 업데이트하십시오.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel 설정

[!DNL Amazon Sales Channel] 확장 프로그램이 설치되면 Amazon 영업 채널에 대한 Admin에 기본값이 설정됩니다. 이러한 설정은 Amazon 저장소의 구성 설정에서 수정할 수 있습니다. 이러한 설정은 다음과 같습니다.

- 활동 로그 기록을 지우는 간격
- 소스 선택
- 로그 동기화 옵션

## 상거래 채널 설정 수정

1. _관리_ 사이드바에서 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**로 이동합니다.

1. 왼쪽 패널에서 **[!UICONTROL Sales Channels]**&#x200B;을(를) 확장하고 **[!UICONTROL Global Settings]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Clear Log History]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - `Once Daily` - 매일 한 번 스토어 활동 내역을 지우도록 선택합니다.

   - `Once Weekly` - 일주일에 한 번 스토어 활동 내역을 지우도록 선택합니다.

   - `Once Monthly` - (기본값) 한 달에 한 번 스토어 활동 내역을 지우도록 선택합니다.

1. **[!UICONTROL Background Tasks (CRON) Source]**&#x200B;에 대해 `Magento CRON`을 선택합니다.

   이 옵션을 사용하면 Amazon 영업 채널에서 [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) 설정을 사용하여 [!DNL Amazon Seller Central]과의 통신 및 데이터 동기화 간격을 결정할 수 있습니다.

1. **[!UICONTROL Enable Debug Logging]**&#x200B;의 경우 문제 해결 필요 시 추가 동기화 데이터를 수집하려면 `Enabled`을 선택합니다.

   Amazon 영업 채널 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 파일에 기록되며 [개발자 모드](https://docs.magento.com/user-guide/magento/installation-modes.html){:target=&quot;_blank&quot;}에서 볼 수 있습니다. 로깅은 문제 해결 중 `Enabled`이어야 하며 문제가 완료되면 `Disabled`이어야 합니다.

1. **[!UICONTROL Save Config]** 을 클릭합니다.

![Sales Channel 구성 설정](assets/config-sales-channel-global-settings.png)
