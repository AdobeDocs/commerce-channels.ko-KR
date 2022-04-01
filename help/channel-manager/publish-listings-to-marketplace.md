---
title: Walmart에 목록 게시
description: 판매를 시작하려면 Walmart Marketplace에 상거래 제품 목록을 게시하십시오.
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: a10ab3f7fa7049e48d83a942f6c5441d8147b12c
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Walmart에 목록 게시

다른 시장들과 마찬가지로, 월마트는 서드파티 판매자들이 다른 사람들이 파는 품목들을 나열하도록 허락한다.

플랫폼은 UPC 및 GTIN과 같은 제품 식별자를 사용하여 이미 판매 중인 항목을 일치시킵니다.
일치하는 제품의 경우 기존 Walmart Marketplace에서 Commerce 제품 오퍼를 포함하도록 업데이트를 나열합니다.

가격이 가장 낮은 제품이 우선 결과에 나오지만 평가 등 다른 요소들도 배치에 영향을 미친다.

## 제품 일치

제품에 일치하면 Channel Manager는 제품 데이터를 Walmart Marketplace에 보내 매핑된 Commerce 제품 속성과 일치하는 속성 값으로 기존 목록을 검색합니다. 일치 기준은 [속성 매핑 구성](map-product-attributes-for-matching.md) 저장소 채널에 사용할 수 있습니다.

일치하는 항목이 있으면 기존 제품 목록이 업데이트되어 오퍼를 추가합니다.

### 전제 조건

제품에 일치하기 전에 제품 카탈로그 속성 값이 Mart 요구 사항을 충족하는지 확인하고 속성 설정을 구성합니다. 자세한 내용은 [제품 일치 구성](map-product-attributes-for-matching.md)

#### 제품 선택 및 일치

1. 연결된 영업 채널을 엽니다.

1. From **[!UICONTROL Listings]**&#x200B;에 일치하는 제품을 선택합니다. *[!UICONTROL Draft]* 상태.

   ![목록에서 제품을 선택하고 일치하는 항목을 보내기](assets/products-in-marketplace-sales-channel.png)

1. 선택 **[!UICONTROL Match Products]**.

   메시지를 통해 일치를 위해 전송된 제품 수를 나타냅니다.

   ![연결된 영업 채널로 제품 전송](assets/products-submit-for-matching.png)

   선택한 제품의 상태가 [!UICONTROL *처리 중*] 일치 작업이 완료될 때까지. Walmart Marketplace에서 일치 작업을 완료하는 데 최대 30분이 걸릴 수 있습니다.

### 일치 상태 확인

1. 선택 **제품 새로 고침** 최신 제품 상태를 업데이트하려면

