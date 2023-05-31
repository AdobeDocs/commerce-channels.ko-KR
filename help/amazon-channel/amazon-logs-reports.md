---
title: Amazon 목록에 대한 로그 및 보고서 저장
description: 로그 및 저장소 보고서를 사용하여 Adobe Commerce 또는 Magento Open Source 저장소 및 Amazon Marketplace 목록에서 발생하는 상황을 확인할 수 있습니다.
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Amazon 목록에 대한 로그 및 보고서 저장

Amazon 판매 채널 확장에는 Amazon 목록 및 주문에 영향을 주는 변경 사항을 볼 수 있는 몇 가지 중요한 로그 및 스토어 보고서가 포함되어 있습니다. 이러한 보고서를 사용하여 스토어에서 일어나는 일을 확인하고 다양한 목록 상태를 이해할 수 있습니다.

로그 또는 저장소 보고서는 검토 전용 기능이므로 이 보고서에 사용할 수 있는 작업이 없습니다.

다음에서 액세스할 수 있는 로그: [대시보드 저장](./amazon-store-dashboard.md).

- 다음 [변경 로그 나열](./listing-changes-log.md) 은 Amazon 판매 채널 설정의 반영으로 Amazon 판매자 계정에서 발생한 변경 사항을 보여 줍니다.

- 다음 [통신 오류 로그](./communication-errors-log.md) Amazon에서 보고된 통신 오류를 표시합니다.

다음 저장소별 보고서는 [대시보드 저장](./amazon-store-dashboard.md).

- 다음 [경쟁력 있는 가격 분석](./competitive-price-analysis.md) 보고서에 Amazon이 _착륙 가격_ (목록 가격 + 배송 가격) [Buy Box](./buy-box-competitor-pricing.md) 가격 및 [가장 낮은 경쟁자](./lowest-competitor-pricing.md) 가격.

- 다음 [목록 개선 사항](./listing-improvements.md) 보고서는 선택한 스토어에 대해 Amazon에서 제공하는 모든 제안된 목록 개선 사항을 보여줍니다.

>[!TIP]
>
>문제 해결이 필요할 때 로그 파일에서 추가 정보를 확인할 수도 있습니다. 다음을 참조하십시오 [판매 채널 관리자 설정](./sales-channel-settings.md). Amazon 판매 채널 동기화 로깅은 `{Commerce Root}/var/log/channel_amazon.log` 에서 볼 수 있는 파일 [개발자 모드](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes).
