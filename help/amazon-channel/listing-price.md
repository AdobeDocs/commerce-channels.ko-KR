---
title: 목록 가격
description: 가격 목록 설정을 사용하여 Amazon 목록의 가격 소스와 기본(기본값) 가격 값을 결정합니다.
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 목록 가격

[!UICONTROL Listing Price] 설정은 저장소 목록 설정의 일부입니다. 목록 설정은 [대시보드 저장](./amazon-store-dashboard.md).

이러한 설정은 [!DNL Commerce] 가격 소스로 사용할 가격책정 속성입니다. Amazon 목록의 기본(기본값) 가격 값입니다. 이러한 설정은 [가격 규칙](./pricing-rule-general-settings.md) 에 설정된 값에 따라 Amazon 목록 가격을 자동으로 조정하려면 _[!UICONTROL Magento Price Source]_.

을 구성할 수 있습니다 [가격 범위](./price-scope.md) 를 글로벌 또는 웹 사이트로 지원합니다. 가격책정 범위가 `Global`모든 스토어/웹 사이트에 대해 단일 가격 소스가 있습니다. 가격책정 범위가 `Website`를 사용하는 경우, 가격 소스는 웹 사이트 가격의 폴백 로직(사용 가능한 경우) 다음에 기본(글로벌) 가격을 사용합니다.

목록 규칙이 둘 이상의 웹 사이트에 적용되도록 설정된 경우, 웹 사이트 가격이 사용되는 순서는 [목록 규칙](./listing-rules.md). 이러한 규칙을 사용하면 카탈로그에서 제품 가격을 정의할 수 있습니다. 웹 사이트 가격 범위를 사용 중인지 확인하려면 [카탈로그 가격 범위](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target=&quot;_blank&quot;}.

에 나열된 옵션 _[!UICONTROL Magento Price Source]_,_[!UICONTROL Minimum Advertised Price (Map)]_, 및 _[!UICONTROL Strike Through Price (MSRP)]_구성된 가격책정 속성을 포함합니다. 가격책정 속성은 다음과 같습니다 [!DNL Commerce] 저장소 소유자에 대한 카탈로그 입력 유형이 로 설정된 제품 속성 `Price`. 자세한 내용은 [속성 입력 유형](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target=&quot;_blank&quot;}.

## 목록 가격 설정 구성 {#configure-listing-price-settings}

1. 클릭 **[!UICONTROL Listing Settings]** 저장 대시보드에서

1. 를 확장합니다. _[!UICONTROL Listing Price]_섹션을 참조하십시오.

1. 대상 **[!UICONTROL Magento Price Source]** (필수) 옵션을 선택합니다.

   기본값은 입니다. `Price`. 이 설정은 Amazon 목록에 사용되는 가격 소스를 결정합니다. 사용자가 [가격 규칙](./pricing-products.md)여기서 선택한 속성에 대해 정의된 값에 규칙이 적용됩니다. 구성된 가격책정 속성을 선택할 수 있습니다. 그러나 선택한 속성이 제품에 대해 입력되지 않으면 제품의 가격 출처는 기본적으로 로 설정됩니다 `Price` 가격책정 규칙이 적용되어 게시된 Amazon 목록 가격을 결정할 때

1. **[!UICONTROL Minimum Advertised Price (MAP)**]옵션을 선택합니다.

   기본값은 선택 사항이 아닙니다. 이 설정을 사용하면 제품에 대한 최소 광고 가격(MAP)을 사용할 수 있습니다. 가격책정 속성을 정의하고 제품에 대한 목록 가격이 결정 최소 가격(가격책정 출처 및 규칙에 따라)보다 낮으면 이 값이 목록의 MAP이 됩니다. 이 설정을 사용하면 다음을 구현할 수 있습니다 [가격 규칙](./pricing-products.md)과 동시에 제품에 대한 최소 가격을 제어합니다. 목록 가격이 너무 낮게 표시되지 않도록 하려면 MAP으로 사용할 가격 속성을 선택하십시오. 그러나 선택한 가격책정 필드가 제품에 대해 정의되지 않은 경우 MAP이 사용되지 않습니다.

