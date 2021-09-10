---
title: 주문 설정
description: 주문 설정을 사용하여 Amazon 주문을 상거래 저장소로 가져오고 처리하는 방법을 결정합니다.
redirect_from: /sales-channels/asc/ob-order-settings.html: 
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 1462
ht-degree: 0%

---

# 순서 설정

순서 설정은 Amazon 주문을 [!DNL Commerce]에 가져와서 처리하는지 여부와 방법을 정의하고 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있습니다.

주문 가져오기 설정은 기본적으로 `Enabled` 로 설정되며, 이는 Amazon 주문이 저장소 대시보드에 나타나고 해당 [!DNL Commerce] 주문을 작성함을 의미합니다. 가져온 주문은 [!DNL Commerce] [주문](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} 워크플로우에서 관리할 수 있습니다.

>[!NOTE]
>
>주문 설정에 관계없이 스토어 통합 전에 존재했던 Amazon 주문은 가져올 수 없습니다.

[스토어 통합](./store-integration.md)이 완료되면 주문 설정을 변경할 수 있습니다. 주문 설정을 `Disabled`으로 설정하면 Amazon 주문이 저장소 대시보드에 표시되지만 [!DNL Amazon Seller Central] 계정에서 관리해야 합니다.

Amazon에서 주문이 만들어지면 즉시 [!DNL Commerce]으로 가져오지 않습니다. Amazon은 새로 만든 주문에 `Pending` 상태를 할당합니다. Amazon이 주문 및 결제 방법을 확인한 후 주문의 상태가 `Unshipped`으로 변경됩니다. 이 상태 변경은 주문 가져오기를 트리거하고 [!DNL Commerce]은 일치하는 해당 순서를 생성합니다.

Amazon에서 가져온 주문은 [!DNL Commerce] [주문 워크플로우](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}에서 관리할 수 있습니다. [주문 관리](./managing-orders.md)도 참조하십시오.

## 주문 설정 구성 {#configure-order-settings}

1. 저장소 대시보드에서 **[!UICONTROL Order Settings]** 을 클릭합니다.

1. **[!UICONTROL Import Amazon Orders]**(필수)에 대해 다음 옵션을 선택합니다.

   - `Disabled` - Amazon에서 새 주문을 받을  [!DNL Commerce] 때 에서 해당 주문을 만들지 않으려는 경우를 선택합니다. 선택한 경우 이 페이지의 다른 모든 필드는 비활성화됩니다.

   - `Enabled` - (기본값) Amazon에서 새 주문 [!DNL Commerce] 을 받을 때 해당 주문을 만들 시기를 선택합니다. [!DNL Commerce] 주문은 Amazon 상태 및 재고 수준을 기반으로 만들어집니다.

      >[!NOTE]
      >
      >[!DNL Commerce] [주문](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} 워크플로우에서 Amazon 주문을 관리하려면 Amazon 주문 가져오기를 `Enabled`로 설정해야 합니다. `Disabled`으로 설정하면 Amazon 주문에 해당하는 [!DNL Commerce] 주문 번호가 없으므로 [!DNL Commerce]에서 관리할 수 없습니다. 이러한 주문은 [!DNL Amazon Seller Central] 계정에서 관리합니다.

1. **[!UICONTROL Import Amazon Orders Into Magento Store]**&#x200B;에 대해 [!DNL Commerce]에서 해당 순서가 만들어질 때 Amazon 주문이 연결된 [!DNL Commerce]을 선택합니다.

   이 설정은 [Amazon store](./store-integration.md)를 추가할 때 선택한 웹 사이트에 대한 스토어 보기 로 설정됩니다. 이 설정을 변경하려면 옵션 목록은 구성에 설정한 [!DNL Commerce] 저장소에 따라 다릅니다. [저장소](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){:target=&quot;_blank&quot;}를 참조하십시오.

