---
title: '주문 보기 및 관리 [!DNL Channel Manager]'
description: '보기 및 관리 [!DNL Walmart Marketplace] 주문 [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source의 경우'
exl-id: c2779c72-4793-445c-858a-867ea8389662
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 다음에서 주문 보기 및 추적 [!DNL Channel Manager]

[!DNL Walmart Marketplace] 다음에 대한 데이터 주문 [!DNL Commerce] 제품이 자동으로 다음에 동기화됨 [!DNL Channel Manager] 이후 [!DNL Walmart] 주문을 처리합니다.

다음에서 [!DNL Commerce] 성공적으로 동기화하면 다음 작업이 트리거됩니다.

- [!DNL Channel Manager] 월마트에 주문 승인을 보냅니다.

- 해당 [!DNL Commerce] 주문은 월마트 주문에서 생성됩니다.

- 업데이트된 주문 정보는 [!DNL Channel Manager] 주문 대시보드.

Storefront 관리자로부터 주문 데이터를 볼 수 있습니다. [!DNL Channel Manager] sales channel 스토어를 열고 **[!UICONTROL Orders]**.

![관리할 채널 관리자 주문 보기 [!DNL Walmart Marketplace] 주문 수](assets/orders-dashboard-view.png){width="600" zoomable="yes"}

>[!NOTE]
>
>한 번에 최대 35분 정도 소요될 수 있습니다 [!DNL Walmart Marketplace] 에 표시할 순서 [!DNL Channel Manager] 주문 목록입니다. [!DNL Walmart] 받는 주문을 처리하고 (으)로 전송하는 데 약 30분 소요 [!DNL Channel Manager]. Channel Manager 가 주문을 받으면 Adobe Commerce 또는 Magento Open Source에서 주문을 만들고 표시하는 데 약 5분이 더 소요됩니다.

## 주문 컨트롤 및 열 설명

다음 표에서는 Orders에 사용할 수 있는 컨트롤 및 열에 대해 설명합니다.

**컨트롤[!UICONTROL Orders]**

