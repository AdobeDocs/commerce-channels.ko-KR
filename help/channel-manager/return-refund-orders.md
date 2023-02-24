---
title: 반품 및 환불 주문
description: '수신된 반품 요청에 대해 전체 또는 일부 환불을 실행하는 지침 [!DNL Walmart Marketplace] 변환 전: [!DNL Channel Manager] Adobe Commerce 및 Magento Open Source용.'
exl-id: 45617011-4add-444c-819b-6bb4164d03e4
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 반품 및 환불 주문

구매자가 구매 주문 품목에 대한 반품을 요청하는 경우 [!DNL Walmart Marketplace], Walmart가 반환 요청을 만듭니다. [!DNL Channel Manager] 이러한 요청에 대한 마켓플레이스 채널을 모니터링하고 반환 요청 정보를 자동으로 채널 관리자에 동기화합니다.

상거래 측에서 반환 요청이 다음 워크플로우를 시작합니다.

1. 채널 관리자는 수신된 상태로 해당 반환 요청을 만들고 반환 ID 번호( )를 추가합니다[!UICONTROL RMA #]) [!UICONTROL Returns] 대시보드 . 설정 [!DNL Orders] 대시보드, 반품 업데이트와 연관된 주문에 대한 상태 세부 정보를 포함하여 [!UICONTROL Return requested] 링크를 클릭하여 반품을 보고 처리합니다.

1. 상인은 다음과 같은 다음에 대변 메모를 생성하여 반품과 관련된 환불을 처리합니다 [Adobe Commerce 환불 워크플로우](https://docs.magento.com/user-guide/sales/credit-memos.html#refund-workflow). 모든 환불은 오프라인 방법을 사용하여 처리됩니다.

1. [!DNL Channel Manager] Walmart marketplace에 환급 업데이트를 보내 Adobe Commerce에서 완료된 환불을 반영하도록 반환 상태를 업데이트할 수 있습니다.

Storfront Admin에서는 영업 채널 저장소를 열고 를 선택하여 채널 관리자에서 반품을 보고 처리할 수 있습니다 **[!UICONTROL Returns]**.

![채널 관리자 대시보드에서 받은 반환 요청에 대한 환불을 처리하기 위해 대시보드를 반환합니다 [!DNL Walmart Marketplace]](assets/returns-dashboard-view.png)

>[!NOTE]
>
>출하 주문에 대해서만 환불을 처리할 수 있습니다. in [!DNL Channel Manager]로 지정하는 경우 주문 상태는 [!UICONTROL Shipped]. in [!DNL Walmart Marketplace] 판매자 계정입니다. 주문은 [!UICONTROL Delivered].

## 컨트롤 및 열 설명 반환

다음 표에서는 [!DNL Channel Manager] 를 반환합니다.

**컨트롤[!UICONTROL Returns]**

<table>
<tr>
<td><strong>제어</strong></td>
<td><strong>설명</strong></td>
</tr>
<tr>
<td>[!UICONTROL Filter returns]</td>
<td>다음 중 하나를 선택하여 보기를 필터링합니다 [!UICONTROL Return Status] 카드.</td>
</tr>
<tr>
<td>상태 세부 정보</td>
<td>를 사용하는 반환 항목의 경우 [!UICONTROL Received] 또는 [!UICONTROL Refunded] 상태 상세내역 열에서 링크된 텍스트를 선택하여 환불을 위한 대변 메모를 생성하거나 조회할 수 있습니다.</td>
</tr>
<tr>
<td>[!UICONTROL View order detail]</td>
<td>주문 상세내역을 조회하려면 [!DNL Commerce] 주문 번호 [!UICONTROL Order] 상거래 주문을 열 표</td>
</tr>
<tr>
<td>[!UICONTROL Channel Settings]</td>
<td>채널 구성을 수정하려면 채널 Mart 연결 자격 증명, 매핑된 속성 또는 운송 식별자를 선택합니다. [!DNL Commerce] 주문 번호 [!UICONTROL Order] 테이블. 그런 다음 [!DNL Commerce] 주문 옵션을 사용하여 주문을 처리합니다.</td>
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
<td>수신된 반환 요청과 연관된 반품 상품 인증 번호 [!DNL Walmart Marketplace]. 이 번호는 Walmart Marketplace에서 생성합니다 [!UICONTROL Returns] 반환 프로세스가 시작되면</td>
</tr>
<tr>
<td>[!DNL Commerce] 주문 번호</td>
<td>다음 [!DNL Commerce] Walmart Marketplace의 반환 요청에 포함된 항목과 연관된 주문 번호입니다. 주문 번호를 선택하여 주문 상세내역을 조회합니다.</td>
</tr>
<tr>
<td>요청</td>
<td>반환 요청 날짜 [!DNL Walmart Marketplace]
를 현지 시간으로 변환했습니다.</td>
</tr>
<tr>
<td>[!UICONTROL Return By]</td>
<td>반환이 필요한 날짜를 충족해야 합니다 [!DNL Walmart Marketplace] [요구 사항](https://sellerhelp.walmart.com/seller/s/guide?language=en_US&amp;article=000007176f)이 현지 시간으로 변환됩니다.</td>
</tr>
<tr>
<td>[!UICONTROL Items]</td>
<td>반품에 나열된 각 항목에 대한 SKU와 수량을 나열합니다.</td>
</tr>
<tr>
<td>[!UICONTROL Refund amount]</td>
<td>반품된 품목에 대해 환불되는 총 값입니다.</td>
</tr>
<tr>
<td>[!UICONTROL Status]</td>
<td>에서 현재 반환 상태를 나타냅니다. [!DNL Commerce] return workflow-<i>수신</i>, <i>환급</i>, 또는 <i>오류</i>.</td>
</tr>
<tr>
<td>[!UICONTROL Status Details]</td>
<td>입고 및 환불된 반품 입력사항에 대해 상태 세부 정보는 환급 처리를 위한 대변 메모에 액세스할 수 있는 링크를 제공합니다. 다음 중에 오류가 발생하는 경우 [!DNL Channel Manager] Adobe Commerce과 간의 동기화 프로세스 [!DNL Walmart marketplace]로 지정하는 경우 이 필드에 오류 설명이 표시됩니다.</td>
</tr>
</table>

## 반환 상태

[!UICONTROL Return Status] 의 현재 상태에 대한 정보를 제공합니다. [!DNL Walmart Marketplace] Adobe Commerce 또는 Magento Open Source에서 관리되는 요청을 반환합니다.

다음 경우에 상태 업데이트 반환 [!DNL Channel Manager] 에서 반환 요청을 받습니다. [!DNL Walmart Marketplace] 또는 [!DNL Commerce] 반환된 품목에 대한 환불을 처리하기 위해 대변 메모가 생성됩니다.

반환에는 다음 상태가 있을 수 있습니다.

* **[!UICONTROL Received]**-에서 받은 반환 요청의 초기 상태입니다. [!DNL Walmart Marketplace] 저장. 상인은 반품을 선택하고 환불을 처리할 수 있습니다 **[!UICONTROL Create credit memo]** 에서 [!UICONTROL Status details].

* **[!UICONTROL Refunded]**- 반환된 항목에 대한 환불을 발행하기 위해 대변 메모가 생성되었음을 나타냅니다. 판매자는 다음을 선택하여 환불 정보를 볼 수 있습니다 **[!UICONTROL View credit memo]** 에서 [!UICONTROL Status details].

* **[!UICONTROL Error]**- 오류가 있는 요청을 반환합니다. Walmart의 반환 요청에 데이터가 없거나 잘못된 경우 오류가 발생할 수 있습니다. 또는, [!DNL Channel Manager] 환불 갱신 통지를 월마트에 보낼 수 없습니다.

## 시나리오 반환

다음 시나리오에서는 다양한 유형의 반환 요청에 대해 환불을 발행하는 방법에 대해 설명합니다 [!DNL Channel Manager].

* **전체 반환**—Walmart Marketplace 반품 요청이 주문 중인 모든 품목에 대해 이루어진 경우 대변 메모 수량을 갱신하여 모든 품목을 환불하십시오.

* **부분 반환**-월마트 마켓플레이스 반품 요청이 일부 주문품에만 해당되는 경우, 환불할 품목에 대해서만 대변 메모 수량을 갱신하십시오.

* **Walmart Marketplace를 통해 이미 환불된 반환**&quot;어떤 경우에는 환불이 처리됩니다 [!DNL Walmart Marketplace] 채널 관리자에서 반품을 처리하기 전에 예를 들어, 월마트가 요구하는 48시간 환불 처리 기간 내에 상거래 주문이 반환되지 않으면, 월마트는 자동으로 주문을 환불 받습니다. 이런 경우 채널 관리자는 여전히 반환 요청을 Adobe Commerce에 동기화하므로 반환을 처리하고 대변 메모를 발급할 수 있습니다. 이 워크플로우에서는 주문 세부 사항이 [!DNL Commerce] walmart Marketplace의 주문 정보에 일치합니다.

>[!NOTE]
>
> 과(와) 동기화하기 위해 업데이트를 환불하는 데 최대 5분이 걸릴 수 있습니다 [!DNL Walmart Marketplace]. 에서 현재 반환 상태를 확인할 수 있습니다. [!DNL Channel Manager] [!UICONTROL Returns] 대시보드 .

## 환불 요청 처리

1. 를 엽니다. [!UICONTROL Returns] 판매 채널 저장소에 대한 대시보드 를 참조하십시오.

   * 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 판매 채널 저장소에 대한 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

   * 를 선택하여 반품을 검토할 수 있습니다 **[!UICONTROL Returns]** 탭.

      또한 [!UICONTROL Orders] 페이지. 찾기 [!UICONTROL Shipped] 반품 요청이 있는 주문. 그런 다음 `Return requested` 링크 위치 [!UICONTROL Status Details] 열을 눌러 요청을 보고 처리합니다.

1. 반환 테이블에서 *[!UICONTROL Received]* 상태.

1. 품목 열에서 환불할 주문 품목 및 수량 목록을 검토합니다.

1. 대변 메모를 발행하여 환불을 처리합니다.

   * 에서 [!UICONTROL Status Details] 열, 선택 **[!UICONTROL Create credit memo]** 주문 세부 사항 페이지를 열려면 [!DNL Commerce].

      주문에 대한 송장이 발행되지 않은 경우 주문 세부 정보 페이지에 주문 번호를 생성하라는 오류 메시지가 표시됩니다. 선택 **[!UICONTROL Create invoice]**. 그럼, [송장 생성 및 저장](https://docs.magento.com/user-guide/sales/invoices.html).

   * 주문 세부 사항 페이지에서 **[!UICONTROL Credit Memo]**.

   * in [!UICONTROL Items to Refund] 섹션 [!UICONTROL Credit Memo], 업데이트 **[!UICONTROL Qty to refund]** 및 **[!UICONTROL Return to Stock]** 반환 요청에 포함된 항목에 대한 정보입니다.

      반환 요청에 나열된 항목만 반환하도록 하십시오.

   * 설명을 추가하려면 **[!UICONTROL Credit Memo Comments]**

   * 선택 **[!UICONTROL Refund Offline]**.

환불을 완료한 후, [!DNL Channel Manager] 에서 반환 상태를 업데이트합니다. [!UICONTROL Returns] 대시보드 대상 [!UICONTROL Refunded] 그리고 업데이트를 Walmart에 동기화하여 marketplace의 반환 상태를 업데이트합니다.


## 반품에 대한 환불 정보 보기

반품 요청 및 환불 처리에 대한 정보를 [!UICONTROL Returns] 대시보드 .

1. 판매 채널 저장소에 대한 반환 대시보드를 엽니다.

   * 관리자에서 을(를) 선택합니다. **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

   * 판매 채널 저장소에 대한 눈 모양 아이콘을 선택하여 저장소 보기를 엽니다.

   * 선택 **[!UICONTROL Returns]**.

1. 을(를) 선택하여 환불 주문 보기 **[!UICONTROL Refunded]** 상태 카드

1. 다음을 선택하여 반품에 대한 환불 세부 정보를 봅니다. **[!UICONTROL View credit memo]**.

   ![반품을 위한 대변 메모 [!DNL Walmart Marketplace] 주문](assets/refund-credit-memo-for-marketplace-order.png)

>[!NOTE]
>
>주문이 반환되면, [!UICONTROL Orders] 대시보드에 반환 정보가 표시되지 않습니다. 반환 정보를 보려면 [!DNL Channel Manager] 대시보드를 반환합니다. 자세한 반품 및 환불 정보는 주문 세부 사항 페이지에서도 확인할 수 있습니다.

## 반환 오류를 수정합니다.

반환 정보를 [!DNL Walmart Marketplace]또는 [!DNL Channel Manager] 상태 업데이트 동기화 [!DNL Commerce] to [!DNL Walmart Marketplace].

반환 업데이트에 대한 동기화 작업이 실패하면 [!DNL Channel Manager] 대시보드를 보여주는 반환 *[!UICONTROL Error]* 반환 항목의 상태입니다. 반품 및 환불 정보가 Walmart Marketplace 계정에 정확하게 반영되도록 하려면 [!DNL Walmart Marketplace] 저장.
