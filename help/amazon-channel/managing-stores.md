---
title: "[!UICONTROL Amazon Stores] view"
description: 각 Amazon 스토어에 대한 기본 통계를 빠르게 검토하고 관리 옵션에 액세스하려면 Amazon 스토어 보기로 이동합니다.
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores] 보기

Amazon 판매 채널 홈 페이지를 볼 때 _Amazon 스토어_ 기본적으로 보기가 열립니다.

![Amazon 스토어 보기](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

다음 _[!UICONTROL Amazon Stores]_보기는 몇 가지 기본 통계 및 관리 옵션과 함께 각 Amazon 스토어에 대한 &quot;스토어 카드&quot;를 표시합니다. 각 카드에 표시된 요약 정보에는 각 저장소 상태, 만든 날짜, 마지막 업데이트 날짜, 주의가 필요한 목록(예: 미완료 목록) 및 할당된 항목이 포함됩니다. [!DNL Commerce] 웹 사이트입니다.

를 볼 때 _[!UICONTROL Amazon Store]_각 스토어 카드를 통해 다음을 수행할 수 있습니다.

- 스토어를 열려면 [대시보드](./amazon-store-dashboard.md), 클릭 **[!UICONTROL View Store]**.

- 저장소 상태를 변경하거나 저장소를 삭제하려면 **[!UICONTROL Action]** 다음을 선택합니다.

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** - 스토어 상태를 다음으로 변경 `Active` 또는 `Inactive`, 각각

      변경 `Inactive` 저장 위치: `Active` 상태는 스토어의 현재 스토어 설정(예: 목록 설정, 가격 규칙 및 무시)을 사용하여 스토어에 대한 목록 및 주문 활동을 활성화합니다.

      다음에서 저장소 상태 변경 `Active` 끝 `Inactive` 상태는 스토어에 대한 목록 및 주문 활동을 일시 중단합니다. 비활성 스토어는 모든 스토어 설정 및 목록을 유지하지만 스토어가 다시 로 변경될 때까지 가격책정, 수량 및 주문 관리의 동기화를 일시적으로 중지합니다. `Active` 상태. 이 기능을 사용하면 Amazon 스토어를 다시 만들거나 재통합할 필요, 과거 주문 및 판매 데이터의 손실 없이 지역 수준에서 스토어 활동을 제어할 수 있습니다.

   - **[!UICONTROL Delete]** - 더 이상 필요하지 않은 저장소를 삭제하도록 선택합니다.

      기존 Amazon 스토어와 해당 통합 설정을 삭제할 시기를 선택합니다. [!DNL Amazon Seller Central] 계정입니다. 계정을 삭제하면 Amazon 판매 채널에서 스토어와 함께 이 스토어와 관련된 모든 계정 설정, 목록, 로그 및 기타 정보가 제거됩니다. 삭제 후에는 스토어를 검색할 수 없습니다. 새 스토어를 만들어야 합니다.

>[!NOTE]
>통합 중에 스토어에 할당된 웹 사이트를 변경하려면 스토어를 삭제하고 스토어 통합 중에 정의된 다른 웹 사이트로 스토어를 다시 추가해야 합니다.

| 카드 저장 | 설명 |
|--- |--- |
| 상위 섹션 | 포함 사항: <br>다음에 정의된 저장소의 영역 아이콘 [스토어 통합](./store-integration.md).<br> 할당됨 _[!UICONTROL Magento Website]_, 저장소 통합 중에 정의됩니다.<br>다음_[!UICONTROL Status]_ 스토어에서 가져왔습니다. 옵션: **[!UICONTROL Active]** - 스토어 통합이 완료되고 Amazon을 통해 확인되었으며 판매 활동에 사용할 수 있습니다. **[!UICONTROL Inactive]** - 스토어 통합이 완료되었으나 영업 활동에 사용 중이거나 사용할 수 없습니다. 날짜 `Inactive`, Amazon 판매가 일시 중지되었습니다. 날짜 `Active`, 판매 수익 및 추가 설정은 활성화 전에 업데이트하기 위해 저장됩니다.<br>다음 *[!UICONTROL Last Updated]* Amazon 스토어 설정에 대한 가장 최근의 변경 날짜입니다.<br>다음 *[!UICONTROL Created]* Amazon 판매 채널에 Amazon 스토어가 생성된 날짜입니다. |
| 중간 섹션 | 지난 30일 동안의 스토어 활동 요약 차트와 주의가 필요한 모든 목록에 대한 및 경고가 포함됩니다. |
| 아래 섹션 | [저장소 보기] 및 [작업] 옵션을 포함합니다.<br>스토어를 열려면 [대시보드](./amazon-store-dashboard.md), 클릭 **[!UICONTROL View Store]**.<br>스토어를 활성화, 비활성화 또는 삭제하려면 **[!UICONTROL Actions]**. |
