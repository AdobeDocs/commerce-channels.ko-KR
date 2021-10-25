---
title: '''온보딩: 목록 규칙 만들기'''
description: Amazon 판매 채널 온보딩 프로세스를 완료하는 동안 페이지에 대한 Amazon 목록을 생성하는 초기 목록 규칙을 만듭니다 [!DNL Commerce] 제품.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 온보딩: 목록 규칙 만들기

목록 규칙은 온보딩 중에 정의할 수 있지만 언제든지 수정할 수 있습니다. 온보딩 후에는 [목록 규칙](./listing-rules.md) 매장 [대시보드](./amazon-store-dashboard.md).

## 온보딩 중 목록 규칙 만들기

1. 스토어가 연결되면 **[!UICONTROL View Store]** 추가 스토어용.

   가게 [대시보드](./amazon-store-dashboard.md) 이 `No products listed to Amazon` 메시지를 표시합니다.

1. 클릭 **[!UICONTROL Preview and List Eligible Products]**.

   다음 _[!UICONTROL Listing Rules]_페이지가 나타납니다.

1. Amazon에 나열할 제품 자격에 대해 원하는 조건을 정의하고 을(를) 클릭합니다 **[!UICONTROL Preview changes]**&#x200B;또는 **[!UICONTROL Preview changes]** 이 단계를 건너뛰려면 다음을 수행하십시오.

   자세한 내용은 [예: 조건 정의](./ob-define-condition-example.md).

1. 목록 미리 보기에서 목록을 검토합니다.

   ![미리 보기 나열](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정에 따라 Amazon 목록에 사용할 수 없습니다.

      부적격 제품은 Amazon에 게시되지 않습니다. 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 과 일치시키는 경우 [!DNL Commerce] 카탈로그 제품, 변경 사항이 나열된 Amazon의 수량 `0` 제품의 판매를 막기 위해. Amazon에서 목록을 수동으로 제거하려면 다음을 참조하십시오 [Amazon 목록 종료](./end-listings-manually.md). Amazon 요구 사항에 맞지 않는 제품은 여기에 나열되어 있지 않습니다. 이러한 제품들은 [[!UICONTROL Inactive Listings] 탭](./inactive-listings.md).

      를 변경하려면 `Ineligible` 다음으로 나열 `Eligible` 목록을 나열하고 이 프로세스를 반복하고 목록 규칙을 수정합니다.

   - **[!UICONTROL Eligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정에 따라 Amazon 목록에 포함될 수 있으며 Amazon 요구 사항에 따라 자격을 갖습니다. 이 탭에는 가져오게 된 기존 Amazon 목록이 포함되어 있습니다(있는 경우) **[!UICONTROL Import Third Party Listings]** 설정 `Import Listing` 다음 위치에서 [목록 설정](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - 이 탭에 나열된 제품에는 [!DNL Commerce] 현재 목록 규칙 설정을 기반으로 Amazon 목록에 새로 적합한 카탈로그 제품을 만들고 Amazon 목록을 만듭니다.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save and Close]**.

   가게 [대시보드](./amazon-store-dashboard.md) 엽니다.

스토어에 온보딩이 완료되면, 정보 동기화 [!DNL Commerce] 그리고 Amazon이 시작됩니다. Amazon 목록을 가져올 위치 [!DNL Commerce] 그리고 [!DNL Commerce] 카탈로그.

Amazon 주문 정보는 _[!UICONTROL Recent Orders]_저장소 대시보드의 섹션. 자세한 내용은 [대시보드 저장](./amazon-store-dashboard.md) 또는 [주문 관리](./managing-orders.md).

>[!IMPORTANT]
>
>새 저장소에 대한 기본값이 있는 몇 가지 중요한 저장소 설정(목록, 가격, 규칙, 이행 등)이 있습니다. 저장소가 특정 요구에 맞게 설정되었는지 확인하려면 [저장 설정](./default-store-settings.md) .

![다음 아이콘](assets/btn-next.png) [**기본 저장소 설정으로 계속 이동**](./default-store-settings.md)
