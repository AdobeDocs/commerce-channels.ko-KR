---
title: 작업별 제품 목록 관리
description: Amazon 목록을 관리할 때 개별 또는 여러 목록에 작업을 적용할 수 있습니다.
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 작업별 제품 목록 관리

다음 _[!UICONTROL Product Listings]_페이지에는 모든 목록의 상태를 보고 제품을 Amazon 목록에 연결할 수 있는 몇 개의 탭이 있습니다.

사용 가능한 목록 작업은 각 탭에서 약간 다르지만 [작업 영역 컨트롤](./workspace-controls.md) 동일하며 목록에 표시되는 데이터를 사용자 지정할 수 있습니다.

아래의 옵션 **[!UICONTROL Actions]** 옵션을 사용하여 여러 목록에 작업을 적용할 수 있습니다 **[!UICONTROL Select]** 에서 _[!UICONTROL Action]_열은 개별 목록에 작업만 적용합니다.

참조 - [상태/탭별 목록 관리](./managing-listings-by-tab.md).

| 작업 | 설명 | 탭 |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 불완전한 제품을 일치 프로세스를 통해 다시 이동하는 데 사용됩니다. 다시 일치시키려면 [목록](./listing-settings.md) 및 [카탈로그 검색](./catalog-search.md) 자동 일치 가능성을 높이도록 설정합니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 일치시킬 목록을 선택하거나 일치시킬 ASIN을 입력하거나 누락된 조건을 할당하여 카탈로그 제품을 Amazon 목록에 수동으로 일치시킵니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 개별 SKU/제품에 대한 변경 사항을 표시하는 목록 활동 로그를 비롯한 활성 제품에 대한 추가 정보를 봅니다. | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | 만들기 [!DNL Commerce] Amazon 목록과 함께 가져온 정보를 사용하여 카탈로그 제품을 만듭니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 자동 일치 시도 | 자동 일치 [!DNL Commerce] 검색 기준 설정에 따라 카탈로그 및 Amazon 목록을 만듭니다. 다시 일치시키려면 [목록](./listing-settings.md) 및 [카탈로그 검색](./catalog-search.md) 자동 일치 가능성을 높이도록 설정합니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | 에서 기존 제품을 수동으로 선택합니다 [!DNL Commerce] 카탈로그를 만들어 Amazon 목록에 할당합니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | 만들기 [!DNL Commerce] Amazon 목록과 함께 가져온 정보를 사용하여 카탈로그 제품을 만듭니다. | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | (일괄 작업) 완료된 목록을 다시 나열하거나 목록 규칙 자격 조건을 충족하지만 사용자의 _[!UICONTROL Product Listing Actions]_이 설정되지 않음 `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | (단일 목록 작업) 종료된 목록을 릴리스하기 위해 사용됩니다. 이 작업은 다음 경우에 목록 규칙 자격 조건을 충족하는 제품을 수동으로 나열하는 데 사용됩니다 _[!UICONTROL Product Listing Actions]_이 설정되지 않음 `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | (일괄 작업) Amazon에 있는 제품에 대한 목록을 수동으로 종료 및 제거하는 데 사용됩니다. 종료 목록은 목록 규칙 자격 조건을 충족하는 한 신뢰할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | (일괄 조치) 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 노트 텍스트를 설정하는 기존 &quot;대체&quot;를 수동으로 편집하여 다른 목록 기본값, 설정 및 규칙을 무시합니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 다른 목록 기본값, 설정 및 규칙을 무시하고 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 노트 텍스트를 설정하는 &quot;무시&quot;를 수동으로 생성합니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 카탈로그 제품에 일치하는 ASIN을 수정해야 하는 경우 사용됩니다(예: 제품이 잘못된 목록 ASIN과 일치한 경우). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 다음 두 가지 기능을 제공할 수 있습니다.<br><br>카탈로그 제품과 두 Amazon 목록 간에 1~2 관계를 만드는 데 사용할 수 있습니다. 예: Amazon에는 다른 ASIN 값과 함께 나열된 제품이 있습니다. 하나의 카탈로그 제품을 제품에 대한 ASIN 목록 모두에 일치시킬 수 있습니다.<br><br>다른 Amazon 영역에서 목록을 제어하는 데 사용할 수 있습니다. 예: Amazon 지역을 기반으로 다른 배송 방법이 정의된 카탈로그 제품이 있습니다(미국 지역은 FBA이고 캐나다 지역은 FBM임). 재고/수량을 제어하려면 별칭 판매자 SKU를 만들고 다른 판매자 SKU를 사용하여 해당 지역에서 동일한 제품을 릴리즈할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 제품과 연결된 이행 방법을 수정하는 데 사용됩니다(Amazon에 의해 수행됨). 머천트에 의한 FBA 또는 이행: FBM). | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | (단일 목록 작업) Amazon에 있는 제품에 대한 목록을 수동으로 종료 및 제거하는 데 사용됩니다. 종료 목록은 목록 규칙 자격 조건을 충족하는 한 신뢰할 수 있습니다. | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | (단일 목록 작업) 다른 목록 기본값, 설정 및 규칙을 무시하고 개별 목록에 대한 가격, 처리 시간, 조건 및 판매자 노트 텍스트를 설정하는 기존 &quot;대체&quot;를 수동으로 편집합니다. | [[!UICONTROL Overrides]](./overrides.md) |

## 제품 목록 액세스

1. 설정 _관리_ 사이드바, 다음 위치로 이동 **마케팅** > _채널_ > **Amazon Sales Channel**.

1. 클릭 **저장소 보기** 매장 카드 위에

1. 저장소 대시보드에서 **목록 관리** 에서 _목록 저장_ 섹션을 참조하십시오.
