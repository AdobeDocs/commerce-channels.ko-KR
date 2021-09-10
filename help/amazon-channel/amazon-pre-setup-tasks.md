---
title: 사전 설정 작업
description: Amazon Sales Channel에서 Adobe Commerce 또는 Magento Open Source 스토어를 통합하기 전에 완료해야 하는 필수 작업을 검토하십시오.
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# 사전 설정 작업

[통합 저장](./store-integration.md) 전에 [!DNL Amazon Seller Central] 계정 및 [!DNL Commerce] 계정이 통합 준비가 되었는지 확인해야 합니다. 성공적으로 통합하려면 몇 가지 필수 사전 설정 작업이 있습니다.

Amazon 판매 채널에서 첫 번째 Amazon 저장소를 설정하면 설정 작업 목록이 나타납니다. [Amazon 스토어를 추가](./store-integration.md)하기 전에 이러한 작업을 검토하는 것이 좋습니다. 첫 번째 저장소를 추가한 후 Amazon 판매 채널 [홈 페이지](./amazon-sales-channel-home.md)의 학습 및 준비 보기에서 이러한 작업을 검토할 수 있습니다.

## 1. [!DNL Commerce]에서 백그라운드 작업을 활성화합니다

[!DNL Commerce] 과 Amazon 사이에 동기화된 모든 제품 및 데이터는 [클론 작업](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}에 의해 관리됩니다. 목록 추가 또는 업데이트 및 주문 수신 등의 작업을 완료하면 cron 작업이 [!DNL Commerce] 백엔드와 [!DNL Amazon Seller Central] 계정 간에 데이터를 보내고 받습니다.

- [ [!DNL Commerce] Enablecron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}.

