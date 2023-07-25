---
title: 사전 설정 작업 [!DNL Amazon sales channel]
description: Amazon Sales Channel에서 Adobe Commerce 또는 Magento Open Source 저장소를 통합하기 전에 완료해야 하는 필수 작업을 검토하십시오.
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# 사전 설정 작업 [!DNL Amazon sales channel]

다음 이전 [스토어 통합](./store-integration.md), 다음을 확인해야 합니다. [!DNL Amazon Seller Central] 계정 및 사용자 [!DNL Commerce] 계정을 통합할 준비가 되었습니다. 를 성공적으로 통합하려면 몇 가지 필수 사전 설정 작업이 있습니다.

Amazon 판매 채널에서 첫 번째 Amazon 스토어를 설정하면 설정 작업 목록이 나타납니다. 다음 작업을 검토하는 것이 좋습니다. [Amazon 스토어 추가](./store-integration.md). 첫 번째 스토어를 추가한 후 Amazon 판매 채널의 학습 및 준비 보기에서 이러한 작업을 검토할 수 있습니다 [홈 페이지](./amazon-sales-channel-home.md).

## 1. 백그라운드 작업 활성화 [!DNL Commerce]

모든 제품 및 데이터 동기화 대상 [!DNL Commerce] 및 Amazon은 [cron job](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). 목록 추가 또는 업데이트와 같은 작업을 완료하고 주문을 받으면 cron 작업이 [!DNL Commerce] 백엔드 및 사용자 [!DNL Amazon Seller Central] 계정입니다.

