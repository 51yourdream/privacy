# Virtual Memorial Space 개인정보 처리방침

**시행일: 2026년 11월 1일**

## 1. 소개

Virtual Memorial Space(이하 "앱", "당사")는 비공개 추모 공간을 만들고, 추모 의식을 하고, 편지를 쓸 수 있는 iOS 앱입니다. 본 개인정보 처리방침은 앱이 어떤 정보를 다루는지, 그 정보가 어디에 저장되는지, 그리고 사용자가 선택할 수 있는 사항을 설명합니다.

앱은 계정이 필요하지 않습니다. 추모 콘텐츠는 사용자의 기기에만 저장됩니다. 당사 서버는 더 정성스러운 헌물 스타일에 사용하는 선택형 앱 내 토큰인 '메모리얼 토큰'에만 사용됩니다.

앱을 사용함으로써 사용자는 본 개인정보 처리방침을 읽고 이해했음을 인정합니다.

## 2. 수집하지 않는 정보

앱은 다음을 수집하거나 요청하지 않습니다.

- 사용자의 이름, 이메일 주소, 전화번호 또는 로그인 계정
- 추모 공간의 이름, 사진, 날짜, 소개, 편지 또는 메시지
- 사진 보관함 전체에 대한 접근 권한, 카메라, 마이크, 연락처 또는 위치
- 결제 카드 정보
- 광고 식별자(IDFA). 앱은 다른 회사의 앱이나 웹사이트에 걸쳐 사용자를 추적하지 않으며, 앱 추적 투명성(ATT) 권한 요청 창을 표시하지 않습니다.
- 분석 데이터 또는 사용 이벤트. 앱에는 분석 SDK나 광고가 없습니다.

## 3. 기기에만 저장되는 추모 콘텐츠

다음 항목은 iPhone 또는 iPad의 앱 전용 저장 공간에 저장됩니다.

- 추모 공간: 이름, 유형(예: 소중한 사람, 배우자·연인, 친구, 반려동물), 소개, 생일, 기일·기념일, 테마, 알림 설정
- 추모 공간에 추가한 사진
- 의식 기록: 사용한 초, 꽃, 종이 헌물의 종류, 사용한 토큰 수, 시간, 추가한 메시지
- 작성한 편지(임시 저장본 포함)
- 환경설정: 언어, 효과 간소화, 전통 종이 헌물 표시 여부, 온보딩 완료 여부, 구매 동기화 대기 표시, 평가 요청 횟수를 제한하기 위한 카운터
- 당사 서버에서 마지막으로 받은 토큰 잔액(오프라인 표시용으로만 사용)

이 콘텐츠는 당사 서버로 업로드되지 않으며, 광고나 인공지능(AI) 기능 또는 학습에 사용되지 않습니다. iCloud 백업이 켜져 있으면 iOS가 이 데이터를 기기 백업에 포함할 수 있으며, 이는 Apple이 사용자의 Apple ID에 따라 처리합니다. 앱 자체의 클라우드 동기화는 없습니다.

**사진.** 사진은 시스템 사진 선택기로 고릅니다. 앱은 사용자가 선택한 사진만 받으며 사진 보관함 전체에 접근하지 않습니다. 선택한 사진은 압축된 사본이 앱 저장 공간에 저장됩니다.

## 4. 메모리얼 토큰과 당사 서버

메모리얼 토큰은 소모성 앱 내 구매 항목입니다. 앱을 다시 설치해도 잔액이 사라지지 않도록 잔액은 당사 서버('appapi')에 보관됩니다. 이 서버는 Vercel에서 운영되며 데이터는 Vercel KV(Upstash Redis)에 저장됩니다.

서버에는 다음 항목만 저장됩니다.

- 무작위로 생성된 사용자 ID(사용자의 이름, 이메일 주소, Apple ID와 연결되지 않음)
- 해당 사용자 ID에 발급된 액세스 토큰의 다이제스트(해시). 토큰 자체는 서버에 저장되지 않습니다.
- 토큰 잔액
- 구매 기록: 상품 ID, Apple 거래 ID, 토큰 수, 시간
- 사용 기록: 헌물 ID(예: 초의 종류), 토큰 수, 이중 차감을 막기 위한 요청 키, 사용 후 잔액, 시간
- 지급, 사용, 환불 내역(수량 및 관련 거래 ID 또는 사용 ID)

서버로 보내는 각 요청에는 앱 버전과 기기 식별자(iOS identifierForVendor)도 포함되며, 요청 서명 검증에 사용됩니다. 일반적인 웹 서비스와 마찬가지로, 호스팅 제공업체는 서비스 제공과 보호를 위해 일반 요청 로그에서 사용자의 IP 주소를 처리할 수 있습니다.

서버는 사용자의 이름, 이메일 주소를 저장하지 않으며, 추모하는 사람이나 반려동물에 관한 어떤 정보(추모 대상의 이름, 사진, 편지, 메시지)도 저장하지 않습니다.

사용자 ID와 토큰은 기기의 iOS 키체인에 저장됩니다. iCloud 키체인을 통해 동기화될 수 있으므로, 앱을 다시 설치한 후나 같은 Apple ID로 로그인한 다른 기기에서도 잔액을 사용할 수 있습니다.

## 5. 구매

- **Apple(App Store)** 이 사용자의 Apple ID를 통해 모든 결제를 처리합니다. 당사는 결제 카드 정보를 받지 않습니다. Apple 개인정보 처리방침: https://www.apple.com/legal/privacy/
- **RevenueCat** 이 거래를 검증합니다. RevenueCat은 위의 무작위 사용자 ID, 거래 정보(상품 ID, Apple 거래 ID, 구매 시간 등), 그리고 앱 버전, 운영체제 버전, App Store 국가 등 기본 기술 정보를 받습니다. 당사 서버는 RevenueCat에 구매를 확인하고, RevenueCat은 구매와 환불을 당사 서버에 알립니다. 이를 통해 토큰은 거래당 한 번만 지급되고 환불 후에는 회수됩니다. RevenueCat 개인정보 처리방침: https://www.revenuecat.com/privacy

