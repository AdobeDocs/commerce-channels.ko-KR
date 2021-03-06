---
title: '''[!DNL Amazon Sales Channel] 릴리스 정보'''
description: 모든 정보에 대해서는 릴리스 노트 를 검토하십시오 [!DNL Amazon Sales Channel] 릴리스.
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: adf86495e7de53f9ee7bc916b2a7398f04e7cbd4
workflow-type: tm+mt
source-wordcount: '2130'
ht-degree: 0%

---

# 릴리스 정보

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] 클라우드 인프라 버전 2.3.x 및 2.4.x에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce을 사용하는 인스턴스에 설치할 수 있습니다. 확장은 Adobe Commerce 2.1, Magento Open Source 2.2 또는 Magento 1에서 더 이상 지원되지 않습니다.
> <br>지원 대상 [!DNL Amazon sales channel]  Adobe Commerce 2.3.x 버전의 4.0.0 및 4.1.0만 해당.
> <br>[!DNL Amazon sales channel] 버전 4.2.0+는 Adobe Commerce 2.3.x 버전과 호환되지만, Adobe Commerce 2.4.x 버전에서만 지원됩니다.

이러한 릴리스 노트는 [!DNL Amazon sales channel] 다음을 포함합니다.

![새로 만들기](../assets/new.svg) 새로운 기능
![해결된 문제](../assets/fix.svg) 수정 사항 및 향상된 기능
![알려진 문제](../assets/bug.svg) 알려진 문제