- [사용 [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- 성능을 최대화하려면 [set [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) 5분마다 한 번씩 실행합니다.

## 2. 다음을 만듭니다. [!DNL Amazon Seller Central] account

Amazon 판매 채널 설정을 시작하려면 먼저 활성 상태가 있어야 합니다 [!DNL Amazon Seller Central] 계정입니다. 에 기존 Amazon 판매자 계정이 없는 경우 [북미 (US, CA, MX)](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} 지역에서는 Amazon의 판매자 계정 설정 프로세스를 완료할 수 있습니다.

Amazon 판매 채널에는 [!DNL Professional Seller] 다음에 대한 계정 [!DNL Amazon Seller Central]. Amazon은 월 구독료와 판매 수수료를 부과합니다. 다음을 참조하십시오 [Amazon: 판매 계획 선택](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3. 승인된 Amazon 판매자인지 확인합니다

통합하려면 승인된 가 있어야 합니다. [!DNL Amazon Seller Central] 계정입니다. 계정에는 제품 또는 범주에 대한 제한이 없어야 합니다. 일부 제품 및 범주는 목록을 만들기 전에 승인이 필요합니다. 범주 및 제품 승인에 대한 Amazon 정책을 검토하여 제품이 승인되었는지 확인합니다. 다음을 참조하십시오 [Amazon: 승인이 필요한 카테고리 및 제품](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} (판매자 Central 로그인 필요).

에서 다음을 구성했는지 확인하는 것도 중요합니다 [!DNL Amazon Seller Central] 계정:

- 반품 정책이 Amazon 반품 정책보다 우수하거나 우수한지 확인합니다. 다음을 참조하십시오 [Amazon: 반환 정책](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- 세금 설정이 구성되었는지 확인합니다. 다음을 참조하십시오 [Amazon: 세금 정책](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} (판매자 Central 로그인 필요).

- 배송 방법이 정확하게 구성되었는지 확인하십시오. 다음과 같은 운송 방법을 설정하려면 [!DNL Commerce] 은(는) 고객에게 Amazon 주문을 이행하고 [Amazon: 배송 설정](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} (으)로 [!DNL Amazon Seller Central] 계정입니다.

## 4. 상점에 대해 VAT가 구성되어 있는지 확인합니다

(주로 영국 판매자가 사용합니다.) Amazon은 다음에 등록할 것을 권장합니다. [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. 다른 방식을 택할 경우 부가가치세 준수에 대한 책임이 귀하에게 있다.

>[!NOTE]
>
>Amazon에서 VAT 계산 서비스 계정을 확인하고 활성화하는 데 10~14일이 걸릴 수 있습니다.

## 5. 자동 카탈로그 일치 수 늘리기

온보딩 중에 Amazon 판매 채널은 제품 속성을 사용하여 기존 Amazon 목록(해당하는 경우)을 의 기존 제품에 일치시킵니다. [!DNL Commerce] 카탈로그. 온보딩 후 이러한 제품 속성을 사용하여 [!DNL Commerce] 카탈로그 항목을 Amazon 목록에 추가하고 제품 데이터를 [!DNL Commerce] 그리고 Amazon.

의 수가 가장 많음 [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하면 다음에 대한 제품 속성 세트를 만들어야 합니다. [!DNL Commerce] 카탈로그. Amazon 판매 채널 스토어를 설정하기 전에 [!DNL Commerce] 이러한 Amazon 속성과 일치하는 제품 속성(예: ASIN, EAN, ISBN, UPC 또는 GCID). 다음을 참조하십시오 [에서 제품 속성 만들기 [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6. 통화 및 전환 구성(필요한 경우)

Amazon 스토어에서 를 위해 구성된 것과 다른 통화를 사용하는 경우 [!DNL Commerce] 저장, [통화 활성화](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) 및 설정 [통화 전환율](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7. 제품 조건 속성 만들기(필요한 경우)

Amazon 목록에 둘 이상의 제품 조건이 포함된 경우(예: _신규_, _사용됨_, 또는 _새것처럼_), 다음을 생성합니다. [!DNL Commerce] 속성을 지정하고 조건 값을 할당합니다. 온보딩 중에 이 속성을 Amazon 조건 제품 속성에 매핑해야 합니다. 다음을 참조하십시오 [Amazon에 대한 속성 만들기](./ob-creating-magento-attributes.md).

## 8. 구성 [!DNL Amazon Seller Central] 배송 방법

Amazon 주문 이행을 위해 제공하려는 배송 방법을 설정하려면 다음을 참조하십시오. _설정 및 배송 설정_ (으)로 [!DNL Amazon Seller Central] 계정입니다.

## 추가 구성

Amazon 계정이 설정되고 활성화되면 몇 가지 옵션이 있습니다 [!DNL Commerce] Amazon 판매 채널 온보딩 프로세스를 간소화하는 데 도움이 되는 권장 사항입니다.

### 제외하려는 제품을 검토하고 기록합니다

일부 제품이 Amazon에 나열되지 않도록 할 수 있습니다. Amazon sales channel 에는 Amazon에 게시할 수 있는 제품을 결정하는 데 사용되는 목록 규칙 엔진이 있습니다. [규칙 나열](./listing-rules.md) 에 게시(또는 게시 안 함)할 제품 하위 집합을 선택할 수 있습니다. [!DNL Amazon Seller Central] 범주 선택 또는 하나 이상의 제품 속성 정의와 같은 계정. 좋아요 [!DNL Commerce] [카탈로그](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) 또는 [장바구니](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) Amazon 목록 적격성에 사용되는 가격 규칙, 제품 속성은 다음을 포함해야 합니다. **[!UICONTROL Use for Promo Rule Conditions]** 을 로 설정 `Yes`. 다음을 참조하십시오. **[!UICONTROL Use for Promo Rule Conditions]** 위치: [제품 속성](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### 설정 [!DNL Amazon Seller Central] 비활성 지역

통합 중에 오류 없는 데이터 전환을 용이하게 하려면 Amazon 영역을 로 설정하는 것이 좋습니다. `Inactive` 설정 > 계정 정보 > 휴가 설정의 상태. 설정이 완료되면 상태를 다시 다음으로 변경 `Active` Amazon.

![다음 아이콘](assets/btn-next.png) [**계속 만들기 [!DNL Commerce] 속성**](./ob-creating-magento-attributes.md)
