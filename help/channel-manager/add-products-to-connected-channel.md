---
title: 채널 저장소에 제품 추가
description: 카탈로그의 제품을 판매 채널에 추가하여 Marketplace 판매에 대한 제품 분류를 만듭니다
source-git-commit: 905bedaf1eacdc45b2b7f222e7703e1f7b3dfd9c
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# 채널 저장소에 제품 추가

채널 관리자에서 [!DNL Commerce] 월마트 마켓플레이스 판매 카탈로그

제품을 판매 채널에 동기화하려면 선택한 제품에 다음 속성 구성이 있어야 합니다.

- **[!UICONTROL Publish to Channel Manager]** 속성이 활성화됨

- 하나 이상의 제품 특성이 [필수 Walmart Marketplace 특성](map-product-attributes-for-matching.md)-GTIN, ISBN, ISN, UPC, EAN

선택 사항을 저장하면 채널 관리자는 제품 데이터를 채널로 가져옵니다. 이 프로세스는 최대 30분이 걸릴 수 있습니다.

## 영업 채널에 제품 추가

1. 채널 관리자 스토어와 연결된 제품 카탈로그를 엽니다.

   연결된 영업 채널 저장소에서 **제품 추가**.

   ![연결된 채널에 제품 추가](assets/add-initial-products-to-connected-channel.png)

   카탈로그가 새 탭에 열립니다.

1. 카탈로그 제품 그리드에서 Walmart Marketplace에서 판매할 제품을 선택합니다.

   ![연결된 채널로 제품 보내기](assets/select-products-from-catalog.png)

1. 를 활성화합니다 **[!UICONTROL Publish to Channel Manager]** 선택한 항목에 대한 속성입니다.

   - From **[!UICONTROL Actions]**, 선택 **[!UICONTROL Update attributes]**.

   - 로 스크롤합니다. **[!UICONTROL Publish to Channel Manager]** 속성을 설정하고 활성화합니다.

   - 제품 속성에 필요한 Walmart 제품 ID 중 하나 이상이 포함되어 있는지 확인합니다.

   - 선택 **[!UICONTROL Save]**.

   확인 메시지가 표시됩니다.

   ![카탈로그에서 판매 채널 확인 메시지로 제품 가져오기](assets/product-import-from-catalog-confirmation.png)

   업데이트가 예약되었음을 알리는 메시지가 표시되면 [큐:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] 명령을 사용하여 업데이트를 즉시 처리합니다.

   ```bash
   $ bin/magento queue:consumers:start product_action_attribute.update
   ```

1. 에서 연결된 영업 채널로 돌아갑니다. [!DNL Channel Manager].

   가져오기 작업이 완료되면, **[!UICONTROL Listings]**. 처음에는 제품이 *초안* 상태. 선택 [!UICONTROL Refresh products]**를 사용하여 테이블을 업데이트합니다.

   ![연결된 영업 채널에 가져온 제품](assets/products-in-marketplace-sales-channel.png)