<table>
<tr>
<td><strong>제어</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter orders]</td>
<td>다음 중 하나를 선택하여 보기 정렬 [!UICONTROL Order Status] 카드.</td>
</tr>
<tr>
<td>상태 세부 정보</td>
<td>주문 오류 및 반환 요청에 대한 정보를 제공합니다. 주문에 대한 반품 정보 및 환불 상태를 조회하려면 <strong>[!UICONTROL Return requested]</strong> 텍스트 열기 [!UICONTROL Returns] 대시보드입니다.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>주문 세부 사항을 보려면 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 를 사용합니다. [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>채널 구성을 수정하려면 채널 Walmart 연결 자격 증명, 매핑된 속성 또는 배송 식별자를 선택하고 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 를 사용합니다. [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다.</td>
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
<td>주문의 주문에 지정된 구매 주문 번호 [!DNL Walmart Marketplace]. 처음에 주문을 (으)로 가져오는 경우 [!DNL Channel Manager], 만 [!DNL Walmart] 주문 번호가 표시됩니다. 다음의 경우 [!DNL Commerce] 순서가 생성되면 [!DNL Walmart] 주문 번호는 [!UICONTROL External ID] 제품 특성입니다.</td>
</tr>
<tr>
<td>[!DNL Commerce] 주문 번호</td>
<td>에 할당된 번호 [!DNL Commerce] 다음에서 생성된 순서: [!DNL Walmart Marketplace] 주문.</td>
</tr>
<tr>
<td>항목</td>
<td>주문한 항목 수 [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Order Value]</td>
<td>주문 품목의 총 비용.</td>
</tr>
<tr>
<td>[!UICONTROL Ordered]</td>
<td>주문이 (으)로 제출된 날짜 [!DNL Walmart Marketplace] 로컬 시간대로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Ship By (timezone)]</td>
<td>주문을 납품해야 충족되는 일자 [!DNL Walmart Marketplace] 로컬 시간대로 변환된 요구 사항입니다.
</td>
</tr>
<tr>
<td>[!UICONTROL Deliver By (timezone)]</td>
<td>주문을 충족하기 위해 고객에게 납품해야 하는 일자 [!DNL Walmart Marketplace] 로컬 시간대로 변환된 요구 사항입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Ship Method]</td>
<td>다음 [[!DNL Walmart Marketplace] 배송 방법](https://sellerhelp.walmart.com/s/guide?language=en_US&amp;article=000007893%29)이 주문에 대해 선택되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Last Update]</td>
<td>주문 데이터가 마지막으로 업데이트된 시간을 나타내는 타임스탬프 [!DNL Channel Manager] 현지 시간대로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>의 현재 주문 상태를 나타냅니다. [!DNL Commerce] 주문 워크플로우입니다. 다음에서 가져온 주문에 대한 초기 상태: [!DNL Walmart Marketplace] 은(는) _Open_입니다. 다음과 같은 경우 추가 상태 업데이트가 발생합니다. [!DNL Commerce] 주문이 처리되고 [!DNL Channel Manager] 에 대한 선적, 부분 선적 및 취소 업데이트를 성공적으로 동기화합니다. [!DNL Walmart Marketplace].</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>오류가 있거나 환불 요청이 있는 주문에 대한 자세한 정보를 제공합니다.</td>
</tr>
</table>

## 주문 상태

[!UICONTROL Order Status] 의 현재 상태에 대한 정보를 제공합니다. [!DNL Walmart Marketplace] Adobe Commerce 또는 Magento Open Source에서 관리되는 주문. 주문 상태 업데이트는 다음 경우에 수행됩니다. [!DNL Channel Manager] 다음 중 하나에서 업데이트된 주문 정보를 받습니다. [!DNL Walmart Marketplace] 또는 [!DNL Commerce] 시스템 주문. 주문의 상태는 다음과 같습니다.

- **[!UICONTROL Shipped]**- 출고된 주문 [!DNL Commerce] 저장. 주문이 배송되면, [!DNL Channel Manager] (으)로 업데이트를 보냅니다. [!DNL Walmart Marketplace] 월마트에서 배송 상태를 업데이트하고 배송에 대한 주문 추적 번호를 제공합니다. 주문이 배송된 후, 월마트가 반품 승인 양식을 발행하면 주문 품목의 일부 또는 전부를 환불할 수 있습니다. 다음을 참조하십시오 [반환 및 환불](return-refund-orders.md).

- **[!UICONTROL Partially Shipped]**- 일부 품목이 출하됨으로 표시되고 다른 품목이 출하되기를 기다리는 주문 주문하신 상품이 배송될 때, [!DNL Channel Manager] (으)로 업데이트를 보냅니다. [!DNL Walmart Marketplace] 운송 상태를 다음으로 갱신하려면 _[!DNL Partially Shipped]_Walmart에서 배송에 대한 주문 추적 번호를 제공하십시오.

- **[!UICONTROL Canceled]**- 다음에서 취소된 주문 [!DNL Commerce] 저장.

   주문 취소가 완료되면 [!DNL Commerce] 반품된 품목을 반영하도록 재고 수량이 업데이트됩니다. 그런 다음, [!DNL Channel Manager] 업데이트를 로 동기화합니다. [!DNL Walmart Marketplace].

- **[!UICONTROL Return requested]**—Walmart Marketplace에서 배송된 주문 품목의 반품을 요청하는 경우 `Return requested` 에 링크가 표시됩니다. [!UICONTROL Status details] 열. 링크를 선택하면 [!UICONTROL Returns] 대시보드를 사용하여 반품을 조회하고 환불 프로세스를 관리합니다.

- **[!UICONTROL Error]**- 오류가 있는 주문입니다. 주문 업데이트 작업이 실패할 경우 오류가 발생할 수 있습니다. 예를 들어 다음과 같은 경우 오류가 발생합니다. [!DNL Channel Manager] 월마트에서 새 주문을 받을 수 없습니다. 다음과 같은 경우에도 발생할 수 있습니다. [!DNL Channel Manager] 주문 배송 또는 취소 업데이트를 다음으로 보낼 수 없음 [!DNL Walmart Marketplace]. 작업이 실패하면 [주문] 페이지에 _오류_ 주문 상태. 자세한 내용은 [주문 오류 수정](process-orders.md#fix-shipping-and-cancellation- errors).

- **[!UICONTROL Status details]**- 정보 누락 또는 잘못된 값, 잘못된 배송 세부 정보 또는 주문 취소 실패 등의 문제로 인해 발생하는 주문 오류에 대한 자세한 정보를 제공합니다. 설명은 [!DNL Commerce] 인스턴스 또는 [!DNL Walmart Marketplace].

>[!NOTE]
>
>주문 품목이 여러 배송으로 전송된 경우 주문 상태 [!DNL Channel Manager] 사용 가능한 마지막 주문 상태를 반영합니다. 예를 들어 주문 업데이트가 로 동기화될 때 첫 번째 항목이 배송되고 오류가 반환되지 않는 경우 [!DNL Channel Manager] 및 [!DNL Walmart Marketplace], [!DNL Channel Manager] 주문 상태: _[!UICONTROL Partially Shipped]_. 두 번째 품목이 출하된 경우 [!DNL Channel Manager] 오류를 반환합니다. 주문 상태가 다음으로 업데이트됩니다._[!UICONTROL Error]_.

## 주문 검토

1. 책임자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** 을(를) 열려면 [!UICONTROL Channel Manager Marketplace Stores] 페이지를 가리키도록 업데이트하는 중입니다.

1. 저장소 항목 행에서 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

1. 주문 정보를 보려면 *[!UICONTROL *Orders]**.

1. 주문에 대한 정보를 얻고 다음을 확인하여 다음 단계를 결정합니다. **[상태](#order-status)** 열.

## 주문 세부 사항 검토

마켓플레이스에서 주문을 받고 판매 채널 스토어로 가져온 후에는 [!DNL Commerce] Adobe Commerce에서 주문 세부 사항을 보기 위한 주문 ID.

출처: **[!UICONTROL Orders]**&#x200B;를 선택하고 **[!UICONTROL Commerce Order Number]** 을(를) 열려면 [!DNL Commerce] 주문 세부 사항.

![다음에 대한 상거래 주문 세부 사항 보기 [!DNL Walmart Marketplace] 주문](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

Commerce 상점 첫 화면의 [!DNL Walmart Marketplace] 주문 데이터에 다음 추가 정보가 포함되어 있습니다.

- **결제 정보 및 배송 방법**-월마트에서 임포트된 주문에는 지급 및 운송 필드에 대한 다음 값이 포함됩니다.

   - **[!UICONTROL Offline Channel Payment]**- 다음 사용자가 주문 결제를 오프라인으로 처리함을 나타냅니다. [!DNL Walmart Marketplace].

   - **[!UICONTROL External Order Number]**- 를 표시합니다. [!DNL Walmart Marketplace] 주문 번호.

   - **[!UICONTROL Channel Shipping - Value]**-배송료가 다음을 통해 처리됨을 나타냅니다. [!DNL Walmart Marketplace].

   - **[!UICONTROL Cancellation Reason]**-이 필드는에서 가져온 주문인 경우에만 표시됩니다. [!DNL Walmart Marketplace] 이(가) 취소되었습니다. 취소 사유는 다음과 같습니다.

      - [!UICONTROL Price or other listing errors.]
      - [!UICONTROL The item is out of stock.]
      - [!UICONTROL Unavailable carrier or shipping information.]
      - [!UICONTROL Additional information is required by our Credit or Fraud Avoidance department.]

- **주문한 항목**- 이 섹션에는 모든 상거래 주문에 대한 주문 항목이 나열됩니다. 다음 [!UICONTROL Qty] 열은 주문 항목에 대한 상태 기록을 제공합니다. 예를 들어 주문의 송장이 발행되고, 배송되고, 환불된 경우 상태 전환을 볼 수 있습니다.

   ![주문 상세내역 주문 품목 상태 내역 [!DNL Walmart Marketplace] 주문 수](assets/order-detail-status-history.png){width="600" zoomable="yes"}

다음을 선택하여 품목 송장 및 환불 상세내역 조회 [!UICONTROL Invoice] 및 [!UICONTROL Credit Memo] 탐색 메뉴의 옵션을 선택합니다. 다음에서 직접 대변 메모에 액세스할 수도 있습니다. [[!UICONTROL Returns]](return-refund-orders.md) 판매 채널 스토어의 대시보드입니다.
