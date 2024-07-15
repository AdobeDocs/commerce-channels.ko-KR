---
title: 판매 채널 설정
description: Amazon 판매 채널 기능에 대한 로깅, 크론 소스 및 동기화를 관리하려면 Commerce 구성을 업데이트합니다.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 판매 채널 설정

[!DNL Amazon Sales Channel] 확장이 설치되면 Amazon 판매 채널의 관리에서 기본값이 설정됩니다. 이러한 설정은 Amazon 스토어에 대한 구성 설정에서 수정할 수 있습니다. 이러한 설정에는 다음이 포함됩니다.

- 활동 로그 기록을 지우기 위한 간격
- 크론 소스 선택
- 로그 동기화 옵션

## Commerce 채널 설정 수정

1. _관리자_ 사이드바에서 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**(으)로 이동합니다.

1. 왼쪽 패널에서 **[!UICONTROL Sales Channels]**&#x200B;을(를) 확장하고 **[!UICONTROL Global Settings]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Clear Log History]**&#x200B;에 대해 다음 옵션을 선택하십시오.

   - `Once Daily` - 매일 한 번 저장소 활동 기록을 지우도록 선택합니다.

   - `Once Weekly` - 매주 한 번 저장소 활동 기록을 지우도록 선택합니다.

   - `Once Monthly` - (기본값) 매월 한 번 저장소 활동 기록을 지우도록 선택합니다.

1. **[!UICONTROL Background Tasks (CRON) Source]**&#x200B;의 경우 `Magento CRON`을(를) 선택하십시오.

   이 옵션을 사용하면 Amazon 판매 채널이 [!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) 설정을 사용하여 [!DNL Amazon Seller Central]과의 통신 및 데이터 동기화 간격을 결정할 수 있습니다.

1. **[!UICONTROL Enable Debug Logging]**&#x200B;의 경우 문제 해결이 필요할 때 추가 동기화 데이터를 수집하려면 `Enabled`을(를) 선택하십시오.

   Amazon 판매 채널 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 파일에 기록되며 [개발자 모드](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes)에서 볼 수 있습니다. 로깅은 문제 해결 중에만 `Enabled`이어야 하고, 문제 해결이 완료되면 `Disabled`이어야 합니다.

1. **[!UICONTROL Read-Only Mode]**&#x200B;에 대해 `Enabled`을(를) 선택하여 나가는 모든 상태 변경 API 요청을 차단합니다.

   이 설정을 사용하면 [!UICONTROL Read-Only Mode]을(를) 사용하지 않도록 설정할 때까지 잠재적인 변경 내용이 저장되지만 전송되지 않습니다. 읽기 전용 모드를 활성화하려면 구성 캐시를 지워야 합니다. 데이터 전송을 다시 시작하려면 `Disabled`을(를) 선택하십시오.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode]은(는) 스테이징 또는 QA와 같은 프로덕션 인스턴스의 복사본용으로 디자인되었으므로 프로덕션 인스턴스에서 사용해서는 안 됩니다.
   >
   >데이터베이스가 인스턴스의 새 복사본으로 마이그레이션되면(저장소의 URL이 구성에서 변경될 때 검색됨) [!UICONTROL Read-Only Mode]이(가) 자동으로 활성화됩니다.

1. **[!UICONTROL Save Config]**&#x200B;을(를) 클릭합니다.

![Sales Channel 구성 설정](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
