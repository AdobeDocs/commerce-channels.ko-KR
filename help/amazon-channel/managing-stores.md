---
title: Amazon 저장소 보기
description: Amazon 저장소 보기로 이동하여 각 Amazon 저장소에 대한 기본 통계를 빠르게 검토하고 관리 옵션에 액세스합니다.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon 저장소 보기

Amazon 판매 채널 홈 페이지를 볼 때 기본적으로 _Amazon 저장소_ 보기가 열립니다.

![Amazon 저장소 보기](assets/amazon-sales-channel-home-tabs.png)

_[!UICONTROL Amazon Stores]_보기는 일부 기본 통계 및 관리 옵션과 함께 각 Amazon 저장소에 대한 &quot;스토어 카드&quot;를 표시합니다. 각 카드에 표시되는 요약 정보에는 각 저장소 상태, 생성 날짜, 마지막 업데이트 날짜, 주의가 필요한 목록(예: 불완전한 목록) 및 할당된 [!DNL Commerce] 웹 사이트입니다.

_[!UICONTROL Amazon Store]_보기를 볼 때 각 저장소 카드를 사용하여 다음을 수행할 수 있습니다.

- 저장소 [대시보드](./amazon-store-dashboard.md)를 열려면 **[!UICONTROL View Store]**&#x200B;를 클릭합니다.

- 저장소 상태를 변경하거나 저장소를 삭제하려면 **[!UICONTROL Action]** 을 클릭하고 다음을 선택합니다.

   - **[!UICONTROL Activate]** /  **[!UICONTROL Deactivate]** - 저장소의 상태를 각각 또 `Active` 는  `Inactive`로 변경하도록 선택합니다.

      `Inactive` 저장소를 `Active` 상태로 변경하면 현재 저장소 설정(목록 설정, 가격 규칙 및 무시 등)을 사용하여 저장소에 대한 목록 및 주문 활동을 활성화합니다.

      저장소 상태를 `Active`에서 `Inactive` 상태로 변경하면 저장소의 목록 및 주문 활동이 일시 중단됩니다. 비활성 저장소는 모든 저장소 설정 및 목록을 유지하지만, 스토어가 다시 `Active` 상태로 변경될 때까지 가격, 수량 및 주문 관리 동기화를 일시적으로 중지합니다. 이 기능을 사용하면 Amazon 스토어를 다시 만들거나 재통합하거나 이전 주문 및 판매 데이터의 손실 없이 지역 수준에서 저장소 활동을 제어할 수 있습니다.

   - **[!UICONTROL Delete]** - 더 이상 필요하지 않은 저장소를 삭제하도록 선택합니다.

      기존 Amazon 스토어와 [!DNL Amazon Seller Central] 계정을 사용한 통합 설정을 삭제할 시점을 선택합니다. 계정을 삭제하면 Amazon 판매 채널에서 모든 계정 설정, 목록, 로그 및 이 스토어와 관련된 기타 정보와 함께 저장소가 제거됩니다. 삭제 후에는 저장소를 검색할 수 없습니다. 새 저장소를 만들어야 합니다.

>[!NOTE]
>통합 중에 저장소에 할당된 웹 사이트를 변경하려면 저장소를 삭제하고 스토어 통합 중에 정의된 다른 웹 사이트로 스토어를 다시 추가해야 합니다.

| 스토어 카드 | 설명 |
|--- |--- |
| 상위 섹션 | 다음을 포함합니다. <br>저장소 통합](./store-integration.md) 중에 정의된 저장소의 영역 아이콘입니다.[<br> 저장소 통합  _[!UICONTROL Magento Website]_중에 정의된 지정된 차원입니다.<br>매장_[!UICONTROL Status]_ 의 옵션: **[!UICONTROL Active]** - 스토어 통합이 Amazon에서 완료되고 확인되며, 판매 활동에 사용 가능합니다. **[!UICONTROL Inactive]** - 스토어 통합이 완료되었지만 사용 중이거나 판매 활동에 사용할 수 없습니다. `Inactive` 이 되면 Amazon 매출이 일시 중지됩니다. `Active`이면 판매 매출과 추가 설정이 활성화되기 전에 업데이트되도록 저장됩니다.<br>Amazon  *[!UICONTROL Last Updated]* 저장소 설정에 대한 최근 변경 날짜입니다.<br>Amazon  *[!UICONTROL Created]* 영업 채널에서 Amazon 스토어를 만든 날짜입니다. |
| 중간 섹션 | 최근 30일 동안의 저장소 활동 요약 차트를 포함하며 주의가 필요한 모든 목록을 포함 및 알려줍니다. |
| 아래쪽 섹션 | 저장소 보기 및 작업 옵션이 포함됩니다.<br>저장소 대시보드 [를](./amazon-store-dashboard.md) 열려면 를 클릭합니다  **[!UICONTROL View Store]**.<br>저장소를 활성화, 비활성화 또는 삭제하려면 를 클릭합니다  **[!UICONTROL Actions]**. |
