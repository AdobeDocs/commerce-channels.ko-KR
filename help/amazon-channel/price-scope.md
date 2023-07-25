---
title: Amazon 판매 채널 - 가격 범위
description: 여러 웹 사이트 또는 전 세계에 따라 가격을 관리하려면 Commerce 가격 범위를 사용하십시오.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# 가격 범위

[!DNL Commerce] 는에 대한 구성을 제공합니다. [가격 범위](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) 로 설정 `Global` 또는 `Website`. 가격이 다음으로 설정된 경우 `Global`, 모든 웹 사이트에 대한 단일 가격 소스가 있습니다. 가격이 다음으로 설정된 경우 `Website`, 웹 사이트의 가격이 서로 다를 수 있으며 기본 대체 가격 값이 있습니다(참조). [가격 범위](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html)).

카탈로그 가격 범위를에서 변경하면 `Global` 끝 `Website`, 모든 가격 유형 속성도 다음으로 변경됩니다. `Website`. 다음을 참조하십시오 [웹 사이트 추가](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

웹 사이트 가격을 선택하면 두 가지 가격 소스가 있습니다.

- 웹 사이트 가격
- 기본(폴백) 가격

Amazon 판매 채널 통합의 경우 [규칙 나열](./listing-rules.md), 여러 웹 사이트의 제품을 하나로 매핑할 수 있습니다 [!DNL Amazon Marketplace] 국가(다음 기간 동안 정의됨) [스토어 통합](./store-integration.md)). 그러나 이 매핑에서는 제품이 다른 가격이 있는 여러 웹 사이트에 있는 경우 게시해야 하는 가격의 문제를 소개합니다.
