---
title: 활성 Amazon 목록
description: Amazon 판매 채널에서는 활성 Amazon 목록을 모니터링하고 Adobe Commerce 카탈로그의 제품에 일치하는 활성 탭을 제공합니다.
feature: Sales Channels, Products, Merchandising, Catalog Management
exl-id: c9105abc-74d6-442b-8d7a-e5aaea8872e4
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 활성 Amazon 목록

다음 _[!UICONTROL Active]_탭은에 활성 목록을 표시합니다. [!DNL Amazon Marketplace] 이(가) 의 제품과 일치합니다. [!DNL Commerce] 카탈로그.

에서 사용 가능한 작업 _[!UICONTROL Active]_탭에는 다음이 포함됩니다.

아래 _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: 선택한 모든 목록을 다음에서 제거하도록 선택합니다 [!DNL Amazon Marketplace]. 다음을 참조하십시오 [Amazon 목록 종료](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: 목록에 대한 무시 설정을 변경하려면 선택합니다. 다음을 참조하십시오 [재정의](./overrides.md) 또는 [재정의 편집 또는 제거](./creating-editing-overrides.md#edit-override-single-listing).

아래 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_열:

- **[!UICONTROL View Details]**: 다음을 포함한 목록 세부 정보를 보도록 선택합니다. [활동 로그 나열](./product-listing-details.md#listing-activity-log), [Buy Box 경쟁업체 가격](./product-listing-details.md#buy-box-competitor-pricing), 및 [경쟁사 최저 가격](./product-listing-details.md#lowest-competitor-pricing). 이 작업은 보기 전용입니다. 목록 세부 사항을 변경할 수 없습니다. 다음을 참조하십시오 [세부 사항 보기](./product-listing-details.md).

- **[!UICONTROL Create Override]**: 재정의를 생성하고 이 목록에 적용하도록 선택합니다. 다음을 참조하십시오 [재정의 만들기](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: 카탈로그 제품에 할당된 ASIN을 수정하도록 선택합니다. 카탈로그의 제품이 잘못된 ASIN과 일치하는 경우 이 작업을 사용합니다. 다음을 참조하십시오 [할당된 ASIN 편집](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: 동일한 카탈로그 제품에서 Amazon 목록을 만드는 데 사용할 수 있는 별칭 SKU를 만들 수 있습니다. 다음을 참조하십시오 [별칭 판매자 SKU 만들기](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: 주문과 연관된 이행 방법을 변경하도록 선택합니다. 다음을 참조하십시오 [이행된 사용자 설정 구성](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: 목록에서 제거하려면 선택합니다. [!DNL Amazon Marketplace]. 다음을 참조하십시오 [Amazon 목록 종료](./end-listings-manually.md).

>[!NOTE]
>
>목록이 처리 중인 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![활성 목록](assets/amazon-active-listings.png){width="700" zoomable="yes"}

Amazon 판매 채널 홈 페이지는 몇 가지 공통점을 공유합니다. [작업 영역 컨트롤](./workspace-controls.md) 을 사용하면 표시되는 데이터를 사용자 정의할 수 있습니다.

| 열 | 설명 |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit). |
| [!UICONTROL ASIN] | 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유 블록입니다. <br><br>ASIN은 [!DNL Amazon Standard Identification Number]. ASIN은 항목을 식별하는 10개의 문자 및/또는 숫자로 구성된 고유한 블록입니다. 책의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 확인할 수 있으며, 항목과 관련된 자세한 내용도 확인할 수 있습니다. |
| [!UICONTROL Product Listing Name] | 제품 이름. |
| [!UICONTROL Condition] | 다음 [조건](./product-listing-condition.md) 제품. |
| [!UICONTROL Landed Price] | 제품의 목록 가격과 배송 가격을 더한 값입니다. |
| [!UICONTROL Amazon Quantity] | 제품이 출시된 후 사용 가능한 수량은 Amazon에 활발하게 나열됩니다. |
| [!UICONTROL Status] | Amazon으로 정의된 목록의 상태. |
| [!UICONTROL Buy Box Won] | 제품 목록이 다음 항목에서 승리했는지 여부: [Buy Box](./buy-box-competitor-pricing.md) 위치. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 **[!UICONTROL Select]** 다음에서 _[!UICONTROL Action]_옵션을 표시할 열:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[[!UICONTROL Create Override]](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
