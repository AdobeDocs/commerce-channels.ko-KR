---
title: 채널 관리자에 제품 추가
description: '''에 대한 제품 조합 만들기 [!DNL Walmart Marketplace] Channel Manager''에 구성된 영업 채널에 카탈로그의 제품을 추가하여 판매합니다. '
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# 에 제품 추가 [!DNL Channel Manager]

에 제품을 추가하려면 [!DNL Walmart Marketplace] 영업 채널에서 선택 [!DNL Commerce] 제품 카탈로그를 로 가져와 [!DNL Channel Manager].
선택한 제품 수에 따라 가져오기 프로세스가 최대 30분 이상 걸릴 수 있습니다.

## 전제 조건

**[카탈로그 속성 매핑](map-catalog-attributes.md)**- [!DNL Channel Settings] 구성, 적어도 한 개의 속성을 매핑합니다 [!DNL Commerce] 필수 Walmart 제품 식별자 —-GTIN, ISBN, ISN, UPC, EAN에 대한 제품 카탈로그

## 목록 요구 사항

[!DNL Commerce] 제품 목록에는 다음 필수 속성 구성이 있어야 합니다.

- **[!UICONTROL Connect to Channel Manager]** 속성이 활성화됨

- 필수 Walmart 속성에 유효한 값을 제공합니다.

   - 필수 속성 중 하나와 일치하는 제품 속성이 하나 이상 있습니다 [!DNL Walmart Marketplace] 제품 식별자-GTIN, ISBN, ISN, UPC, EAN.

   - 예를 들어 최대 2개의 소수 자리까지 지정된 제품 가격 `9.99`

   - 예를 들어 최대 소수점 이하 두 자리로 지정된 제품 가중치 `1.25`

>[!TIP]
>
>판매 채널에 대한 목록 최적화에 대한 자세한 내용은 [Walmart Marketplace 목록 품질 최적화 안내서](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## 제품 추가

1. 연결된 영업 채널 저장소에서 **제품 추가** 를 클릭하여 제품 카탈로그를 엽니다.

   ![영업 채널 저장소에 제품 추가](assets/add-initial-products-to-connected-channel.png)

   카탈로그가 새 탭에 열립니다.

1. 카탈로그 제품 그리드에서 판매할 제품을 선택합니다 [!DNL Walmart Marketplace].

   ![판매 채널 스토어로 제품 전송](assets/select-products-from-catalog.png)

1. 를 활성화합니다 **[!UICONTROL Connect to Channel Manager]** 선택한 항목에 대한 속성입니다.

   - From **[!UICONTROL Actions]**, 선택 **[!UICONTROL Update attributes]**.

   - 로 스크롤합니다. **[!UICONTROL Connect to Channel Manager]** 속성을 설정하고 활성화합니다.

   - 제품 속성에 필요한 항목 중 하나 이상이 포함되어 있는지 확인합니다 [!DNL Walmart Product IDs].

   - 선택 **[!UICONTROL Save]**.

      확인 메시지가 표시됩니다.

      ![카탈로그에서 판매 채널 확인 메시지로 제품 가져오기](assets/product-import-from-catalog-confirmation.png)

      업데이트가 예약되었음을 알리는 메시지가 표시되면 [큐:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] 명령을 사용하여 업데이트를 즉시 처리합니다.

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. 가져오기 작업이 완료되면, [!DNL Channel Manager] 및 선택 **[!UICONTROL Listings]**.

   처음에는 제품이 *초안* 상태. 선택 **[!UICONTROL Refresh products]** 를 눌러 테이블을 업데이트합니다.

1. 보기를 업데이트하여 채널을 선택하여 채널 관리자에 추가된 새 제품을 표시합니다 **[!UICONTROL Draft]** 상태 카드

   ![연결된 영업 채널에 가져온 제품](assets/products-in-marketplace-sales-channel.png)


