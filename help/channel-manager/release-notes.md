---
title: '[!DNLChannel Manager] 릴리스 노트'
description: "에 대한 최신 릴리스 정보 [!DNL Channel Manager] Adobe Commerce"
source-git-commit: 501a76a126f090805f95e64078ec2c73de003aa4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 2%

---

# [!DNL Channel Manager] 릴리스 정보

이러한 릴리스 노트는 [!DNL Channel Manager] 다음을 포함합니다.

![새로 만들기](../assets/new.svg) 새로운 기능
![해결된 문제](../assets/fix.svg) 수정 사항 및 향상된 기능
![알려진 문제](../assets/bug.svg) 알려진 문제


## v1.1.0

![새로 만들기](../assets/new.svg)<!--CHAN-5204--> **반환 및 반환**- 이제 Adobe Commerce 및 Magento Open Source 채널 관리자 스토어를 통해 출하된 주문에 대해 Walmart Marketplace 반품 및 환불 프로세스를 처리할 수 있습니다. 반환 및 환불에 대한 정보 및 업데이트는 Walmart와 Adobe Commerce 간에 동기화되어 현재 데이터를 [!DNL Commerce] 상점 및 [!DNL Walmart Marketplace]. 자세한 내용은 [반품 및 환불 주문](return-refund-orders.md).

![고정](../assets/fix.svg)<!--CHAN-5661--> 수정 사항 `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 채널 관리자를 사용하여 데이터를 다시 동기화할 때 발생하는 오류 `bin/magento saas:resync --feed orders` 명령. Sales Data Exporter 모듈에서 이름이 변경된 Channel Manager 패키지 종속성을 업데이트하여 오류가 해결되었습니다. `magento/module-sales-data-exporter` to `magento/module-sales-orders-data-exporter`.

## v1.0.0

다음 상거래 버전과 호환되는 초기 릴리스:

* 오픈 소스(CE): 2.4.x
* Adobe Commerce (EE): 2.4.x
* ECE(Adobe Commerce for Cloud): 2.4.x
* 안정성: 안정적인