1. **[!UICONTROL Customer Creation]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - `No Customer Creation (guest)` - (기본값) Amazon 주문에서 가져온 고객 데이터를  [!DNL Commerce] 사용하여 고객 계정을 만들지 않으려는 경우를 선택합니다. 선택한 경우, [!DNL Commerce]은 [!DNL Commerce]에서 게스트 체크아웃을 처리하는 것과 동일한 방식으로 가져온 Amazon 순서를 처리합니다.

   - `Build New Customer Account` - Amazon 주문과 함께 가져온 고객 데이터를  [!DNL Commerce] 사용하여 새 고객 계정을 만들 시기를 선택합니다. 이 옵션은 Amazon 주문에서 고객 데이터베이스를 빌드하는 데 도움이 됩니다.

1. **[!UICONTROL Order Number Source]**&#x200B;에 대해 다음 옵션을 선택합니다.

   - `Build Using Magento Order Number` - (기본값) 점진적으로 지정된 주문 ID를  [!DNL Commerce] 사용하여 해당 Amazon 주문에 대해 고유한 주문 번호를  [!DNL Commerce] 생성할 시점을 선택합니다.

   - `Build Using Amazon Order Number` - 해당 Amazon 지정  [!DNL Commerce] 주문 번호를 사용하여 주문 번호를 생성할 시점을 선택합니다.
   >[!NOTE]
   >
   >주문을 가져온 후 Amazon 주문 번호는 저장소 대시보드의 _[!UICONTROL Recent Orders]_목록에 표시됩니다. [!DNL Commerce] 주문 번호는 [!DNL Commerce] [주문](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} 작업 영역에서 주문 세부 사항을 볼 때 표시됩니다.

