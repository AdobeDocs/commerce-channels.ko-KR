---
title: 목록 관리
description: 'Adobe Commerce 및 Magento Open Source용 채널 관리자를 사용하여  [!DNL Commerce] 스토어의 판매 채널 목록을 관리합니다.'
feature: Sales Channels, Merchandising, Products
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# 목록 관리

채널 관리자 UI에서 [!DNL Walmart Marketplace] 판매 채널에 대한 제품 목록을 관리합니다.

개별 목록에 대한 상태는 [!DNL Channel Manager] 워크플로에서 제품이 있는 위치를 나타내므로 다음 단계를 결정하고 오류를 해결할 수 있습니다.

![연결된 판매 채널의 목록 페이지](assets/listings-dashboard-view.png){width="500" zoomable="yes"}

목록 보기에서 다음 작업을 완료할 수 있습니다.

* 현재 목록 보기
* 목록 정렬 및 필터링
* 제품 추가
* 제품 일치
* 목록 상태 추적
* 오류 상태의 목록에 대한 오류 설명 검토

## 제품 목록 보기

1. 관리자의 경우 [!UICONTROL **마케팅** > **채널 관리자**](으)로 이동합니다.

1. 저장소 목록에서 저장소 항목 행의 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

1. [!UICONTROL **목록**]&#x200B;을 선택하세요.

1. *나열* 테이블에서 열 머리글을 선택하여 *나열* 보기를 정렬합니다.

1. 상태 수 카드 중 하나를 선택하여 *나열* 보기를 필터링합니다.

1. **제품 새로 고침**&#x200B;을 선택하여 정렬 순서를 재설정하고 필터를 제거하십시오.

## 채널 관리자에 [!DNL Commerce] 제품 추가

다음 작업을 완료하여 [!DNL Walmart Marketplace] 채널에 대한 제품 분류를 만듭니다.

* [ [!DNL Commerce] 제품 카탈로그의 제품을  [!DNL Channel Manager]에 추가](add-products-to-channel-store.md)

