---
title: 주문 설정
description: 주문 설정을 사용하여 Amazon 주문을 상거래 상점으로 가져와서 처리하는 방법을 결정합니다.
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# 주문 설정

주문 설정은 Amazon 주문을으로 가져오고 처리하는 여부와 방법을 정의합니다. [!DNL Commerce] 및에서 액세스할 수 있습니다. [대시보드 저장](./amazon-store-dashboard.md).

주문 가져오기 설정이 (으)로 설정되었습니다. `Enabled` 기본적으로, 즉, Amazon 주문이 스토어 대시보드에 표시되고 해당 주문이 생성됩니다 [!DNL Commerce] 주문. 가져온 주문은 [!DNL Commerce] [주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 워크플로입니다.

>[!NOTE]
>
>주문 설정에 관계없이 스토어 통합 전에 있었던 Amazon 주문은 가져올 수 없습니다.

다음 이후 [스토어 통합](./store-integration.md) 이(가) 완료되었습니다. 주문 설정을 변경할 수 있습니다. 주문 설정을 다음으로 설정하면 `Disabled`, Amazon 주문은 스토어 대시보드에 표시되지만 [!DNL Amazon Seller Central] 계정입니다.

Amazon에서 주문이 만들어지면 즉시 (으)로 가져오지는 않습니다 [!DNL Commerce]. Amazon에서 `Pending` 상태가 새로 생성된 주문입니다. Amazon에서 주문 및 결제 방법을 확인한 후 주문 상태가 (으)로 변경됩니다. `Unshipped`. 이 상태 변경은 주문 가져오기를 트리거하며, [!DNL Commerce] 일치하는 해당 순서를 만듭니다.

Amazon에서 가져온 주문은 [!DNL Commerce] [주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}. 참조: [주문 관리](./managing-orders.md).

## 주문 설정 구성 {#configure-order-settings}

1. 클릭 **[!UICONTROL Order Settings]** 스토어 대시보드에서 을(를) 클릭합니다.

1. 대상 **[!UICONTROL Import Amazon Orders]** (필수) 다음 옵션을 선택합니다.

   - `Disabled` - 해당 주문을 생성하지 않으려는 경우 선택합니다. [!DNL Commerce] Amazon에서 새 주문을 받는 경우. 이 옵션을 선택하면 이 페이지의 다른 모든 필드가 비활성화됩니다.

   - `Enabled` - (기본값) 해당하는 항목을 만들 시기를 선택합니다 [!DNL Commerce] Amazon에서 새 주문을 받을 때 주문합니다. [!DNL Commerce] 주문은 Amazon 상태 및 재고 수준을 기반으로 생성됩니다.

      >[!NOTE]
      >
      >Amazon 주문 가져오기는 다음으로 설정되어야 합니다. `Enabled` 에서 Amazon 주문을 관리하려면 [!DNL Commerce] [주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 워크플로입니다. 로 설정된 경우 `Disabled`, Amazon 주문에는 해당하는 이 없습니다. [!DNL Commerce] 주문 번호 및 를 관리할 수 없음 [!DNL Commerce]. 에서 이러한 주문을 관리합니다. [!DNL Amazon Seller Central] 계정입니다.

1. 대상 **[!UICONTROL Import Amazon Orders Into Magento Store]**, 선택 [!DNL Commerce] 해당 주문이 생성되는 시점과 연관된 Amazon 주문을 저장합니다. [!DNL Commerce].

   이 설정은 기본적으로 다음 경우에 선택한 웹 사이트에 대한 스토어 보기로 설정됩니다. [Amazon 스토어가 추가됨](./store-integration.md). 이 설정을 변경하려면 옵션 목록은 [!DNL Commerce] 구성에 설정한 저장소입니다. 다음을 참조하십시오 [스토어](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target="_blank"}.

1. 대상 **[!UICONTROL Customer Creation]**&#x200B;옵션을 선택합니다.

   - `No Customer Creation (guest)` - (기본값)에서 고객 계정을 만들지 않으려면 선택합니다. [!DNL Commerce] Amazon 주문에서 가져온 고객 데이터 사용. 선택하면, [!DNL Commerce] 에서 게스트 체크아웃을 처리하는 것과 동일한 방식으로 가져온 Amazon 주문을 처리합니다. [!DNL Commerce].

   - `Build New Customer Account` - 에서 새 고객 계정을 만들 때 선택합니다. [!DNL Commerce] Amazon 주문과 함께 가져온 고객 데이터 사용. 이 옵션은 Amazon 주문에서 고객 데이터베이스를 빌드하는 데 도움이 됩니다.

1. 대상 **[!UICONTROL Order Number Source]**&#x200B;옵션을 선택합니다.

   - `Build Using Magento Order Number` - (기본값) 고유한 을(를) 만들 시기를 선택합니다 [!DNL Commerce] 를 사용하는 해당 Amazon 주문의 주문 번호 [!DNL Commerce] 증분 할당된 주문 ID입니다.

   - `Build Using Amazon Order Number` - 만들 시기 선택 [!DNL Commerce] 해당 Amazon 지정 주문 번호를 사용하는 주문 번호.
   >[!NOTE]
   >
   >주문을 가져오면 Amazon 주문 번호가 _[!UICONTROL Recent Orders]_스토어 대시보드에 를 표시합니다. 다음 [!DNL Commerce] 에서 주문 세부 사항을 볼 때 주문 번호가 표시됩니다. [!DNL Commerce] [주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 작업 영역.

1. 대상 **[!UICONTROL Order Status]** (필수) 다음 옵션을 선택합니다.

   - `Default Order Status` - (기본값) Amazon에서 임포트한 신규 생성 주문에 신규 주문에 대해 정의된 기본 주문 상태가 지정되도록 할 시기를 선택합니다. 새 주문에 대한 기본 상태(새 주문에 대한 사용자 지정 주문 상태를 생성하지 않은 경우)는 입니다. `Pending`. 다음을 참조하십시오 [처리 주문](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

   - `Custom Order Status` - Amazon에서 임포트한 새로 생성된 주문에 기본값이 아닌 상태가 지정되도록 할 시기를 선택합니다.

   - `Processing Order Status` - 다음과 같은 경우에 활성화됨 **[!UICONTROL Order Status]** 이(가) (으)로 설정됨 `Custom Order Status`. Amazon에서 가져온 새로 생성된 주문에 사용할 상태를 선택합니다. 이 필드의 옵션은 의 기본 상태 옵션을 기반으로 합니다. [!DNL Commerce]. 다음을 참조하십시오 [주문 상태](https://docs.magento.com/user-guide/sales/order-status.html). 선택을 위해 여기에 표시할 사용자 지정 순서 상태를 만들 수도 있습니다. 사용자 지정 주문 상태를 만들려면 다음을 참조하십시오. [사용자 정의 주문 상태](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}.

1. 완료되면 다음을 클릭하십시오. **[!UICONTROL Save order settings]**.

![주문 설정](assets/amazon-order-settings.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Import Amazon Orders] | 옵션:<ul><li>**[!UICONTROL Disabled]** - 해당 주문을 생성하지 않으려는 경우 선택합니다. [!DNL Commerce] Amazon에서 새 주문을 받는 경우. 이 옵션을 선택하면 이 페이지의 다른 모든 필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - (기본값) 해당하는 항목을 만들 시기를 선택합니다 [!DNL Commerce] Amazon에서 새 주문을 받을 때 주문합니다. [!DNL Commerce] 주문은 Amazon 상태 및 재고 수준을 기반으로 생성됩니다.</li></ul><br><br>`Enabled` 에서 Amazon 주문을 관리하도록 선택해야 합니다. [!DNL Commerce]. 날짜 `Disabled` 이(가) 선택되면 Amazon 주문이 스토어 대시보드에 표시되지만 주문은 다음에서 관리되어야 합니다. [!DNL Amazon Seller Central] 계정입니다. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | 선택 [!DNL Commerce] 주문이에서 생성될 때와 연결된 Amazon 주문을 저장합니다. [!DNL Commerce] [주문 수](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workspace. This setting defaults to the Store View for the [!DNL Commerce] website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target="_blank"}. |
| [!UICONTROL Customer Creation] | 옵션:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (기본값)에서 고객 계정을 만들지 않으려면 선택합니다. [!DNL Commerce] Amazon 주문에서 가져온 고객 데이터 사용. 이 옵션을 선택하면 다음이 표시됩니다 [!DNL Commerce] 가져온 Amazon 주문을 처리하려면 게스트 체크아웃을 처리하는 것과 동일한 방식으로 하십시오.</li><li>**[!UICONTROL Build New Customer Account]** - 에서 새 고객 계정을 만들 시기를 선택합니다. [!DNL Commerce] Amazon 주문과 함께 가져온 고객 데이터를 사용하는 고객 데이터베이스. 이 옵션은 다음을 빌드하는 데 도움이 됩니다. [!DNL Commerce] Amazon 주문의 고객 데이터베이스.</li></ul> |
| 주문 번호 소스 | 옵션:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (기본값) 고유한 을(를) 만들 시기를 선택합니다 [!DNL Commerce] 를 사용하는 해당 Amazon 주문의 주문 번호 [!DNL Commerce] 증분 할당된 주문 ID입니다. </li><li>**Amazon 주문 번호를 사용하여 빌드** - 만들 시기 선택 [!DNL Commerce] 해당 Amazon 지정 주문 번호를 사용하는 주문 번호.</li></ul> |
| 보류 중인 주문 | 옵션:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - 원하지 않는 경우 선택 [!DNL Commerce] Amazon 주문의 영향을 받는 재고 수량입니다. 이행 프로세스(FBA)에 Amazon을 사용할지 여부를 선택합니다. 이 옵션을 선택하고 Amazon 주문을 받으면 주문 수량은 에 영향을 주지 않습니다. [!DNL Commerce] 재고 수량.</li><li>**[!UICONTROL Reserve Quantity]** - Amazon 주문의 주문 수량을 주문에서 &quot;예약&quot;되도록 할 때 선택합니다. [!DNL Commerce] 재고 수량. 이 옵션을 선택하고 Amazon 주문을 받으면 주문 수량이 다음에 &quot;예약됩니다&quot;. [!DNL Commerce] 다음을 방지하기 위한 재고 수량 [!DNL Commerce] &quot;과잉 판매&quot;의 주식. &quot;예약된&quot; 수량은 다음을 통해 구매할 수 없습니다. [!DNL Commerce] 가게 앞이야</li></ul> |
| [!UICONTROL Order Status] | 옵션:<ul><li>**[!UICONTROL Default Order Status]** - (기본값) Amazon에서 임포트한 신규 생성 주문에 신규 주문에 대한 기본 주문 상태를 지정할 시기를 선택합니다. 새 주문에 대한 기본 상태(새 주문에 대한 사용자 지정 주문 상태를 생성하지 않은 경우)는 입니다. `Pending`. 다음을 참조하십시오 [처리 주문](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]** - Amazon에서 임포트한 새로 생성된 주문에 기본값이 아닌 상태가 지정되도록 할 시기를 선택합니다. 선택하면, **[!UICONTROL Processing Order Status]** 을(를) 사용하면 Amazon에서 가져온 새로 생성된 주문에 사용할 상태를 선택할 수 있습니다.</li></ul> |
| [!UICONTROL Processing Orders Status] | 활성화된 경우 _[!UICONTROL Order Status]_이(가) (으)로 설정됨 `Custom Order Status`. 신규 주문에 지정할 주문 상태를 선택합니다. 이 필드의 옵션은 의 기본 상태 옵션에 따라 다릅니다. [!DNL Commerce]. 다음을 참조하십시오 [주문 상태](https://docs.magento.com/user-guide/sales/order-status.html){target="_blank"}. You can also create a custom order status to show here. To create a custom order status, see [Custom Order Status](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}. |

## [!DNL Commerce] 주문 제작

[!DNL Commerce] 주문은 다음 상태 및 재고 상태를 기준으로 Amazon 주문에 대해 생성됩니다.

### Inventory management을 사용한 주문 만들기

>[!NOTE]
>
>Adobe Commerce 및 Magento Open Source 2.3.x 통합에서만 지원됩니다.

| 이행 채널 | [!DNL Commerce] 재고 상태 | Amazon 주문 상태 | [!UICONTROL Create Magento Order] 설정 | 인벤토리 예약됨 |
|---|---|---|---|---|
| FBA | 재고 있음<br>품절<br>관리 안 함 | 보류 중 | 아니요 | 아니요 |
| FBA | 재고 있음<br>품절<br>관리 안 함 | PendingAvailability | 아니요 | 아니요 |
| FBA | 재고 있음<br>품절<br>관리 안 함 | 취소됨 | 아니요 | 아니요 |
| FBA | 재고 있음<br>품절<br>관리 안 함 | 오류 | 아니요 | 아니요 |
| FBA | 재고 있음<br>품절<br>관리 안 함 | 배송되지 않음 | 아니요 | 아니요 |
| FBA | 재고 있음<br>품절<br>관리 안 함 | 부분적으로 배송됨 | 아니요 | 아니요 |
| FBA | 재고 있음<br>관리 안 함 | 배송됨 | 예 | 아니요 |
| FBA | 품절 | 배송됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>품절<br>관리 안 함 | 보류 중 | 아니요 | 아니요 |
| FBM | 재고 있음<br>품절<br>관리 안 함 | PendingAvailability | 아니요 | 아니요 |
| FBM | 재고 있음<br>품절<br>관리 안 함 | 취소됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>품절<br>관리 안 함 | 오류 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리 안 함 | 배송되지 않음 | 예 | 예 |
| FBM | 품절 | 배송되지 않음 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리 안 함 | 부분적으로 배송됨 | 예 | 예 |
| FBM | 품절 | 부분적으로 배송됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리 안 함 | 배송됨 | 예 | 예 |
| FBM | 품절 | 배송됨 | 아니요 | 아니요 |

>[!NOTE]
>Amazon 주문을 가져오는 경우 `Partially Shipped` 또는 `Shipped` 상태, 생성된 재고 예약은 주문의 모든 품목에 대한 것입니다. Amazon 판매 채널은 이전에 배송된 품목에 대해 보상하지 않습니다.
>
>주문이 FBA(Amazon)에 의해 이행되었지만 항목이 포함된 경우 `out of stock` 상태, [!DNL Commerce] 해당 주문을 만들 수 없습니다. 이는 Inventory management 통합의 제한 사항입니다.
