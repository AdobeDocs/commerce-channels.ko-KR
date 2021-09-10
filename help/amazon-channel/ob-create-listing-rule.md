---
title: '''온보딩: 목록 규칙 만들기'''
description: Amazon 판매 채널 온보딩 프로세스를 완료하는 동안 [!DNL Commerce] 제품에 대한 Amazon 목록을 생성하는 초기 목록 규칙을 만듭니다.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 온보딩: 목록 규칙 만들기

목록 규칙은 온보딩 중에 정의할 수 있지만 언제든지 수정할 수 있습니다. 온보딩 후에는 [대시보드](./amazon-store-dashboard.md)에서 [목록 규칙](./listing-rules.md)에 액세스할 수 있습니다.

## 온보딩 중 목록 규칙 만들기

1. 스토어가 연결되면 추가된 스토어의 **[!UICONTROL View Store]** 을 클릭합니다.

   [대시보드](./amazon-store-dashboard.md) 저장소가 `No products listed to Amazon` 메시지와 함께 나타납니다.

1. **[!UICONTROL Preview and List Eligible Products]** 을 클릭합니다.

   _[!UICONTROL Listing Rules]_페이지가 나타납니다.

1. Amazon에 나열할 제품의 자격에 대해 원하는 조건을 정의하고 **[!UICONTROL Preview changes]** 을 클릭하거나 **[!UICONTROL Preview changes]** 을 클릭하여 이 단계를 건너뜁니다.

   [예제: 조건](./ob-define-condition-example.md)을 정의합니다.

1. 목록 미리 보기에서 목록을 검토합니다.

   ![미리 보기 나열](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정에 따라 Amazon 목록에 사용할 수 없습니다.

      부적격 제품은 Amazon에 게시되지 않습니다. 부적격 제품이 이미 Amazon에 나열되고 Amazon 목록을 [!DNL Commerce] 카탈로그 제품에 일치시키는 경우 Amazon 목록 수량이 `0` (으)로 변경되어 제품 판매를 방지할 수 있습니다. Amazon에서 목록을 수동으로 제거하려면 [Amazon 목록 종료](./end-listings-manually.md)를 참조하십시오. Amazon 요구 사항에 맞지 않는 제품은 여기에 나열되어 있지 않습니다. 이러한 제품은 [[!UICONTROL Inactive Listings] 탭](./inactive-listings.md)에 나열되어 있습니다.

      `Ineligible` 목록을 `Eligible` 목록으로 변경하려면 이 프로세스를 반복하여 목록 규칙을 수정합니다.

   - **[!UICONTROL Eligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정에 따라 Amazon 목록에 포함될 수 있으며 Amazon 요구 사항에 따라 자격을 갖습니다. 이 탭에는 가져오게 되는 기존 Amazon 목록이 포함되어 있습니다( [목록 설정](./listing-settings.md)에 **[!UICONTROL Import Third Party Listings]**&#x200B;이 `Import Listing`로 설정된 경우).

   - **[!UICONTROL New Listings]** - 이 탭에 나열된 제품에는 현재 목록  [!DNL Commerce] 규칙 설정에 따라 Amazon 목록에 새로 적합한 카탈로그 제품이 포함되며 Amazon 목록을 만듭니다.

1. 완료되면 **[!UICONTROL Save and Close]** 을 클릭합니다.

   [대시보드](./amazon-store-dashboard.md)가 열립니다.

스토어에 온보딩이 완료되면 [!DNL Commerce] 과 Amazon 간의 정보 동기화가 시작됩니다. Amazon 목록을 [!DNL Commerce]로 가져와 [!DNL Commerce] 카탈로그의 제품과 일치시키려고 합니다.

저장소 대시보드의 _[!UICONTROL Recent Orders]_섹션에서 Amazon 주문 정보를 볼 수 있습니다. [대시보드 저장](./amazon-store-dashboard.md) 또는 [주문 관리](./managing-orders.md)를 참조하십시오.

>[!IMPORTANT]
>
>새 저장소에 대한 기본값이 있는 몇 가지 중요한 저장소 설정(목록, 가격, 규칙, 이행 등)이 있습니다. 저장소가 특정 요구에 맞게 설정되었는지 확인하려면 [스토어 설정](./default-store-settings.md) 을 검토하십시오.

![다음 ](assets/btn-next.png) [**아이콘기본 저장소 설정으로 계속**](./default-store-settings.md)
