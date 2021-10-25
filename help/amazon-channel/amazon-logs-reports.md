---
title: 로그 및 저장소 보고서
description: 로그 및 저장소 보고서를 사용하여 Adobe Commerce 또는 Magento Open Source 스토어와 Amazon Marketplace 목록에서 발생하는 내용을 확인할 수 있습니다.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 보고서 로그 및 저장

Amazon 판매 채널 확장에는 Amazon 목록 및 주문에 영향을 주는 변경 사항을 볼 수 있는 몇 가지 중요한 로그 및 저장소 보고서가 포함되어 있습니다. 이러한 보고서를 사용하여 저장소에서 발생하는 상황을 확인하고 다양한 목록 상태를 이해할 수 있습니다.

검토 전용 기능이므로 로그 또는 저장소 보고서에 사용할 수 있는 작업은 없습니다.

다음 로그는 [대시보드 저장](./amazon-store-dashboard.md).

- 다음 [변경 내용 로그 나열](./listing-changes-log.md) Amazon 판매 채널 설정의 반영으로 Amazon 판매자 계정에서 발생한 변경 사항을 표시합니다.

- 다음 [통신 오류 로그](./communication-errors-log.md) Amazon과 보고된 통신 오류를 표시합니다.

다음 저장소별 보고서는 [대시보드 저장](./amazon-store-dashboard.md).

- 다음 [경쟁력 분석](./competitive-price-analysis.md) 보고서는 Amazon을 보여줍니다. _단가_ (가격 및 운송 가격 목록) [Buy Box](./buy-box-competitor-pricing.md) 가격 및 [최저 경쟁사](./lowest-competitor-pricing.md) 가격.

- 다음 [목록 개선 사항](./listing-improvements.md) 이 보고서는 선택한 스토어에 대해 Amazon에서 제공하는 모든 추천 목록 개선 사항을 보여줍니다.

>[!TIP]
>
>문제 해결 시 로그 파일에서 추가 정보를 확인할 수도 있습니다. 자세한 내용은 [영업 채널 관리 설정](./sales-channel-settings.md). Amazon 영업 채널 동기화 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 파일 및에서 볼 수 있습니다. [개발자 모드](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}.