자세한 내용은 [예정된 릴리스](https://devdocs.magento.com/release/)버전 관리, 지원 및 호환성을 위한 {target=&quot;_blank&quot;}.

## v4.4.3

[!DNL Amazon sales channel]  4.4.3은 Adobe Commerce 버전 2.3.x 및 2.4.0과 호환되지만, 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.1 이상에서만 지원됩니다.

이 버전의 [!DNL Amazon sales channel] 다음 수정 사항을 포함합니다.

![수정](../assets/fix.svg) Adobe Commerce 2.4.4에 대한 지원이 추가되었습니다.

## v4.4.2

[!DNL Amazon sales channel]  4.4.2는 Adobe Commerce 버전 2.3.x 및 2.4.0과 호환되지만, 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.1 이상에서만 지원됩니다.

이 버전의 [!DNL Amazon sales channel] 다음 수정 사항을 포함합니다.

![수정](../assets/fix.svg) 업데이트된 다른 확장을 지원하도록 종속성이 업데이트되었습니다.
![수정](../assets/fix.svg) PHP 8.1에 대한 지원을 추가했습니다.

## v4.4.1

[!DNL Amazon sales channel] 4.4.1은 Adobe Commerce 버전 2.3.x 및 2.4.0과 호환되지만, 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.1 이상에서만 지원됩니다.

이 버전의 [!DNL Amazon sales channel]  다음 수정 사항을 포함합니다.

![수정](../assets/fix.svg) Adobe Commerce이 을 수신하는 방식이 변경되었습니다 _사용자 이름_ Amazon 필드. 이전에는 _사용자 이름_ 필드에 특수 문자가 포함되어 있습니다. 이제 Adobe Commerce이 _사용자 이름_ 데이터를 필터링하고 특수 문자를 필터링하여 순서를 성공적으로 만들 수 있습니다.

## v4.4.0

[!DNL Amazon sales channel] 4.4.0은 Adobe Commerce 버전 2.3.x 및 2.4.0과 호환되지만, 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.1 이상에서만 지원됩니다.

이 버전의 [!DNL Amazon sales channel] 다음 개선 사항 및 수정 사항이 포함되어 있습니다.

![새로 만들기](../assets/new.svg) 구성에 읽기 전용 모드 지원이 추가되었습니다. 자세한 내용은 [판매 채널 설정](sales-channel-settings.md).

![수정](../assets/fix.svg) 동일한 인스턴스의 여러 복사본이 동시에 업데이트를 가져올 수 있도록 데이터 흐름을 변경했습니다.

![수정](../assets/fix.svg) 계정 정보를 동기화하기 위해 동기화 프로세스를 변경했습니다. 원격 계정과 동기화할 크론 작업이 추가되고 CLI 명령에 동일한 기능이 추가되었습니다.

![수정](../assets/fix.svg) 보다 정밀한 제어를 위해 CLI 명령 인수 및 플래그를 추가했습니다.

![수정](../assets/fix.svg) 시스템 구성에서 백그라운드 작업(cron) 소스를 수정했습니다.

![수정](../assets/fix.svg) 국가 코드가 푸에르토리코(PR)로 설정되어 있을 때 주문이 생성되지 않는 문제를 수정했습니다.

## v4.3.0

[!DNL Amazon sales channel] 4.3.0은 Adobe Commerce 버전 2.3.x 및 2.4.0과 호환됩니다. 이 지원은 클라우드 인프라의 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.1+에만 사용할 수 있습니다.

이 버전의 [!DNL Amazon sales channel] 다음 개선 사항 및 수정 사항이 포함되어 있습니다.

![수정](../assets/fix.svg) <!--CHAN-xxxx-->다음 _주문 세부 사항_ 기능은 다시 디자인되었으며 더 이상 에 의존하지 않습니다 _주문 가져오기_ 설정 이제 모든 주문에 대한 Amazon Sales Channel 인터페이스에 주문 세부 사항이 표시됩니다.

![수정](../assets/fix.svg) 에서 _[!UICONTROL Marketing]_관리 메뉴의 이름이_[!UICONTROL Amazon]_ to _[!UICONTROL Amazon Sales Channel]_.

![알려진 문제](../assets/bug.svg) **중요 사항**: Adobe Commerce 2.4.0 호환성과 관련된 알려진 문제는 Adobe Commerce 2.4.1 릴리스에서 해결되었습니다.

- 의 Amazon cron 프로세스 `error` state
- 데이터베이스에 저장소를 만들 때 Commerce 2.4.0을 사용하여 설치할 수 없습니다
- MSI가 설치된 경우 제품 만들기가 실패합니다

## v4.2.0

[!DNL Amazon sales channel] 4.2.0은 Adobe Commerce 버전 2.3.x와 호환되지만 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.4.x에서만 지원됩니다. 이전 버전이 있는 경우 [!DNL Amazon sales channel] 버전이 설치되어 있고 Adobe Commerce을 버전 2.4.0으로 업데이트하려고 하면 Adobe Commerce 업데이트를 완료하기 전에 확장을 업데이트하라는 메시지가 표시됩니다.

이 버전의 [!DNL Amazon sales channel] 개선 사항 및 수정 사항과 함께 새로운 기능이 포함되어 있습니다.

![알려진 문제](../assets/bug.svg) When [!DNL Amazon sales channel] 4.2.0은 버전 2.4.0과 통합되었으며, [Inventory management](https://docs.magento.com/user-guide/catalog/inventory.html) 이 활성화되어 있으면 전자 상거래 카탈로그에 제품이 추가되지 않는 알려진 문제가 있습니다. 이 문제는 향후 상거래 릴리스에서 해결될 예정입니다.

![새로 만들기](../assets/new.svg) [!DNL Amazon sales channel] 는 텍스트 기반 주소 데이터를 적용하고 도시, 주 및 우편 번호를 포함하여 표준화된 주소 형식에 일치시키도록 개선되었습니다. 이 업데이트를 통해 주문 및 배송 데이터는 주소 오류 없이 Amazon과 동기화(동기화)할 수 있습니다.<br/>예를 들어 쇼핑객은 도시, 주, 우편 번호를 `Escondido, californiA 92025-1501`. Amazon Sales Channel을 사용하여 데이터를 가져오고 표준 형식으로 일치시킵니다. `Escondido, CA 92025`를 만든 다음 Amazon에 동기화하여 표준화된 형식으로 만듭니다.

![새로 만들기](../assets/new.svg) PHP 7.4에 대한 지원이 추가되었습니다.

![새로 만들기](../assets/new.svg) <!--CHAN-4334-->Adobe Commerce 2.4.x에 대한 지원이 추가되었습니다. 이전 버전은 Commerce 2.4.x와 호환될 수 있지만, 지원되지 않습니다. 자세한 내용은 [예정된 릴리스](https://devdocs.magento.com/release/)버전 호환성에 대한 {:target=&quot;_blank&quot;}. Adobe Commerce 2.4.0 업데이트를 완료하려면 먼저 Amazon Sales Channel을 4.2.0으로 업데이트해야 합니다.

![수정](../assets/fix.svg) <!--CHAN-4431-->을(를) 발생시킨 문제를 수정했습니다. _액세스 거부_ 라는 오류가 발생했습니다.

![수정](../assets/fix.svg) <!--CHAN-4394-->Amazon 배송 상태가 해당 상거래 주문으로 동기화되지 않아 주문의 배송 상태를 &quot;잠금&quot;으로 설정하는 문제를 수정했습니다 `Pending` 상거래 및 `Unshipped` Amazon. 새로운 표준화된 주소 기능을 사용하여 이러한 배송 상태 오류가 해결되었습니다.

![수정](../assets/fix.svg) <!--ticket#-->실패한 주문 가져오기를 무시하도록 주문 동기화(동기화)를 업데이트하여 여러 동기화 시도를 줄이고 5분마다 제출된 주문 동기화 요청을 통해 후속 가져오기를 처리할 수 있습니다. 동기화 오류는 여전히 오류 로그에 기록되지만 추가 로깅 기능을 위해 &quot;처리됨&quot;으로 표시됩니다. 또한, [!DNL Amazon sales channel] 이제 에서는 상거래에 생성되지 않은 주문에 대해 수집된 초과 데이터를 자동으로 제거합니다.

![수정](../assets/fix.svg) 발견되지 않은 예외 및 확장 업데이트 오류에 대한 자세한 정보를 수집하도록 오류 로깅이 업데이트되었습니다.

![수정](../assets/fix.svg) <!--ticket#-->의 초기 동기화를 초래한 문제를 수정했습니다 _최저 가격_ 누락으로 인해 데이터 실패 _가격_ 값.

![수정](../assets/fix.svg) <!--CHAN-4410-->에서 필터링 오류를 일으킨 문제를 수정했습니다. _Amazon 주문_ 날짜 범위 필드를 비워 두면 확인.

![수정](../assets/fix.svg) <!--CHAN-4439-->수량 관련 재고 및 이행 동기화 오류를 일으킨 문제를 수정했습니다. 이제 확장은 Amazon과 동기화하기 전에 소수 값으로 입력된 수량 값을 반올림합니다.<br/> 예를 들어 머천트가 수동으로 수량을 입력하는 경우 `2.5`를 설정하는 경우 확장은 값을 로 반올림합니다. `2` 그런 다음 업데이트된 수량을 Amazon과 동기화합니다.

## v4.1.0

Amazon Sales Channel 4.1.0은 클라우드 인프라에서 Commerce Open Source, Adobe Commerce 및 Adobe Commerce의 Adobe Commerce 2.3.x와 호환됩니다. 이 버전의 Amazon Sales Channel에는 사소한 버그 수정과 함께 사용자 인터페이스 개선 사항이 포함되어 있습니다.

![새로 만들기](../assets/new.svg) <!--4247, 4230-->상거래 주문 요구 사항에 맞게 주문 가져오기 프로세스를 변경했습니다. 이러한 변경 사항은 Commerce가 가져온 주문에 대해 해당 순서를 만들지 못하는 문제를 해결합니다. 자세한 내용은 [주문 관리](managing-orders.md) 주문 차단기 및 솔루션에 대한 자세한 정보

![새로 만들기](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->업데이트 날짜: _최근 주문_ 저장소 대시보드의 섹션을 새로 추가했습니다 _모든 주문_ 더 많은 주문을 보기 위한 필터 옵션 및 페이지 매김을 포함하여 모든 Amazon 주문을 표시하는 보기. 자세한 내용은 [Amazon 스토어 대시보드](amazon-store-dashboard.md) 및 [Amazon 주문 보기](amazon-orders-all.md).

![새로 만들기](../assets/new.svg) 가 추가되었습니다. _[!UICONTROL Order Notes]_재설계된 열의 열_[!UICONTROL Amazon Orders]_ 두 테이블 모두 _[!UICONTROL Recent Orders]_및_[!UICONTROL All Orders]_ 보기. _[!UICONTROL Order Notes]_상인에게 주문품의 수입에 문제가 있음을 알려주세요. 자세한 내용은 [Amazon 주문 보기](amazon-orders-all.md).

![새로 만들기](../assets/new.svg) <!--CHAN-4013-->와 일치하도록 제품 조건 매개 변수를 업데이트했습니다. [Amazon 갱신됨](https://sell.amazon.com/programs/renewed) 프로그램. 자세한 내용은 [갱신된 제품](renewed-products.md).

![새로 만들기](../assets/new.svg) <!--CHAN-3680-->업데이트됨 [Amazon 주문 세부 사항](amazon-order-details.md) Amazon에 의해 이행되는 주문에 &quot;일반 데이터&quot;를 포함하도록 업데이트되고, 자세한 내용은 [다음 기간 동안 이행](fulfilled-by.md).

![수정](../assets/fix.svg) <!--CHAN-4069-->스토어 카드에서 아이콘이 왜곡되는 문제를 수정했습니다.

![수정](../assets/fix.svg) <!--CHAN-4165-->오류를 수정하여 _로그인_ 세션 시간이 초과된 후에 표시되는 화면입니다.

![수정](../assets/fix.svg) <!--CHAN-4211-->Amazon 주문 세액을 새 상거래 주문으로 가져올 수 없는 문제를 해결했습니다.

![수정](../assets/fix.svg) <!--CHAN-4234-->저장소 대시보드에 표시된 매출 합계가 `Canceled` 또는 `Error` 상태.

![수정](../assets/fix.svg) <!--CHAN-4326-->을 사용하는 타사 확장과 연결된 주문 가져오기 오류가 발생하는 문제를 해결했습니다 _Magento Shipping_ 주문 생성 방법.

![수정](../assets/fix.svg) <!--CHAN-4357-->크론 동기화를 실행할 때 오류가 발생하는 문제를 수정했습니다. 두 cron 작업이 동시에 동기화되지 않도록 하는 CLI 명령에 잠금이 추가되었습니다.

![수정](../assets/fix.svg) Commerce 버전 2.3.5를 지원하도록 컨텐츠 보안 정책이 업데이트되었습니다.

## v4.0.0

Amazon Sales Channel 4.0.0은 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.3.0, 2.3.1, 2.3.2, 2.3.3 및 2.3.4와 호환됩니다. 이 버전의 Amazon Sales Channel에는 사소한 버그 수정과 함께 많은 사용자 인터페이스 업그레이드가 포함되어 있습니다.

>[!IMPORTANT]
>
>Amazon Sales Channel 4.0.0은 Adobe Commerce 2.3.5에서 지원되지 않습니다. Adobe Commerce 2.3.5를 지원하려면 Amazon Sales Channel 4.1.0으로 업그레이드하십시오.

![새로 만들기](../assets/new.svg) 새로운 기능 소개 [Amazon Sales Channel](amazon-sales-channel-home.md) 스토어 정보에 대한 &quot;카드 보기&quot;가 개선된 홈 페이지.

![새로 만들기](../assets/new.svg) 새로운 기능 소개 [대시보드 저장](amazon-store-dashboard.md) 목록 작성, 최근 주문 및 저장 설정 정보

![새로 만들기](../assets/new.svg) 간단하고 간소화된 [온보딩 프로세스](amazon-onboarding-home.md) 및 [기본 저장소 설정](default-store-settings.md) 보다 신속하게 스토리지를 통합할 수 있습니다.

![알려진 문제](../assets/bug.svg) <!--CHAN-4102--> When [속성 만들기](managing-attributes.md) 목록 및 **보기 저장** 가 로 설정되어 있습니다. `All Store Views (Global)`: 알려진 문제로 인해 이미지를 모든 저장소 보기로 가져올 수 없습니다. 에 대한 설정을 변경하는 경우 **보기 저장 (값을 로 가져오기)** 특정 저장소에 대해 이미지를 가져오면 해당 저장소에 가져옵니다.

## v3.0.1

Amazon Sales Channel 3.0.1은 클라우드 인프라에서 Adobe Commerce 버전 2.2.4 이상 및 Magento Open Source, Adobe Commerce 및 Adobe Commerce 2.3.x와 호환됩니다.

![수정](../assets/fix.svg) **숫자 필드 설정**: <!--CHAN-3779-->숫자 기반 값이 필요한 필드가 숫자 문자만 허용하도록 업데이트되었습니다. 예: 가격책정 규칙 설정 > 조정 금액 필드

![수정](../assets/fix.svg) **사용 안내서 링크**: <!--CHAN-3778-->잘못된 _사용 안내서_ 링크가 수정되었습니다.

![수정](../assets/fix.svg) **Amazon 목록 복제**: <!--CHAN-3593-->이제 중복 Amazon 목록이 발생하는 이전에 보고된 문제가 수정되었습니다. 이 릴리스 전에 확장은 목록을 가져올 때 Amazon 지역의 국가 코드를 SKU 값에 추가했습니다. 목록이 카탈로그 항목과 일치하지만 확장에서 추가된 SKU를 사용하여 새 중복 목록을 만들었습니다. 이 릴리스를 통해 확장은 가져온 목록에 대한 SKU를 수정하지 않고 기존 목록을 변경하지 않습니다. 를 사용할 수 있습니다 [!UICONTROL End Listing(s)] Amazon 옵션에서 중복 목록을 제거합니다.

## v3.0.0

Amazon Sales Channel 3.0.0은 클라우드 인프라에서 Adobe Commerce 버전 2.2.4 이상 및 Magento Open Source, Adobe Commerce 및 Adobe Commerce 2.3.x와 호환됩니다.

![새로 만들기](../assets/new.svg) **Amazon UK Marketplace 지금 사용 가능**: 사용자는 상거래 스토어를 만들고 통합할 때 영국 마켓플레이스를 선택할 수 있습니다. 이 UK 업그레이드에는 다음에 대한 추가 지원이 포함되어 있습니다.

- [Amazon VAT 계산 서비스](https://sell.amazon.co.uk/learn/vat-resources){target=&quot;_blank&quot;}

- [제품 세금 코드](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;} 정보.

![새로 만들기](../assets/new.svg) **향상된 로깅**: <!--CHAN-3642, 3672-->구현됨 **디버그 로깅 활성화** 문제 해결 필요 시 추가 동기화 데이터를 수집할 수 있는 기능입니다. 자세한 내용은 [Sales Channel 설정](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) 구성 참조의 항목을 참조하십시오.

![수정](../assets/fix.svg) **제품 카탈로그**: <!--CHAN-3687-->Amazon 목록과 함께 가져온 이미지가 해당 전자 상거래 카탈로그 제품에 적용되지 않는 문제를 수정했습니다.

![수정](../assets/fix.svg) **주문 생성**: <!--CHAN-3708-->Commerce가 상거래 카탈로그 제품과 일치하지 않는 Amazon 주문에 대한 주문을 만들지 못하는 문제를 해결했습니다.

![알려진 문제](../assets/bug.svg) **Amazon 목록 복제**: <!--CHAN-3593-->이 문제로 인해 카탈로그에서 동일한 SKU를 사용하지만 끝에 지역 코드가 추가된 가져온 목록에 대한 항목을 만듭니다. 그러면 Amazon이 수정된 SKU를 새 항목으로 처리하고 목록을 만듭니다. 이 문제는 향후 릴리스에서 해결될 예정입니다.

## v2.0.0

Amazon Sales Channel 2.0.0은 클라우드 인프라에서 Magento Open Source, Adobe Commerce 및 Adobe Commerce 버전 2.2.4 이상 및 2.3.x와 호환됩니다.

>[!NOTE]
>
>버전 1.0.0은 제한된 릴리스에서만 사용할 수 있었습니다.

![새로 만들기](../assets/new.svg)  **간소화된 온보딩 및 유지 관리**: 관리자를 통해 사용할 수 있는 세부 지침과 함께 단계별 프로세스를 통해 Amazon 판매자 계정을 추가 및 통합하는 방법을 제공합니다. 하나의 대시보드를 통해 저장소, 계정 및 나열된 제품을 유지 관리합니다.

![새로 만들기](../assets/new.svg)  **여러 계정 지원**: 관리자를 통해 여러 Amazon 브랜드 및 마켓 플레이스 리전을 관리하고 모니터링할 수 있습니다.

![새로 만들기](../assets/new.svg)  **지능형 가격 책정**: 자동 가격 조정 규칙을 설정하여 Buy Box에 대한 가능성을 높입니다. 현재 Buy Box 가격 또는 가장 낮은 경쟁업체 가격에 동적으로 조정하도록 가격을 설정합니다. 마진을 보호하기 위해 가격 조정을 위해 제한을 설정합니다.

![새로 만들기](../assets/new.svg)  **목록 관리**: 목록 규칙을 사용하여 제품 목록을 자동화하고 상거래 카탈로그를 Amazon Marketplace에 동기화합니다. 특정 오버라이드를 추가하여 오퍼링을 세밀하게 제어할 수 있습니다. 모든 목록을 관리자로부터 직접 모니터링하고 관리합니다.

![새로 만들기](../assets/new.svg)  **일관된 Inventory management**: 상거래 및 Amazon 재고 수량을 지속적으로 동기화합니다.

![새로 만들기](../assets/new.svg)  **주문 및 이행 관리**: 원활한 커뮤니케이션 및 인벤토리 업데이트를 통해 Amazon 주문을 추적할 수 있습니다. Amazon, Merchant 이행 또는 다양한 방법에 의해 이행된 주문 선적을 완료 및 추적합니다.

![알려진 문제](../assets/bug.svg)  제품 수량을 업데이트하는 대기 시간이 오래 걸릴 수 있습니다. 제품 수량에 대한 업데이트는 동기화하는 데 최대 2시간이 걸릴 수 있습니다.

![알려진 문제](../assets/bug.svg)  가져온 주문에는 _Prime_ 또는 _Premium_ 주문. Amazon 판매자 계정에서 이러한 주문을 확인해야 합니다.

![알려진 문제](../assets/bug.svg)  번들 제품은 Amazon에서 목록에 적합한 것으로 표시될 수 있습니다. 번들 제품 내의 제품 중 하나는 적합하지 않을 수 있습니다. 문제가 발생하면 번들 제품 항목에 대한 자격 상태를 확인합니다.

![알려진 문제](../assets/bug.svg)  Commerce 2.3.x용 Inventory management을 사용하는 경우 주문이 작성될 때 부분 주식 재색인이 트리거되지 않을 수 있습니다. 판매 가능 수량은 시간별로 재계산되며, 이 업데이트 간격 동안 초과 판매를 초래할 수 있습니다.
