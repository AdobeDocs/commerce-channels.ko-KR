---
title: 목록 관리
description: 에 대한 영업 채널 목록 관리 [!DNL Commerce] Adobe Commerce 및 Magento Open Source용 채널 관리자를 사용하여 저장합니다.
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 71ad5e3bc9ff6b909943a161472e4db7d375683f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# 목록 관리

에 대한 제품 목록 관리 [!DNL Walmart Marketplace] 판매 채널 [!UICONTROL Listings] 채널 저장소 보기에서 다음을 수행합니다. 개별 목록의 상태는 제품이 있는 위치를 나타냅니다 [!DNL Channel Manager] 워크플로우에서 다음 단계를 결정하고 오류를 해결할 수 있습니다.

개별 목록의 상태는 제품이 있는 위치를 나타냅니다 [!DNL Channel Manager] 워크플로우에서 다음 단계를 결정하고 오류를 해결할 수 있습니다.

![연결된 영업 채널에 대한 목록 페이지](assets/product-listing-landing.png)

목록 보기에서 다음 작업을 완료할 수 있습니다.

* 현재 목록 보기
* 목록 정렬 및 필터링
* 제품 추가
* 제품 일치
* 목록 상태 추적

## 제품 목록 보기

1. 관리자에서 로 이동합니다. [!UICONTROL **마케팅** > 채널 > **채널 관리자**].

1. 채널 저장소 목록에서 저장소 항목 행에 있는 연필 아이콘을 선택하여 저장소 보기를 엽니다.

1. 선택 [!UICONTROL **목록**].

1. 정렬 *목록* 보기 *목록* 테이블.

1. 필터 *목록* 상태 카운트 카드 중 하나를 선택하여 봅니다.

1. 정렬 순서를 재설정하고 선택 **제품 새로 고침**.

## 채널 관리자에 상거래 제품 추가

다음 작업을 완료하여 Walmart Marketplace 채널에 대한 제품 섹션을 만듭니다.

* [상거래 제품 카탈로그의 제품을 채널 관리자에 추가합니다](add-products-to-channel-store.md)

