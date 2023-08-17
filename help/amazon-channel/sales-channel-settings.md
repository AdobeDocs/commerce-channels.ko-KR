---
title: 판매 채널 설정
description: Amazon 판매 채널 기능에 대한 로깅, 크론 소스 및 동기화를 관리하려면 Commerce 구성을 업데이트합니다.
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 판매 채널 설정

다음의 경우 [!DNL Amazon Sales Channel] 확장 프로그램이 설치되고, Amazon 판매 채널에 대한 관리자에서 기본값이 설정됩니다. 이러한 설정은 Amazon 스토어에 대한 구성 설정에서 수정할 수 있습니다. 이러한 설정에는 다음이 포함됩니다.

- 활동 로그 기록을 지우기 위한 간격
- 크론 소스 선택
- 로그 동기화 옵션

## 상거래 채널 설정 수정

1. 다음에서 _관리자_ 사이드바, 이동 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. 왼쪽 패널에서 를 확장합니다. **[!UICONTROL Sales Channels]** 및 선택 **[!UICONTROL Global Settings]**.

1. 대상 **[!UICONTROL Clear Log History]**&#x200B;옵션을 선택합니다.

   - `Once Daily` - 매일 한 번 저장소 활동 기록을 지우도록 선택합니다.

   - `Once Weekly` - 매주 한 번 스토어 활동 내역을 지우도록 선택합니다.

   - `Once Monthly` - (기본값) 한 달에 한 번 저장소 활동 기록을 지우도록 선택합니다.

1. 대상 **[!UICONTROL Background Tasks (CRON) Source]**, 선택 `Magento CRON`.

   이 옵션을 사용하면 Amazon 판매 채널에서 다음을 사용할 수 있습니다 [!DNL Commerce] [크론](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) 과의 통신 및 데이터 동기화 간격을 결정하는 설정 [!DNL Amazon Seller Central].

1. 대상 **[!UICONTROL Enable Debug Logging]**, 선택 `Enabled` 문제 해결이 필요할 때 추가 동기화 데이터를 수집하기 위해

   Amazon 판매 채널 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 에서 볼 수 있는 파일 [개발자 모드](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes). 로깅은 다음과 같아야 합니다. `Enabled` 문제 해결 도중 및 다음 작업 수행 `Disabled` 문제 해결이 완료되면.

1. 대상 **[!UICONTROL Read-Only Mode]**, 선택 `Enabled` 나가는 모든 상태 변경 API 요청을 차단합니다.

   이 설정을 사용하면 잠재적인 변경 사항이 저장되지만 그때까지 전송되지 않습니다. [!UICONTROL Read-Only Mode] 이(가) 비활성화되었습니다. 읽기 전용 모드를 활성화하려면 구성 캐시를 지워야 합니다. 데이터 전송을 다시 시작하려면 다음을 선택합니다. `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] 는 스테이징 또는 QA와 같은 프로덕션 인스턴스의 사본용으로 설계되었으므로 프로덕션 인스턴스에서 사용해서는 안 됩니다.
   >
   >데이터베이스가 인스턴스의 새 사본으로 마이그레이션되는 경우(저장소의 URL이 구성에서 변경될 때 감지됨) [!UICONTROL Read-Only Mode] 이(가) 자동으로 활성화됩니다.

1. 클릭 **[!UICONTROL Save Config]**.

![Sales Channel 구성 설정](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
