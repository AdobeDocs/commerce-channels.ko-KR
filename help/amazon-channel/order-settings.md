---
title: Amazon 주문 설정
description: 주문 설정을 사용하여 Amazon 주문을 Commerce 스토어로 가져오고 처리하는 방법을 결정합니다.
feature: Sales Channels, Orders, Inventory, Configuration
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: a93ba31a95f32cc6ea285aed2399255021985693
workflow-type: tm+mt
source-wordcount: '1388'
ht-degree: 0%

---

# Amazon 주문 설정

순서 설정은 Amazon 주문을 [!DNL Commerce]로 가져와서 처리하고 [스토어 대시보드](./amazon-store-dashboard.md)에서 액세스할 수 있는지 여부와 방법을 정의합니다.

주문 가져오기 설정은 기본적으로 `Enabled`(으)로 설정되어 있습니다. 즉, Amazon 주문이 스토어 대시보드에 표시되고 해당 [!DNL Commerce]개의 주문이 만들어집니다. 가져온 주문은 [!DNL Commerce] [주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 워크플로우에서 관리할 수 있습니다.

>[!NOTE]
>
>주문 설정에 관계없이 스토어 통합 전에 있었던 Amazon 주문은 가져올 수 없습니다.

[스토어 통합](./store-integration.md)이 완료되면 주문 설정을 변경할 수 있습니다. 주문 설정을 `Disabled`(으)로 설정하면 Amazon 주문이 스토어 대시보드에 표시되지만 [!DNL Amazon Seller Central] 계정에서 관리되어야 합니다.

Amazon에서 주문이 만들어지면 [!DNL Commerce](으)로 바로 가져오지 않습니다. Amazon이 새로 만든 주문에 `Pending` 상태를 할당합니다. Amazon에서 주문 및 결제 방법을 확인한 후 주문 상태가 `Unshipped`(으)로 변경됩니다. 이 상태 변경은 순서 가져오기를 트리거하며 [!DNL Commerce]은(는) 일치하는 해당 순서를 만듭니다.

Amazon에서 가져온 주문은 [!DNL Commerce] [주문 워크플로우](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)에서 관리할 수 있습니다. [주문 관리](./managing-orders.md)도 참조하세요.

## 주문 설정 구성 {#configure-order-settings}

1. 스토어 대시보드에서 **[!UICONTROL Order Settings]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Import Amazon Orders]**(필수)에 대해 다음 옵션을 선택하십시오.

   - `Disabled` - Amazon에서 새 주문을 받을 때 [!DNL Commerce]에서 해당 주문을 만들지 않으려는 경우 선택합니다. 이 옵션을 선택하면 이 페이지의 다른 모든 필드가 비활성화됩니다.

   - `Enabled` - (기본값) Amazon에서 새 주문을 받을 때 해당 [!DNL Commerce] 주문을 만들 때 선택합니다. Amazon 상태 및 재고 수준을 기반으로 하여 [!DNL Commerce]개의 주문이 만들어집니다.

     >[!NOTE]
     >
     >[!DNL Commerce] [주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 워크플로우에서 Amazon 주문을 관리하려면 Amazon 주문 가져오기를 `Enabled`(으)로 설정해야 합니다. `Disabled`(으)로 설정된 경우 Amazon 주문에는 해당 [!DNL Commerce] 주문 번호가 없으며 [!DNL Commerce]에서 관리할 수 없습니다. [!DNL Amazon Seller Central] 계정에서 이러한 주문을 관리합니다.

1. **[!UICONTROL Import Amazon Orders Into Magento Store]**&#x200B;의 경우 [!DNL Commerce]에서 해당 순서가 만들어질 때 연결된 Amazon 주문을 저장하는 [!DNL Commerce]을(를) 선택하십시오.

   이 설정은 [Amazon 스토어를 추가](./store-integration.md)할 때 선택한 웹 사이트에 대한 스토어 보기로 기본 설정됩니다. 이 설정을 변경하려면 구성에 설정한 [!DNL Commerce] 저장소에 따라 옵션 목록이 달라집니다. [스토어](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html)를 참조하세요.

1. **[!UICONTROL Customer Creation]**&#x200B;에 대해 다음 옵션을 선택하십시오.

   - `No Customer Creation (guest)` - (기본값) Amazon 주문에서 가져온 고객 데이터를 사용하여 [!DNL Commerce]에서 고객 계정을 만들지 않으려는 경우 선택합니다. 선택한 경우 [!DNL Commerce]은(는) 가져온 Amazon 주문을 [!DNL Commerce]에서 게스트 체크아웃을 처리하는 것과 같은 방식으로 처리합니다.

   - `Build New Customer Account` - Amazon 주문과 함께 가져온 고객 데이터를 사용하여 [!DNL Commerce]에서 새 고객 계정을 만들 시기를 선택합니다. 이 옵션은 Amazon 주문에서 고객 데이터베이스를 빌드하는 데 도움이 됩니다.

1. **[!UICONTROL Order Number Source]**&#x200B;에 대해 다음 옵션을 선택하십시오.

   - `Build Using Magento Order Number` - (기본값) 점진적으로 할당된 [!DNL Commerce] 주문 ID를 사용하여 해당 Amazon 주문에 대해 고유한 [!DNL Commerce] 주문 번호를 만들려는 경우 선택합니다.

   - `Build Using Amazon Order Number` - 해당 Amazon에서 할당한 주문 번호를 사용하여 [!DNL Commerce] 주문 번호를 만들 때 선택합니다.

   >[!NOTE]
   >
   >주문을 가져오면 스토어 대시보드의 _[!UICONTROL Recent Orders]_목록에 Amazon 주문 번호가 표시됩니다. [!DNL Commerce] [주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 작업 영역에서 주문 세부 사항을 볼 때 [!DNL Commerce] 주문 번호가 표시됩니다.

1. **[!UICONTROL Order Status]**(필수)에 대해 다음 옵션을 선택하십시오.

   - `Default Order Status` - (기본값) Amazon에서 가져온 새로 만든 주문에 새 주문에 대해 정의된 기본 주문 상태를 할당할 시기를 선택합니다. 새 주문에 대한 사용자 지정 주문 상태를 만들지 않은 경우 새 주문의 기본 상태는 `Pending`입니다. [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)를 참조하세요.

   - `Custom Order Status` - Amazon에서 가져온 새로 만들어진 주문에 기본값이 아닌 다른 상태가 할당되도록 할 시기를 선택합니다.

   - `Processing Order Status` - **[!UICONTROL Order Status]**&#x200B;이(가) `Custom Order Status`(으)로 설정된 경우 활성화됩니다. Amazon에서 가져온 새로 생성된 주문에 사용할 상태를 선택합니다. 이 필드의 옵션은 [!DNL Commerce]의 기본 상태 옵션을 기반으로 합니다. [주문 상태](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html)를 참조하세요. 선택을 위해 여기에 표시할 사용자 지정 순서 상태를 만들 수도 있습니다. 사용자 지정 순서 상태를 만들려면 [사용자 지정 순서 상태](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html#custom-order-status)를 참조하세요.

1. 완료되면 **[!UICONTROL Save order settings]**&#x200B;을(를) 클릭합니다.

![순서 설정](assets/amazon-order-settings.png){width="600" zoomable="yes"}

| 필드 | 설명 |
|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | 옵션:<ul><li>**[!UICONTROL Disabled]** - Amazon에서 새 주문을 받을 때 [!DNL Commerce]에서 해당 주문을 만들지 않으려는 경우 선택합니다. 이 옵션을 선택하면 이 페이지의 다른 모든 필드가 비활성화됩니다.</li><li>**[!UICONTROL Enabled]** - (기본값) Amazon에서 새 주문을 받을 때 해당 [!DNL Commerce] 주문을 만들 때 선택합니다. Amazon 상태 및 재고 수준을 기반으로 하여 [!DNL Commerce]개의 주문이 만들어집니다.</li></ul>[!DNL Commerce]에서 Amazon 주문을 관리하려면 <br><br>`Enabled`을(를) 선택해야 합니다. `Disabled`을(를) 선택하면 Amazon 주문이 스토어 대시보드에 표시되지만 주문은 [!DNL Amazon Seller Central] 계정에서 관리되어야 합니다. |
| [!UICONTROL Import Amazon Orders Into Magento Store] | [!DNL Commerce] [주문](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) 작업 영역에서 만들 때 연결된 Amazon 주문을 저장할 [!DNL Commerce]을(를) 선택하십시오. 이 설정은 [Amazon 스토어를 추가](./store-integration.md)할 때 선택한 [!DNL Commerce] 웹 사이트에 대한 스토어 보기로 기본 설정됩니다. 이 설정을 변경하려면 구성에 설정한 [!DNL Commerce] 저장소에 따라 옵션 목록이 달라집니다. [스토어](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html)를 참조하세요. |
| [!UICONTROL Customer Creation] | 옵션:<ul><li>**[!UICONTROL No Customer Creation (guest)]** - (기본값) Amazon 주문에서 가져온 고객 데이터를 사용하여 [!DNL Commerce]에서 고객 계정을 만들지 않으려는 경우 선택합니다. 이 옵션을 선택하면 [!DNL Commerce]이(가) 게스트 체크아웃을 처리하는 것과 같은 방식으로 가져온 Amazon 주문을 처리하도록 합니다.</li><li>**[!UICONTROL Build New Customer Account]** - Amazon 주문과 함께 가져온 고객 데이터를 사용하여 [!DNL Commerce] 고객 데이터베이스에 새 고객 계정을 만들 시기를 선택합니다. 이 옵션은 Amazon 주문에서 [!DNL Commerce] 고객 데이터베이스를 빌드하는 데 도움이 됩니다.</li></ul> |
| 주문 번호 Source | 옵션:<ul><li>**[!UICONTROL Build Using Magento Order Number]** - (기본값) 점진적으로 할당된 [!DNL Commerce] 주문 ID를 사용하여 해당 Amazon 주문에 대해 고유한 [!DNL Commerce] 주문 번호를 만들려는 경우 선택합니다. </li><li>**Amazon 주문 번호를 사용하여 빌드** - 해당 Amazon에서 할당한 주문 번호를 사용하여 [!DNL Commerce] 주문 번호를 만들 때 선택합니다.</li></ul> |
| 보류 중인 주문 | 옵션:<ul><li>**[!UICONTROL Do Not Reserve Quantity]** - Amazon 주문의 영향을 받는 [!DNL Commerce] 재고 수량을 원하지 않는 경우 선택합니다. 이행 프로세스(FBA)에 Amazon을 사용할지 여부를 선택합니다. 이 옵션을 선택하면 Amazon 주문이 배송됩니다. 주문 수량은 [!DNL Commerce] 재고 수량에 영향을 주지 않습니다.</li><li>**[!UICONTROL Reserve Quantity]** - Amazon 주문의 주문 수량을 [!DNL Commerce] 재고 수량으로 &quot;예약&quot;하려는 경우 선택합니다. 이 옵션을 선택하고 Amazon 주문을 받으면 주문 수량은 [!DNL Commerce] 재고 수량으로 &quot;예약&quot;되어 [!DNL Commerce] 재고가 &quot;초과 판매&quot;되지 않도록 합니다. &quot;예약된&quot; 수량은 [!DNL Commerce] 상점 앞에서 구입할 수 없습니다.</li></ul> |
| [!UICONTROL Order Status] | 옵션:<ul><li>**[!UICONTROL Default Order Status]** - (기본값) Amazon에서 가져온 새로 만든 주문에 새 주문에 대한 기본 주문 상태를 할당할 시기를 선택합니다. 새 주문에 대한 사용자 지정 주문 상태를 만들지 않은 경우 새 주문의 기본 상태는 `Pending`입니다. [주문 처리](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)를 참조하세요.</li><li>**[!UICONTROL Custom Order Status]** - Amazon에서 가져온 새로 만들어진 주문에 기본값이 아닌 다른 상태가 할당되도록 할 시기를 선택합니다. 이 옵션을 선택하면 **[!UICONTROL Processing Order Status]**&#x200B;에서 Amazon에서 가져온 새로 생성된 주문에 사용할 상태를 선택할 수 있습니다.</li></ul> |
| [!UICONTROL Processing Orders Status] | _[!UICONTROL Order Status]_이(가) `Custom Order Status`(으)로 설정된 경우 활성화됩니다. 신규 주문에 지정할 주문 상태를 선택합니다. 이 필드의 옵션은 [!DNL Commerce]의 기본 상태 옵션에 따라 다릅니다. [주문 상태](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-status.html)를 참조하세요. 여기에 표시할 사용자 지정 주문 상태를 만들 수도 있습니다. 사용자 지정 순서 상태를 만들려면 [사용자 지정 순서 상태]를 참조하세요. |

## [!DNL Commerce] 순서 만들기

다음 상태 및 재고 상태를 기반으로 하여 Amazon 주문에 대해 [!DNL Commerce]개의 주문이 만들어집니다.

### Inventory management을 사용한 주문 만들기

>[!NOTE]
>
>Adobe Commerce 및 Magento Open Source 2.3.x 통합에서만 지원됩니다.

| 이행 채널 | [!DNL Commerce] 인벤토리 상태 | Amazon 주문 상태 | [!UICONTROL Create Magento Order] 설정 | 인벤토리 예약됨 |
|---------------------|-------------------------------------------|---------------------|-------------------------------------------|--------------------|
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | 보류 중 | 아니요 | 아니요 |
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | PendingAvailability | 아니요 | 아니요 |
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | 취소됨 | 아니요 | 아니요 |
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | 오류 | 아니요 | 아니요 |
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | 배송되지 않음 | 아니요 | 아니요 |
| FBA | 재고 있음<br>재고 부족<br>관리하지 않음 | 부분적으로 배송됨 | 아니요 | 아니요 |
| FBA | 재고 있음<br>관리하지 않음 | 배송됨 | 예 | 아니요 |
| FBA | 품절 | 배송됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>재고 부족<br>관리하지 않음 | 보류 중 | 아니요 | 아니요 |
| FBM | 재고 있음<br>재고 부족<br>관리하지 않음 | PendingAvailability | 아니요 | 아니요 |
| FBM | 재고 있음<br>재고 부족<br>관리하지 않음 | 취소됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>재고 부족<br>관리하지 않음 | 오류 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리하지 않음 | 배송되지 않음 | 예 | 예 |
| FBM | 품절 | 배송되지 않음 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리하지 않음 | 부분적으로 배송됨 | 예 | 예 |
| FBM | 품절 | 부분적으로 배송됨 | 아니요 | 아니요 |
| FBM | 재고 있음<br>관리하지 않음 | 배송됨 | 예 | 예 |
| FBM | 품절 | 배송됨 | 아니요 | 아니요 |

>[!NOTE]
>Amazon 주문을 `Partially Shipped` 또는 `Shipped` 상태로 가져오는 경우 만들어지는 인벤토리 예약은 해당 주문의 모든 항목에 대한 것입니다. Amazon 판매 채널은 이전에 배송된 품목에 대해 보상하지 않습니다.
>
>주문이 FBA(Amazon)에 의해 이행되었지만 항목이 `out of stock` 상태인 경우 [!DNL Commerce]에서 해당 주문을 만들 수 없습니다. 이는 Inventory management 통합의 제한 사항입니다.
