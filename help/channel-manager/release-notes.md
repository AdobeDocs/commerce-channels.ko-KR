---
title: '[!DNL Channel Manager] 릴리스 노트'
description: Adobe Commerce의  [!DNL Channel Manager] 에 대한 최신 릴리스 정보입니다.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# [!DNL Channel Manager] 릴리스 정보

이 릴리스 노트는 [!DNL Channel Manager]의 초기 릴리스에 대해 설명하고 다음을 포함합니다.

새 기능 ![개](../assets/new.svg)개
![해결된 문제](../assets/fix.svg) 수정 사항 및 개선 사항
![알려진 문제](../assets/bug.svg)알려진 문제

릴리스 일정 및 지원에 대한 자세한 내용은 [예정된 릴리스](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)를 참조하세요.

이 확장을 지원하는 Adobe Commerce 버전을 알아보려면 [제품 가용성](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)을 참조하세요.

## v2.1.0

*2023년 10월 3일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로운](../assets/new.svg) 채널 관리자가 이제 [Adobe Commerce 버전 2.4.7 베타](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) 릴리스와 호환됩니다.

## v2.0.0

*2023년 3월 20일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새](../assets/new.svg)<!--CHAN-5893--> 채널 관리자가 이제 Adobe Commerce 버전 2.4.6과 호환됩니다.

## v1.1.0

*2022년 11월 23일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로 만들기](../assets/new.svg)<!--CHAN-5204--> **반품 및 환불**—이제 Adobe Commerce 및 Magento Open Source Channel Manger 스토어를 통해 배송된 주문에 대한 Walmart Marketplace 반품 및 환불 프로세스를 처리할 수 있습니다. 반품 및 환불에 대한 정보 및 업데이트가 월마트와 Adobe Commerce 간에 동기화되어 현재 데이터는 [!DNL Commerce] 상점 및 [!DNL Walmart Marketplace] 모두에서 사용할 수 있습니다. [반품 및 환불 주문](return-refund-orders.md)을 참조하세요.

![수정](../assets/fix.svg)<!--CHAN-5661--> `bin/magento saas:resync --feed orders` 명령을 사용하여 채널 관리자 주문 데이터를 다시 동기화할 때 발생하는 `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 오류를 해결했습니다. 판매 데이터 내보내기 모듈에 대한 채널 관리자 패키지 종속성을 업데이트하여 오류가 해결되었습니다. 판매 데이터 내보내기 모듈의 이름은 `magento/module-sales-data-exporter`에서 `magento/module-sales-orders-data-exporter`(으)로 변경되었습니다.

## v1.0.0

*2022년 1월 14일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

일반 가용성을 위한 채널 관리자의 ![새로운](../assets/new.svg) 초기 릴리스

