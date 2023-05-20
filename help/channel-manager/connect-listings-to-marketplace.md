---
title: 목록을 Walmart에 연결
description: '다음에 대한 목록 연결: [!DNL Commerce] 제품 대상 [!DNL Walmart Marketplace]판매를 시작합니다.'
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 0%

---

# 목록을 Walmart에 연결

다른 장터들처럼 [!DNL Walmart] 서드파티 판매자가 다른 판매자가 판매하는 항목을 나열할 수 있도록 허용합니다.

- [!DNL Walmart Marketplace] 는 UPC 및 GTIN과 같은 제품 식별자를 사용하여 제품을 기존 제품에 일치시킵니다 [!DNL Walmart Marketplace] 목록.

- 일치하는 제품의 경우 Walmart Marketplace에서 업데이트를 나열하면 [!DNL Commerce] 에서 제품을 연결할 때 제품 오퍼 [!DNL Channel Manager].

- 일반적으로 가격이 가장 낮은 제품 오퍼가 [!DNL Walmart Marketplace] 나열하지만 리뷰와 같은 다른 요소는 배치에 영향을 줍니다.

## 제품 일치

제품이 일치하면 Channel Manager가 제품 데이터를 로 보냅니다. [!DNL Walmart Marketplace] 매핑된 와(과) 일치하는 속성 값이 있는 기존 목록을 검색하려면 [!DNL Commerce] 제품 특성입니다. 일치 기준은 다음에 의해 결정됩니다. [속성 매핑 구성](map-catalog-attributes.md) 스토어 채널용입니다.

일치하는 항목이 있으면 오퍼를 추가하도록 기존 제품 목록이 업데이트됩니다.

### 전제 조건

제품을 일치시키기 전에 제품 카탈로그 속성 값이 Walmart 요구 사항을 충족하는지 확인하고 제품 속성 설정을 구성합니다. 다음을 참조하십시오 [카탈로그 속성 매핑](map-catalog-attributes.md).

#### 제품 선택 및 일치

1. 연결된 판매 채널을 엽니다.

1. 출처: **[!UICONTROL Listings]**&#x200B;에 있는 일치 제품 선택 *[!UICONTROL Draft]* 상태.

   ![목록에서 제품을 선택하고 일치시키기 위해 전송](assets/products-in-marketplace-sales-channel.png)

1. 선택 **[!UICONTROL Match Products]**.

   대응을 위해 보낸 제품 수를 나타내는 메시지가 표시됩니다.

   선택한 제품의 상태가 (으)로 변경됩니다. [!UICONTROL *처리 중*] 일치 작업이 완료될 때까지. 월마트 마켓플레이스가 매치 작전을 완료하는 데 최대 30분이 소요될 수 있다.

### 일치 상태 확인

일치가 완료되면 다음을 선택합니다. **[!UICONTROL Refresh products]** 현재 제품 상태를 봅니다. *일치* 또는 *오류*.

