---
title: '[!DNL Amazon Sales Channel] 릴리스 노트'
description: 모든 [!DNL Amazon Sales Channel] 릴리스에 대한 정보는 릴리스 정보를 검토하십시오.
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2010'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 릴리스 정보

>[!IMPORTANT]
>
> [!DNL Amazon sales channel]은(는) 클라우드 인프라 버전 2.3.x 및 2.4.x에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce이 있는 인스턴스에 설치할 수 있습니다. 확장 프로그램은 Adobe Commerce 2.1, Magento Open Source 2.2 또는 Magento 1에서 더 이상 지원되지 않습니다.
> <br>Adobe Commerce 2.3.x 버전에서만 [!DNL Amazon sales channel] 버전 4.0.0 및 4.1.0을 지원할 수 있습니다.
> <br>[!DNL Amazon sales channel] 버전 4.2.0+는 Adobe Commerce 2.3.x 버전과 호환되지만 Adobe Commerce 2.4.x 버전에서만 지원할 수 있습니다.
>

이 릴리스 노트는 [!DNL Amazon sales channel]의 초기 릴리스에 대해 설명하고 다음을 포함합니다.

새 기능 ![개](../assets/new.svg)개
![해결된 문제](../assets/fix.svg) 수정 사항 및 개선 사항
![알려진 문제](../assets/bug.svg)알려진 문제

버전 관리, 지원 및 호환성에 대해서는 [예정된 릴리스](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)를 참조하십시오.

이 확장을 지원하는 Adobe Commerce 버전을 알아보려면 [제품 가용성](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)을 참조하세요.

## v4.5.0

*2023년 8월 30일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로 만들기](../assets/new.svg) 향상된 인증 보안을 위해 MAGI에서 변경되는 Adobe.IO API 게이트웨이를 추가했습니다. `ServicesId`은(는) 다른 [Adobe Commerce 서비스](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html)와(과) 유사한 Adobe.IO 자격 증명을 관리할 수 있는 새 UI를 제공합니다.

>[!NOTE]
>
>판매자는 [비공개 및 공개 API 키](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html)가 프로덕션에 대해 업데이트되었는지 확인해야 합니다.


![문제 해결](../assets/fix.svg) 구성 설정 문제를 식별하고 주문 생성 흐름을 해결했습니다.

## v4.4.4

*2023년 3월 7일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![문제가 해결되었습니다](../assets/fix.svg) Adobe Commerce 2.4.6 및 PHP 8.2에 대한 지원이 추가되었습니다.

![해결된 문제](../assets/fix.svg) 로그에서 소음이 감소되었습니다.

![문제를 해결했습니다](../assets/fix.svg) 끌어오기 업데이트의 안정성을 개선했습니다.

![해결된 문제](../assets/fix.svg) 단일 작업과 유사한 가져오기를 실행하거나 CLI에서 적용하는 프로세스를 간소화했습니다.

![문제를 해결했습니다](../assets/fix.svg) `magento/services-connector`에 대한 종속성을 업그레이드했습니다.

![해결된 문제](../assets/fix.svg) 국가 코드가 잘못된 영국 계정의 동기화 문제를 해결했습니다.

![해결된 문제](../assets/fix.svg) 카탈로그 제품 엔터티의 entity_type_id가 하드코딩되면 Magento 가격 Source에 문제가 발생합니다.

![문제 해결](../assets/fix.svg) 다른 인스턴스의 백엔드에서 삭제된 계정이 UI에서도 삭제되지 않도록 하는 문제가 수정되었습니다.

![해결된 문제](../assets/fix.svg) 일부 장바구니 규칙이 주문 가져오기를 중단하는 문제를 해결했습니다.

## v4.4.3

*2023년 3월 7일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![수정](../assets/fix.svg) Adobe Commerce 2.4.4에 대한 지원을 추가했습니다.

## v4.4.2

*2021년 11월 11일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![수정](../assets/fix.svg) 다른 업데이트된 확장을 지원하도록 종속성이 업데이트되었습니다.
![수정](../assets/fix.svg) PHP 8.1에 대한 지원을 추가했습니다.

## v4.4.1

*2021년 11월 11일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![수정](../assets/fix.svg) Adobe Commerce이 Amazon에서 _사용자 이름_ 필드를 받는 방식을 변경했습니다. 이전에는 _사용자 이름_ 필드에 특수 문자가 포함되어 있을 때 주문을 만드는 동안 오류가 발생했습니다. 이제 Adobe Commerce이 _사용자 이름_ 데이터를 받고 순서를 성공적으로 만들 수 있도록 특수 문자를 필터링합니다.