- 최대 성능을 위해 [cron [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;}을 5분마다 한 번 실행되도록 설정합니다.

## 2. [!DNL Amazon Seller Central] 계정을 만듭니다.

Amazon 판매 채널 설정을 시작하려면 먼저 활성 [!DNL Amazon Seller Central] 계정이 있어야 합니다. [북미(미국, CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;} 또는 [유럽(UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;} 영역에 기존 Amazon 판매자 계정이 없는 경우 Amazon의 판매자 계정 설정 프로세스를 완료할 수 있습니다.

Amazon 판매 채널에는 [!DNL Amazon Seller Central]에 [!DNL Professional Seller] 계정이 필요합니다. Amazon은 매월 구독료를 받고 판매료를 받습니다. [Amazon을 참조하십시오. 판매 계획](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}을 선택합니다.

## 3. 승인된 Amazon 판매자인지 확인합니다.

통합하려면 승인된 [!DNL Amazon Seller Central] 계정이 있어야 합니다. 계정에는 제품 또는 카테고리에 대한 제한이 없어야 합니다. 일부 제품 및 카테고리는 목록을 만들기 전에 승인이 필요합니다. 카테고리 및 제품 승인을 위해 Amazon 정책을 검토하여 제품이 승인되었는지 확인합니다. [Amazon을 참조하십시오. 승인](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;}이 필요한 카테고리 및 제품(판매자 중앙 로그인 필요).

또한 [!DNL Amazon Seller Central] 계정에 다음 사항을 구성했는지 확인하는 것이 중요합니다.

- 반환 정책이 Amazon 반환 정책보다 크거나 같은지 확인합니다. [Amazon을 참조하십시오. 반환 정책](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}.

- 세금 설정이 구성되어 있는지 확인합니다. [Amazon을 참조하십시오. 세금 정책](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;}(판매자 중앙 로그인 필수).

- 배송 방법이 정확하게 구성되었는지 확인합니다. Amazon 주문을 수행하기 위해 [!DNL Commerce] 이 고객에게 제공되는 배송 방법을 설정하려면 [Amazon을 업데이트하십시오. [!DNL Amazon Seller Central] 계정의 배송 설정](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;}.

## 4. VAT가 스토어에 맞게 구성되어 있는지 확인합니다

(주로 영국 판매자가 사용합니다.) Amazon은 [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}에 등록할 것을 권장합니다. 다른 방법을 선택하면 VAT 규정 준수에 대한 책임이 있습니다.

>[!NOTE]
>
>Amazon에서 VAT 계산 서비스 계정을 확인하고 활성화하는 데 10~14일이 걸릴 수 있습니다.

## 5. 자동 카탈로그 일치 횟수 증가

온보딩 중에 Amazon 판매 채널은 제품 속성을 사용하여 [!DNL Commerce] 카탈로그의 기존 Amazon 목록(해당되는 경우)과 일치시킵니다. 온보딩 후 이러한 제품 특성은 [!DNL Commerce] 카탈로그 항목을 Amazon 목록에 게시하고 [!DNL Commerce] 와 Amazon 간에 제품 데이터를 동기화하는 데 사용됩니다.

가장 많은 [!DNL Commerce] 제품이 Amazon 목록과 자동으로 일치하도록 하려면 [!DNL Commerce] 카탈로그에 대한 제품 특성 세트를 만들어야 합니다. Amazon 판매 채널 저장소를 설정하기 전에 다음 Amazon 속성과 일치하도록 [!DNL Commerce] 제품 속성을 추가해야 합니다. 예: ASIN, EAN, ISBN, UPC 또는 GCID입니다. [제품 속성 만들기 [!DNL Commerce]](./ob-creating-magento-attributes.md)를 참조하십시오.

## 6. 통화 및 전환을 구성합니다(필요에 따라).

Amazon 저장소가 [!DNL Commerce] 저장소에 대해 구성된 것과 다른 통화를 사용하는 경우 [currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;}를 사용하도록 설정하고 [통화 전환율](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}을 설정하십시오.

## 7. 제품 조건 속성을 만듭니다(필요에 따라).

Amazon 목록에 둘 이상의 제품 조건(예: _new_, _used_ 또는 _new_&#x200B;처럼)이 있는 경우 [!DNL Commerce] 속성을 만들고 조건 값을 지정하십시오. 온보딩 중에 이 속성을 Amazon 조건 제품 속성에 매핑해야 합니다. [Amazon용 속성 만들기](./ob-creating-magento-attributes.md)를 참조하십시오.

## 8. [!DNL Amazon Seller Central] 배송 방법을 구성합니다

Amazon 주문 이행을 위해 제공할 배송 방법을 설정하려면 [!DNL Amazon Seller Central] 계정에서 [설정 및 배송 설정][10] 을 참조하십시오.

## 추가 구성

Amazon 계정이 설정되고 활성화되면 Amazon 판매 채널 온보딩 프로세스를 간소화하는 데 도움이 되는 몇 가지 [!DNL Commerce] 권장 사항이 있습니다.

### 제외할 제품을 검토하고 기록해 둡니다

일부 제품은 Amazon에 나열하지 않을 수 있습니다. Amazon 판매 채널에는 Amazon에 게시할 수 있는 제품을 결정하는 데 사용되는 목록 규칙 엔진이 있습니다. [목록 규칙](./listing-rules.md) 을 사용하면  [!DNL Amazon Seller Central] 카테고리 선택 사항별로 또는 하나 이상의 제품 속성을 정의하여 계정에 게시(또는 게시되지 않음)할 제품 하위 세트를 선택할 수 있습니다. [!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;} 또는 [장바구니](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} 가격 규칙과 마찬가지로 Amazon 목록 자격에 사용되는 제품 특성에는 **[!UICONTROL Use for Promo Rule Conditions]**&#x200B;가 `Yes`로 설정되어 있어야 합니다. [제품 속성](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}에서 **[!UICONTROL Use for Promo Rule Conditions]**&#x200B;을 참조하십시오.

### [!DNL Amazon Seller Central] 영역을 비활성 상태로 설정합니다.

통합 중에 오류가 없는 데이터 전환을 쉽게 할 수 있도록 설정 > 계정 정보 > 휴가 설정에서 Amazon 지역을 `Inactive` 상태로 설정하는 것이 좋습니다. [Amazon 를 참조하십시오. 휴가 상태 나열][11]. 설치가 완료되면 상태를 다시 Amazon의 `Active`으로 변경합니다.

![다음 ](assets/btn-next.png) [**아이콘속성 생성을  [!DNL Commerce] 계속합니다**](./ob-creating-magento-attributes.md)
