---
title: 가격 범위
description: 상거래 가격 범위를 사용하여 여러 웹 사이트 또는 전 세계에 따른 가격을 관리합니다.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 가격 범위

[!DNL Commerce] 또는 로  [설정할 가격 범위에 대한 구성](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} `Global` 을  `Website`제공합니다. 가격을 `Global`으로 설정하면 모든 웹 사이트에 대해 단일 가격 소스가 있습니다. 가격이 `Website`으로 설정된 경우, 웹 사이트에서는 가격을 달리할 수 있으며 기본 가격 대비도 있습니다. 코어 상거래 사용 안내서에서 [카탈로그 가격](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;}을 참조하십시오.

카탈로그 가격 범위를 `Global`에서 `Website`(으)로 변경하면 모든 가격 유형 속성도 `Website`로 변경됩니다. [웹 사이트 추가](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){:target=&quot;_blank&quot;}를 참조하십시오.

웹 사이트 가격이 선택되면 두 가지 가격 소스가 있습니다.

- 웹 사이트 가격
- 기본(폴백) 가격

Amazon 판매 채널 통합의 경우 [목록 규칙](./listing-rules.md)을 기반으로 여러 웹 사이트의 제품을 단일 [!DNL Amazon Marketplace] 국가([스토어 통합](./store-integration.md)에 정의됨)에 매핑할 수 있습니다. 그러나 이러한 매핑은 가격이 다른 여러 웹 사이트에 제품이 있을 경우 가격을 게시해야 하는 문제를 소개합니다.
