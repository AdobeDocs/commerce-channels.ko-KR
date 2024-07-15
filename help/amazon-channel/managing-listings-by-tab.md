---
title: 상태/탭별 Amazon 제품 목록 관리
description: Amazon 목록을 관리할 때 상태에 따라 목록에 작업을 적용할 수 있습니다.
feature: Sales Channels, Products
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 상태/탭별 Amazon 제품 목록 관리

_[!UICONTROL Product Listings]_페이지에는 모든 목록의 상태를 보고 제품을 Amazon 목록에 일치시킬 수 있는 몇 가지 탭이 있습니다.

각 탭에서 사용할 수 있는 목록 작업은 약간 다르지만 [작업 영역 컨트롤](./workspace-controls.md)은 동일하며 목록에 대해 표시되는 데이터를 사용자 지정할 수 있도록 해 줍니다.

**[!UICONTROL Actions]** 아래의 옵션은 여러 목록에 작업을 적용할 수 있지만 _[!UICONTROL Action]_열의&#x200B;**[!UICONTROL Select]**아래의 옵션은 개별 목록에만 작업을 적용합니다.

[작업별 목록 관리](./managing-listings-by-action.md)도 참조하세요.

![제품 목록 탭](assets/amazon-product-listings-tabs.png){width="600" zoomable="yes"}

| 탭 | 설명 | 작업 |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 정의된 목록 설정을 충족하지만 목록에 대해 Amazon에 필요한 정보가 없는 [!DNL Commerce] 카탈로그 제품을 표시합니다.<br><br>[_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정에서 _[!UICONTROL Automatic List Action]_이(가) `Automatically List Eligible Products`(으)로 설정되어 있으면 이 항목이&#x200B;**[!UICONTROL In Progress Listings]**입니다. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | [!DNL Commerce] 카탈로그의 제품과 일치하지 않는 기존 Amazon 목록(Amazon에서 받은 정보를 기반으로 함)을 표시합니다. | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>자동 일치 시도<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Amazon 목록을 만들 준비가 되었지만 새 목록을 자동으로 게시하지 않도록 스토어가 설정된 카탈로그 제품을 표시합니다. 이 탭은 새 목록을 수동으로 게시하는 데 사용됩니다.<br><br>[_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정에서 _[!UICONTROL Automatic List Action]_이(가) `Do Not Automatically List Eligible Products`(으)로 설정되어 있으면 이 항목이&#x200B;**[!UICONTROL In Progress Listings]**입니다. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Amazon에 게시되었지만 Amazon이 활성 상태에 대한 목록을 승인하지 않은 카탈로그 제품을 표시합니다. | Amazon에 [종료개 나열](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/판매자가 이행한 것으로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | [!DNL Commerce] 카탈로그의 제품과 일치하고, Amazon에 게시하고, Amazon에서 활성 상태로 유지한 Amazon 목록을 표시합니다. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/판매자가 이행한 상태로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 정의된 재정의 기준과 재정의가 적용된 Amazon 목록을 표시합니다. 재정의는 다른 계정 설정보다 우선합니다. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 정의된 [목록 설정](./listing-settings.md)을(를) 기반으로 더 이상 사용할 수 없는 기존 Amazon 목록을 표시합니다. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/판매자가 이행한 상태로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Amazon에서 수동으로 종료(제거)된 Amazon 목록을 표시합니다. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 제품 목록 액세스

1. _관리자_ 사이드바에서 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**(으)로 이동합니다.

1. 저장소 카드에서 **[!UICONTROL View Store]**&#x200B;을(를) 클릭합니다.

1. 스토어 대시보드의 _[!UICONTROL Store Listings]_섹션에서&#x200B;**[!UICONTROL Manage Listings]**을(를) 클릭합니다.