- **[!UICONTROL Match]** 제품이 성공적으로 일치했음을 나타냅니다. 제품 오퍼가 기존 Walmart Marketplace 목록에 연결되었습니다. 다음과 같은 경우 [마켓플레이스 저장소가 활성화되지 않음](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* 다음에표시됨: *[!UICONTROL Status detail]* 열. 스테이징된 제품은 [!DNL Walmart Marketplace] 저장소가 활성화되었습니다.

- **[!UICONTROL Error]** 다음 문제 중 하나로 인해 일치 작업이 실패했음을 나타냅니다.

   - [!DNL Channel Manager] 연결 문제로 인해 일치를 위해 을(를) 보낼 수 없습니다.

   - 일치하는 항목을 찾을 수 없습니다.

   - 일치하는 항목을 찾았지만 다음 이유로 목록을 연결할 수 없습니다. [!DNL Walmart Marketplace] 에서 오류 코드를 반환했습니다. 다음을 참조하십시오. **[!UICONTROL Error Description]** 을 참조하십시오.

### Walmart의 수표 목록

제품을 대응시킨 후 업데이트된 제품 목록을 검토하고 제품에서 제품 세부 사항, 가격 및 재고 수량을 확인합니다. [[!UICONTROL Walmart Marketplace Seller Account Items] 대시보드](https://seller.walmart.com/items-and-inventory/manage-items) 을 클릭하여 업데이트된 제품을 검토합니다.

### 제품 일치 오류 문제 해결

제품 일치 작업이 오류와 함께 실패하면 오류 메시지가 *[!UICONTROL Status detail]* 열의 [!UICONTROL Channel Manager] 제품 목록.

반환된 일반적인 오류는 잘못된 형식의 제품 ID 값이거나 필수 속성이 없습니다.

#### 제품 ID 값 수정

| 유형 | 설명 | 예 |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, 확인 숫자를 포함한 12자리 숫자. </br></br>UPC가 8자리 UPC-E와 같이 12자리 미만인 경우 요구 사항을 충족하도록 끝 0을 추가합니다. | 다음에서 변경 `45678912345` 끝 `045678912345` |
| GTIN | GTIN-14, 확인 숫자를 포함한 14자리 숫자. </br></br>GTIN의 자릿수가 14자리 미만인 경우 앞에 0을 추가합니다 </br>요구 사항을 충족하기 위해 | 변경 `456789123456` 끝 `0045678912345` |
| EAN | GTIN-13, 확인 숫자를 포함한 13자리 숫자. </br></br>EAN이 13자리 미만인 경우 행간을 추가합니다. </br>0 을 입력하여 요구 사항을 충족합니다. | 다음에서 변경 `4567891234` 끝 `0004567891234` |

Walmartplace 오류 코드에 대한 자세한 내용은 다음을 참조하십시오. [Walmart Seller 도움말](https://sellerhelp.walmart.com/s/guide?article=000005844).

## 새 제품 목록 업로드

Walmart Marketplace에 일치하는 항목이 없는 제품의 경우 Walmart 제품 범주 Excel 템플릿을 사용하여 제품 목록을 대량으로 업로드하십시오. 에서 내보낸 제품 카탈로그 데이터를 사용하여 Walmart 템플릿을 채웁니다. [!DNL Commerce] 인스턴스.

새 제품 목록의 경우 제품 카탈로그를 확인하여 Walmart Marketplace에서 판매하려는 제품에 Walmart Marketplace 제품 목록에 필요한 속성이 있는지 확인하십시오.

**Walmart Marketplace 목록 속성 요구 사항**

| **속성** | **요구 사항 수준** |
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

- 다음을 충족하는지 확인합니다. [Walmart 요구 사항](walmart-requirements.md).

- 내 [!DNL Commerce] 제품 카탈로그에서 Walmart Marketplace에 나열할 제품에 대한 카탈로그 구성에 모든 필수 특성이 있는지 확인하고 Walmarketplace 콘텐츠 지침을 충족하는지 확인하십시오.

- 내보내기 작업을 완료하기 위해 cron 작업이 실행 중인지 확인하십시오.

   - 온-프레미스 인스턴스의 경우 [cron 구성 및 실행](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - Adobe 클라우드 인프라의 경우 다음을 참조하십시오. [cron 작업 설정](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### 업로드할 제품 데이터 파일 만들기

1. 출처: [Walmart Seller 계정](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller), Walmart Seller Center에서 제품 목록 템플릿을 다운로드합니다.

   - Product Catalog Items 페이지에서 **[!UICONTROL Add Items]**. 그런 다음 을 선택합니다. **[!UICONTROL Add items in bulk]**.

      ![Walmart Marketplace 항목 구성에서 일괄 옵션 항목 추가](assets/walmart-seller-account-add-items-bulk.png)

   - 다운로드 페이지에서 를 선택합니다. **[!UICONTROL Full Setup]**. 그런 다음 항목 카테고리를 선택하고 카테고리 템플릿을 다운로드합니다.

      ![Walmart Marketplace 항목 구성에서 카테고리 템플릿 옵션 다운로드](assets/walmart-seller-account-full-setup-download.png)

   - 템플릿에 제품 목록에 대한 필수 속성과 권장 속성이 포함되어 있는지 확인합니다.

1. 다음에서 [!DNL Commerce] 책임자는 Adobe에서 내보낼 제품 데이터를 선택합니다 [!DNL Commerce] 사이트.

   - 책임자에서 을(를) 선택합니다. [!UICONTROL **시스템** > 데이터 전송 > **내보내기**].

   - 다음에서 [!UICONTROL Export] 페이지의 [!UICONTROL Entity Type] 필드, 선택 [!UICONTROL **제품**].

   - 다음에서 [!UICONTROL Entity Attributes] 표에서 제품 데이터 내보내기에 대한 선택 기준을 구성합니다.
   ![에서 제품 데이터 내보내기 페이지 [!UICONTROL [!DNL Commerce] Admin]](assets/walmart-seller-account-full-setup-download.png)

   필터를 사용하여 판매하는 제품 범주에 적용되는 속성 값을 선택하고 구성합니다. Walmart의 필수 특성과 권장 특성을 포함해야 합니다. (참조: [데이터 내보내기](https://docs.magento.com/user-guide/system/data-export.html) Adobe 내 [!DNL Commerce] 자세한 지침은 사용 안내서 를 참조하십시오.)

   내보내기에서 속성을 생략하려면 [!UICONTROL **제외**] 행의 시작 부분에 있는 확인란입니다.

1. 속성 테이블의 끝으로 스크롤하여 을 선택합니다. [!UICONTROL **계속**] 데이터 내보내기를 시작합니다.

   CSV 내보내기 파일은 cron 작업을 사용하여 메시지 대기열을 통해 처리되고 `var/export/folder`. (참조: [메시지 대기열 관리](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) 다음에서 *Commerce 개발자 안내서*.)

1. Walmart Marketplace 제품 범주에 대한 Excel 템플릿을 열고 Excel 매크로 기능을 사용하여 내보낸 제품 데이터를 Excel 템플릿에 병합합니다.

1. 내보낸 제품 데이터로 Excel 파일을 업로드합니다.

   - 의 제품 카탈로그 항목 페이지로 돌아갑니다. [월마트 셀러 센터](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - 선택 [!UICONTROL **항목 추가** > **일괄 항목 추가**].
   - 완료된 스프레드시트를 업로드 섹션으로 드래그합니다.
   - 선택 [!UICONTROL **제출**].
   - 다음 항목 선택&#x200B;[!UICONTROL  **활동 피드**] 진행률을 확인합니다.

전체 지침은 [전체 품목 사양을 사용하여 품목을 일괄적으로 추가](https://sellerhelp.walmart.com/s/guide?article=000007680) 다음에서 [!DNL *Walmart Seller 도움말*].
