---
title: Amazon Marketplace에 대하여
description: Amazon Marketplace에서 제품 카탈로그를 목록으로 활용하여 Adobe 상거래 또는 Magento Open Source 스토어의 범위를 확장합니다.
exl-id: d4943d40-773e-4635-aca4-ae40f8ada7bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# [!DNL Amazon Marketplace] 정보

[[!DNL Amazon Marketplace]](https://sell.amazon.com/){target=&quot;_blank&quot;}은 타사 판매자가 신규 또는 사용된 제품을 판매할 수 있도록 Amazon이 소유하고 운영하는 전자 상거래 플랫폼입니다. 타사 판매자는 [!DNL Amazon Marketplace]을 사용하여 Amazon의 전 세계 고객 기반에 액세스할 수 있습니다. Adobe Commerce 또는 Magento Open Source 사용자를 포함하여 Amazon에 판매할 제품을 나열하는 상인은 Amazon에서 &quot;타사 판매자&quot;로 정의됩니다.

모든 크기의 타사 판매자는 [!DNL Amazon Seller Central] 계정을 만들고 [!DNL Amazon Marketplace] 을 사용하여 Amazon의 글로벌 고객 기반에 연결할 수 있습니다. 계정이 생성되어 활성화되면 판매자는 판매 제품을 추가 및 나열하고 주문과 재고를 관리하고 주문을 이행할 수 있습니다.

## Amazon 목록

Amazon 목록에는 다음 두 가지 정보 카테고리가 있습니다. **제품 정보** 및 **정보**&#x200B;나열

### 제품 정보

제품 정보는 Amazon에 나열된 동일한 제품의 모든 인스턴스에 공통되는 데이터를 제공합니다. 예를 들어, 몇몇 판매자들은 Amazon에 특정 브랜드의 요가 바지를 나열할 수 있습니다. 이름 및 모델 번호와 같은 제품에 대한 일반 세부 사항은 제품이 나열될 때마다 동일합니다. 두 명 이상의 판매자가 제품에 데이터를 기여할 때 Amazon에서 제품 세부 사항 페이지에 표시되는 판매자의 제품 정보를 결정합니다.

### 목록 정보

목록 정보는 제품에 대한 판매자별 정보를 제공합니다. 이러한 세부 사항은 같은 제품에 대한 다른 판매자의 목록과 종종 다릅니다. 예를 들어 다른 판매자와 동일한 요가 바지를 판매할 수 있지만 품목 번호, 조건, 가격 또는 배송 방법/시간이 다를 수 있습니다. 이러한 세부 사항은 제품 목록에 고유합니다.

제품 정보를 제공하거나 제품 세부 사항 페이지에서 잘못된 정보를 수정하려면 [Amazon을 참조하십시오. 제품 세부 정보](https://sellercentral.amazon.com/gp/help/external/200335450){target=&quot;_blank&quot;}.

## Amazon 이행

Amazon은 주문 이행 및 배송을 위한 두 가지 옵션을 제공합니다.

- **머천트(FBM)에 의해 처리됨**: 서드파티 판매자들은 자신의 재고를 저장합니다. 고객이 주문을 하면 판매자가 포장과 배송을 고객에게 처리합니다. 이 옵션을 사용하면 Adobe 상거래 및 Magento Open Source 또는 다른 타사를 통해 납품을 완료할 수 있습니다.

- **Amazon(FBA)에 의해 처리됨**: 타사 판매자는 전 세계 Amazon의 이행 센터에 재고를 저장합니다. 고객이 주문을 하면 Amazon에서 고객에게 포장 및 배송을 처리합니다. 주문 세부 사항 및 상태가 Adobe 상거래 또는 Magento Open Source으로 전송됩니다.

[!DNL Amazon Sales Channel] 확장은 이러한 주문을 받고 추적하는 두 옵션을 모두 지원합니다. 완료를 완료하면 주문 상태가 자동으로 업데이트됩니다. [이행 워크플로우](./fulfillment-workflows.md)를 참조하십시오.

## Amazon에서 판매 전

Amazon은 모든 판매자와 제품이 지정된 지침을 준수하도록 하기 위해 일련의 정책 및 워크플로우를 따릅니다. 제품 및 계정이 승인되고 목록에 포함될 수 있도록 하려면 다음 Amazon 정보 및 정책을 검토해야 합니다.

- [Amazon 판매자에 대한 도움말](https://sellercentral.amazon.com/gp/help/external/help-page.html?itemID=2&amp;language=en_US/){target=&quot;_blank&quot;}
- [배송 정책](https://sellercentral.amazon.com/gp/help/external/201901620?language=en-US){target=&quot;_blank&quot;}
- [프로그램 정책](https://sellercentral.amazon.com/gp/help/external/521?language=en-US){target=&quot;_blank&quot;}
- [영업 정책 및 행동](https://sellercentral.amazon.com/gp/help/external/1801?language=en-US) 수칙{target=&quot;_blank&quot;}
- [Amazon](https://sell.amazon.com/programs/renewed){target=&quot;_blank&quot;}에서 갱신된(재생된, 사전 소유 및 오픈 박스) 제품 나열
