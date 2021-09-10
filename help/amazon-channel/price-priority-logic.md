---
title: 가격 우선순위 논리
description: Amazon 판매 채널은 Amazon 목록에 대해 게시된 가격을 결정할 때 우선 순위를 적용합니다.
exl-id: 3aa5ce5e-bb8b-4f9e-ae95-d961565474bd
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# 가격 우선순위 논리

다음 예에서는 시스템이 $31.99, $24.99 또는 $27.99를 게시해야 하는지 여부를 어떻게 결정합니까?

![상거래 가격 범위](assets/amazon-price-scope.png)

제품이 두 개의 웹 사이트에 있고 웹 사이트당 가격이 다른 경우 사용할 가격을 결정하려면 가격 우선 순위 논리( [정렬 순서](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} 값으로 결정됨)를 사용하십시오.

저장소의 정렬 순서를 보려면 _관리_ 사이드바의 **[!UICONTROL Stores]** > **[!UICONTROL All Stores]**&#x200B;으로 이동하십시오. _[!UICONTROL Web Site]_열에서 웹 사이트 이름을 클릭합니다._[!UICONTROL Web Site Information]_ 페이지에는 웹 사이트의 우선순위를 결정하는 웹 사이트에 대한 _[!UICONTROL Sort Order]_설정이 표시됩니다. `1` 값은 가장 높은 우선 순위를 나타냅니다.

제품 가격이 `Use Default`으로 설정된 경우 웹 사이트 가격 값이 아닌 기본 가격 값으로 돌아갑니다.

## 예제 1

|  | 웹 사이트 우선 순위 | 가격(웹 사이트) | 기본값 사용 |
|---|---|---|---|
| 기본값 | 0 | US$31.99 | — |
| 스토어 1 | 1 | US$24.99 | 아니요 |
| 스토어 2 | 2개 | US$27.99 | 예 |

- **[!UICONTROL Magento Price Source]**([목록 가격](./listing-price.md)에 정의됨)이 `Price` 특성으로 설정됩니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트를 확인합니다. 이 웹 사이트는 스토어 1([정렬 순서](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} 값으로 정의됨).
- 스토어 1이 웹 사이트 가격을 사용하도록 설정되어 있으므로(기본값 사용 = 아니요) 게시된 가격은 $24.99입니다.

## 예제 2

|  | 웹 사이트 우선 순위 | 가격 웹 사이트 | 기본값 사용 |
|---|---|---|---|
| 기본값 | 0 | US$31.99 | — |
| 스토어 1 | 1 | US$24.99 | 예 |
| 스토어 2 | 2개 | US$27.99 | 아니요 |

- **[!UICONTROL Magento Price Source]**([목록 가격](./listing-price.md)에 정의됨)이 `Price` 특성으로 설정됩니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트를 확인합니다. 이 웹 사이트는 스토어 1([정렬 순서](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} 값으로 정의됨)입니다.
- 스토어 1 **이 웹 사이트 가격을 사용하도록 설정된**&#x200B;이 아니므로 (기본값 사용 = 예) 정렬 순서로 다음 웹 사이트를 확인하십시오.
- 스토어 2 **이 웹 사이트 가격을 사용하도록 설정된**&#x200B;이므로(기본값 사용 = 아니요) 게시된 가격은 $27.99입니다.

## 예제 3

|  | 웹 사이트 우선 순위 | 가격 웹 사이트 | 기본값 사용 |
|---|---|---|---|
| 기본값 | 0 | US$31.99 | 30달러 |
| 스토어 1 | 1 | US$24.99 | — |
| 스토어 2 | 2개 | US$27.99 | 20달러 |

이 예에서는 _[!UICONTROL Magento Price Source_]([목록 가격](./listing-price.md) 설정에 정의됨)에 대해 다른 값을 선택하는 경우 사용되는 비가격 값을 추가합니다. 가격이 아닌 값은 항상 가격을 대체 가격으로 사용합니다.

- **[!UICONTROL Magento Price Source]**([[!UICONTROL Listing Price]](./listing-price.md) 설정에 정의됨)이 `Non-Price`로 설정됩니다.
- 웹 사이트 우선 순위가 가장 높은 웹 사이트를 봅니다. 이 웹 사이트는 `Store 1`([정렬 순서](https://docs.magento.com/user-guide/stores/stores-all-create-view.html){:target=&quot;_blank&quot;} 값으로 정의됨).
- `Non-Price` 속성을 사용하도록 Store 1 **이**&#x200B;설정되어 있지 않으므로 정렬 순서로 다음 웹 사이트를 확인하십시오.
- **스토어 2는 `Non-Price` 속성(비 가격 [웹 사이트] = $20.00)을 사용하도록 설정된 것이므로 게시된 가격은 $20.00입니다.**
