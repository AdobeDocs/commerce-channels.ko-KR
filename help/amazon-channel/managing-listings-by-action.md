---
title: 작업별 Amazon 제품 목록 관리
description: Amazon 목록을 관리할 때 개별 또는 여러 목록에 작업을 적용할 수 있습니다.
feature: Sales Channels, Products
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 작업별 Amazon 제품 목록 관리

_[!UICONTROL Product Listings]_페이지에는 모든 목록의 상태를 보고 제품을 Amazon 목록에 일치시킬 수 있는 몇 가지 탭이 있습니다.

각 탭에서 사용할 수 있는 목록 작업은 약간 다르지만 [작업 영역 컨트롤](./workspace-controls.md)은 동일하며 목록에 대해 표시되는 데이터를 사용자 지정할 수 있도록 해 줍니다.

**[!UICONTROL Actions]** 아래의 옵션은 여러 목록에 작업을 적용할 수 있지만 _[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래의 옵션은 개별 목록에만 작업을 적용합니다.

[상태별 목록 관리/탭](./managing-listings-by-tab.md)도 참조하세요.

| 작업 | 설명 | 탭 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 불완전 제품을 일치 프로세스를 통해 다시 이동하는 데 사용됩니다. 다시 일치시키려면 [목록](./listing-settings.md) 및 [카탈로그 검색](./catalog-search.md) 설정을 수정하여 자동 일치의 가능성을 높여야 합니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 일치시킬 목록을 선택하거나, 일치시킬 ASIN을 입력하거나, 누락된 조건을 할당하여 카탈로그 제품을 Amazon 목록에 수동으로 일치시킵니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 개별 SKU/제품에 대한 변경 사항을 표시하는 목록 활동 로그를 포함하여 활성 제품에 대한 추가 정보를 봅니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | Amazon 목록으로 가져온 정보를 사용하여 [!DNL Commerce] 카탈로그 제품을 만듭니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 자동 일치 시도 | 검색 조건 설정을 기반으로 [!DNL Commerce] 카탈로그와 Amazon 목록 간의 자동 일치를 시도합니다. 다시 일치시키려면 [목록](./listing-settings.md) 및 [카탈로그 검색](./catalog-search.md) 설정을 수정하여 자동 일치의 가능성을 높여야 합니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | [!DNL Commerce] 카탈로그에서 기존 제품을 수동으로 선택하고 Amazon 목록에 지정하십시오. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | Amazon 목록으로 가져온 정보를 사용하여 [!DNL Commerce] 카탈로그 제품을 만듭니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | (일괄 작업) 종료된 목록을 다시 나열하거나 목록 규칙 자격 조건을 충족하지만 _[!UICONTROL Product Listing Actions]_이(가) `Automatically list new products`(으)로 설정되지 않은 제품을 수동으로 나열하는 데 사용됩니다. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | (단일 목록 작업) 종료된 목록을 다시 나열하는 데 사용됩니다. 이 작업은 _[!UICONTROL Product Listing Actions]_이(가) `Automatically list new products`(으)로 설정되지 않은 경우 목록 규칙 자격 조건을 충족하는 제품을 수동으로 나열하는 데에도 사용됩니다. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | (대량 작업) Amazon에 있는 제품 목록을 수동으로 종료하거나 제거하는 데 사용됩니다. 종료된 목록은 목록 규칙 적격성을 충족시키는 한 재평가할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | (일괄 조치) 다른 목록 기본값, 설정 및 규칙을 무시하고 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 노트 텍스트를 설정하는 기존 &quot;대체&quot;를 수동으로 편집합니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 다른 목록 기본값, 설정 및 규칙을 무시하고 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 메모 텍스트를 설정하는 &quot;재정의&quot;를 수동으로 만듭니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 카탈로그 제품과 일치하는 ASIN을 수정해야 하는 경우 사용됩니다(예: 제품이 잘못된 목록 ASIN과 일치하는 경우). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 두 가지 기능을 사용할 수 있습니다.<br><br>카탈로그 제품과 두 Amazon 목록 간의 1 대 2 관계를 만드는 데 사용할 수 있습니다. 예: Amazon에는 다른 ASIN 값과 함께 나열된 제품이 있습니다. 하나의 카탈로그 제품을 제품의 두 ASIN 목록에 일치시킬 수 있습니다.<br><br>다른 Amazon 지역에서 목록을 제어하는 데 사용할 수 있습니다. 예: Amazon 지역(미국 지역은 FBA이고 캐나다 지역은 FBM)을 기준으로 정의된 다른 운송 방법이 있는 카탈로그 제품이 있습니다. 재고/수량을 제어하기 위해 별칭 판매자 SKU를 만들고 해당 지역의 동일한 제품을 다른 판매자 SKU로 다시 나열할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 제품에 연결된 이행 방법(Amazon에서 이행함: FBA 또는 판매자에서 이행함: FBM)을 수정하는 데 사용됩니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | (단일 목록 작업) Amazon에 있는 제품 목록을 수동으로 종료하고 제거하는 데 사용됩니다. 종료된 목록은 목록 규칙 적격성을 충족시키는 한 재평가할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | (단일 목록 작업) 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 메모 텍스트를 설정하는 기존 &quot;재정의&quot;를 수동으로 편집하여 다른 목록 기본값, 설정 및 규칙을 무시합니다. | [[!UICONTROL Overrides]](./overrides.md) |

## 제품 목록 액세스

1. _관리자_ 사이드바에서 **마케팅** > _채널_ > **Amazon Sales Channel**(으)로 이동합니다.

1. 저장소 카드에서 **저장소 보기**&#x200B;를 클릭합니다.

1. 스토어 대시보드의 _스토어 목록 관리_ 섹션에서 **목록 관리**&#x200B;를 클릭합니다.