메모리얼 토큰에는 실제 금전적 가치가 없습니다. 환불은 Apple의 규정에 따라 Apple이 처리합니다. 이용약관은 Apple 표준 사용권 계약입니다: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. 알림(선택)

추모 공간의 기념일 알림을 켜면 앱은 알림 권한을 요청하고 기기에서 로컬 알림을 예약합니다. 알림은 당사 서버를 거치지 않습니다. 앱 안이나 iOS '설정'에서 끌 수 있습니다.

## 7. 정보 이용 목적

당사는 위 정보를 다음 목적으로만 사용합니다.

- 기기에서 추모 공간, 의식 기록, 편지를 표시하고 보관
- 토큰 지갑을 만들고, 거래당 한 번만 토큰을 지급하고, 유료 헌물을 선택할 때 토큰을 차감하며, 환불 후 토큰을 회수
- 요청을 검증하고 부정 사용이나 중복 지급을 방지
- 고객 지원 요청에 응답

당사는 개인정보를 판매하거나 대여하지 않으며, 광고에 사용하지 않고, 광고 프로필을 만들지 않습니다.

## 8. 정보 공유

당사는 앱 운영에 필요한 서비스 제공업체(Apple, RevenueCat, 호스팅 및 저장소를 제공하는 Vercel / Upstash)와만 정보를 공유하거나, 법률 또는 적법한 법적 절차에 따라 요구되는 경우에만 공유합니다.

## 9. 데이터 삭제

앱의 '설정'에서:

- **모든 데이터 삭제(Delete All Data)** 는 이 기기의 모든 추모 콘텐츠(추모 공간, 사진, 의식 기록, 편지, 메시지)를 삭제합니다.
- **토큰 데이터 삭제(Delete Token Data)** 는 당사 서버의 지갑(사용자 ID 기록, 토큰 해시, 잔액, 구매·사용 기록, 내역)을 삭제합니다. 잔액은 0이 되며 복구할 수 없습니다. 같은 구매가 다시 지급되지 않도록, 사용자 ID를 제거한 Apple 거래 ID(및 해당 상품 ID)만 보관합니다. 이후 사용자 ID와 토큰도 키체인에서 삭제됩니다.

앱을 삭제하면 기기의 로컬 콘텐츠는 지워지지만, 당사 서버의 지갑 데이터는 **삭제되지 않습니다**. 삭제하려면 앱을 삭제하기 전에 '토큰 데이터 삭제'를 사용하거나 당사에 문의하세요. 삭제한 로컬 데이터는 Apple이 교체하거나 삭제할 때까지 이전 iCloud 기기 백업에 남아 있을 수 있습니다.

RevenueCat이 보관 중인 구매 기록의 삭제를 RevenueCat에 요청해 달라고 당사에 요청할 수도 있습니다.

## 10. 보안 및 보관 기간

당사 서버, Apple, RevenueCat과의 연결에는 암호화된 HTTPS를 사용합니다. 요청은 서명되며, 서버에는 토큰의 해시만 저장되고, 사용자 식별 정보는 iOS 키체인에 보관됩니다. 완벽하게 안전한 저장 또는 전송 방법은 없습니다.

- 로컬 콘텐츠는 사용자가 삭제하거나 앱을 삭제할 때까지 보관됩니다.
- 서버의 지갑 데이터는 '토큰 데이터 삭제'를 사용하거나 당사에 삭제를 요청할 때까지 보관됩니다.
- 사용자 ID가 없는 Apple 거래 ID는 중복 지급 방지를 위해 보관됩니다.
- Apple과 RevenueCat은 각자의 정책과 법적 의무에 따라 구매 기록을 보관합니다.

## 11. 아동 개인정보

Virtual Memorial Space는 아동을 대상으로 하지 않습니다. 당사는 13세 미만(또는 거주 국가에서 정한 최소 연령 미만) 아동의 개인정보를 고의로 수집하지 않습니다. 아동이 당사에 개인정보를 제공했다고 생각되면 연락해 주세요. 해당 정보를 삭제하겠습니다.

## 12. 국외 처리

당사의 호스팅·저장소 제공업체와 RevenueCat은 미국 또는 사용자의 거주 국가가 아닌 다른 국가에서 데이터를 처리할 수 있습니다. 당사는 이러한 처리에 대해 해당 업체들의 보호 조치에 의존합니다.

## 13. 사용자의 권리

거주 지역에 따라 사용자는 개인정보에 대한 열람, 정정, 삭제 또는 처리 제한을 요구할 권리가 있을 수 있습니다. 대부분의 데이터는 사용자의 기기에 있으며 사용자가 직접 관리합니다. 당사 서버의 데이터는 '토큰 데이터 삭제'를 사용하거나 당사에 문의하세요. 관련 기록을 찾는 데 필요한 정보를 요청할 수 있습니다.

## 14. 방침 변경

당사는 본 개인정보 처리방침을 변경할 수 있으며, 변경 시 상단의 날짜가 바뀝니다. 앱이 새로운 종류의 데이터를 수집하기 시작하는 경우, 먼저 본 방침을 업데이트합니다.

## 15. 문의

본 개인정보 처리방침에 관한 문의는 아래로 연락해 주세요.

- 이메일: lpjustdoit@163.com

---

## 다른 언어

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
