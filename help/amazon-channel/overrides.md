---
title: 무시
description: Amazon Sales Channel은 Amazon 목록에서 무시를 적용하는 방법을 식별하고 관리하는 데 도움이 되는 무정부 항목 탭을 제공합니다.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 무시

_[!UICONTROL Overrides]_탭에는 무시를 적용한 Amazon 목록이 표시됩니다. 재정의는 정의된 값을 목록으로 설정할 수 있는 목록별 설정입니다. 목록에 적용된 무효화는 목록에 적합한 다른 정의된 목록 설정이나 규칙과 관계없이 목록에 대한 설정을 정의합니다. 목록에 재정의를 적용하면 목록이_[!UICONTROL Overrides]_ 탭에 나타납니다. 재정의에 정의된 값이 목록의 해당 열에 나타납니다. 적용할 수 있는 네 가지 유형의 무시가 있습니다. 가격, 처리 시간, 조건 및 판매자 노트

## 무시 유형

| 유형 | 설명 |
|---|---|
| 가격 | 목록에 대한 다른 모든 가격 설정을 무시하고 목록의 가격을 설정하는 재정의입니다. <br><br>**예**: 카탈로그의 특정 카테고리의 모든 제품에 적용되는 20% 할인 가격 규칙을 정의했습니다. 시장에 처음 출시되고 수요가 높은 제품이 있으므로 제품이 해당 범주에 속하더라도 목록에 적용되는 할인된 가격을 원하지 않습니다. 목록을 선택하고 [가격 대체](./creating-editing-overrides.md#edit-override-single-listing)를 생성한 다음 가격 대체에 목록 가격을 정의할 수 있습니다. |
| 처리 시간 | 목록 설정에 설정된 기본 처리 시간을 무시하고 목록의 처리 시간을 설정하는 재정의입니다.<br><br>**예**: 목록의 기본 처리 시간은 2일로 설정됩니다. 깨지기 쉬운 제품이 있고 특별한 포장 제품을 배송하기 위해서는 추가 하루가 필요합니다. 목록을 보고 [처리 시간 재정의](./creating-editing-overrides.md#edit-override-single-listing)를 만들고 3일에 처리 시간을 정의할 수 있습니다.<br><br>**참고:** 로 설정된 제품에는 사용할 수  `Fulfilled by Amazon`없습니다. |
| 조건 | 목록에 지정된 조건 속성과 관계없이 목록의 조건 값을 설정하는 재정의입니다.<br><br>**예**: 카탈로그에 있는 대부분의 제품이 새 상태이지만, 새로 단장한 상태가 됩니다. 목록을 보고 [조건 무시](./creating-editing-overrides.md#edit-override-single-listing)를 만들고 목록에 대해 새로 고침 조건을 정의할 수 있습니다.<br><br>**참고:** 로 설정된 제품에는 사용할 수  `Fulfilled by Amazon`없습니다. |
| 판매자 노트 | 목록의 _판매자 노트_ 섹션을 정의하는 재정의입니다. 이 필드를 사용하여 제품 또는 적용된 무시와 관련된 추가 정보를 추가할 수 있으며, 일반적으로 &quot;새 제품이 아닌&quot; 제품의 조건을 설명하는 데 사용됩니다. 이 필드의 텍스트는 구매자 목록과 함께 표시됩니다. 조건 값이 `New`인 목록에 판매자 메모를 추가할 수 없습니다. <br><br>**예**: 상태가 좋은 제품이  `Refurbished` 있습니다 일반적으로 이 조건에 있는 제품에는 설명서나 문서가 포함되지 않지만, 이 제품에 대한 다른 공급자가 있으며, 이 제품에는 매뉴얼이 포함되어 있습니다. 목록을 보고 [판매자 메모 override](./creating-editing-overrides.md#edit-override-single-listing)를 작성하고, 구매자가 이 목록이 포함되어 있음을 알 수 있도록 이 설명서에 대한 고유한 텍스트 메모를 추가할 수 있습니다.<br><br>**참고**: 제품에 정의된 조건이  `New`있는 경우 판매자 노트 재지정을 입력할 수 있지만 Amazon은 제품에 대한 판매자 노트를  `New` 표시하지 않습니다. |

[단일 목록](./creating-editing-overrides.md#edit-override-single-listing)에 대한 무시를 만들거나, 편집하거나, 제거할 수 있습니다. _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ 및 _[!UICONTROL Ineligible]_탭에서_[!UICONTROL Action]_ 열의 **[!UICONTROL Select]**&#x200B;을 클릭하고 **[!UICONTROL Create Override]**&#x200B;를 선택할 수 있습니다. _[!UICONTROL Edit Overrides]_작업은 목록에 재정의가 적용되어_[!UICONTROL Overrides]_ 탭에서 표시되는 경우에만 사용할 수 있습니다.

[여러 목록](./creating-editing-overrides.md#edit-override-multiple-listings)에 대한 무시를 만들거나, 편집하거나, 제거할 수도 있습니다. _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ 및 _[!UICONTROL Ineligible]_탭에서_[!UICONTROL Action]_ 열의 **[!UICONTROL Select]**&#x200B;을 클릭하고 **[!UICONTROL Edit Listing Overrides]**&#x200B;를 선택할 수 있습니다.

무시를 제거하면 목록에 목록 설정 및 규칙으로 정의된 값을 사용할 수 있습니다.

대체를 정의할 때 하나의 대체 유형 또는 유형의 조합을 입력할 수도 있습니다.

[무시 만들기 및 편집](./creating-editing-overrides.md)을 참조하십시오.

>[!NOTE]
>
>진행 중인 목록이 있는 경우 탭 위의 메시지에 목록 수가 표시됩니다.

![무시 탭](assets/amazon-overrides.png)

Amazon 판매 채널 홈 페이지는 표시되는 데이터를 사용자 지정할 수 있는 몇 가지 일반적인 [작업 공간 컨트롤](./workspace-controls.md)을 공유합니다.

## 기본 열

| 열 | 설명 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 제품, 옵션, 가격 및 제조업체를 식별하기 위해 Amazon이 제품에 할당한 SKU(Stock Keeping Unit)입니다. |
| [!UICONTROL ASIN] | 항목을 식별하는 10자 및/또는 숫자로 된 고유한 블록입니다.<br><br>ASIN은 Amazon 표준 식별 번호를 의미합니다. ASIN은 항목을 식별하는 10자 및/또는 숫자로 이루어진 고유한 블록입니다. 장부의 경우 ASIN은 ISBN 번호와 동일하지만 다른 모든 제품의 경우 항목이 카탈로그에 업로드되면 새 ASIN이 생성됩니다. 항목에 대한 세부 정보와 함께 Amazon의 제품 세부 사항 페이지에서 ASIN 항목을 찾을 수 있습니다. |
| [!UICONTROL Condition Override] | 재정의에 정의된 새 조건입니다. 목록에 적용된 재정의가 조건 재정의가 아닌 경우 이 열에 `Not Selected`이 나타납니다. |
| [!UICONTROL Product Listing Name] | 제품의 이름입니다. |
| [!UICONTROL Seller Notes Override] | 재정의에 정의된 새 판매자 노트입니다. 목록에 적용된 재정의가 이 유형의 재정의가 아닌 경우 이 열은 비어 있습니다. |
| [!UICONTROL Handling Override] | 재정의에 정의된 새 처리 시간(일)입니다. 목록에 적용된 재정의가 처리 시간 재정의가 아닌 경우 이 열은 비어 있습니다. |
| [!UICONTROL List Price Override] | 재정의에 정의된 새 목록 가격. 목록에 적용된 대체가 가격 대체가 아닌 경우 이 열에 `N/A`이 나타납니다. |
| [!UICONTROL Action] | 특정 목록에 적용할 수 있는 사용 가능한 작업 목록입니다. 작업을 적용하려면 _[!UICONTROL Action]_열에서&#x200B;**[!UICONTROL Select]**을 클릭하고 옵션을 선택합니다.<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
