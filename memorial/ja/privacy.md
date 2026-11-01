# Virtual Memorial Space プライバシーポリシー

**発効日：2026年11月1日**

## 1. はじめに

Virtual Memorial Space（以下「本アプリ」「当方」）は、プライベートな追悼スペースを作成し、追悼の儀式を行い、手紙を書くための iOS アプリです。本プライバシーポリシーでは、本アプリが扱う情報、その保存場所、およびお客様が選択できる事項について説明します。

本アプリはアカウント登録を必要としません。追悼コンテンツはお客様のデバイス内にのみ保存されます。当方のサーバーは、より上質なお供えのスタイルに使える任意のアプリ内トークン「メモリアルトークン」のためだけに使用されます。

本アプリを使用することにより、お客様は本プライバシーポリシーを読み、理解したことを認めるものとします。

## 2. 収集しない情報

本アプリは以下を収集せず、求めることもありません。

- お客様の氏名、メールアドレス、電話番号、またはログインアカウント
- 追悼スペース内の名前、写真、日付、紹介文、手紙、メッセージ
- 写真ライブラリ全体へのアクセス、カメラ、マイク、連絡先、位置情報
- お支払いカード情報
- 広告識別子（IDFA）。本アプリは他社のアプリやウェブサイトをまたいでお客様をトラッキングせず、App Tracking Transparency の許可ダイアログも表示しません。
- 分析データや利用イベント。本アプリには分析 SDK も広告も含まれていません。

## 3. デバイス内にのみ保存される追悼コンテンツ

以下は iPhone または iPad 上の本アプリ専用ストレージに保存されます。

- 追悼スペース：名前、種類（例：大切な人、パートナー、友人、ペット）、紹介文、誕生日、命日・記念日、テーマ、リマインダー設定
- 追悼スペースに追加した写真
- 儀式の記録：使用したろうそく・花・紙のお供え、消費したトークン数、日時、追加したメッセージ
- 書いた手紙（下書きを含む）
- 設定：言語、エフェクトの簡略化、伝統的な紙のお供えを表示するかどうか、オンボーディング完了の有無、購入同期待ちのフラグ、評価依頼の回数を制限するためのカウンター
- 当方のサーバーから最後に受け取ったトークン残高（オフライン表示のみに使用）

これらのコンテンツは当方のサーバーにアップロードされず、広告にも、人工知能（AI）の機能や学習にも使用されません。iCloud バックアップがオンの場合、iOS がこれらのデータをデバイスのバックアップに含めることがあり、それは Apple がお客様の Apple ID のもとで取り扱います。本アプリ独自のクラウド同期はありません。

**写真について。** 写真はシステムの写真ピッカーで選択します。本アプリが受け取るのは選択された写真のみで、写真ライブラリ全体にはアクセスしません。選択された写真は圧縮したコピーが本アプリのストレージ内に保存されます。

## 4. メモリアルトークンと当方のサーバー

メモリアルトークンは消耗型のアプリ内課金アイテムです。アプリを再インストールしても残高が失われないよう、残高は当方のサーバー（「appapi」）に保存されます。このサーバーは Vercel 上で稼働し、データは Vercel KV（Upstash Redis）に保存されます。

サーバーに保存されるのは以下のみです。

- ランダムに生成されたユーザー ID（お客様の氏名、メールアドレス、Apple ID とは紐付きません）
- そのユーザー ID に発行したアクセストークンのダイジェスト（ハッシュ値）。トークンそのものはサーバーに保存されません。
- トークン残高
- 購入記録：商品 ID、Apple 取引 ID、トークン数、日時
- 消費記録：お供え ID（例：ろうそくの種類）、トークン数、二重課金を防ぐためのリクエストキー、消費後の残高、日時
- 付与・消費・返金の履歴（数量と関連する取引 ID または消費 ID）

サーバーへの各リクエストには、アプリのバージョンとデバイス識別子（iOS の identifierForVendor）も含まれ、リクエスト署名の検証に使用されます。一般的なウェブサービスと同様に、ホスティング事業者がサービスの提供と保護のため、通常のリクエストログでお客様の IP アドレスを処理することがあります。

サーバーには、お客様の氏名やメールアドレス、追悼している人やペットに関する情報（追悼対象の名前、写真、手紙、メッセージ）は一切保存されません。

ユーザー ID とトークンはデバイスの iOS キーチェーンに保存されます。iCloud キーチェーンで同期される場合があり、アプリの再インストール後や同じ Apple ID でサインインした別のデバイスでも残高を利用できます。

## 5. 購入

