---
title: ' [!DNL Channel Manager]의 주문 보기 및 관리'
description: 'Adobe Commerce 및 Magento Open Source에 대해  [!DNL Channel Manager] 을(를) 사용하여  [!DNL Walmart Marketplace] 주문 보기 및 관리'
feature: Sales Channels, Orders
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

# [!DNL Channel Manager]의 주문 보기 및 추적

[!DNL Walmart]에서 주문을 처리한 후 [!DNL Commerce] 제품에 대한 [!DNL Walmart Marketplace] 주문 데이터가 [!DNL Channel Manager]에 자동으로 동기화됩니다.

[!DNL Commerce] 측에서 동기화가 성공하면 다음 작업이 트리거됩니다.

- [!DNL Channel Manager]이(가) 주문 승인을 Walmart로 보냅니다.

- Walmart 주문에서 해당 [!DNL Commerce] 주문이 만들어집니다.

- 업데이트된 주문 정보가 [!DNL Channel Manager] 주문 대시보드에 표시됩니다.

Storefront 관리자는 판매 채널 스토어를 열고 **[!UICONTROL Orders]**&#x200B;을(를) 선택하여 [!DNL Channel Manager]의 주문 데이터를 볼 수 있습니다.

[!DNL Walmart Marketplace]개 주문을 관리하기 위한 ![채널 관리자 주문 보기](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>[!DNL Walmart Marketplace] 순서가 [!DNL Channel Manager] 순서 목록에 표시되는 데 최대 35분이 걸릴 수 있습니다. [!DNL Walmart]에서 들어오는 주문을 처리하고 [!DNL Channel Manager](으)로 보내는 데 약 30분이 필요합니다. Channel Manager 가 주문을 받으면 Adobe Commerce 또는 Magento Open Source에서 주문을 만들고 표시하는 데 약 5분이 더 소요됩니다.

## 주문 컨트롤 및 열 설명

다음 표에서는 Orders에 사용할 수 있는 컨트롤 및 열에 대해 설명합니다.

[!UICONTROL Orders]**에 대한**&#x200B;컨트롤

<table>
<tr>
<td><strong>제어</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>[!UICONTROL Order Status]개 카드 중 하나를 선택하여 보기를 정렬합니다.</td>
</tr>
<tr>
<td>상태 세부 정보</td>
<td>주문 오류 및 반환 요청에 대한 정보를 제공합니다. 주문에 대한 반환 정보와 환불 상태를 보려면 <strong>[!UICONTROL Return requested]</strong> 텍스트를 선택하여 [!UICONTROL Returns] 대시보드를 여십시오.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>주문 세부 사항을 보려면 [!UICONTROL Order] 테이블에서 [!DNL Commerce] 주문 번호를 선택하십시오. 그런 다음 [!DNL Commerce] 순서 옵션을 사용하여 순서를 처리합니다.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>채널 구성을 수정하려면 채널 Walmart 연결 자격 증명, 매핑된 특성 또는 배송 식별자를 선택하고, 설정은 [!UICONTROL Order] 테이블에서 [!DNL Commerce] 주문 번호를 선택합니다. 그런 다음 [!DNL Commerce] 순서 옵션을 사용하여 순서를 처리합니다.</td>
</tr>
</table>


**열 설명**

<table>
<tr>
<td>필드</td>
<td>설명</td>
</tr>
<tr>
<td>[!UICONTROL Walmart Order #]</td>
<td>[!DNL Walmart Marketplace]의 주문에 할당된 구매 주문 번호입니다. 처음 주문을 [!DNL Channel Manager](으)로 가져오면 [!DNL Walmart] 주문 번호만 표시됩니다. [!DNL Commerce] 순서가 만들어지면 [!DNL Walmart] 순서 번호가 [!UICONTROL External ID] 제품 특성에 저장됩니다.</td>
</tr>
<tr>
<td>[!DNL Commerce] 주문 번호</td>
<td>[!DNL Walmart Marketplace] 주문에서 만든 [!DNL Commerce] 주문에 할당된 번호입니다.</td>
</tr>
<tr>
<td>항목</td>
<td>[!DNL Walmart Marketplace]에 정렬된 항목 수입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>주문 품목의 총 비용.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>[!DNL Walmart Marketplace]에 주문이 제출된 날짜로 현지 시간대로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>로컬 시간대로 변환된 [!DNL Walmart Marketplace] 요구 사항을 충족하기 위해 주문을 배송해야 하는 날짜입니다.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>로컬 시간대로 전환된 [!DNL Walmart Marketplace] 요구 사항을 충족하기 위해 주문이 고객에게 전달되어야 하는 날짜입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>주문에 대해 선택된 [[!DNL Walmart Marketplace] 배송 방법](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29)</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>[!DNL Channel Manager]에서 주문 데이터가 마지막으로 업데이트된 시간을 나타내는 타임스탬프가 현지 표준 시간대로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>[!DNL Commerce] 주문 워크플로우의 현재 주문 상태를 나타냅니다. [!DNL Walmart Marketplace]에서 가져온 주문의 초기 상태는 _Open_입니다. [!DNL Commerce] 주문이 처리되고 [!DNL Channel Manager]이(가) 선적, 부분 선적 및 취소 업데이트를 [!DNL Walmart Marketplace]에 성공적으로 동기화할 때 추가 상태 업데이트가 발생합니다.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>오류가 있거나 환불 요청이 있는 주문에 대한 자세한 정보를 제공합니다.</td>
</tr>
</table>

## 주문 상태

[!UICONTROL Order Status]은(는) Adobe Commerce 또는 Magento Open Source에서 관리되는 [!DNL Walmart Marketplace]개 주문의 현재 상태에 대한 정보를 제공합니다. 주문 상태 업데이트는 [!DNL Channel Manager]이(가) [!DNL Walmart Marketplace] 또는 [!DNL Commerce] 주문 시스템에서 업데이트된 주문 정보를 받을 때 발생합니다. 주문의 상태는 다음과 같습니다.

- **[!UICONTROL Shipped]** - [!DNL Commerce] 저장소에서 배송된 주문입니다. 주문이 배송되면 [!DNL Channel Manager]이(가) [!DNL Walmart Marketplace](으)로 업데이트를 보내 월마트의 배송 상태를 업데이트하고 배송에 대한 주문 추적 번호를 제공합니다. 주문이 배송된 후, 월마트가 반품 승인 양식을 발행하면 주문 품목의 일부 또는 전부를 환불할 수 있습니다. [반환 및 환불](return-refund-orders.md)을 참조하세요.

- **[!UICONTROL Partially Shipped]**—일부 품목이 배송된 것으로 표시되고 다른 품목은 배송 대기 중인 주문입니다. 주문 배송에 있는 항목이 배송되면 [!DNL Channel Manager]에서 [!DNL Walmart Marketplace](으)로 업데이트를 보내 배송 상태를 Walmart에서 _[!DNL Partially Shipped]_(으)로 업데이트하고 배송에 대한 주문 추적 번호를 제공합니다.

- **[!UICONTROL Canceled]** - [!DNL Commerce] 저장소에서 취소된 주문입니다.

  주문 취소가 완료되면 반환된 항목을 반영하도록 [!DNL Commerce] 재고 수량이 업데이트됩니다. 그런 다음 [!DNL Channel Manager]이(가) 업데이트를 [!DNL Walmart Marketplace](으)로 동기화합니다.

- **[!UICONTROL Return requested]**—Walmart Marketplace에서 배송된 주문 품목의 반품을 요청하면 [!UICONTROL Status details] 열에 `Return requested` 링크가 표시됩니다. 링크를 선택하면 [!UICONTROL Returns] 대시보드가 열려 반품을 확인하고 환불 프로세스를 관리합니다.

- **[!UICONTROL Error]** - 오류가 있는 주문입니다. 주문 업데이트 작업이 실패할 경우 오류가 발생할 수 있습니다. 예를 들어 [!DNL Channel Manager]이(가) Walmart에서 새 주문을 받을 수 없는 경우 오류가 발생합니다. [!DNL Channel Manager]이(가) 주문 배송 또는 취소 업데이트를 [!DNL Walmart Marketplace](으)로 보낼 수 없는 경우에도 이러한 문제가 발생할 수 있습니다. 작업이 실패할 경우 주문 페이지에 주문에 대한 _오류_ 상태가 표시됩니다. 자세한 내용은 [주문 오류 수정](process-orders.md#fix-shipping-and-cancellation- errors)을 참조하십시오.

- **[!UICONTROL Status details]**-정보 누락 또는 잘못된 값, 잘못된 배송 세부 정보 또는 주문 취소 실패 등의 문제로 인해 발생하는 주문 오류에 대한 자세한 정보를 제공합니다. 설명은 [!DNL Commerce] 인스턴스 또는 [!DNL Walmart Marketplace]에서 오류가 발생했는지 확인하는 데 도움이 됩니다.

>[!NOTE]
>
>주문 품목이 여러 번 배송된 경우 [!DNL Channel Manager]의 주문 상태는 사용 가능한 마지막 주문 상태를 반영합니다. 예를 들어 주문 업데이트가 [!DNL Channel Manager] 및 [!DNL Walmart Marketplace](으)로 동기화되는 경우 첫 번째 항목이 배송되고 오류가 반환되지 않으면 [!DNL Channel Manager] 주문 상태는 _[!UICONTROL Partially Shipped]_입니다. 두 번째 항목이 배송된 후 [!DNL Channel Manager]에서 오류가 반환되면 주문 상태가_[!UICONTROL Error]_(으)로 업데이트됩니다.

## 주문 검토

1. 관리자에서 **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**&#x200B;을(를) 선택하여 [!UICONTROL Channel Manager Marketplace Stores] 페이지를 엽니다.

1. 저장소 항목 행에서 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

1. 주문 정보를 보려면 *[!UICONTROL *Orders]**을(를) 선택하십시오.

1. **[상태](#order-status)** 열을 확인하여 주문에 대한 정보를 확인하고 다음 단계를 결정합니다.

## 주문 세부 사항 검토

마켓플레이스에서 주문을 받고 판매 채널 스토어로 가져온 후에는 [!DNL Commerce] 주문 ID를 사용하여 Adobe Commerce에서 주문 세부 사항을 볼 수 있습니다.

**[!UICONTROL Orders]**&#x200B;에서 **[!UICONTROL Commerce Order Number]**&#x200B;을(를) 선택하여 [!DNL Commerce] 주문 세부 정보를 엽니다.

[!DNL Walmart Marketplace] 주문에 대한 ![Commerce 주문 세부 정보 보기](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

Commerce 상점 첫 화면의 [!DNL Walmart Marketplace]에서 가져온 주문에는 주문 데이터에 다음 추가 정보가 포함되어 있습니다.

- **결제 정보 및 배송 방법**-Walmart에서 가져온 주문에는 결제 및 배송 필드에 대한 다음 값이 포함됩니다.

   - **[!UICONTROL Offline Channel Payment]**—주문 결제가 [!DNL Walmart Marketplace]에 의해 오프라인으로 처리됨을 나타냅니다.

   - **[!UICONTROL External Order Number]**—주문 번호 [!DNL Walmart Marketplace]을(를) 표시합니다.

   - **[!UICONTROL Channel Shipping - Value]**-배송 비용이 [!DNL Walmart Marketplace]을(를) 통해 처리됨을 나타냅니다.

   - **[!UICONTROL Cancellation Reason]**-이 필드는 [!DNL Walmart Marketplace]에서 가져온 주문이 취소된 경우에만 표시됩니다. 취소 사유는 다음과 같습니다.

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **주문한 항목**—이 섹션에는 모든 Commerce 주문의 주문 항목이 나열됩니다. [!UICONTROL Qty] 열은 주문 항목에 대한 상태 기록을 제공합니다. 예를 들어 주문의 송장이 발행되고, 배송되고, 환불된 경우 상태 전환을 볼 수 있습니다.

  ![주문 세부 사항 주문 항목 상태 기록 [!DNL Walmart Marketplace]개 주문](assets/order-detail-status-history.png){width="600" zoomable="yes"}

탐색 메뉴에서 [!UICONTROL Invoice] 및 [!UICONTROL Credit Memo] 옵션을 선택하여 항목 송장 및 환불 세부 정보를 봅니다. 판매 채널 스토어의 [[!UICONTROL Returns]](return-refund-orders.md) 대시보드에서 직접 대변 메모에 액세스할 수도 있습니다.