* [카탈로그 속성 매핑](map-catalog-attributes.md#configure-product-attribute-settings)

## [!DNL Walmart]의 제품 일치

제품 일치를 사용하거나 새 제품에 대한 제품 목록을 수동으로 업로드하여 [!DNL Walmart Marketplace]에서 제품 오퍼를 만들 수 있습니다.

* **[Walmart에서 제품 일치](connect-listings-to-marketplace.md)**—같은 제품을 판매하는 기존 목록을 업데이트하여 채널의 제품 목록을 [!DNL Walmart Marketplace]에 연결합니다. 일치 기준은 채널의 [특성 매핑 구성](map-catalog-attributes.md)에 의해 결정됩니다.

* **[새 목록을 수동으로 업로드](connect-listings-to-marketplace.md#upload-new-product-listings)**—[!DNL Walmart Marketplace]의 기존 목록과 일치하지 않는 제품의 경우 [!DNL Walmart] 제품 범주 Excel 템플릿을 사용하여 제품 목록을 대량으로 업로드하십시오.

## 컨트롤 및 열 설명 나열

다음 표에서는 [!UICONTROL Listings]에서 사용할 수 있는 컨트롤 및 열에 대해 설명합니다.

[!UICONTROL Listings]**에 대한**&#x200B;컨트롤

| **컨트롤** | **설명** |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | [!UICONTROL Admin Product Catalog] 페이지를 열어 [!DNL Walmart Marketplace] 분류에 추가할 제품을 선택하거나 Walmart Marketplace 목록 요구 사항을 충족하도록 제품 특성을 업데이트합니다. |
| [!UICONTROL Match products on Walmart] | [!UICONTROL Draft] 상태에서 하나 이상의 제품을 선택한 후 [!UICONTROL Match products on Walmart]을(를) 선택하여 기존 [!DNL Walmart Marketplace] 목록에 추가할 수 있는 제품 오퍼를 확인하십시오. |
| [!UICONTROL Refresh products] | 디스플레이를 최신 목록 및 상태로 업데이트합니다. 또한 이 컨트롤은 목록 보기를 기본 정렬 순서로 재설정하고 필터를 제거합니다. |
| [!UICONTROL Filter by *상태*] | 목록 테이블 위에 있는 상태 카드 중 하나를 선택하여 특정 상태의 목록만 표시합니다. **[!UICONTROL Refresh products]**&#x200B;을(를) 선택하여 필터를 제거하십시오. |
| [!UICONTROL Sort products] | 열 헤더를 선택하여 나열할 정렬 순서를 변경합니다. |


**열 설명**

| **필드** | **설명** |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | [!DNL Commerce] 스토어 카탈로그의 제품 이름입니다. |
| [!UICONTROL SKU (Unique ID)] | [!DNL Commerce] 카탈로그의 제품에 할당된 SKU입니다. |
| [!UICONTROL  Quantity] | Adobe Commerce 또는 Magento Open Source에서 사용할 수 있는 재고 양입니다. |
| [!UICONTROL Price] | [!DNL Commerce] 스토어 카탈로그의 제품 가격입니다. 카탈로그 가격 업데이트가 채널 관리자에 동기화된 후 [!DNL Walmart Marketplace]에 전송되어 나열된 항목에 현재 가격이 표시됩니다. |
| [!UICONTROL Status] | [!DNL Commerce] 주문 워크플로우의 현재 주문 상태를 나타냅니다. [!DNL Channel Manager]에 제품을 성공적으로 추가했을 때와 마켓플레이스에서 제품을 일치시킬 때 상태가 업데이트됩니다. 작업이 실패하면 목록에 오류 상태가 표시됩니다. 오류를 수정한 후 [!DNL Channel Manager]이(가) 작업을 다시 시도하고 상태를 업데이트합니다. |
| [!UICONTROL Error Description] | `[!DNL Error]` 상태의 제품에 대한 추가 오류 정보를 제공합니다. |

### 목록 상태 정보

목록 작업 영역에서 상태 레이블은 [!DNL Channel Manager] 워크플로에서 제품이 있는 위치를 표시하므로 다음 단계를 결정하고 오류를 해결할 수 있습니다. 목록에는 다음 상태 레이블이 있을 수 있습니다.

* **[!UICONTROL Draft]** - [이(가) 아닌 제품을 일치 [!DNL Walmart] 을(를) 위해 제출](connect-listings-to-marketplace.md#match-products)한 제품을 식별합니다.

* **[!UICONTROL Processing]** - [!DNL Walmart Marketplace]에 일치하기 위해 제출된 제품을 식별합니다. 제품은 [!DNL Walmart]이(가) 일치의 성공 여부 또는 오류가 있는지 여부를 나타내는 HTTP 상태 메시지를 반환할 때까지 *처리 중* 상태로 유지됩니다. [!DNL Walmart Marketplace]에서 일치 작업을 완료하는 데 최대 30분이 걸릴 수 있습니다.

* **[!UICONTROL Match]** - [!DNL Walmart]에서 일치하는 제품을 식별합니다.

  제품 속성 값(예: UPC 코드)이 기존 [!DNL Walmart Marketplace] 목록의 UPC 값과 일치하면 일치가 발생합니다. 제품이 일치하면 Commerce 제품 오퍼가 기존 목록에 추가됩니다.

  [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) 대시보드를 확인하여 업데이트된 제품 목록을 검토하고 제품 세부 사항, 가격 및 재고 수량을 확인하십시오.

* **[!UICONTROL Match - Match in Stage]** - [!DNL Walmart Marketplace] 스토어가 라이브될 때까지 연결할 수 없는 [!DNL Walmart]에 일치하는 제품을 식별합니다. [!DNL Walmart Marketplace] 스토어가 활성 상태가 되면 이 상태의 제품이 자동으로 연결됩니다.

* **[!UICONTROL Error]** - 기존 [!DNL Walmart Marketplace] 목록과 일치하지 않는 제품을 식별합니다.

* **[!UICONTROL Error description]** - 목록 오류에 대한 자세한 정보를 제공합니다.

  오류를 해결한 후 일치하는 제품을 다시 제출합니다. [제품 일치 오류 문제 해결](connect-listings-to-marketplace.md#troubleshoot-product-match-errors)을 참조하세요.