1. 대상 **[!UICONTROL Strike Through Price (MSRP)]**&#x200B;옵션을 선택합니다.

   기본값은 선택 사항이 아닙니다. 이 설정은 제품에 대해 제조업체의 권장 소매 가격(MSRP)으로 사용되는 가격책정 속성을 결정합니다. 목록 가격이 정의된 MSRP보다 작으면 계산된 &quot;You Save&quot; 금액 및 백분율과 함께 더 낮은 목록 가격과 함께 MSRP 가격의 취소와 함께 Amazon 목록이 표시됩니다. 그러나 선택한 가격책정 필드가 제품에 대해 정의되지 않은 경우 MSRP가 계산되지 않습니다.

   >[!NOTE]
   >
   >이 설정은 [Buy Box](./buy-box-competitor-pricing.md) 위치. 이 Buy Box은 FBA/Prime 배송, 가용성, 판매자의 성과 등 다른 요인과 함께 일반적으로 가장 좋은 가격에 제품을 상장한 판매자에게 제공됩니다.

1. 대상 **부가가치세 적용(VAT)**&#x200B;다음 옵션을 선택합니다.

   - `Disabled` - (기본값) 목록 가격에 VAT를 적용하지 않으려는 경우를 선택합니다.

   - `Enabled` - 목록 가격에 VAT를 적용할 시기를 선택합니다. VAT는 일반적으로 유럽 국가에서 판매세로 사용되며 Amazon 내에서 최종 나열된 가격에 추가됩니다. VAT는 지능형 가격책정 규칙 내에서 사용되는 목록의 최종 가격에는 적용되지 않습니다. [가격](./floor-price.md) 이(가) 히트되었습니다.
   >[!NOTE]
   >
   >유럽 연합(EU)의 기업들은 고객이 세금을 송금할 수 있도록 업무 구매자에게 송장을 보내야 한다. 이러한 송장을 생성하고 세금을 직접 계산하거나 Amazon의 VAT 계산 서비스와 같은 세금 계산 서비스를 사용할 수 있습니다. Amazon에 등록할 것을 권장합니다. [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target=&quot;_blank&quot;}. 다른 방법을 선택하면 VAT 규정 준수에 대한 책임이 있습니다.>
   >
   >Amazon에서 VAT 계산 서비스 계정을 확인하고 활성화하는 데 10~14일이 걸릴 수 있습니다.

1. 대상 **[!UICONTROL VAT Percentage]**&#x200B;를 입력합니다. VAT 요금에 대한 값을 입력합니다.

   기본값은 입니다. `0.00`. 이 값은 목록 가격에 추가할 VAT 금액을 계산하는 데 사용됩니다. If `10.2` 이 입력되면 목록 가격에 10.20% VAT가 적용됩니다. VAT(부가가치세) 적용 필드가 로 설정된 경우 이 필드가 비활성화됩니다 `Disabled`.

1. **(영국 매장만)** 대상 **[!UICONTROL Amazon Product Tax Code (PTC)]**&#x200B;다음 옵션을 선택합니다.

   - `Do Not Manage PTC` - (기본값) 제3자 세금 계산 서비스를 사용하고 있거나 이미 모든 세금 계산을 [!DNL Amazon Seller Central] 계정이 필요합니다. 선택한 경우 Amazon 판매 채널은 제품 세금 코드 정보를 [!DNL Amazon Seller Central] 계정이 필요합니다.

   - `Set Default PTC` - 모든 제품에 사용할 범용 제품 세금 코드(PTC)가 있는 경우 선택합니다. 선택한 경우 완료해야 합니다 _[!UICONTROL Default PTC]_.

      - 대상 **[!UICONTROL Default PTC]**&#x200B;을 입력합니다. 적합한 모든 Amazon 목록에 사용할 기본 PTC를 입력합니다. 기본 PTC가 [!DNL Amazon Seller Central] account, 이 필드를 비워 둡니다. 이 필드를 변경해도 기존 Amazon 목록에는 영향을 주지 않습니다. 기존 목록에 대한 기본 PTC를 변경하려면 목록을 [종료](./end-listings-manually.md) 및 새 목록이 생성되었습니다.
   >[!NOTE]
   >
   >Amazon의 VAT 계산 서비스를 사용하는 경우 제품에 대한 세금 범주를 알고 있어야 합니다. PTC는 EU에서 B2B 구매를 위한 Amazon의 세금 범주 ID 코드입니다. 자세한 내용은 [Amazon 제품 세금 코드](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}.

1. 대상 **[!UICONTROL Currency Conversion]**&#x200B;옵션을 선택합니다.

   기본값은 입니다. `Disabled`. 이러한 옵션은 [!DNL Commerce] [통화](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;} 설정. 사용 가능한 옵션이 없으면 통화 설정을 설정하십시오.

1. 완료되면 를 클릭합니다. **[!UICONTROL Save listing settings]**.

![목록 가격](assets/amazon-listing-price.png)

