---
title: '[!DNL Channel Manager] 릴리스 정보'
description: 의 최신 릴리스 정보 [!DNL Channel Manager] Adobe Commerce에서.
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 3%

---

# [!DNL Channel Manager] 릴리스 정보

이 릴리스 노트는 의 초기 릴리스에 대해 설명합니다. [!DNL Channel Manager] 및 포함:

![신규](../assets/new.svg) 새로운 기능
![해결된 문제](../assets/fix.svg) 수정 사항 및 향상된 기능
![알려진 문제](../assets/bug.svg) 알려진 문제

다음을 참조하십시오 [예정된 릴리스](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) 릴리스 일정 및 지원에 대해 알아봅니다.

다음을 참조하십시오 [제품 가용성](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 이 확장을 지원하는 Adobe Commerce 버전을 알아봅니다.

## v2.1.0

*2023년 10월 3일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![신규](../assets/new.svg) 채널 관리자는 이제 와 호환됩니다. [Adobe Commerce 버전 2.4.7 베타](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) 릴리스.

## v2.0.0

*2023년 3월 20일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![신규](../assets/new.svg)<!--CHAN-5893--> 채널 관리자는 이제 Adobe Commerce 버전 2.4.6과 호환됩니다.

## v1.1.0

*2022년 11월 23일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![신규](../assets/new.svg)<!--CHAN-5204--> **반환 및 환불**—이제 Adobe Commerce 및 Magento Open Source Channel Manager 스토어를 통해 배송된 주문에 대한 Walmart Marketplace 반품 및 환불 프로세스를 처리할 수 있습니다. 반품 및 환불에 대한 정보와 업데이트는 월마트와 Adobe Commerce 간에 동기화되므로 현재 데이터는 두 곳에서 모두 사용할 수 있습니다. [!DNL Commerce] 상점 앞에 및 [!DNL Walmart Marketplace]. 다음을 참조하십시오 [반품 및 환불 주문](return-refund-orders.md).

![고정](../assets/fix.svg)<!--CHAN-5661--> 을(를) 수정했습니다. `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 채널 관리자 주문 데이터를 다시 동기화하는 동안 오류가 발생했습니다. `bin/magento saas:resync --feed orders` 명령입니다. Sales Data Exporter 모듈에 대한 Channel Manager 패키지 종속성을 업데이트하여 오류를 해결했습니다. 이 모듈은에서 이름이 변경되었습니다. `magento/module-sales-data-exporter` 끝 `magento/module-sales-orders-data-exporter`.

## v1.0.0

*2022년 1월 14일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![신규](../assets/new.svg) Channel Manager 의 초기 릴리즈를 통한 일반 공급

