---
title: Amazon Marketplace 정보
description: 제품 카탈로그를 Amazon Marketplace의 목록으로 활용하여 Adobe Commerce 또는 Magento Open Source 스토어의 범위를 확장합니다.
exl-id: d4943d40-773e-4635-aca4-ae40f8ada7bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# 정보 [!DNL Amazon Marketplace]

[[!DNL Amazon Marketplace]](https://sell.amazon.com/){target="_blank"} Amazon이 소유 및 운영하는 전자상거래 플랫폼으로 서드파티 판매자가 신규 또는 중고 상품을 판매할 수 있다. 사용 [!DNL Amazon Marketplace], 서드파티 판매자는 Amazon의 전 세계 고객 기반을 액세스할 수 있습니다. Adobe Commerce 또는 Magento Open Source 사용자를 포함하여 Amazon에 판매용 제품을 나열하는 판매자는 Amazon에서 &quot;서드파티 판매자&quot;로 정의됩니다.

규모에 관계없이 서드파티 판매자는 [!DNL Amazon Seller Central] 계정 및 사용 [!DNL Amazon Marketplace] Amazon의 글로벌 고객 기반에 도달하기 위해. 계정이 만들어지고 활성화된 후 판매자는 판매용 제품을 추가 및 나열하고 주문 및 재고를 관리하며 주문을 이행할 수 있습니다.

## Amazon 목록

Amazon 목록에는 두 가지 범주의 정보가 포함되어 있습니다. **제품 정보** 및 **목록 정보**.

### 제품 정보

제품 정보는 Amazon에 나열된 동일한 제품의 모든 인스턴스에 공통되는 데이터를 제공합니다. 예를 들어, 여러 판매자가 Amazon에 특정 브랜드의 요가 바지를 나열할 수 있습니다. 제품 이름, 모델 번호 등 제품에 대한 일반적인 세부 사항은 제품을 나열할 때마다 동일합니다. 두 명 이상의 판매자가 제품에 데이터를 기여하면 Amazon은 제품 세부 사항 페이지에 표시되는 판매자의 제품 정보를 결정합니다.

### 목록 정보

목록 정보는 제품에 대한 판매자별 정보를 제공합니다. 이러한 세부 내용은 동일한 상품에 대한 다른 판매자의 상장과 다른 경우가 많다. 예를 들어 다른 판매자와 동일한 요가 바지를 판매할 수도 있지만, 상품 번호, 상태, 가격, 배송 방법/시간 등이 다를 수 있습니다. 이러한 세부 사항은 제품 목록에 고유합니다.

제품 정보를 제공하거나 제품 세부 사항 페이지의 잘못된 정보를 수정하려는 경우 [Amazon: 제품 세부 사항](https://sellercentral.amazon.com/gp/help/external/200335450){target="_blank"}.

## Amazon 이행

Amazon은 주문 이행 및 배송에 대한 두 가지 옵션을 제공합니다.

- **판매자가 이행함(FBM)**: 서드파티 판매자가 자체 인벤토리를 저장합니다. 고객이 주문하면 판매자가 고객에게 포장과 배송을 처리한다. 이 옵션을 사용하면 Adobe Commerce 및 Magento Open Source 또는 다른 서드파티를 통해 납품을 완료할 수 있습니다.

- **Amazon(FBA)에서 이행**: 서드파티 판매자는 전 세계 Amazon의 이행 센터에 재고를 저장합니다. 고객이 주문하면 Amazon이 포장부터 배송까지 모두 처리한다. 주문 세부 사항 및 상태가 Adobe Commerce 또는 Magento Open Source으로 전송됩니다.

다음 [!DNL Amazon Sales Channel] 확장은 이러한 주문 수신 및 추적 옵션을 모두 지원합니다. 이행을 완료하면 주문 상태가 자동으로 업데이트됩니다. 다음을 참조하십시오 [Fulfillment 워크플로](./fulfillment-workflows.md).

## Amazon에서 판매 전

Amazon은 모든 판매자와 제품이 지정된 지침을 준수하도록 일련의 정책 및 워크플로를 따릅니다. 제품 및 계정이 승인되고 목록에 추가될 수 있는지 확인하려면 다음 Amazon 정보 및 정책을 검토해야 합니다.

- [Amazon 판매자를 위한 도움말](https://sellercentral.amazon.com/gp/help/external/help-page.html?itemID=2&amp;language=en_US/){target="_blank"}
- [배송 정책](https://sellercentral.amazon.com/gp/help/external/201901620?language=en-US){target="_blank"}
- [프로그램 정책](https://sellercentral.amazon.com/gp/help/external/521?language=en-US){target="_blank"}
- [영업 정책 및 행동 수칙](https://sellercentral.amazon.com/gp/help/external/1801?language=en-US){target="_blank"}
- [Amazon에서 갱신한(재생됨, 사전 소유 및 오픈 박스) 제품 목록](https://sell.amazon.com/programs/renewed){target="_blank"}
