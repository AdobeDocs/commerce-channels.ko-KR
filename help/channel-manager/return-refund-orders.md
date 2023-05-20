---
title: 반품 및 환불 주문
description: '다음에서 수신된 반품 요청에 대한 전체 또는 부분 환불 발급 지침 [!DNL Walmart Marketplace] 출처: [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source.'
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 반품 및 환불 주문

구매자가 다음을 통해 구매된 주문 품목에 대한 반품을 요청할 때 [!DNL Walmart Marketplace], Walmart는 반환 요청을 생성합니다. [!DNL Channel Manager] 이러한 요청에 대해 marketplace 채널을 모니터링하고 반환 요청 정보를 Channel Manager에 자동으로 동기화합니다.

Commerce 측에서 반환 요청은 다음 워크플로우를 시작합니다.

1. Channel Manager는 수신 상태의 해당 반환 요청을 만들고 반환 ID 번호( )를 추가합니다.[!UICONTROL RMA #]) 로 이동합니다. [!UICONTROL Returns] 대시보드입니다. 다음에서 [!DNL Orders] 대시보드, 반품 업데이트와 연관된 주문에 대한 상태 세부 정보 [!UICONTROL Return requested] 반환을 보고 처리하는 링크입니다.

1. 상인은 다음 내용에 따라 대변 메모를 생성하여 반품과 관련된 환불을 처리합니다. [Adobe Commerce 환불 워크플로우](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow). 모든 환불은 오프라인 방식으로 진행됩니다.

1. [!DNL Channel Manager] Adobe Commerce에서 환불 완료를 반영하도록 반환 상태를 업데이트할 수 있도록 반환 업데이트를 Walmart marketplace에 보냅니다.

Storefront 관리자는 판매 채널 스토어를 열고 를 선택하여 Channel Manager로부터 반환을 보고 처리할 수 있습니다 **[!UICONTROL Returns]**.

![채널 관리자는에서 받은 반환 요청에 대한 반환을 처리하기 위해 대시보드를 반환합니다. [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>출하된 주문에 대한 환불만 처리할 수 있습니다. 위치 [!DNL Channel Manager], 주문 상태는 다음과 같아야 합니다. [!UICONTROL Shipped]. 위치 [!DNL Walmart Marketplace] 판매자 계정, 주문은 다음과 같아야 합니다. [!UICONTROL Delivered].

## 컨트롤 및 열 설명 반환

다음 표에서는 사용 가능한 컨트롤과 열에 대해 설명합니다. [!DNL Channel Manager] 를 반환합니다.

**컨트롤[!UICONTROL Returns]**

<table>
<tr>
<td><strong>제어</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>다음 중 하나를 선택하여 보기 필터링 [!UICONTROL Return Status] 카드.</td>
</tr>
<tr>
<td>상태 세부 정보</td>
<td>를 포함하는 반환 항목의 경우 [!UICONTROL Received] 또는 [!UICONTROL Refunded] 상태 상세내역 열에서 연결된 텍스트를 선택하여 환불에 대한 대변 메모를 생성하거나 조회할 수 있습니다.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>주문 세부 사항을 보려면 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 전자 상거래 주문을 여는 테이블입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>채널 구성을 수정하려면 채널 Walmart 연결 자격 증명, 매핑된 속성 또는 배송 식별자를 선택하고 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 를 사용합니다. [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다.</td>
</tr>
</table>

**열 설명**

<table>
<tr>
<td><strong>필드</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr>
<td>[!UICONTROL RMA #]</td>
<td>(으)로부터 수신된 반품 요청과 연관된 반품 상품 승인 번호 [!DNL Walmart Marketplace]. 이 번호는 Walmart Marketplace에서 생성됩니다. [!UICONTROL Returns] 반품 프로세스가 시작되면</td>
</tr>
<tr>
<td>[!DNL Commerce] 주문 번호</td>
<td>다음 [!DNL Commerce] Walmart Marketplace에서 반품 요청에 포함된 품목과 연계된 주문 번호. 주문 번호를 선택하여 주문 세부 사항을 조회합니다.</td>
</tr>
<tr>
<td>요청됨</td>
<td>반환이 요청된 날짜: [!DNL Walmart Marketplace]
현지 시간으로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>충족하기 위해 반환해야 하는 일자 [!DNL Walmart Marketplace] [requirements](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)가 현지 시간으로 변환되었습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>반품에 나열된 각 항목에 대한 SKU 및 수량을 나열합니다.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>반환된 항목에 대해 반환할 총 값입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>의 현재 반환 상태를 나타냅니다. [!DNL Commerce] 재방문 워크플로우-<i>받음</i>, <i>환불</i>, 또는 <i>오류</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>입고 및 환불 반품 항목의 경우 상태 상세내역은 환불 처리를 위해 대변 메모에 액세스할 수 있는 링크를 제공합니다. 다음 기간 동안 오류가 발생하는 경우 [!DNL Channel Manager] Adobe Commerce과 간의 동기화 프로세스 [!DNL Walmart marketplace], 이 필드는 오류 설명을 제공합니다.</td>
</tr>
</table>

## 반환 상태

[!UICONTROL Return Status] 의 현재 상태에 대한 정보를 제공합니다. [!DNL Walmart Marketplace] Adobe Commerce 또는 Magento Open Source에서 관리되는 반환 요청입니다.

반환 상태 업데이트는 다음 경우에 수행됩니다. [!DNL Channel Manager] 에서 반환 요청을 받습니다. [!DNL Walmart Marketplace] 또는 [!DNL Commerce] 반품된 품목에 대한 환불을 처리하기 위해 대변 메모가 생성됩니다.

반품은 다음과 같은 상태를 가질 수 있습니다.

* **[!UICONTROL Received]**-에서 받은 반환 요청의 초기 상태입니다. [!DNL Walmart Marketplace] 저장. 가맹점은 다음을 선택하여 반품 환불을 처리할 수 있습니다. **[!UICONTROL Create credit memo]** 다음에서 [!UICONTROL Status details].

* **[!UICONTROL Refunded]**- 반품된 항목에 대한 환불을 발행하기 위해 대변 메모가 생성되었음을 나타냅니다. 판매자는 다음을 선택하여 환불 정보를 볼 수 있습니다. **[!UICONTROL View credit memo]** 다음에서 [!UICONTROL Status details].

* **[!UICONTROL Error]**- 오류가 있는 요청을 반환합니다. Walmart의 반환 요청에 누락되거나 잘못된 데이터가 있을 때 오류가 발생할 수 있습니다. 또는 다음과 같은 경우 [!DNL Channel Manager] 환불 업데이트 알림을 Walmart에 보낼 수 없습니다.

## 재방문 시나리오

다음 시나리오에서는에서 다양한 유형의 반품 요청에 대해 환불을 발행하는 방법을 설명합니다 [!DNL Channel Manager].

* **전액 반환**—Walmart Marketplace 반품 요청이 주문의 모든 품목에 대한 것이면 대변 메모 수량을 업데이트하여 모든 품목을 환불합니다.

* **부분 반환**-월마트 마켓플레이스 반품 요청이 일부 주문 품목에 대해서만 적용되는 경우, 환불될 품목에 대해서만 대변 메모 수량을 갱신합니다.

* **이미 Walmart Marketplace를 통해 환불된 반품**-경우에 따라 환불 처리 [!DNL Walmart Marketplace] 채널 관리자에서 반환 을 처리하기 전에. 예를 들어 월마트에서 요구하는 48시간 환불 처리 기간 내에 커머스 주문이 환불되지 않으면 월마트가 자동으로 주문을 환불한다. 이 경우 Channel Manager는 반환 요청을 Adobe Commerce에 동기화하므로 반환을 처리하고 대변 메모를 발행할 수 있습니다. 이 워크플로우는에서 주문 세부 사항을 확인합니다. [!DNL Commerce] 는 Walmart Marketplace의 주문 정보와 일치합니다.

>[!NOTE]
>
> 환불 업데이트를 동기화하려면 최대 5분이 걸릴 수 있습니다. [!DNL Walmart Marketplace]. 다음에서 현재 반환 상태를 확인할 수 있습니다. [!DNL Channel Manager] [!UICONTROL Returns] 대시보드입니다.

## 환불 요청 처리

1. 를 엽니다. [!UICONTROL Returns] 판매 채널 스토어에 대한 대시보드.

   * 책임자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 판매 채널 스토어의 눈 모양 아이콘을 선택하여 스토어 보기를 엽니다.

   * 다음을 선택하여 결과를 검토할 수 있습니다. **[!UICONTROL Returns]** 탭.

      다음에서 반환 정보에 액세스할 수도 있습니다. [!UICONTROL Orders] 페이지를 가리키도록 업데이트하는 중입니다. 다음을 찾습니다. [!UICONTROL Shipped] 반품 요청이 있는 주문. 그런 다음 `Return requested` 링크 [!UICONTROL Status Details] 열을 사용하여 요청을 보고 처리합니다.

1. 반환 테이블에서 *[!UICONTROL Received]* 상태.

1. 품목 열에서 환불 주문 품목 및 수량 목록을 검토합니다.

1. 대변 메모를 발행하여 환불을 처리합니다.

   * 다음에서 [!UICONTROL Status Details] 열에서 선택 **[!UICONTROL Create credit memo]** 에서 주문 세부 사항 페이지를 열려면 [!DNL Commerce].

      주문이 송장 발행되지 않은 경우 주문 세부 사항 페이지에 주문 세부 사항을 생성하라는 오류 메시지가 표시됩니다. 선택 **[!UICONTROL Create invoice]**. 그런 다음, [송장 생성 및 저장](https://docs.magento.com/user-guide/sales/invoices.html).

   * 주문 세부 사항 페이지에서 **[!UICONTROL Credit Memo]**.

   * 위치 [!UICONTROL Items to Refund] 의 섹션 [!UICONTROL Credit Memo], 업데이트 **[!UICONTROL Qty to refund]** 및 **[!UICONTROL Return to Stock]** 반환 요청에 포함된 항목에 대한 정보입니다.

      반환 요청에 나열된 항목만 반환해야 합니다.

   * 댓글을 추가하려면 **[!UICONTROL Credit Memo Comments]**

   * 선택 **[!UICONTROL Refund Offline]**.

환불 완료 후, [!DNL Channel Manager] 에서 반환 상태를 업데이트합니다. [!UICONTROL Returns] 대시보드 대상 [!UICONTROL Refunded] 를 클릭하고 업데이트를 Walmart에 동기화하여 마켓플레이스에서 반환 상태를 업데이트합니다.


## 반품에 대한 환불 정보 보기

다음 위치에서 반품 요청 및 환불 처리에 대한 정보를 볼 수 있습니다. [!UICONTROL Returns] 대시보드입니다.

1. 판매 채널 스토어에 대한 반환 대시보드를 엽니다.

   * 책임자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 판매 채널 스토어의 눈 모양 아이콘을 선택하여 스토어 보기를 엽니다.

   * 선택 **[!UICONTROL Returns]**.

1. 다음을 선택하여 환불 주문 보기 **[!UICONTROL Refunded]** 상태 카드입니다.

1. 다음을 선택하여 반품에 대한 환불 세부 정보 보기 **[!UICONTROL View credit memo]**.

   ![다음에 대한 반품 항목을 환불하기 위한 대변 메모 [!DNL Walmart Marketplace] 주문](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>주문이 환불된 후 [!UICONTROL Orders] 대시보드에 반환 정보가 표시되지 않습니다. 반환 정보를 보려면 [!DNL Channel Manager] 대시보드를 반환합니다. 자세한 반품 및 환불 정보는 주문 상세 페이지에서도 확인할 수 있습니다.

## 반환 오류 수정

다음에서 반환 정보를 받을 때 오류가 발생할 수 있습니다. [!DNL Walmart Marketplace], 또는 [!DNL Channel Manager] 에서 상태 업데이트 동기화 [!DNL Commerce] 끝 [!DNL Walmart Marketplace].

반환 업데이트에 대한 동기화 작업이 실패하면 [!DNL Channel Manager] 대시보드에 다음 항목이 표시됨 반환 *[!UICONTROL Error]* 반환 항목의 상태입니다. 반품 및 환불 정보가 Walmart Marketplace 계정에 정확하게 반영되도록 하려면 [!DNL Walmart Marketplace] 저장.
