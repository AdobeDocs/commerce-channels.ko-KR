---
title: Sales Channel 설정
description: Amazon 영업 채널 기능에 대한 로깅, 로그온 소스 및 동기화를 관리하려면 상거래 구성을 업데이트하십시오.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 5508fe6e6b2193eaaebc78f485aae972504554cc
workflow-type: tm+mt
source-wordcount: '280'
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

1. 대상 **[!UICONTROL Read-Only Mode]**, 선택 `Enabled` 나가는 상태 변경 API 요청을 모두 차단하려면 다음을 수행하십시오.

   이 설정을 사용하면 잠재적인 변경 사항이 저장되지만 전송되지 않는 한 [!UICONTROL Read-Only Mode] 이 비활성화되어 있습니다. 읽기 전용 모드를 사용하려면 구성 캐시를 지워야 합니다. 데이터 전송을 다시 시작하려면 다음을 선택합니다 `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] 는 스테이징 또는 QA와 같은 프로덕션 인스턴스의 사본을 위해 설계되었으며, 프로덕션 인스턴스에서 사용해서는 안 됩니다.
   >
   >데이터베이스가 인스턴스의 새 복사본으로 마이그레이션되면(구성에서 저장소의 URL이 변경될 때 감지) [!UICONTROL Read-Only Mode] 이 자동으로 활성화되어 있습니다.

1. 클릭 **[!UICONTROL Save Config]**.

![Sales Channel 구성 설정](assets/config-sales-channel-global-settings.png)