1. 제품 상태를 확인합니다.

   일치가 완료되면 상태를 확인할 수 있습니다 *일치* 또는 *오류*.

   * **[!UICONTROL Match]** 제품이 일치했음을 나타냅니다. 제품 오퍼가 기존 Walmart Marketplace 목록에 게시되었습니다.

   * **[!UICONTROL Error]** 다음 중 하나를 나타냅니다.

      * 오류가 발생하여 일치 작업이 실패했습니다.

      * 일치하는 항목이 없습니다.

      * 일치하는 항목이 있지만 [마켓플레이스 저장소가 활성 상태가 아닙니다.](walmart-prerequisites.md#walmart-marketplace-store-status).

### 월마트 목록 확인

일치하는 제품을 찾은 후 업데이트된 제품 목록을 검토하고 제품 세부 사항, 가격 및 재고 수량을 [[!UICONTROL Walmart Marketplace Seller Account Items] 대시보드](https://seller.walmart.com/items-and-inventory/manage-items) 를 클릭하여 업데이트된 제품을 검토합니다.

### 제품 일치 오류 문제 해결

제품 일치 작업이 실패하면 Walmart Marketplace에서 오류 코드를 반환하고 Channel Manager가 제품 목록 정보에 오류 상태를 표시합니다.

마우스로 를 가리키면 오류 메시지 세부 정보를 볼 수 있습니다. **오류** 상태 레이블입니다. 반환된 일반적인 오류는 올바른 형식의 제품 ID 값이나 필수 속성이 누락되었습니다.

#### 제품 ID 값 수정

| 유형 | 설명 | 예 |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12, 12자리 숫자(확인 자리 포함). </br></br>UPC의 자릿수가 8자리인 UPC-E와 같이 12자리 미만이면 요구 사항을 충족하기 위해 종료 0을 추가합니다. | 변경 대상 `45678912345` to `045678912345` |
| GTIN | GTIN-14, 14자리 숫자(확인 숫자 포함). </br></br>GTIN에 14자리 미만의 숫자가 있는 경우 앞에 0을 추가합니다 </br>요구 사항을 충족하기 위해 | 변경 `456789123456` to `0045678912345` |
| EAN | GTIN-13, 13자리 숫자(확인 숫자 포함). </br></br>EAN에 13자리 미만의 숫자가 있는 경우 선행 값을 추가합니다 </br>요구 사항을 충족하기 위해 0을 사용합니다. | 변경 대상 `4567891234` to `0004567891234` |

Walmart Marketplace 오류 코드에 대한 자세한 내용은 [Walmart Seller 도움말](https://sellerhelp.walmart.com/s/guide?article=000005844).

## 새 제품 목록 업로드

Walmart Marketplace와 일치하지 않는 제품의 경우 Walmart 제품 카테고리 Excel 템플릿을 사용하여 제품 목록을 벌크로 업로드하십시오. Commerce 인스턴스에서 내보낸 제품 카탈로그 데이터를 사용하여 Walmart 템플릿을 채웁니다.

새 제품 목록을 보려면 제품 카탈로그를 확인하여 Walmart Marketplace에서 판매하려는 제품에 Walmart Marketplace 제품 목록에 필요한 특성이 있는지 확인하십시오.

**Walmart Marketplace 목록 속성 요구 사항**

| **속성** | **요구 사항 수준** |
|--------------------------|-----------------------|
| SKU | 필수 여부 |
| 제품 이름 | 필수 여부 |
| 제품 ID 유형 | 필수 여부 |
| 제품 ID | 필수 여부 |
| 브랜드 | 필수 여부 |
| 간단한 설명 | 필수 여부 |
| 판매 가격 | 필수 여부 |
| 사이트 설명 | 필수 여부 |
| 기본 이미지 URL | 필수 여부 |
| 배송 중량 | 필수 여부 |
| 주요 기능 | 권장 |
| 모델 번호 | 권장 |
| 제조업체 이름 | 권장 |
| 제조업체 부품 번호 | 권장 |
| 크기 | 권장 |
| 색상 | 권장 |
| 기본 이미지 URL | 선택 사항입니다 |
| 추가 이미지 URL | 선택 사항입니다 |
| 제조업체 | 선택 사항입니다 |

### 전제 조건

* 을(를) 충족하는지 확인합니다. [월마트의 사전 요구 사항](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.k2lo9voad1gx).

* Commerce 제품 카탈로그에서 Walmart Marketplace에 나열된 제품에 대한 카탈로그 구성에 모든 필수 특성이 있으며 Walmart Marketplace 콘텐츠 지침을 충족하는지 확인합니다.

* 내보내기 작업을 완료하기 위해 크론 작업이 실행 중인지 확인합니다.

   * 온-프레미스 인스턴스에 대해서는 [크론 구성 및 실행](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   * Adobe 클라우드 인프라의 경우 다음을 참조하십시오 [크론 작업 설정](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### 업로드할 제품 데이터 파일 만들기

1. 사용 [월마트 판매자 계정](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)Walmart Seller Center에서 제품 목록 템플릿을 다운로드합니다.

   * 제품 카탈로그 항목 페이지에서 **[!UICONTROL Add Items]**. 그런 다음 **[!UICONTROL Add items in bulk]**.

      ![Walmart Marketplace 항목 구성에서 일괄 옵션에서 항목 추가](assets/walmart-seller-account-add-items-bulk.png)

   * 다운로드 페이지에서 를 선택합니다 **[!UICONTROL Full Setup]**. 그런 다음 항목 카테고리를 선택하고 카테고리 템플릿을 다운로드합니다.

      ![Walmart Marketplace 항목 구성에서 카테고리 템플릿 옵션 다운로드](assets/walmart-seller-account-full-setup-download.png)

   * 템플릿에 제품 목록에 필요한 및 권장 속성이 포함되어 있는지 확인합니다.

1. 에서 [!DNL Commerce] 관리자는 Adobe Commerce 사이트에서 내보낼 제품 데이터를 선택합니다.

   * 관리자에서 을(를) 선택합니다. [!UICONTROL **시스템** > 데이터 전송 > **내보내기**].

   * 설정 [!UICONTROL Export] 페이지의 [!UICONTROL Entity Type] 필드, 선택 [!UICONTROL **제품**].

   * 에서 [!UICONTROL Entity Attributes] 테이블에서 제품 데이터 내보내기에 대한 선택 기준을 구성합니다.
   ![에서 제품 데이터 페이지 내보내기 [!UICONTROL Commerce Admin]](assets/walmart-seller-account-full-setup-download.png)

   필터를 사용하여 판매하는 제품 카테고리에 적용되는 속성 값을 선택하고 구성합니다. Walmart의 필수 및 권장 속성을 포함해야 합니다( [데이터 내보내기](https://docs.magento.com/user-guide/system/data-export.html) ( Adobe Commerce 사용 안내서에서)를 참조하십시오.

   내보내기에서 속성을 생략하려면 [!UICONTROL **제외**] 행의 시작 부분에 있는 확인란.

1. 속성 테이블의 끝으로 스크롤하여 [!UICONTROL **계속**] 데이터 내보내기를 시작하려면 다음을 수행하십시오.

   CSV 내보내기 파일은 cron 작업을 사용하여 메시지 큐를 통해 처리되고 `var/export/folder`. (자세한 내용은 [메시지 큐 관리](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) 에서 *Commerce Developer 안내서*)

1. Walmart Marketplace 제품 범주에 대한 Excel 템플릿을 열고 Excel 매크로 기능을 사용하여 내보낸 제품 데이터를 Excel 템플릿에 병합합니다.

1. 내보낸 제품 데이터로 Excel 파일을 업로드합니다.

   * 의 제품 카탈로그 항목 페이지로 돌아갑니다. [월마트 판매자 센터](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   * 선택 [!UICONTROL **항목 추가** > **항목을 벌크로 추가**].
   * 완료된 스프레드시트를 업로드 섹션으로 드래그합니다.
   * 선택 [!UICONTROL **제출**].
   * 을(를) 선택합니다&#x200B;[!UICONTROL  **활동 피드**] 진행 상태를 보려면 다음을 수행하십시오.

전체 지침은 [전체 품목 사양을 사용하여 일괄 항목 추가](https://sellerhelp.walmart.com/s/guide?article=000007680) 에서 [!DNL *Walmart Seller 도움말*].
