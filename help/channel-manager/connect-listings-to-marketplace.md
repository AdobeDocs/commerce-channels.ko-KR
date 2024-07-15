---
title: 목록을 Walmart에 연결
description: '판매를 시작하려면  [!DNL Commerce] 제품 목록을  [!DNL Walmart Marketplace]에 연결하세요.'
feature: Sales Channels, Integration, Products, Tools and External Services
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# 목록을 Walmart에 연결

다른 마켓플레이스와 마찬가지로 [!DNL Walmart]을(를) 사용하면 타사 판매자가 다른 판매자가 판매하는 항목을 나열할 수 있습니다.

- [!DNL Walmart Marketplace]은(는) UPC 및 GTIN과 같은 제품 식별자를 사용하여 제품을 기존 [!DNL Walmart Marketplace] 목록에 일치시킵니다.

- 일치하는 제품의 경우 [!DNL Channel Manager]의 제품에 연결할 때 [!DNL Commerce] 제품 오퍼를 포함하도록 업데이트를 나열하는 Walmart Marketplace입니다.

- 일반적으로 가격이 가장 낮은 제품 오퍼가 [!DNL Walmart Marketplace] 목록에 먼저 표시되지만 리뷰와 같은 다른 요소도 배치에 영향을 줍니다.

## 제품 일치

제품이 일치하면 Channel Manager가 제품 데이터를 [!DNL Walmart Marketplace]에 보내 매핑된 [!DNL Commerce] 제품 특성과 일치하는 특성 값이 있는 기존 목록을 검색합니다. 일치 기준은 저장소 채널의 [특성 매핑 구성](map-catalog-attributes.md)에 의해 결정됩니다.

일치하는 항목이 있으면 오퍼를 추가하도록 기존 제품 목록이 업데이트됩니다.

### 전제 조건

제품을 일치시키기 전에 제품 카탈로그 속성 값이 Walmart 요구 사항을 충족하는지 확인하고 제품 속성 설정을 구성합니다. [카탈로그 특성 매핑](map-catalog-attributes.md)을 참조하세요.

#### 제품 선택 및 일치

1. 연결된 판매 채널을 엽니다.

1. **[!UICONTROL Listings]**&#x200B;에서 *[!UICONTROL Draft]* 상태의 일치하는 제품을 선택하십시오.

   ![목록에서 제품을 선택하고 일치시키기 위해 보내기](assets/products-in-marketplace-sales-channel.png){width="500" zoomable="yes"}

1. **[!UICONTROL Match Products]**&#x200B;을(를) 선택합니다.

   대응을 위해 보낸 제품 수를 나타내는 메시지가 표시됩니다.

   일치 작업이 완료될 때까지 선택한 제품의 상태가 [!UICONTROL *처리 중*](으)로 변경됩니다. 월마트 마켓플레이스가 매치 작전을 완료하는 데 최대 30분이 소요될 수 있다.

### 일치 상태 확인

일치가 완료되면 **[!UICONTROL Refresh products]**&#x200B;을(를) 선택하여 현재 제품 상태를 확인합니다. *일치* 또는 *오류*.

- **[!UICONTROL Match]**&#x200B;은(는) 제품이 성공적으로 일치했음을 나타냅니다. 제품 오퍼가 기존 Walmart Marketplace 목록에 연결되었습니다. [Marketplace 저장소가 활성화되지 않은 경우](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]*&#x200B;이(가) *[!UICONTROL Status detail]* 열에 표시됩니다. 스테이징된 제품은 [!DNL Walmart Marketplace] 스토어가 활성화되면 자동으로 연결됩니다.

- **[!UICONTROL Error]**&#x200B;은(는) 다음 문제 중 하나로 인해 일치 작업이 실패했음을 나타냅니다.

   - 연결 문제로 인해 [!DNL Channel Manager]에서 일치 항목을 보낼 수 없습니다.

   - 일치하는 항목을 찾을 수 없습니다.

   - 일치하는 항목을 찾았지만 [!DNL Walmart Marketplace]에서 오류 코드를 반환했기 때문에 목록을 연결할 수 없습니다. 문제에 대한 자세한 내용은 **[!UICONTROL Error Description]**&#x200B;을(를) 참조하세요.

