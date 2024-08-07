---
title: ' [!DNL Amazon sales channel]에 대한 모범 사례 및 제한 사항'
description: Adobe Commerce 및 Magento Open Source용 Amazon 판매 채널을 사용할 때의 모범 사례와 제한 사항을 검토하십시오.
role: Leader, Admin, User
feature: Sales Channels, Best Practices
exl-id: 7f7faae1-7aa7-413c-b534-1039e6a35173
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# [!DNL Amazon sales channel]에 대한 모범 사례 및 제한 사항

모범 사례는 다음과 같습니다.

- Amazon 판매 채널은 가격 인상 또는 인하, 제품 정보 동기화(사용 가능한 재고 포함), 목록 추가, 업데이트 및 종료(삭제)를 통해 Amazon 목록에 영향을 줄 수 있습니다. 설정 중 상태별로 목록을 검토하고 설정([설정 나열](./listing-settings.md), [규칙 나열](./listing-rules.md), [가격 규칙](./pricing-products.md), [재정의](./overrides.md) 등)을 조정한 후 스토어 설정을 완료합니다. 이러한 설정은 필요에 따라 설정 후 수정할 수도 있습니다.

- Amazon 판매 채널은 목록 가격을 자동으로 조정하도록 가격책정 규칙을 설정할 수 있습니다. 자동 가격 보호 장치에는 [지능형 가격 조정 규칙](./intelligent-repricing-rules.md)의 [최저 가격](./floor-price.md) 및 [선택적 최고 가격](./optional-ceiling-price.md) 기능이 포함됩니다. 이러한 안전 장치를 사용하면 목록 가격이 비용 또는 정의된 가격 이상으로 내려가지 않도록 할 수 있습니다.

- Amazon 판매 채널과 Amazon 간의 데이터 동기화는 [[!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html) 설정에 의해 제어됩니다. [!DNL Commerce]과(와) Amazon 간의 기본 제공 조절은 원활하고 효율적인 데이터 전송을 돕는 데 도움이 되지만, 전자 상거래 트래픽 시간(예: 블랙 프라이데이) 동안 Amazon의 시스템을 업데이트하는 데 평소보다 더 오래 걸릴 수 있습니다. [!DNL Commerce] 크론이 5분마다 한 번 실행되도록 설정하십시오.

- Amazon sales channel 은 Amazon 주문 정보를 가져옵니다. Amazon 판매 채널에서 Amazon 주문을 관리하려면 각 Amazon 주문에 대해 해당 [!DNL Commerce] 주문을 가져오고 만들기 위해 [주문 설정](./order-settings.md)이 정의되어 있는지 확인해야 합니다. 정의되지 않은 경우 Amazon 주문 정보만 볼 수 있습니다. Amazon을 통한 판매에 대한 모든 세금은 여전히 [!DNL Amazon Seller Central] 계정을 통해 관리하고 송금됩니다. 일부 주에서는 Amazon에서 세금을 자동으로 징수하여 송금하도록 규정하고 있다. 다른 주의 경우 판매자는 수동으로 세금을 계산하거나 자동으로 세금을 계산할 수 있는 옵션이 있습니다. [Amazon: 세금 정책](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=200405820&amp;language=en_US/){target="_blank"}을 참조하세요. Amazon 세금 정책 설명서를 보려면 [!DNL Amazon Seller Central] 계정에 로그인해야 할 수 있습니다.

- 영국 지역의 경우 Amazon 판매 채널을 온보딩하기 전에 [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources/){target="_blank"}에 등록하는 것이 좋습니다.

  >[!NOTE]
  >
  >Amazon에서 VAT 계산 서비스 계정을 확인하고 활성화하는 데 10~14일이 걸릴 수 있습니다.

제한 사항은 다음과 같습니다.

- [!DNL Commerce] 카탈로그에 포함된 번들, 기프트 카드 및 그룹화된 제품 유형은 Amazon 판매 채널에서 Amazon에 나열할 수 없습니다.

- Amazon 판매 채널은 기존 또는 이전 Amazon 목록이 없는 제품에 대한 목록을 만들 수 없습니다. ASIN이 있는 [!DNL Amazon Seller Central]에 제품이 없는 경우 Amazon에서 제품에 ASIN을 할당할 수 있도록 [!DNL Amazon Seller Central]에 제품을 추가해야 합니다. Amazon에 제품이 추가되고 목록이 생성되면 해당 목록은 Amazon 판매 채널의 카탈로그와 일치하고 동기화할 수 있습니다.
