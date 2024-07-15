---
title: Amazon 목록에 대한 로그 및 보고서 저장
description: 로그 및 저장소 보고서를 사용하여 Adobe Commerce 또는 Magento Open Source 저장소 및 Amazon Marketplace 목록에서 발생하는 상황을 확인할 수 있습니다.
feature: Sales Channels, Logs
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Amazon 목록에 대한 로그 및 보고서 저장

Amazon 판매 채널 확장에는 Amazon 목록 및 주문에 영향을 주는 변경 사항을 볼 수 있는 몇 가지 중요한 로그 및 스토어 보고서가 포함되어 있습니다. 이러한 보고서를 사용하여 스토어에서 일어나는 일을 확인하고 다양한 목록 상태를 이해할 수 있습니다.

로그 또는 저장소 보고서는 검토 전용 기능이므로 이 보고서에 사용할 수 있는 작업이 없습니다.

[스토어 대시보드](./amazon-store-dashboard.md)에서 다음 로그에 액세스할 수 있습니다.

- [목록 변경 로그](./listing-changes-log.md)에는 Amazon 판매 채널 설정의 반영으로 Amazon 판매자 계정에서 발생한 변경 내용이 표시됩니다.

- [통신 오류 로그](./communication-errors-log.md)에 Amazon에서 보고된 통신 오류가 표시됩니다.

[스토어 대시보드](./amazon-store-dashboard.md)에서 다음 스토어별 보고서에 액세스할 수 있습니다.

- [경쟁업체 가격 분석](./competitive-price-analysis.md) 보고서에 따르면 [Buy Box](./buy-box-competitor-pricing.md) 가격 및 [가장 낮은 경쟁업체](./lowest-competitor-pricing.md) 가격과 관련하여 Amazon _도착 가격_(목록 가격과 배송 가격)이 표시됩니다.

- [목록 개선 사항](./listing-improvements.md) 보고서는 선택한 저장소에 대해 Amazon에서 제공하는 모든 제안된 목록 개선 사항을 보여줍니다.

>[!TIP]
>
>문제 해결이 필요할 때 로그 파일에서 추가 정보를 확인할 수도 있습니다. [판매 채널 관리자 설정](./sales-channel-settings.md)을 참조하세요. Amazon 판매 채널 동기화 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 파일에 기록되며 [개발자 모드](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes)에서 볼 수 있습니다.