* [카탈로그 속성 매핑](map-catalog-attributes.md#configure-product-attribute-settings)

## Walmart에 제품 게시

제품 일치 기능을 사용하거나 새 제품에 대한 제품 목록을 수동으로 업로드하여 Walmart Marketplace에서 제품 오퍼를 만들 수 있습니다.

* **[Walmart에서 제품 일치](publish-listings-to-marketplace.md)**—채널에서 로 제품 목록을 게시합니다. [!DNL Walmart Marketplace] 동일한 제품을 판매하는 기존 목록을 업데이트하여 일치 기준은 [속성 매핑 구성](map-catalog-attributes.md) 채널용.

* **[수동으로 새 목록 업로드](publish-listings-to-marketplace.md#upload-new-product-listings)**- Walmart Marketplace의 기존 목록과 일치하지 않는 제품의 경우 Walmart 제품 카테고리 Excel 템플릿을 사용하여 제품 목록을 벌크로 업로드하십시오.

## 목록 컨트롤 및 열 설명

다음 표에서는 [!UICONTROL Listings].

**컨트롤[!UICONTROL Listings]**

| **제어** | **설명** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Add Products] | 를 엽니다. [!UICONTROL Admin Product Catalog] 페이지에 추가할 제품을 선택하는 페이지 [!DNL Walmart Marketplace] Walmart Marketplace 목록 요구 사항을 충족하도록 제품 특성을 분류하거나 업데이트합니다. |
| [!UICONTROL Match products on Walmart] | 초안 상태에서 하나 이상의 제품을 선택한 후 Mart에서 제품 일치 를 선택하여 기존 제품에 추가할 수 있는 제품 오퍼를 확인합니다 [!DNL Walmart Marketplace] 목록. |
| [!UICONTROL Refresh products] | 디스플레이를 최신 목록 및 상태로 업데이트합니다. 또한 이 컨트롤은 목록 보기를 기본 정렬 순서로 재설정하고 필터를 제거합니다. |
| [!UICONTROL Filter by *상태*] | 목록 테이블 위에 있는 상태 카운트 카드 중 하나를 선택하여 특정 상태의 목록만 표시합니다. 를 사용하십시오 *제품 새로 고침* 필터를 제거합니다. |
| [!UICONTROL Sort products] | 열 헤더를 선택하여 나열할 정렬 순서를 변경합니다. |


**열 설명**

| **필드** | **설명** |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | 제품의 이름 [!DNL Commerce] 카탈로그를 저장합니다. |
| [!UICONTROL SKU (Unique ID)] | 마켓플레이스의 제품과 일치하는 데 사용되는 매핑된 속성입니다. 이 필드 이름은 매핑 대상 속성 구성에 따라 달라집니다 [!DNL Channel Manager] 목록. 이 경우 제품 일치 작업은 [!DNL Commerce] 카탈로그 [!DNL Walmart Marketplace]  다음 항목의 SKU 값과 일치하는 SKU 값을 사용하여 나열 [!DNL Commerce] 제품 속성을 사용합니다. |
| [!UICONTROL  Quantity] | Adobe Commerce 또는 Magento Open Source에서 사용할 수 있는 재고량. |
| [!UICONTROL Price] | 제품 가격은 [!DNL Commerce] 카탈로그를 저장합니다. 카탈로그 가격 업데이트는 채널 관리자에 동기화된 다음 [!DNL Walmart Marketplace]  따라서 나열된 항목들은 현재 가격을 보여줍니다. |
| [!UICONTROL Status] | 에서 현재 주문 상태를 나타냅니다. [!DNL Commerce] 주문 워크플로우입니다. 에 제품을 성공적으로 추가하면 상태가 업데이트됩니다 [!DNL Channel Manager] 및 를 사용하여 시장에서 제품을 일치시킬 수 있습니다. 작업이 실패하면 목록에 오류 상태가 표시됩니다. 오류를 수정한 후 [!DNL Channel Manager] 작업을 다시 시도하고 상태를 업데이트합니다. |
| [!UICONTROL Status Detail] | 다음을 사용하는 제품에 대한 추가 정보를 제공합니다. *오류* 또는 *일치* 상태. |

### 목록 상태 정보

목록 작업 영역에서 상태 레이블에 제품이 있는 위치가 표시됩니다 [!DNL Channel Manager] 워크플로우에서 다음 단계를 결정하고 오류를 해결할 수 있습니다. 목록에는 다음 상태 레이블이 있을 수 있습니다.

* **[!UICONTROL Draft]**-이전부터 사용하지 않은 제품을 식별합니다 [제출됨 [!DNL Walmart] 일치하는 항목](publish-listings-to-marketplace.md#match-products).

* **[!UICONTROL Processing]**—에서 일치하기 위해 제출된 제품을 식별합니다. [!DNL Walmart Marketplace]. 제품이 다음 위치에 남아 있음 *처리 중* 상태 [!DNL Walmart] 일치 성공 여부 또는 오류 여부를 나타내는 HTTP 상태 메시지를 반환합니다. 에서 일치 작업을 완료하는 데 최대 30분이 걸릴 수 있습니다. [!DNL Walmart Marketplace].

* **[!UICONTROL Match]**-에 대해 일치하는 제품을 식별합니다 [!DNL Walmart].

   제품 속성 값(예: UPC 코드)이 기존[!DNL Walmart Marketplace] 목록. 제품이 일치하면 상거래 제품 오퍼가 기존 Walmart 목록에 추가됩니다.

   을(를) 확인합니다. [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) 대시보드 를 사용하여 업데이트된 제품 목록을 검토하고 제품 세부 사항, 가격 및 재고 수량을 확인합니다.

* **[!UICONTROL Match - Match in Stage]**- 일치하는 제품을 식별합니다. [!DNL Walmart] 게시할 때까지 [!DNL Walmart Marketplace] 스토어는 라이브입니다. 이 상태가 있는 제품은 [!DNL Walmart Marketplace] 가게 라이브로

* **[!UICONTROL Error]**- 기존 제품과 일치하지 않는 제품을 식별합니다. [!DNL Walmart Marketplace] 목록.

* **[!UICONTROL Error description]**- 목록 오류에 대한 자세한 정보를 제공합니다.

   오류를 해결한 후 일치하는 제품을 다시 제출합니다. 자세한 내용은 [제품 일치 오류 문제 해결](publish-listings-to-marketplace.md#troubleshoot-product-match-errors).
