---
title: Amazon 목록 규칙 만들기
description: Amazon 판매 채널 온보딩 프로세스를 완료하는 동안 다음에 대한 Amazon 목록을 생성하기 위한 초기 목록 규칙을 만듭니다. [!DNL Commerce] 제품.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Amazon 목록 규칙 만들기

목록 규칙은 온보딩 중에 정의할 수 있지만, 언제든지 수정할 수도 있습니다. 온보딩 후 다음에 액세스할 수 있습니다 [규칙 나열](./listing-rules.md) 스토어에서 [대시보드](./amazon-store-dashboard.md).

## 온보딩 중 목록 규칙 만들기

1. 스토어가 연결되면 **[!UICONTROL View Store]** 추가된 스토어에 대해.

   스토어 [대시보드](./amazon-store-dashboard.md) 이 표시되고 `No products listed to Amazon` 메시지.

1. 클릭 **[!UICONTROL Preview and List Eligible Products]**.

   다음 _[!UICONTROL Listing Rules]_페이지가 나타납니다.

1. Amazon에 나열할 제품의 자격 조건을 원하는 대로 정의하고 을 클릭합니다. **[!UICONTROL Preview changes]**&#x200B;또는 클릭 **[!UICONTROL Preview changes]** 이 단계를 건너뜁니다.

   다음을 참조하십시오 [예: 조건 정의](./ob-define-condition-example.md).

1. 목록 미리 보기에서 목록을 검토합니다.

   ![목록 미리 보기](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정을 기반으로 하는 Amazon 목록에 적합하지 않습니다.

      부적격 제품은 Amazon에 게시되지 않습니다. 부적격 제품이 이미 Amazon에 나열되어 있고 Amazon 목록을 다음에 일치시키는 경우 [!DNL Commerce] 카탈로그 제품, Amazon 목록 수량이 다음으로 변경됨: `0` 제품을 판매하지 않도록 합니다. Amazon에서 목록을 수동으로 제거하려면 [Amazon 목록 종료](./end-listings-manually.md). Amazon 요구 사항이 적용되지 않는 제품은 여기에 나열되지 않습니다. 이러한 제품은 다음 목록에 있습니다. [[!UICONTROL Inactive Listings] 탭](./inactive-listings.md).

      을(를) 변경하려면 `Ineligible` 에 나열 `Eligible` 목록을 작성하려면 이 프로세스를 반복하고 목록 규칙을 수정합니다.

   - **[!UICONTROL Eligible Listings]** - 이 탭에 나열된 제품은 현재 목록 규칙 설정을 기반으로 Amazon을 나열할 수 있으며 Amazon 요구 사항에 따라 사용할 수 있습니다. 이 탭에는 가져온 기존 Amazon 목록이 포함되어 있습니다(있는 경우). **[!UICONTROL Import Third Party Listings]** 을 로 설정 `Import Listing` (으)로 [목록 설정](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - 이 탭에 나열된 제품에는 [!DNL Commerce] 현재 목록 규칙 설정 및 Amazon 목록 만들기에 따라 Amazon 목록에 새로 사용할 수 있는 카탈로그 제품.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save and Close]**.

   스토어 [대시보드](./amazon-store-dashboard.md) 열림.

스토어 온보딩이 완료되면 다음 사이에 정보가 동기화됩니다. [!DNL Commerce] 그리고 Amazon이 시작되었습니다. Amazon 목록을으로 가져옵니다. [!DNL Commerce] 및 을(를) 의 제품과 일치시키려고 합니다. [!DNL Commerce] 카탈로그.

에서 Amazon 주문 정보를 볼 수 있습니다. _[!UICONTROL Recent Orders]_섹션 을 참조하십시오. 다음을 참조하십시오 [대시보드 저장](./amazon-store-dashboard.md) 또는 [주문 관리](./managing-orders.md).

>[!IMPORTANT]
>
>새 스토어에 대한 기본값이 있는 몇 가지 중요한 스토어 설정 (목록, 가격 책정, 규칙, 이행 등)이 있습니다. 스토어가 특정 요구 사항에 맞게 설정되었는지 확인하려면 다음을 검토하십시오. [스토어 설정](./default-store-settings.md) .

![다음 아이콘](assets/btn-next.png) [**기본 저장소 설정으로 계속**](./default-store-settings.md)
