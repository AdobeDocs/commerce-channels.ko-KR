---
title: 가격 범위
description: 상거래 가격 범위를 사용하여 여러 웹 사이트 또는 전 세계에 따른 가격을 관리합니다.
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 가격 범위

[!DNL Commerce] 은 [가격 범위](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target=&quot;_blank&quot;}을(를) (으)로 설정할 수 있습니다. `Global` 또는 `Website`. 가격을 로 설정한 경우 `Global`모든 웹 사이트에 대해 단일 가격 소스가 있습니다. 가격을 로 설정한 경우 `Website`과 같은 경우, 웹 사이트에서는 요금이 다를 수 있으며, 기본 요금도 대체됩니다. 자세한 내용은 [카탈로그 가격](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price)코어 상거래 사용 안내서의 {target=&quot;_blank&quot;}.

카탈로그 가격 범위를 `Global` to `Website`, 모든 가격 유형 속성이 `Website`. 자세한 내용은 [웹 사이트 추가](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target=&quot;_blank&quot;}.

웹 사이트 가격이 선택되면 두 가지 가격 소스가 있습니다.

- 웹 사이트 가격
- 기본(폴백) 가격

Amazon 영업 채널 통합의 경우, [목록 규칙](./listing-rules.md)여러 웹 사이트의 제품을 하나의 웹 사이트로 매핑할 수 있습니다 [!DNL Amazon Marketplace] 국가(다음 기간 동안 정의됨) [스토어 통합](./store-integration.md)). 그러나 이러한 매핑은 가격이 다른 여러 웹 사이트에 제품이 있을 경우 가격을 게시해야 하는 문제를 소개합니다.
