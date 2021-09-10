---
title: Amazon 주문 세부 사항
description: Adobe 상거래 또는 Magento Open Source 관리자에서 Amazon Marketplace 주문에 대한 세부 정보를 볼 수 있습니다.
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon 주문 세부 사항

![Amazon 주문 세부 사항](assets/amazon-order-details-header.png)

## Amazon 주문 세부 사항 보기

1. 스토어 카드에서 **[!UICONTROL View Store]** 을 클릭합니다.

1. _[!UICONTROL Recent Orders]_섹션에서 주문 번호를 클릭합니다.

   _[!UICONTROL Amazon Order Details]_페이지가 열립니다.

>[!NOTE]
>
>[주문 설정](./order-settings.md)에 주문 가져오기를 활성화했으며 주문이 Amazon(FBA)](./fulfilled-by.md)에 의해 이행된 [인 경우 주문 세부 사항에 일부 필드에 대한 더미 데이터가 표시될 수 있습니다. Amazon은 FBA 주문에 대해 다음 데이터를 전송하지 않습니다.
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`


### 주문 및 운송 상세내역 탭

_[!UICONTROL Order and Shipping Details]_탭에는 Amazon에서 받은 대로 자세한 주문 정보가 표시됩니다.

>[!IMPORTANT]
>
>Amazon은 Amazon 판매 채널로 가져올 수 없는 비표준 주소 정보를 허용하므로 일부 주문에 대해 상태/국가 코드가 올바르게 업데이트되지 않습니다. 주소 오류를 수정하려면 순서 세부 사항에서 다음 필드를 편집할 수 있습니다.
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`

>
>편집 후 **주문 저장**&#x200B;을 클릭하는 것을 잊지 마십시오.

![주문 및 배송 세부 정보](assets/amazon-order-details.png)

### 주문 품목 탭

_[!UICONTROL Order Items]_탭에는 Amazon에서 받은 대로 Amazon 주문과 연관된 모든 항목이 표시됩니다.

![주문 품목 세부 정보](assets/amazon-order-item-details.png)

### 추적 탭

_[!UICONTROL Tracking]_탭에는 Amazon 주문과 연관된 추적 정보가 표시됩니다.

![추적 세부 사항](assets/amazon-order-tracking-details.png)