| 필드 | 설명 |
|--- |--- |
| [!UICONTROL Magento Price Source] | Amazon 목록을 만들 때 사용할 가격 소스를 결정합니다. 기본값은 입니다. `Price`. 다음과 같은 다른 속성을 선택하는 경우 `Amazon Price` 또는 `Special Price`에 대해 정의된 값은 Amazon 목록에 사용됩니다. 그러나 선택한 속성이 정의되지 않으면 `Price` 이 사용됩니다. |
| [!UICONTROL Minimum Advertised Price (MAP)] | 다음 [!DNL Commerce] 맵 가격책정에 대한 속성입니다. 맵 옵션을 선택하면 목록 가격이 MAP 가격보다 작은 경우 Amazon 목록이 맵 가격으로 자동으로 설정됩니다. |
| [!UICONTROL Strike Through Price (MSRP)] | 다음 [!DNL Commerce] MSRP 가격을 나타내는 속성입니다. Amazon 목록 가격이 MSRP보다 작은 경우 MSRP 가격과 목록 가격의 취소선이 표시됩니다. 이 설정은 &quot;저장&quot; 금액과 비율을 계산하는 데에도 사용되지만 이 기능은 [Buy Box](./buy-box-competitor-pricing.md) 위치. |
| [!UICONTROL Apply Value Added Tax (VAT)] | VAT는 유럽 연합의 판매자가 사용한다.<br><br>선택 `Disabled` 목록에 VAT를 추가하지 않으려면<br><br>선택 `Enabled` 그런 다음 목록 가격에 VAT를 적용할 VAT 퍼센트를 입력합니다. |
| [!UICONTROL VAT Percentage] | Amazon 목록의 목록 가격에 추가할 VAT 금액을 계산하는 데 사용할 백분율을 정의합니다. <br><br>을 입력하면 `5`그런 다음 모든 가격책정 규칙이 적용된 후 최종 목록 가격에 5% VAT가 적용됩니다. 지능형 가격책정 규칙 내에서 사용되는 목록의 최종 가격에는 VAT 세금이 적용되지 않습니다. [바닥](./floor-price.md) 또는 [천장](./optional-ceiling-price.md) 이(가) 히트되었습니다. |
| [!UICONTROL Amazon Product Tax Code (PTC)] | (영국 저장소에만 표시됨) Amazon 판매 채널이 제품 세금 코드 정보를 [!DNL Amazon Seller Central] 계정이 필요합니다. <br><br>선택 **PTC 관리 안 함** 제3자 세금 계산 서비스를 사용하거나 이미 모든 세금 계산을 [!DNL Amazon Seller Central] 계정이 필요합니다. 이 옵션으로 설정하면 Amazon 판매 채널에서 제품 세금 코드 정보를 [!DNL Amazon Seller Central] 계정이 필요합니다.<br><br>선택 **기본 PTC 설정** 모든 제품에 사용할 범용 제품 세금 코드가 있는 경우.<br><br>자세한 내용은 [Amazon 제품 세금 코드](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}. |
| [!UICONTROL Default PTC] | 은 다음 경우에만 나타납니다 **Amazon 제품 세금 코드(PTC)** 가 로 설정되어 있습니다. `Set Default PTC`. 모든 적합한 Amazon 목록에 사용할 기본 PTC를 입력합니다. 기본 PTC가 [!DNL Amazon Seller Central] account, 이 필드를 비워 둡니다. <br><br>이 필드를 변경해도 기존 목록에 영향을 주지 않습니다. 목록은 [종료](./end-listings-manually.md) 및 변경 사항을 적용하려면 새로 만든 목록입니다. |
| [!UICONTROL Currency Conversion] | 다음 작업을 허용합니다. [!DNL Commerce] storefront 기본 통화를 사용하여 기본 Amazon 통화로 정확하게 변환하여 목록 가격을 적절한 통화로 게시할 수 있습니다. 통화 전환은 항상 [!DNL Commerce] 기본 통화.<br><br>기본값을 계속 볼 수 있습니다 [!DNL Commerce] 및 Amazon 통화를 사용할 수 있습니다. 기본값인 경우 [!DNL Commerce] 통화는 기본 Amazon 통화과 일치하고 통화 변환을 사용하지 않도록 둡니다.<br><br>예를 들어 [!DNL Commerce] 기본 통화는 CAD(캐나다 달러)이고 Amazon 기본 통화는 USD입니다. 통화 변환을 활성화하고 변환율 CAD를 USD로 선택해야 합니다. 제공된 옵션은 기본 제공 [!DNL Commerce] 통화 전환. 원하는 옵션이 표시되지 않으면 [통화 설정 [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;}. |

**빠른 액세스** - [!UICONTROL Listing Settings] 섹션

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