1. **[!UICONTROL Order Status]**(필수)에 대해 다음 옵션을 선택합니다.

   - `Default Order Status` - (기본값) Amazon에서 가져온 새로 만든 주문에 대해 정의된 기본 주문 상태를 새 주문에 지정할 시기를 선택합니다. 새 주문에 대한 기본 상태(새 주문에 대해 사용자 지정 주문 상태를 만들지 않은 경우)는 `Pending`입니다. [처리 주문](https://docs.magento.com/user-guide/sales/order-processing.html){:target=&quot;_blank&quot;}을 참조하십시오.

   - `Custom Order Status` - Amazon에서 가져온 새로 만든 주문에 기본값이 아닌 다른 상태를 지정할 시기를 선택합니다.

   - `Processing Order Status` - 이  **[!UICONTROL Order Status]** 로 설정되어 있을 때  `Custom Order Status`활성화됩니다. Amazon에서 임포트한 새로 생성된 주문에 사용할 상태를 선택합니다. 이 필드의 옵션은 [!DNL Commerce]의 기본 상태 옵션을 기반으로 합니다. [주문 상태](https://docs.magento.com/user-guide/sales/order-status.html)를 참조하십시오. 사용자 정의 주문 상태를 만들어 선택할 수 있도록 여기에 표시할 수도 있습니다. 사용자 지정 주문 상태를 만들려면 [사용자 지정 주문 상태](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}를 참조하십시오.

1. 완료되면 **[!UICONTROL Save order settings]** 을 클릭합니다.

![순서 설정](assets/amazon-order-settings.png)

| 필드 | 설명 |
|---|---|
| [!UICONTROL Import Amazon Orders] | 옵션:<ul><li>**[!UICONTROL Disabled]** - Amazon에서 새 주문을 받을  [!DNL Commerce] 때 에서 해당 주문을 만들지 않으려는 경우를 선택합니다. 선택한 경우 이 페이지의 다른 모든 필드는 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - (기본값) Amazon에서 새 주문 [!DNL Commerce] 을 받을 때 해당 주문을 만들 시기를 선택합니다. [!DNL Commerce] 주문은 Amazon 상태 및 재고 수준을 기반으로 만들어집니다.</li></ul><br><br>`Enabled` 에서 Amazon 주문을 관리하도록 선택해야 합니다  [!DNL Commerce]. `Disabled`을(를) 선택하면 Amazon 주문이 저장소 대시보드에 표시되지만 주문은 [!DNL Amazon Seller Central] 계정에서 관리해야 합니다. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | [!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} 작업 영역에서 만들 때 연결된 Amazon 주문을 저장하는 항목을 선택합니다. [!DNL Commerce] 이 설정은 [Amazon store](./store-integration.md)를 추가할 때 선택한 [!DNL Commerce] 웹 사이트에 대한 스토어 보기 로 설정됩니다. 이 설정을 변경하려면 옵션 목록은 구성에 설정한 [!DNL Commerce] 저장소에 따라 다릅니다. [저장소](https://docs.magento.com/user-guide/stores/stores-all-stores.html){:target=&quot;_blank&quot;}를 참조하십시오. |
| [!UICONTROL Customer Creation] | 옵션:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (기본값) Amazon 주문에서 가져온 고객 데이터를  [!DNL Commerce] 사용하여 고객 계정을 만들지 않으려는 경우를 선택합니다. 선택한 경우, 이 옵션은 [!DNL Commerce]에 게스트 체크아웃을 처리하는 것과 동일한 방식으로 가져온 Amazon 순서를 처리하도록 지시합니다.</li><li>**[!UICONTROL Build New Customer Account]** - Amazon 주문과 함께 가져온 고객 데이터를 사용하여  [!DNL Commerce] 고객 데이터베이스에서 새 고객 계정을 만들 시기를 선택합니다. 이 옵션은 Amazon 주문에서 [!DNL Commerce] 고객 데이터베이스를 빌드하는 데 도움이 됩니다.</li></ul> |
| 주문 번호 출처 | 옵션:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (기본값) 점진적으로 지정된 주문 ID를  [!DNL Commerce] 사용하여 해당 Amazon 주문에 대해 고유한 주문 번호를  [!DNL Commerce] 생성할 시점을 선택합니다. </li><li>**Amazon 주문 번호를 사용하여 작성**  - 해당 Amazon 지정 주문 번호를 사용하여  [!DNL Commerce] 주문 번호를 생성할 시기를 선택합니다.</li></ul> |
| 보류 중인 주문 | 옵션:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Amazon 주문에서  [!DNL Commerce] 재고 수량이 영향을 받지 않게 하려면 선택합니다. 이행 프로세스(FBA)에 Amazon을 사용하는 경우 선택합니다. 선택한 후 Amazon 주문을 받으면 주문 수량이 [!DNL Commerce] 재고 수량에 영향을 주지 않습니다.</li><li>**[!UICONTROL Reserve Quantity]** - Amazon 주문의 주문 수량이  [!DNL Commerce] 재고 수량에서 &quot;예약&quot;되도록 하려면 선택합니다. 선택한 후 Amazon 주문을 받으면 [!DNL Commerce] 재고가 &quot;초과 판매&quot;가 되지 않도록 주문된 수량이 [!DNL Commerce] 주식으로 &quot;예약&quot;됩니다. [!DNL Commerce] 스토어를 통해 구매할 수 있는 &quot;예약된&quot; 수량은 없습니다.</li></ul> |
| [!UICONTROL Order Status] | 옵션:<ul><li>**[!UICONTROL Default Order Status]** - (기본값) Amazon에서 가져온 새로 만든 주문에 새 주문에 대한 기본 주문 상태를 지정할 시기를 선택합니다. 새 주문에 대한 기본 상태(새 주문에 대해 사용자 지정 주문 상태를 만들지 않은 경우)는 `Pending`입니다. [처리 주문](https://docs.magento.com/user-guide/sales/order-processing.html)을 참조하십시오.</li><li>>**[!UICONTROL Custom Order Status]** - Amazon에서 가져온 새로 만든 주문에 기본값이 아닌 다른 상태를 지정할 시기를 선택합니다. 선택한 경우 **[!UICONTROL Processing Order Status]** 을 사용하면 Amazon에서 가져온 새로 만든 주문에 사용할 상태를 선택할 수 있습니다.</li></ul> |
| [!UICONTROL Processing Orders Status] | _[!UICONTROL Order Status]_이 `Custom Order Status`(으)로 설정되면 활성화됩니다. 신규 주문에 지정할 주문 상태를 선택합니다. 이 필드의 옵션은 [!DNL Commerce]의 기본 상태 옵션에 따라 다릅니다. [주문 상태](https://docs.magento.com/user-guide/sales/order-status.html){:target=&quot;_blank&quot;}를 참조하십시오. 여기에 표시할 사용자 지정 주문 상태를 만들 수도 있습니다. 사용자 지정 주문 상태를 만들려면 [사용자 지정 주문 상태](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}를 참조하십시오. |

## [!DNL Commerce] 주문 생성

[!DNL Commerce] 주문은 다음 상태 및 재고 조건을 기반으로 Amazon 주문에 대해 생성됩니다.

### 재고 관리를 통한 주문 생성

>[!NOTE]
>
>Adobe 상거래 및 Magento Open Source 2.3.x 통합에서만 지원됩니다.

| 이행 채널 | [!DNL Commerce] 재고 상태 | Amazon 주문 상태 | [!UICONTROL Create Magento Order] 설정 | 예약된 재고 |
|---|---|---|---|---|
| FBA | In-stock<br>재고 부족<br>관리 안 함 | 보류 중 | 아니요 | 아니요 |
| FBA | In-stock<br>재고 부족<br>관리 안 함 | PendingAvailability | 아니요 | 아니요 |
| FBA | In-stock<br>재고 부족<br>관리 안 함 | 취소됨 | 아니요 | 아니요 |
| FBA | In-stock<br>재고 부족<br>관리 안 함 | 오류 | 아니요 | 아니요 |
| FBA | In-stock<br>재고 부족<br>관리 안 함 | 미출하 | 아니요 | 아니요 |
| FBA | In-stock<br>재고 부족<br>관리 안 함 | 부분적으로 출하됨 | 아니요 | 아니요 |
| FBA | In-stock<br>관리 안 함 | 배송됨 | 예 | 아니요 |
| FBA | 재고 부족 | 배송됨 | 아니요 | 아니요 |
| FBM | In-stock<br>재고 부족<br>관리 안 함 | 보류 중 | 아니요 | 아니요 |
| FBM | In-stock<br>재고 부족<br>관리 안 함 | PendingAvailability | 아니요 | 아니요 |
| FBM | In-stock<br>재고 부족<br>관리 안 함 | 취소됨 | 아니요 | 아니요 |
| FBM | In-stock<br>재고 부족<br>관리 안 함 | 오류 | 아니요 | 아니요 |
| FBM | In-stock<br>관리 안 함 | 미출하 | 예 | 예 |
| FBM | 재고 부족 | 미출하 | 아니요 | 아니요 |
| FBM | In-stock<br>관리 안 함 | 부분적으로 출하됨 | 예 | 예 |
| FBM | 재고 부족 | 부분적으로 출하됨 | 아니요 | 아니요 |
| FBM | In-stock<br>관리 안 함 | 배송됨 | 예 | 예 |
| FBM | 재고 부족 | 배송됨 | 아니요 | 아니요 |

>[!NOTE]
>Amazon 주문을 `Partially Shipped` 또는 `Shipped` 상태로 가져오는 경우, 생성된 재고 예약은 주문의 모든 품목에 대한 것입니다. Amazon 판매 채널은 이전에 출하된 항목을 보상하지 않습니다.
>
>주문이 Amazon(FBA)에 의해 이행되었지만 항목이 `out of stock` 상태에 있는 경우 [!DNL Commerce]에서 해당 주문을 만들 수 없습니다. 이는 Inventory Management 통합의 제한입니다.