- **Apple（App Store）** がお客様の Apple ID を通じてすべての支払いを処理します。当方がお支払いカード情報を受け取ることはありません。Apple のプライバシーポリシー：https://www.apple.com/legal/privacy/
- **RevenueCat** が取引を検証します。RevenueCat は上記のランダムなユーザー ID、取引情報（商品 ID、Apple 取引 ID、購入日時など）、およびアプリのバージョン、OS のバージョン、App Store の国・地域などの基本的な技術情報を受け取ります。当方のサーバーは RevenueCat に購入を確認し、RevenueCat は購入と返金を当方のサーバーに通知します。これにより、トークンは 1 回の購入につき一度だけ付与され、返金後には回収されます。RevenueCat のプライバシーポリシー：https://www.revenuecat.com/privacy

メモリアルトークンに現実の金銭的価値はありません。返金は Apple の規定に従って Apple が取り扱います。利用規約は Apple の標準使用許諾契約です：https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. 通知（任意）

追悼スペースで記念日リマインダーをオンにすると、本アプリは通知の許可を求め、デバイス上でローカル通知を予約します。リマインダーは当方のサーバーを経由しません。アプリ内または iOS の「設定」でオフにできます。

## 7. 情報の利用目的

上記の情報は以下の目的にのみ使用します。

- 追悼スペース、儀式、手紙をデバイス上で表示・保存する
- トークンウォレットを作成し、取引ごとに一度だけトークンを付与し、有料のお供えを選んだときにトークンを差し引き、返金後にトークンを回収する
- リクエストを検証し、不正や二重付与を防止する
- サポートへのお問い合わせに対応する

当方は個人情報を販売・貸与せず、広告に使用せず、広告用プロファイルも作成しません。

## 8. 情報の共有

情報を共有するのは、本アプリの運営に必要なサービス事業者（Apple、RevenueCat、ホスティングとストレージを提供する Vercel / Upstash）のみ、または法令や正当な法的手続きにより求められた場合のみです。

## 9. データの削除

本アプリの「設定」で以下を行えます。

- **すべてのデータを削除（Delete All Data）**：このデバイス上のすべての追悼コンテンツ（追悼スペース、写真、儀式の記録、手紙、メッセージ）を削除します。
- **トークンデータを削除（Delete Token Data）**：当方のサーバー上のウォレット（ユーザー ID の記録、トークンのハッシュ値、残高、購入・消費記録、履歴）を削除します。残高はゼロになり、復元できません。同じ購入が再び付与されるのを防ぐため、ユーザー ID を取り除いた Apple 取引 ID（とその商品 ID）のみを保持します。その後、ユーザー ID とトークンはキーチェーンからも削除されます。

アプリを削除するとデバイス上のローカルコンテンツは消去されますが、当方のサーバー上のウォレットデータは**削除されません**。削除するには、アプリを削除する前に「トークンデータを削除」を使用するか、当方までご連絡ください。削除したローカルデータは、Apple が置き換えるか削除するまで、以前の iCloud デバイスバックアップに残る場合があります。

RevenueCat が保持する購入記録の削除を RevenueCat に依頼するよう、当方に求めることもできます。

## 10. セキュリティと保存期間

当方のサーバー、Apple、RevenueCat との通信には暗号化された HTTPS を使用します。リクエストは署名され、サーバーにはトークンのハッシュ値のみが保存され、お客様の識別情報は iOS キーチェーンに保管されます。完全に安全な保存・通信方法は存在しません。

- ローカルコンテンツは、お客様が削除するかアプリを削除するまで保持されます。
- サーバー上のウォレットデータは、「トークンデータを削除」を使用するか当方に削除を依頼するまで保持されます。
- ユーザー ID を含まない Apple 取引 ID は、二重付与を防ぐために保持されます。
- Apple と RevenueCat は、それぞれのポリシーと法的義務に従って購入記録を保持します。

## 11. 子どものプライバシー

Virtual Memorial Space は子どもを対象としていません。13 歳未満（またはお住まいの国で定められた最低年齢未満）の子どもの個人情報を故意に収集することはありません。子どもが当方に個人情報を提供したと思われる場合はご連絡ください。削除いたします。

## 12. 国外での処理

当方のホスティング・ストレージ事業者および RevenueCat は、米国やお客様の居住国以外の国でデータを処理する場合があります。当方はこうした処理について、これらの事業者の保護措置に依拠しています。

## 13. お客様の権利

お住まいの地域によっては、個人情報へのアクセス、訂正、削除、処理の制限を求める権利がある場合があります。データの大部分はお客様のデバイス上にあり、お客様自身が管理できます。当方のサーバー上のデータについては、「トークンデータを削除」を使用するか当方までご連絡ください。関連する記録を特定するための情報をお伺いする場合があります。

## 14. 本ポリシーの変更

本プライバシーポリシーは更新されることがあり、その際は冒頭の日付が変更されます。本アプリが新たな種類のデータを収集し始める場合は、事前に本ポリシーを更新します。

## 15. お問い合わせ

本プライバシーポリシーに関するご質問は、以下までご連絡ください。

- メール：lpjustdoit@163.com

---

## 他の言語

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
