---
title: Amazon 판매 채널 - 가격 우선 순위 논리
description: Amazon sales channel 은 Amazon 목록에 대해 공시된 가격을 결정할 때 우선 순위를 적용합니다.
feature: Sales Channels, Price Rules
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 2%

---

# 가격 우선 순위 논리

다음 예에서 시스템은 사용자가 $31.99, $24.99 또는 $27.99를 게시해야 하는지 여부를 어떻게 결정합니까?

![Commerce 가격 범위](assets/amazon-price-scope.png){width="400"}

제품이 두 웹 사이트에 있고 웹 사이트당 가격이 다른 경우 사용되는 가격을 결정하려면 가격 우선 순위 논리([정렬 순서](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 값으로 결정됨)를 사용합니다.

스토어의 정렬 순서를 보려면 _관리_ 사이드바에서 **[!UICONTROL Stores]** > **[!UICONTROL All Stores]**(으)로 이동하세요. _[!UICONTROL Web Site]_열에서 웹 사이트 이름을 클릭합니다._[!UICONTROL Web Site Information]_ 페이지에는 웹 사이트의 우선 순위를 결정하는 웹 사이트의 _[!UICONTROL Sort Order]_설정이 표시됩니다. `1` 값은 우선 순위가 가장 높음을 나타냅니다.

제품 가격이 `Use Default`(으)로 설정된 경우 웹 사이트 가격 값 대신 기본 가격 값으로 떨어집니다.

## 예 1

|         | 웹 사이트 우선 순위 | 가격(웹 사이트) | 기본값 사용 |
|---------|------------------|-----------------|-------------|
| 기본값 | 0 | US$31.99 | — |
| 스토어 1 | 1 | US$24.99 | 아니요 |
| 스토어 2 | 2 | US$27.99 | 예 |

- [가격 목록](./listing-price.md)에 정의된 **[!UICONTROL Magento Price Source]**&#x200B;이(가) `Price` 특성으로 설정되어 있습니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트([정렬 순서](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 값으로 정의되는 스토어 1)를 봅니다.
- 스토어 1이 웹 사이트 가격을 사용하도록 설정되었기 때문에(기본값 사용 = 아니요), 게시 가격은 $24.99입니다.

## 예제 2

|         | 웹 사이트 우선 순위 | 가격 웹 사이트 | 기본값 사용 |
|---------|------------------|---------------|-------------|
| 기본값 | 0 | US$31.99 | — |
| 스토어 1 | 1 | US$24.99 | 예 |
| 스토어 2 | 2 | US$27.99 | 아니요 |

- [가격 목록](./listing-price.md)에 정의된 **[!UICONTROL Magento Price Source]**&#x200B;이(가) `Price` 특성으로 설정되어 있습니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트([정렬 순서](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 값으로 정의되는 스토어 1)를 봅니다.
- 스토어 1 **은(는) 웹 사이트 가격(기본값 = 예 사용)을 사용하도록 설정되지 않았으므로 정렬 순서로 다음 웹 사이트를 봅니다.**
- 스토어 2 **is**&#x200B;이(가) 웹 사이트 가격을 사용하도록 설정되어 있으므로(기본값 사용 = 아니요) 게시 가격은 $27.99입니다.

## 예제 3

|         | 웹 사이트 우선 순위 | 가격 웹 사이트 | 기본값 사용 |
|---------|------------------|---------------|-------------|
| 기본값 | 0 | US$31.99 | 30달러 |
| 스토어 1 | 1 | US$24.99 | — |
| 스토어 2 | 2 | US$27.99 | 20달러 |

이 예제에서는 가격이 아닌 값을 추가합니다. 이 값은 [가격 나열](./listing-price.md) 설정에 정의된 _[!UICONTROL Magento Price Source_]에 대해 다른 값을 선택하는 경우 사용됩니다. 비가격 값은 항상 가격을 대체 가격으로 사용합니다.

- [[!UICONTROL Listing Price]](./listing-price.md) 설정에 정의된 **[!UICONTROL Magento Price Source]**&#x200B;이(가) `Non-Price`(으)로 설정되어 있습니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트를 봅니다. `Store 1`([정렬 순서](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/store-views.html) 값으로 정의됨).
- 저장소 1 **은(는) `Non-Price` 특성을 사용하도록 설정되지 않았으므로** 정렬 순서로 다음 웹 사이트를 살펴보십시오.
- 스토어 2 **is**&#x200B;이(가) `Non-Price` 특성(비가격 [웹 사이트] = $20.00)을 사용하도록 설정되었으므로 게시 가격은 $20.00입니다.
