---
title: '"관리 [!DNL Walmart Marketplace] 주문"'
description: '"보기 및 관리 [!DNL Walmart Marketplace] 주문 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source의 경우"'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: eb57189ed866fffa064867d1de5ae9db5b32e283
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 0%

---

# 관리 [!DNL Walmart Marketplace] 주문

[!DNL Walmart Marketplace] 주문 데이터 [!DNL Commerce] 는 자동으로 동기화됩니다 [!DNL Channel Manager] after [!DNL Walmart] 순서를 처리합니다.

상거래 측에서 성공적으로 동기화하면 다음 작업이 트리거됩니다.

- [!DNL Channel Manager] Walmart에 주문 승인을 보냅니다.

- 해당 상거래 주문이 Walmart 주문에서 생성됩니다.

- 업데이트된 주문 정보는 [!DNL Channel Manager] 주문 대시보드.

상점 관리에서 주문 데이터를 볼 수 있습니다 [!DNL Channel Manager] 영업 채널 저장소를 열고 **[!UICONTROL Orders]**.

![채널 관리자 주문 보기 를 통해 관리 [!DNL Walmart Marketplace] 주문](assets/orders-dashboard-view.png)

>[!NOTE]
>
>한 번에 최대 35분이 소요될 수 있습니다 [!DNL Walmart Marketplace] 에 표시할 순서 [!DNL Channel Manager] 주문 목록. [!DNL Walmart] 수신되는 주문을 처리하고 전송하려면 약 30분이 필요합니다 [!DNL Channel Manager]. 채널 관리자가 주문을 받으면 5분 정도 더 걸려서 Adobe Commerce 또는 Magento Open Source에서 순서를 만들고 표시할 수 있습니다.

## 주문 통제 및 열 설명

다음 표에서는 Orders에 사용할 수 있는 컨트롤과 열을 설명합니다.

**컨트롤[!UICONTROL Orders]**
| **제어**                    | **설명**                                                                                                                                                                                                                                                                  | |—|—| | [!UICONTROL Filter orders]     | 다음 중 하나를 선택하여 보기를 정렬합니다 [!UICONTROL Order Status] 카드.                                                                                                                                                                                                           | | 오류 설명 | 오류 상태의 주문에 대한 자세한 정보를 제공합니다.                                                                                                                                                                                                            | | [!UICONTROL View order detail] | 주문 세부 사항을 보려면 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다.                                                                                                                    | | [!UICONTROL Channel Settings]  | 채널 구성을 수정하려면 채널 Walmart 연결 자격 증명, 매핑된 속성 또는 배송 식별자를 선택합니다. 설정은 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다. |


**열 설명**