## v4.4.0

*2021년 4월 9일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로 만들기](../assets/new.svg) 구성에 읽기 전용 모드에 대한 지원이 추가되었습니다. [판매 채널 설정](sales-channel-settings.md)을 참조하세요.

![수정](../assets/fix.svg) 동일한 인스턴스의 여러 복사본이 동시에 업데이트를 가져올 수 있도록 데이터 흐름을 변경했습니다.

![수정](../assets/fix.svg) 계정 정보 동기화를 위한 동기화 프로세스를 변경했습니다. 원격 계정과 동기화하는 cron 작업을 추가하고 CLI 명령에 동일한 기능을 추가했습니다.

![수정](../assets/fix.svg) 더 정밀한 제어를 위해 CLI 명령 인수 및 플래그를 추가했습니다.

![수정](../assets/fix.svg) 시스템 구성에서 Cron(백그라운드 작업) Source을 수정했습니다.

![수정](../assets/fix.svg) 국가 코드가 푸에르토리코(PR)로 설정된 경우 주문을 만들 수 없는 문제를 해결했습니다.

## v4.3.0

*2021년 3월 3일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![수정](../assets/fix.svg) <!--CHAN-xxxx-->주문 세부 정보&#x200B;_기능이 다시 디자인되었으며 더 이상_&#x200B;주문 가져오기&#x200B;_설정을 사용하지 않습니다._ 이제 주문 세부 사항이 모든 주문에 대한 Amazon Sales Channel 인터페이스에 표시됩니다.

![수정](../assets/fix.svg) 관리자의 _[!UICONTROL Marketing]_메뉴에서 이름이_[!UICONTROL Amazon]_&#x200B;에서 _[!UICONTROL Amazon Sales Channel]_(으)로 변경되었습니다.

![알려진 문제](../assets/bug.svg) **중요**: Adobe Commerce 2.4.0 호환성에 대한 알려진 문제는 Adobe Commerce 2.4.1 릴리스에서 해결되었습니다.

- `error` 상태의 Amazon cron 프로세스
- 데이터베이스에 스토어를 만들 때 Commerce 2.4.0을 사용한 설치가 실패합니다
- MSI가 설치되면 제품 만들기가 실패합니다

## v4.2.0

*2021년 3월 3일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

이전 [!DNL Amazon sales channel] 버전이 설치되어 있고 Adobe Commerce을 버전 2.4.0으로 업데이트하려고 하면 Adobe Commerce 업데이트를 완료하기 전에 확장을 업데이트하라는 메시지가 표시됩니다.

![알려진 문제](../assets/bug.svg) [!DNL Amazon sales channel] 4.2.0이 버전 2.4.0과 통합되고 [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en)이(가) 활성화되면 Commerce 카탈로그에 제품을 추가할 수 없는 알려진 문제가 있습니다. 이 문제는 향후 Commerce 릴리스에서 해결될 예정입니다.

![새](../assets/new.svg) [!DNL Amazon sales channel]이(가) 텍스트 기반 주소 데이터를 수락하고 도시, 주, 우편번호를 포함한 표준화된 주소 형식에 맞게 개선되었습니다. 이 업데이트를 통해 주문 및 배송 데이터를 주소 오류 없이 Amazon과 동기화(동기화)할 수 있습니다.<br/>예를 들어 쇼핑객이 도시, 주, 우편번호를 `Escondido, californiA 92025-1501`(으)로 입력했습니다. Amazon Sales Channel은 데이터를 가져와서 표준 형식에 `Escondido, CA 92025`(으)로 일치시킨 다음 표준화된 형식으로 Amazon에 다시 동기화합니다.

![새로 만들기](../assets/new.svg)에서 PHP 7.4에 대한 지원을 추가했습니다.

![새로 만들기](../assets/new.svg) <!--CHAN-4334-->Adobe Commerce 2.4.x에 대한 지원이 추가되었습니다. 이전 버전은 Commerce 2.4.x와 호환될 수 있지만 지원되지 않습니다. 버전 호환성에 대해서는 [예정된 릴리스](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)를 참조하십시오. Adobe Commerce 2.4.0 업데이트를 완료하려면 Amazon Sales Channel을 4.2.0으로 업데이트해야 합니다.

