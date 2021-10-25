---
title: 상태/탭별 제품 목록 관리
description: Amazon 목록을 관리할 때 상태에 따라 목록에 작업을 적용할 수 있습니다.
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 상태/탭별로 제품 목록 관리

다음 _[!UICONTROL Product Listings]_페이지에는 모든 목록의 상태를 보고 제품을 Amazon 목록에 연결할 수 있는 몇 개의 탭이 있습니다.

사용 가능한 목록 작업은 각 탭에서 약간 다르지만 [작업 영역 컨트롤](./workspace-controls.md) 동일하며 목록에 표시되는 데이터를 사용자 지정할 수 있습니다.

아래의 옵션 **[!UICONTROL Actions]** 옵션을 사용하여 여러 목록에 작업을 적용할 수 있습니다 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열은 개별 목록에 작업만 적용합니다.

참조 - [작업별 목록 관리](./managing-listings-by-action.md).

![제품 목록 탭](assets/amazon-product-listings-tabs.png)

| 탭 | 설명 | 작업 |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 다음 항목을 표시합니다. [!DNL Commerce] 정의된 목록 설정을 충족하지만 목록에 Amazon에 필요한 정보가 없는 카탈로그 제품.<br><br>If _[!UICONTROL Automatic List Action]_가 로 설정되어 있습니다. `Automatically List Eligible Products` 다음 위치에서 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정, 이러한 항목은&#x200B;**[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | 의 제품과 일치하지 않는 기존 Amazon 목록(Amazon에서 받은 정보 기반)을 표시합니다 [!DNL Commerce] 카탈로그 | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>자동 일치 시도<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | Amazon 목록을 만들 준비가 된 카탈로그 제품을 표시하지만 스토어가 새 목록을 자동으로 게시하지 않도록 설정되어 있습니다. 이 탭은 새 목록을 수동으로 게시하는 데 사용됩니다.<br><br>If _[!UICONTROL Automatic List Action]_가 로 설정되어 있습니다. `Do Not Automatically List Eligible Products` 다음 위치에서 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 설정, 이러한 항목은&#x200B;**[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | Amazon에 게시되었지만 Amazon이 활성 상태에 대한 목록을 승인하지 않은 카탈로그 제품을 표시합니다. | [종료 Amazon의 목록](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/Merchant에서 충족으로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | 사용자의 제품에 일치된 Amazon 목록을 표시합니다 [!DNL Commerce] 카탈로그가 Amazon에 게시되었으며 Amazon에서 활성 상태를 위해 게시했습니다. | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/Merchant에서 충족으로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 정의된 재정의 기준과 재정의가 적용되는 Amazon 목록을 표시합니다. 재정의는 다른 계정 설정보다 우선합니다. | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 정의한 내용에 따라 더 이상 적합하지 않은 기존 Amazon 목록을 표시합니다 [목록 설정](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>Amazon/Merchant에서 충족으로 전환<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | Amazon에서 수동으로 종료(제거)한 Amazon 목록을 표시합니다. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 제품 목록 액세스

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 클릭 **[!UICONTROL View Store]** 매장 카드 위에

1. 저장소 대시보드에서 **[!UICONTROL Manage Listings]** 에서 _[!UICONTROL Store Listings]_섹션을 참조하십시오.
