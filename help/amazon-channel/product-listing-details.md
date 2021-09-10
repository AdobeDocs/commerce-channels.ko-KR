---
title: 목록 세부 정보 보기
description: Amazon 목록 및 개별 SKU/제품 변경 사항에 대한 경쟁 지표를 이해하려면 제품 목록 세부 사항 페이지를 검토하십시오.
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 목록 세부 사항 보기

_[!UICONTROL Product Listing Details]_페이지에는 개별 SKU/제품의 변경 사항을 보여주는 활동 로그 나열 등 활성 제품 목록에 대한 추가 정보가 표시됩니다. 이 정보는 제품과 개별 SKU/제품 변경 사항에 대한 경쟁업체 지표를 이해하는 데 도움이 됩니다. 이 페이지의 추가 정보에는 다음이 포함됩니다.

- **[!UICONTROL Listing Details]** - 이름 및 Amazon 판매자 SKU를 포함한 제품 세부 사항
- **[!UICONTROL Listing Activity Log]** - 가격 책정 및 수량/재고 변경과 같이 이 목록에 대해 발생한 모든 변경 사항의 기록 추가 작업은 필요하지 않습니다. 이 로그는 변경 내용을 이해할 수 있도록 제공됩니다.
- **[!UICONTROL Buy Box Competitor Pricing]** - Amazon의  [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 상태 및 경쟁업체 가격 데이터
- **[!UICONTROL Lowest Competitor Pricing]** - 가장 낮은 Amazon 경쟁업체의 가격 및 피드백 정보에 대한 정보

Amazon 판매 채널 홈 페이지는 표시되는 데이터를 사용자 지정할 수 있는 몇 가지 일반적인 [작업 공간 컨트롤](./workspace-controls.md)을 공유합니다.

## 목록 세부 정보

표시되는 제품 정보는 다음과 같습니다.

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![목록 세부 정보](assets/amazon-product-listing-details.png)

## 활동 로그 나열 {#listing-activity-log}

Amazon 목록에 대한 모든 최근 활동을 표시합니다. 표시되는 정보는 다음과 같습니다.

- Amazon 판매자 SKU: 목록에 대해 정의된 SKU(Stock Keeping Unit)를 식별합니다.
- ASIN: 10자리 Amazon 제품 식별자를 식별합니다.
- 목록 작업: 목록에 대해 발생한 작업 유형을 식별합니다.
- 댓글: 발생한 목록 작업 유형과 관련된 추가 세부 정보를 제공합니다.
- 실행 위치: 작업이 발생한 날짜 및 시간을 식별합니다.

![제품 목록 세부 사항 - 활동 로그 나열](assets/amazon-listing-activity-log.png)
__

## Buy Box 경쟁업체 가격 책정 {#buy-box-competitor-pricing}

이 탭에는 목록의 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 위치를 가진 Amazon 머천트에 대한 정보가 표시됩니다. 이 정보는 Amazon에서 경쟁 업체의 가격 결정을 이해하는 데 사용할 수 있습니다. 표시되는 정보는 다음과 같습니다.

- ASIN: 10자리 Amazon 제품 식별자입니다.
- 판매자임: [!DNL Buy Box] 판매자인지 식별합니다. 옵션 예 / 아니오.
- 조건: 목록에 대해 정의된 조건을 식별합니다.
- 목록 가격: 목록이 게시된 가격을 식별합니다.
- 배송 가격: 목록에 추가된 운송 가격을 식별합니다.
- 랜딩 가격: 목록의 운송 가격과 함께 목록 가격을 식별합니다.
- 마지막 업데이트 날짜: Amazon에서 가격 정보를 업데이트한 날짜 및 시간을 식별합니다.

![제품 목록 세부 정보: Buy Box 경쟁업체 가격 책정](assets/amazon-listing-details-buy-box-2.png)

## 가장 낮은 경쟁업체 가격 {#lowest-competitor-pricing}

이 탭에는 동일한 목록에 대한 Amazon 경쟁 제품에 대한 정보가 표시됩니다. 이 정보는 가격 포지셔닝 및 [가장 낮은 경쟁업체 가격](./lowest-competitor-pricing.md)을 이해하는 데 사용할 수 있습니다. 표시되는 정보는 다음과 같습니다.

- ASIN: 10자리 Amazon 제품 식별자입니다.
- 조건: 목록에 대해 정의된 조건을 식별합니다.
- 이행 채널: 이행 담당자를 식별합니다. 옵션: 머천트/Amazon.
- 목록 가격: 목록이 게시된 가격을 식별합니다.
- 배송 가격: 목록에 추가된 운송 가격을 식별합니다.
- 랜딩 가격: 목록의 운송 가격과 함께 목록 가격을 식별합니다.
- 피드백 등급: 가장 낮은 가격 매장에 대한 Amazon 피드백 등급을 식별합니다.
- 피드백 수: 가장 낮은 가격 매장에 대한 Amazon 피드백 수를 식별합니다.
- 마지막 업데이트 날짜: Amazon에서 가격 정보를 업데이트한 날짜 및 시간을 식별합니다.

![제품 목록 세부 정보 - 가장 낮은 경쟁업체 가격](assets/amazon-listing-details-lowest-comp.png)