### Walmart의 수표 목록

제품을 일치시킨 후 업데이트된 제품 목록을 검토하고 [[!UICONTROL Walmart Marketplace Seller Account Items] 대시보드](https://seller.walmart.com/items-and-inventory/manage-items)에서 제품 세부 사항, 가격 및 재고 수량을 확인하여 업데이트된 제품을 검토하십시오.

### 제품 일치 오류 문제 해결

제품 일치 작업이 실패하고 오류가 발생하면 [!UICONTROL Channel Manager] 제품 목록의 *[!UICONTROL Status detail]* 열에 오류 메시지가 표시됩니다.

반환된 일반적인 오류는 잘못된 형식의 제품 ID 값이거나 필수 속성이 없습니다.

#### 제품 ID 값 수정

| 유형 | 설명 | 예 |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, 확인 숫자를 포함한 12자리 숫자. </br></br>UPC가 8자리 UPC-E와 같이 12자리 미만인 경우 요구 사항을 충족하도록 끝 0을 추가합니다. | `45678912345`에서 `045678912345`(으)로 변경 |
| GTIN | GTIN-14, 확인 숫자를 포함한 14자리 숫자. </br></br>GTIN의 자릿수가 14자리보다 적은 경우 요구 사항을 충족하려면 선행 0인 </br>을(를) 추가하십시오. | `456789123456`을(를) `0045678912345`(으)로 변경 |
| EAN | GTIN-13, 확인 숫자를 포함한 13자리 숫자. </br></br>EAN의 자릿수가 13자리 미만인 경우 선행 </br>0을(를) 추가하여 요구 사항을 충족하십시오. | `4567891234`에서 `0004567891234`(으)로 변경 |

Walmart Marketplace 오류 코드에 대한 자세한 내용은 [Walmart 판매자 도움말](https://sellerhelp.walmart.com/s/guide?article=000005844)을 참조하세요.

## 새 제품 목록 업로드

Walmart Marketplace에 일치하는 항목이 없는 제품의 경우 Walmart 제품 범주 Excel 템플릿을 사용하여 제품 목록을 대량으로 업로드하십시오. [!DNL Commerce] 인스턴스에서 내보낸 제품 카탈로그 데이터를 사용하여 Walmart 템플릿을 채웁니다.

새 제품 목록의 경우 제품 카탈로그를 확인하여 Walmart Marketplace에서 판매하려는 제품에 Walmart Marketplace 제품 목록에 필요한 속성이 있는지 확인하십시오.

**Walmart Marketplace 목록 특성 요구 사항**

| **특성** | **요구 사항 수준** |
|--------------------------|-----------------------|
| SKU | 필수 |
| 제품 이름 | 필수 |
| 제품 ID 유형 | 필수 |
| 제품 ID | 필수 |
| 브랜드 | 필수 |
| 간단한 설명 | 필수 |
| 판매 가격 | 필수 |
| 사이트 설명 | 필수 |
| 주 이미지 URL | 필수 |
| 배송 무게 | 필수 |
| 주요 기능 | 추천 |
| 모델 번호 | 추천 |
| 제조업체 이름 | 추천 |
| 제조업체 부품 번호 | 추천 |
| 크기 | 추천 |
| 색상 | 추천 |
| 주 이미지 URL | 선택 사항 |
| 추가 이미지 URL | 선택 사항 |
| 제조업체 | 선택 사항 |

### 전제 조건

- [Walmart 요구 사항](walmart-requirements.md)을 충족하는지 확인하십시오.

- [!DNL Commerce] 제품 카탈로그에서 Walmart Marketplace에 나열할 제품에 대한 카탈로그 구성에 필요한 모든 특성이 있는지 확인하고 Walmart Marketplace 콘텐츠 지침을 충족하는지 확인하십시오.

- 내보내기 작업을 완료하기 위해 cron 작업이 실행 중인지 확인하십시오.

   - 온-프레미스 인스턴스의 경우 [cron 구성 및 실행](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/configure-cron-jobs.html)을 참조하세요.

   - Adobe 클라우드 인프라의 경우 [cron 작업 설정](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/properties/crons-property.html)을 참조하십시오.

### 업로드할 제품 데이터 파일 만들기

1. [Walmart 판매자 계정](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)에서 Walmart 판매자 센터에서 제품 목록 템플릿을 다운로드하십시오.

   - 제품 카탈로그 항목 페이지에서 **[!UICONTROL Add Items]**&#x200B;을(를) 선택합니다. **[!UICONTROL Add items in bulk]**&#x200B;을(를) 선택합니다.

     ![Walmart Marketplace 항목 구성에서 일괄 옵션에 항목 추가](assets/walmart-seller-account-add-items-bulk.png){width="600" zoomable="yes"}

   - 다운로드 페이지에서 **[!UICONTROL Full Setup]**&#x200B;을(를) 선택합니다. 그런 다음 항목 카테고리를 선택하고 카테고리 템플릿을 다운로드합니다.

     ![Walmart Marketplace 항목 구성에서 범주 템플릿 옵션 다운로드](assets/walmart-seller-account-full-setup-download.png){width="600" zoomable="yes"}

   - 템플릿에 제품 목록에 대한 필수 속성과 권장 속성이 포함되어 있는지 확인합니다.

1. [!DNL Commerce] 관리자의 Adobe [!DNL Commerce] 사이트에서 내보낼 제품 데이터를 선택합니다.

   - 관리자의 [!UICONTROL **시스템** > 데이터 전송 > **내보내기**]&#x200B;를 선택합니다.

   - [!UICONTROL Entity Type] 필드의 [!UICONTROL Export] 페이지에서 [!UICONTROL **제품**]&#x200B;을 선택합니다.

   - [!UICONTROL Entity Attributes] 테이블에서 제품 데이터 내보내기에 대한 선택 기준을 구성합니다.

     필터를 사용하여 판매하는 제품 범주에 적용되는 속성 값을 선택하고 구성합니다. Walmart의 필수 특성과 권장 특성을 포함해야 합니다. 자세한 지침은 Adobe [!DNL Commerce] 사용 안내서의 [데이터 내보내기](https://experienceleague.adobe.com/docs/commerce-admin/systems/data-transfer/data-export.html)를 참조하십시오.

     내보내기에서 특성을 생략하려면 행의 시작 부분에 있는 [!UICONTROL **제외**] 확인란을 선택하십시오.

1. 특성 테이블의 끝으로 스크롤하고 [!UICONTROL **계속**]&#x200B;을 선택하여 데이터 내보내기를 시작합니다.

   CSV 내보내기 파일은 cron 작업을 사용하여 메시지 큐를 통해 처리되고 `var/export/folder`에 저장됩니다. (*구성 가이드*&#x200B;에서 [메시지 큐 관리](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/message-queues/manage-message-queues.html)를 참조하십시오.)

1. Walmart Marketplace 제품 범주에 대한 Excel 템플릿을 열고 Excel 매크로 기능을 사용하여 내보낸 제품 데이터를 Excel 템플릿에 병합합니다.

1. 내보낸 제품 데이터로 Excel 파일을 업로드합니다.

   - [Walmart Seller Center](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)의 제품 카탈로그 항목 페이지로 돌아갑니다.

   - [!UICONTROL **항목 추가** > **일괄 항목 추가**]&#x200B;를 선택합니다.
   - 완료된 스프레드시트를 업로드 섹션으로 드래그합니다.
   - [!UICONTROL **제출**]&#x200B;을 선택합니다.
   - 진행 상황을 보려면 [!UICONTROL  **활동 피드**]&#x200B;를 선택하십시오.

자세한 지침은 [!DNL *Walmart 판매자 도움말*]&#x200B;에서 [전체 항목 사양을 사용하여 항목 일괄 추가](https://sellerhelp.walmart.com/s/guide?article=000007680)를 참조하십시오.