![수정](../assets/fix.svg) <!--CHAN-4431-->영국 고객에 대해 _액세스 거부_ 오류가 발생한 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4394-->Amazon 배송 상태를 해당 Commerce 주문과 동기화할 수 없는 문제를 해결하여 주문의 배송 상태를 Commerce의 `Pending` 및 Amazon의 `Unshipped`(으)로 &quot;잠글&quot; 수 있습니다. 새로운 표준화된 주소 기능을 통해 이러한 배송 상태 오류가 해결되었습니다.

![수정](../assets/fix.svg) <!--ticket#-->실패한 주문 가져오기를 무시하도록 주문 동기화(동기화)를 업데이트했습니다. 따라서 여러 동기화 시도를 줄이고 5분마다 주문 동기화 요청이 제출되어 후속 가져오기를 처리할 수 있습니다. 동기화 오류는 오류 로그에 여전히 기록되지만 추가 로깅 기능을 위해 &quot;처리됨&quot;으로 표시됩니다. 또한 [!DNL Amazon sales channel]은(는) 이제 Commerce에서 만들지 못한 주문에 대해 수집된 초과 데이터를 자동으로 제거합니다.

![수정](../assets/fix.svg) 발견되지 않은 예외 및 확장 업데이트 오류에 대한 자세한 정보를 수집하기 위해 오류 로깅을 업데이트했습니다.

![수정](../assets/fix.svg) <!--ticket#-->누락된 _가격_ 값으로 인해 _최저 가격_ 데이터의 초기 동기화가 실패하는 문제가 해결되었습니다.

![수정](../assets/fix.svg) <!--CHAN-4410-->날짜 범위 필드가 비어 있을 때 _Amazon 주문_ 보기에서 필터링 오류를 일으킨 문제가 수정되었습니다.

![수정](../assets/fix.svg) <!--CHAN-4439-->수량 관련 재고 및 이행 동기화 오류를 일으킨 문제를 해결했습니다. 이제 확장은 Amazon과 동기화하기 전에 소수로 입력한 수량 값을 내림합니다.<br/> 예를 들어, 판매자가 수동으로 `2.5` 수량을 입력하면 확장 프로그램은 값을 `2`(으)로 반올림한 다음 업데이트된 수량을 Amazon과 동기화합니다.

## v4.1.0

*2020년 5월 7일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로 만들기](../assets/new.svg) <!--4247, 4230-->Commerce 주문 요구 사항에 맞게 주문 가져오기 프로세스를 변경했습니다. 이러한 변경 사항은 Commerce에서 가져온 주문에 대한 해당 주문을 생성하지 못하는 문제를 해결합니다. 주문 차단기 및 솔루션에 대한 자세한 내용은 [주문 관리](managing-orders.md)를 참조하십시오.

