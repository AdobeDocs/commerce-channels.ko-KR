---
title: Amazon 판매 채널 - 가격 범위
description: Commerce 가격 범위를 사용하여 여러 웹 사이트 또는 전 세계에 따른 가격을 관리합니다.
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 가격 범위

[!DNL Commerce]에서 [가격 범위](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price)를 `Global` 또는 `Website`(으)로 설정하는 구성을 제공합니다. 가격이 `Global`(으)로 설정된 경우 모든 웹 사이트에 대해 단일 가격 원본이 있습니다. 가격책정이 `Website`(으)로 설정된 경우 웹 사이트의 가격책정이 변경될 수 있으며 기본 가격 대체 값도 있습니다([가격 범위](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html) 참조).

카탈로그 가격 범위를 `Global`에서 `Website`(으)로 변경하면 모든 가격 유형 특성도 `Website`(으)로 변경됩니다. [웹 사이트 추가](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites)를 참조하십시오.

웹 사이트 가격을 선택하면 두 가지 가격 소스가 있습니다.

- 웹 사이트 가격
- 기본(폴백) 가격

Amazon 판매 채널 통합의 경우 [목록 규칙](./listing-rules.md)을 기반으로 여러 웹 사이트의 제품을 단일 [!DNL Amazon Marketplace] 국가([스토어 통합](./store-integration.md) 중에 정의됨)에 매핑할 수 있습니다. 그러나 이 매핑에서는 제품이 다른 가격이 있는 여러 웹 사이트에 있는 경우 게시해야 하는 가격의 문제를 소개합니다.
