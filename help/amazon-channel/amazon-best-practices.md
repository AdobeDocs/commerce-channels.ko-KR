---
title: Amazon 영업 채널의 우수 사례 및 제한 사항
description: Adobe 상거래 및 Magento Open Source에 Amazon 판매 채널을 사용할 때 모범 사례 및 제한 사항을 검토하십시오.
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Amazon 판매 채널의 우수 사례 및 제한 사항

우수 사례는 다음과 같습니다.

- Amazon 판매 채널은 가격을 올리거나 내리고, 제품 정보(가용 재고 포함)를 동기화하고, 목록을 추가, 업데이트 및 종료(삭제)하여 Amazon 목록에 영향을 줄 수 있습니다. 설정 중에 상태별로 목록을 검토하고 설정([목록 설정](./listing-settings.md), [목록 규칙](./listing-rules.md), [가격 규칙](./pricing-products.md), [overrides](./overrides.md) 등)을 조정한 후 저장소 설정을 완료합니다. 이러한 설정은 설정 후 필요에 따라 수정할 수도 있습니다.

- Amazon 판매 채널에서는 가격 규칙을 설정하여 목록 가격을 자동으로 조정할 수 있습니다. 자동 가격 보호 기능에는 [가격](./floor-price.md) 및 [선택적 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)이 포함됩니다. ](./optional-ceiling-price.md) 이러한 안전장치를 사용하면 목록 가격이 사용자의 비용 또는 정의된 가격 이상으로 상승하지 않도록 할 수 있습니다.

- Amazon 판매 채널과 Amazon 간의 데이터 동기화는 [[!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;} 설정에 의해 제어됩니다. 기본 제공 [!DNL Commerce] 과 Amazon 간의 전송률 조절 기능을 사용하면 매끄럽고 효율적인 데이터 전송을 보장하지만 높은 eCommerce 트래픽 시간(예: 블랙 프라이데이) 동안 Amazon의 시스템을 업데이트하는 데 평소보다 시간이 오래 걸릴 수 있습니다. 5분마다 한 번씩 실행되도록 [!DNL Commerce] 크론을 설정합니다.

- Amazon 판매 채널에서 Amazon 주문 정보를 가져옵니다. Amazon 판매 채널에서 Amazon 주문을 관리하려면, 각 Amazon 주문에 대해 해당 [주문 설정](./order-settings.md)이(가) 정의되어 있는지 확인해야 합니다. [!DNL Commerce] 정의되지 않은 경우 Amazon 주문 정보만 볼 수 있습니다. Amazon을 통한 판매에 대한 모든 세금은 여전히 [!DNL Amazon Seller Central] 계정을 통해 관리 및 수탁됩니다. 일부 주에서는 Amazon이 세금을 자동으로 징수하고 송금해야 합니다. 다른 주에서는, 판매자는 수동으로 또는 자동으로 세금을 계산할 수 있다. [Amazon을 참조하십시오. 세금 정책](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target=&quot;_blank&quot;}. Amazon 세금 정책 설명서를 보려면 [!DNL Amazon Seller Central] 계정에 로그인해야 할 수 있습니다.

- 영국 지역의 경우 Amazon 판매 채널에 온보딩하기 전에 [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources/){target=&quot;_blank&quot;}에 등록하는 것이 좋습니다.


   >[!NOTE]
   >
   >Amazon에서 VAT 계산 서비스 계정을 확인하고 활성화하는 데 10~14일이 걸릴 수 있습니다.

제한 사항은 다음과 같습니다.

- [!DNL Commerce] 카탈로그의 일부인 번들, 기프트 카드 및 그룹화된 제품 유형은 Amazon에 나열하기 위해 Amazon 판매 채널에서 지원하지 않습니다.

- Amazon 판매 채널에서는 기존 또는 이전 Amazon 목록이 없는 제품에 대한 목록을 만들 수 없습니다. ASIN이 있는 [!DNL Amazon Seller Central]에 제품이 없는 경우, Amazon이 제품에 ASIN을 할당할 수 있도록 [!DNL Amazon Seller Central]에 추가해야 합니다. 제품이 Amazon에 추가되고 목록이 만들어지면 해당 목록이 Amazon 판매 채널의 카탈로그와 일치하고 동기화할 수 있습니다.