![새로 만들기](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->스토어 대시보드의 _최근 주문_ 섹션을 업데이트하고 더 많은 주문을 보기 위한 필터 옵션 및 페이지 매김 등 모든 Amazon 주문을 표시하는 새 _모든 주문_ 보기를 추가했습니다. [Amazon 스토어 대시보드](amazon-store-dashboard.md) 및 [Amazon 주문 보기](amazon-orders-all.md)를 참조하세요.

![새로 만들기](../assets/new.svg) _[!UICONTROL Recent Orders]_및_[!UICONTROL All Orders]_ 보기에서 다시 디자인된 _[!UICONTROL Amazon Orders]_테이블의_[!UICONTROL Order Notes]_ 열을 추가했습니다. _[!UICONTROL Order Notes]_이(가) 주문 가져오기에 문제가 있음을 가맹점에 알립니다. [Amazon 주문 보기](amazon-orders-all.md)를 참조하세요.

![새로 만들기](../assets/new.svg) <!--CHAN-4013-->제품 조건 매개 변수를 업데이트하여 [Amazon 갱신됨](https://sell.amazon.com/programs/renewed) 프로그램에 맞추었습니다. [갱신된 제품](renewed-products.md)을 참조하십시오.

![새로 만들기](../assets/new.svg) <!--CHAN-3680-->Amazon에서 이행된 주문에 대해 &quot;일반 데이터&quot;를 포함하도록 [Amazon 주문 세부 사항](amazon-order-details.md)을 업데이트했습니다. [이행됨](fulfilled-by.md)을(를) 참조하십시오.

![수정](../assets/fix.svg) <!--CHAN-4069-->저장소 카드의 아이콘 왜곡을 초래하는 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4165-->세션 시간이 초과된 후 _로그인_ 화면이 표시되지 않도록 하는 오류를 수정했습니다.

![수정](../assets/fix.svg) <!--CHAN-4211-->Amazon 주문 세액을 새 Commerce 주문으로 가져올 수 없는 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4234-->스토어 대시보드에 표시된 매출 합계에 `Canceled` 또는 `Error` 상태의 주문이 포함되는 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4326-->주문을 만드는 데 _Magento Shipping_ 메서드를 사용하는 타사 확장과 관련된 주문 가져오기 오류가 발생하는 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4357-->cron 동기화를 실행할 때 오류가 발생하는 문제를 해결했습니다. CLI 명령에 잠금이 추가되어 두 cron 작업이 동시에 동기화되지 않습니다.

![수정](../assets/fix.svg) Commerce 버전 2.3.5를 지원하도록 콘텐츠 보안 정책을 업데이트했습니다.

## v4.0.0

*2020년 3월 25일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0은 Adobe Commerce 2.3.5에서 지원되지 않습니다. Adobe Commerce 2.3.5에서 지원하려면 Amazon Sales Channel 4.1.0으로 업그레이드하십시오.

![새로 만들기](../assets/new.svg) 스토어 정보에 대한 &quot;카드 보기&quot;가 개선된 새 [Amazon Sales Channel](amazon-sales-channel-home.md) 홈 페이지를 도입했습니다.

![새로 만들기](../assets/new.svg) 목록, 최근 주문 및 스토어 설정 정보가 있는 새 [스토어 대시보드](amazon-store-dashboard.md)를 도입했습니다.

![새로운 기능](../assets/new.svg) 더 빠르고 간편하게 스토어를 통합할 수 있도록 간소화된 [온보딩 프로세스](amazon-onboarding-home.md) 및 [기본 스토어 설정](default-store-settings.md)을 도입했습니다.

![알려진 문제](../assets/bug.svg) <!--CHAN-4102--> 목록에서 이미지를 가져오기 위한 [특성 만들기](managing-attributes.md) 및 **스토어 보기**&#x200B;가 `All Store Views (Global)`(으)로 설정된 경우 알려진 문제로 인해 이미지를 모든 스토어 보기로 가져올 수 없습니다. **스토어 보기(값을 가져오기 위해)**&#x200B;에 대한 설정을 특정 스토어로 변경하면 해당 스토어에 대한 이미지가 가져옵니다.

## v3.0.1

*2019년 11월 11일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![수정](../assets/fix.svg) **숫자 필드 설정**: <!--CHAN-3779-->숫자 기반 값이 필요한 필드가 숫자만 허용하도록 업데이트되었습니다. 예: 가격책정 규칙 설정 > 조정 금액 필드

![수정](../assets/fix.svg) **사용 안내서 링크**: <!--CHAN-3778-->잘못된 _사용 안내서_ 링크가 수정되었습니다.

![수정](../assets/fix.svg) **중복된 Amazon 목록**: <!--CHAN-3593-->중복된 Amazon 목록을 유발하는 이전에 보고된 문제가 이제 수정되었습니다. 이 릴리스 이전에는 목록을 가져올 때 확장 프로그램이 Amazon 지역에 대한 국가 코드를 SKU 값에 추가했습니다. 목록은 카탈로그 항목과 일치하지만, 확장은 추가된 SKU가 있는 새로운 중복 목록을 만들었습니다. 이 릴리스에서는 확장 기능이 가져온 목록의 SKU를 수정하지 않으며 기존 목록이 변경되지 않습니다. Amazon의 [!UICONTROL End Listing(s)] 옵션을 사용하여 중복 목록을 제거할 수 있습니다.

## v3.0.0

*2019년 10월 7일*

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

![새로 만들기](../assets/new.svg) **Amazon UK Marketplace 지금 사용 가능**: 사용자는 Commerce 스토어를 만들고 통합할 때 영국 마켓플레이스를 선택할 수 있습니다. 이 영국 업그레이드에는 다음에 대한 추가 지원이 포함되어 있습니다.

- [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [제품 세금 코드](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} 정보.

![새로 만들기](../assets/new.svg) **개선된 로깅**: <!--CHAN-3642, 3672-->문제 해결이 필요할 때 추가 동기화 데이터를 수집하기 위해 **디버그 로깅 사용** 기능을 구현했습니다. 구성 참조에서 [Sales Channel 설정](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) 항목을 참조하십시오.

![수정](../assets/fix.svg) **제품 카탈로그**: <!--CHAN-3687-->Amazon 목록으로 가져온 이미지가 해당 Commerce 카탈로그 제품에 적용되지 않는 문제를 해결했습니다.

![수정](../assets/fix.svg) **주문 만들기**: <!--CHAN-3708-->Commerce에서 Commerce 카탈로그 제품과 일치하지 않는 Amazon 주문에 대한 주문을 만들 수 없는 문제를 해결했습니다.

![알려진 문제](../assets/bug.svg) **Amazon 목록 복제**: <!--CHAN-3593-->이 문제로 인해 카탈로그에서는 가져온 목록에 대해 동일한 SKU를 사용하지만 끝에 지역 코드가 추가된 항목을 만듭니다. 그런 다음 Amazon은 수정된 SKU를 새 항목으로 처리하고 목록을 만듭니다. 이 문제는 향후 릴리스에서 해결될 예정입니다.

## v2.0.0

[!BADGE 지원됨]{type=Informative tooltip="지원됨"}

>[!NOTE]
>
>버전 1.0.0은 제한된 릴리스에서만 사용할 수 있습니다.

![새로 만들기](../assets/new.svg) **간소화된 온보딩 및 유지 관리**: 관리자가 제공하는 자세한 지침을 통해 단계별 프로세스를 통해 Amazon 판매자 계정을 추가하고 통합합니다. 하나의 대시보드를 통해 스토어, 계정 및 나열된 제품을 유지 관리할 수 있습니다.

![새로 만들기](../assets/new.svg) **여러 계정 지원**: 관리자를 통해 여러 Amazon 브랜드 및 마켓플레이스 지역을 관리하고 모니터링합니다.

![새로운 ](../assets/new.svg) **지능형 가격 책정**: 자동화된 가격 조정 규칙을 설정하여 탐나는 Buy Box에 대한 가능성을 높입니다. 현재 Buy Box 가격 또는 가장 낮은 경쟁업체 가격에 동적으로 조정하려면 가격을 설정하십시오. 마진을 보호하기 위해 가격 조정 제한을 설정하십시오.

![새로운 기능](../assets/new.svg) **목록 관리**: 목록 규칙을 사용하여 제품 목록을 자동화하고 Commerce 카탈로그를 Amazon 마켓플레이스에 동기화합니다. 오퍼링을 세밀하게 제어하기 위해 특정 재정의를 추가합니다. 관리자로부터 직접 모든 목록을 모니터링하고 관리합니다.

![새로 만들기](../assets/new.svg) **일관된 Inventory management**: Commerce 및 Amazon 재고 수량을 지속적으로 동기화합니다.

![새로 만들기](../assets/new.svg) **주문 및 이행 관리**: 매끄러운 통신 및 인벤토리 업데이트로 대시보드를 통해 Amazon 주문을 추적합니다. Amazon에서 이행한 주문 선적, 판매자가 이행한 주문 선적 또는 혼합 방법을 완료 및 추적합니다.

![알려진 문제](../assets/bug.svg) 제품 수량을 업데이트하는 데 더 오래 걸릴 수 있습니다. 제품 수량에 대한 업데이트는 동기화하는 데 ~2시간이 걸릴 수 있습니다.

![알려진 문제](../assets/bug.svg) 가져온 주문의 형식이 _Prime_ 또는 _Premium_ 주문일 수 있습니다. Amazon 판매자 계정에서 이러한 주문을 확인해야 합니다.

![알려진 문제](../assets/bug.svg) 부적격 번들 제품이 Amazon에서 목록에 대해 적격 상태로 표시될 수 있습니다. 번들 제품 내 제품 중 하나가 적합하지 않을 수 있습니다. 문제가 발생하면 번들 제품 항목에 대한 자격 상태를 확인하십시오.

![알려진 문제](../assets/bug.svg) Commerce 2.3.x용 Inventory management을 사용할 때 주문이 생성될 때 부분 재고 색인이 트리거되지 않을 수 있습니다. 판매 가능 수량은 시간별로 다시 계산되며, 이로 인해 이 업데이트 간격 동안 초과 판매가 발생할 수 있습니다.