| 필드 | 설명 |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Walmart Order Number] | 주문에서 주문에 지정된 구매 발주 번호 [!DNL Walmart Marketplace]. 처음에 주문을 로 가져오는 경우 [!DNL Channel Manager], 만 [!DNL Walmart] 주문 번호가 표시됩니다. 이 [!DNL Commerce] 주문이 생성되면 [!DNL Walmart] 주문 번호는 [!UICONTROL External ID] 제품 속성입니다. |
| [!DNL Commerce] 주문 번호 | 에 지정된 번호 [!DNL Commerce] 주문 [!DNL Walmart Marketplace] 주문. |
| 항목 | 주문된 항목 수 [!DNL Walmart Marketplace]. |
| [!UICONTROL Order Value] | 주문 품목의 총 원가. |
| [!UICONTROL Date Ordered] | 주문이 제출된 날짜입니다 [!DNL Walmart Marketplace]. |
| [!UICONTROL Ship By Date] | 주문을 발송해야 하는 일자 [!DNL Walmart Marketplace] 요구 사항. |
| [!UICONTROL Deliver By Date] | 고객이 충족하기 위해 주문을 고객에게 전달해야 하는 일자 [!DNL Walmart Marketplace] 요구 사항(UTC 형식)입니다. |
| [!UICONTROL Ship Method] | 다음 [[!DNL Walmart Marketplace] 배송 방법](https://sellerhelp.walmart.com/s/guide?article=000007893) 선택된 상태로 표시됩니다. |
| [!UICONTROL Last Update At] | 주문 데이터가 마지막으로 업데이트된 시간을 나타내는 타임스탬프 [!DNL Channel Manager] UTC 형식입니다. |
| [!UICONTROL Status] | 에서 현재 주문 상태를 나타냅니다. [!DNL Commerce] 주문 워크플로우입니다. 임포트된 주문의 초기 상태 [!DNL Walmart Marketplace] is _열기_. 상거래 주문이 처리되고 [!DNL Channel Manager] 선적, 부분 선적 및 취소 업데이트를 성공적으로 동기화합니다. [!DNL Walmart Marketplace]. |
| [!UICONTROL Error Description] | 를 사용하여 주문에 대한 자세한 정보를 제공합니다. _[!UICONTROL Error]_상태. |

## 주문 상태


[!UICONTROL Order Status] 의 현재 상태에 대한 정보를 제공합니다. [!DNL Walmart Marketplace] Adobe Commerce 또는 Magento Open Source에서 관리되는 주문. 주문 상태 업데이트는 [!DNL Channel Manager] 다음 중 하나에서 업데이트된 주문 정보를 받습니다. [!DNL Walmart Marketplace] 또는 [!DNL Commerce] 주문 시스템. 주문에는 다음 상태가 있을 수 있습니다.

- **[!UICONTROL Shipped]**&quot;주문에서 배송된 주문 [!DNL Commerce] 저장. 주문이 배송되면 [!DNL Channel Manager] 에 업데이트를 보냅니다. [!DNL Walmart Marketplace] Walmart에서 운송 상태를 갱신하고 출하에 대한 주문 추적 번호를 제공하기 위해.

- **[!UICONTROL Partially Shipped]**- 일부 품목이 출하됨으로 표시된 주문 및 출하되기를 기다리는 주문. 주문 출하시 [!DNL Channel Manager] 에 업데이트를 보냅니다. [!DNL Walmart Marketplace] 운송 상태를 Walmart에서 부분 출하되도록 갱신하고 출하에 대한 주문 추적 번호를 제공하기 위해.

- **[!UICONTROL Canceled]**-주문 취소 [!DNL Commerce] 저장.

   주문 취소가 완료되면 [!DNL Commerce] 반환된 품목을 반영하도록 재고 수량 업데이트. 그럼, [!DNL Channel Manager] 업데이트를에 동기화 [!DNL Walmart Marketplace].

- **[!UICONTROL Error]**- 오류가 있는 주문. 주문 업데이트 작업이 실패할 경우 오류가 발생할 수 있습니다. 예를 들어 다음 경우 오류가 발생합니다 [!DNL Channel Manager] 월마트로부터 새 주문을 받을 수 없습니다. 이러한 매개 변수는 [!DNL Channel Manager] 주문 선적 또는 취소 갱신을 [!DNL Walmart Marketplace]. 작업이 실패하면 주문 페이지에 _오류_ 주문 상태. 자세한 내용은 [주문 오류 수정](process-orders.md#fix-shipping-and-cancellation-errors).

- **[!UICONTROL Error description]**-누락된 정보 또는 잘못된 값, 잘못된 납품 상세내역 또는 주문 취소 실패와 같은 문제로 인해 발생하는 주문 오류에 대한 자세한 정보를 제공합니다. 설명은 오류 발생 여부를 확인하는 데 도움이 됩니다 [!DNL Commerce] 인스턴스 또는 [!DNL Walmart Marketplace].

>[!NOTE]
>
>주문 품목이 복수 출하로 발송되는 경우 주문 상태는 다음과 같습니다 [!DNL Channel Manager] 사용 가능한 마지막 주문 상태를 반영합니다. 예를 들어 주문 업데이트가 로 동기화될 때 첫 번째 항목이 출하되고 오류가 반환되지 않는 경우 [!DNL Channel Manager] 및 [!DNL Walmart Marketplace], [!DNL Channel Manager] 주문 상태는 _[!UICONTROL Partially Shipped]_.  두 번째 품목이 출하되면 [!C채널 관리자] 오류를 반환하면 주문 상태가_[!UICONTROL Error]_.

## 주문 검토

1. 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 열다 [!UICONTROL Channel Manager Marketplace Stores] 페이지.

1. 저장소 항목 행에서 눈 아이콘을 선택하여 저장소 보기를 엽니다.

1. 주문 정보를 보려면 *를 선택합니다.[!UICONTROL *Orders]**.

1. 주문에 대한 정보를 확인하고 **[상태](#about-order-status)** 열을 사용하여 주문에 대한 정보를 얻습니다.

## 주문 세부 사항 보기

마켓플레이스에서 주문을 받고 Adobe Commerce 또는 Magento Open Source으로 가져온 후에는 [!DNL Commerce] 주문 ID를 사용하여 Adobe Commerce에서 순서를 봅니다.

From **[!UICONTROL Orders]**&#x200B;에서 을(를) 선택합니다. **[!UICONTROL Commerce Order Number]** 열다 [!DNL Commerce] 주문 세부 사항.

![전자 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-detail-with-external-order-id.png)

Commerce Store에서 [!DNL Walmart Marketplace] 주문 데이터에 다음과 같은 추가 정보가 포함되어 있습니다.

- **결제 정보 및 운송 방법**-Walmart에서 가져온 주문에는 결제 및 배송 필드에 대해 다음 값이 포함됩니다.

   - **[!UICONTROL Offline Channel Payment]**- 주문 결제가 오프라인으로 처리됨을 나타냅니다. [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**- 를 표시합니다 [!DNL Walmart Marketplace] 주문 번호.

   - **[!UICONTROL Channel Shipping - Value]**-배송비를 처리함을 나타냅니다. [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**-이 필드는 [!DNL Walmart Marketplace] 이(가) 취소되었습니다. 취소 사유에는 다음이 포함됩니다.

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

