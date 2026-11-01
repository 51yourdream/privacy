# Virtual Memorial Space 隱私權政策

**生效日期：2026 年 11 月 1 日**

## 1. 簡介

Virtual Memorial Space（以下簡稱「本 App」、「我們」）是一款 iOS App，用於建立私密的紀念空間、進行紀念儀式和寫信。本隱私權政策說明本 App 處理哪些資訊、這些資訊存放在哪裡，以及你有哪些選擇。

本 App 不需要註冊帳號。你的紀念內容只儲存在你的裝置上。我們的伺服器只用於紀念幣——一種可選的 App 內代幣，用於使用更精緻的供品款式。

使用本 App 即表示你已閱讀並理解本隱私權政策。

## 2. 我們不蒐集的資訊

本 App 不蒐集、也不要求提供：

- 你的姓名、電子郵件、電話號碼或任何登入帳號
- 紀念空間中的名字、照片、日期、簡介、信件或留言
- 整個照片圖庫的存取權限，以及相機、麥克風、聯絡人或位置
- 你的付款卡資訊
- 廣告識別碼（IDFA）。本 App 不會在其他公司的 App 或網站之間追蹤你，也不會跳出「App 追蹤透明度」授權視窗。
- 統計或使用行為資料。本 App 沒有接入任何統計分析 SDK，也沒有廣告。

## 3. 只儲存在你裝置上的紀念內容

以下內容儲存在你的 iPhone 或 iPad 上本 App 的私有儲存空間中：

- 紀念空間：名字、類型（例如親人、伴侶、朋友或寵物）、簡介、生日、紀念日、主題和提醒設定
- 你為紀念空間加入的照片
- 儀式紀錄：使用了哪種蠟燭、鮮花或紙錢供品、消耗的紀念幣數量、時間，以及你加入的留言
- 你寫的信件，包括草稿
- 偏好設定：語言、簡化效果、是否顯示傳統紙錢、是否完成引導、待同步購買標記，以及用於限制評分請求次數的計數
- 上一次從我們伺服器取得的紀念幣餘額，僅用於離線時顯示

這些內容不會上傳到我們的伺服器，不用於廣告，也不用於任何人工智慧（AI）功能或訓練。如果你開啟了 iCloud 雲端備份，iOS 可能會把這些資料包含在裝置備份中，由 Apple 在你的 Apple ID 下處理。本 App 本身沒有雲端同步。

**照片。** 你透過系統照片選擇器選擇照片。本 App 只會收到你選取的照片，不會存取整個照片圖庫。每張選取的照片會壓縮後儲存一份副本在本 App 的儲存空間中。

## 4. 紀念幣與我們的伺服器

紀念幣是消耗型 App 內購買項目。為了在重新安裝 App 後餘額不遺失，餘額儲存在我們的伺服器（「appapi」）上。該伺服器部署在 Vercel，資料儲存在 Vercel KV（Upstash Redis）中。

伺服器只儲存：

- 一個隨機產生的使用者 ID，與你的姓名、電子郵件或 Apple ID 無關聯
- 為該使用者 ID 簽發的存取權杖的摘要（雜湊值）。伺服器不儲存權杖本身。
- 你的紀念幣餘額
- 購買紀錄：商品 ID、Apple 交易 ID、紀念幣數量和時間
- 消費紀錄：供品 ID（例如某種蠟燭）、紀念幣數量、用於防止重複扣幣的請求鍵、消費後的餘額和時間
- 一份記錄加幣、扣幣和退款的流水帳，包括數量及相關的交易 ID 或消費 ID

每次請求伺服器時，還會附帶 App 版本號和一個裝置識別碼（iOS 的 identifierForVendor），用於驗證請求簽章。與任何網路服務一樣，我們的託管服務商可能會在一般請求記錄中處理你的 IP 位址，用於提供和保護服務。

伺服器不儲存你的姓名、電子郵件，也不儲存任何關於你所紀念的人或寵物的資訊：沒有紀念對象的名字、照片、信件或留言。

使用者 ID 和權杖儲存在你裝置的 iOS 鑰匙圈中，可能會透過 iCloud 鑰匙圈同步，因此重新安裝 App 後，或在登入同一 Apple ID 的其他裝置上，你的餘額仍然可用。

## 5. 購買

- **Apple（App Store）** 透過你的 Apple ID 處理所有付款。我們不會取得你的付款卡資訊。Apple 隱私權政策：https://www.apple.com/legal/privacy/
- **RevenueCat** 負責驗證交易。RevenueCat 會收到上述隨機使用者 ID、交易資訊（例如商品 ID、Apple 交易 ID 和購買時間），以及基本技術資訊，例如 App 版本、作業系統版本和 App Store 國家或地區。我們的伺服器向 RevenueCat 確認購買，RevenueCat 也會把購買和退款通知我們的伺服器，從而確保每筆購買只加一次幣，退款後扣回相應紀念幣。RevenueCat 隱私權政策：https://www.revenuecat.com/privacy

紀念幣沒有現實貨幣價值。退款由 Apple 依其規則處理。使用條款為 Apple 標準授權協議：https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. 通知（可選）

如果你為某個紀念空間開啟紀念日提醒，本 App 會請求通知權限，並在你的裝置上安排本機通知。提醒不經過我們的伺服器。你可以在 App 內或 iOS「設定」中關閉提醒。

## 7. 我們如何使用資訊

我們僅將上述資訊用於：

- 在你的裝置上顯示和保存紀念空間、儀式紀錄和信件
- 建立你的紀念幣錢包，每筆交易只加一次幣，在你選擇付費供品時扣幣，並在退款後扣回紀念幣
- 驗證請求，防止詐欺或重複加幣
- 回覆你的支援請求

我們不出售或出租個人資訊，不將其用於廣告，也不建立廣告輪廓。

## 8. 資訊分享

我們只與營運本 App 所必需的服務商分享資訊（Apple、RevenueCat，以及提供託管和儲存的 Vercel / Upstash），或在法律或有效法律程序要求時分享。

## 9. 刪除你的資料

在本 App 的「設定」中：

- **刪除全部資料（Delete All Data）** 會刪除此裝置上的全部紀念內容：紀念空間、照片、儀式紀錄、信件和留言。
- **刪除紀念幣資料（Delete Token Data）** 會刪除我們伺服器上的錢包：使用者 ID 紀錄、權杖雜湊值、餘額、購買與消費紀錄以及流水帳。餘額會歸零且無法復原。為防止同一筆購買再次入帳，我們只保留去除使用者 ID 的 Apple 交易 ID（及其商品 ID）。隨後，使用者 ID 和權杖也會從你的鑰匙圈中刪除。

刪除 App 會移除裝置上的本機內容，但刪除 App **不會**刪除我們伺服器上的錢包資料。如需刪除，請在刪除 App 之前使用「刪除紀念幣資料」，或聯絡我們。已刪除的本機資料可能仍保留在先前的 iCloud 裝置備份中，直到 Apple 取代或刪除這些備份。

你也可以請我們向 RevenueCat 申請刪除其保存的購買紀錄。

## 10. 安全與保存期限

與我們伺服器、Apple 和 RevenueCat 的連線均使用加密的 HTTPS。請求經過簽章，伺服器只儲存權杖的雜湊值，你的身分儲存在 iOS 鑰匙圈中。任何儲存或傳輸方式都無法做到絕對安全。

- 本機內容會一直保留，直到你刪除它或刪除 App。
- 伺服器上的錢包資料會一直保留，直到你使用「刪除紀念幣資料」或請求我們刪除。
- 不含使用者 ID 的 Apple 交易 ID 會被保留，用於防止重複入帳。
- Apple 和 RevenueCat 會依其自身政策和法律義務保留購買紀錄。

## 11. 兒童隱私

Virtual Memorial Space 不以兒童為對象。我們不會故意蒐集 13 歲以下兒童（或你所在國家規定的最低年齡以下兒童）的個人資訊。如果你認為有兒童向我們提供了個人資訊，請聯絡我們，我們會將其刪除。

## 12. 跨境處理

我們的託管和儲存服務商以及 RevenueCat 可能會在美國或你所在地以外的其他國家處理資料。我們依賴這些服務商的保障措施來進行此類處理。

## 13. 你的權利

依你所在地區的法律，你可能有權存取、更正、刪除或限制處理你的個人資訊。大部分資料都在你的裝置上，由你自行控制。對於我們伺服器上的資料，請使用「刪除紀念幣資料」或聯絡我們。我們可能會請你提供有助於找到相關紀錄的資訊。

## 14. 政策變更

我們可能會更新本隱私權政策，屆時頂部的日期會隨之更改。如果本 App 開始蒐集新類型的資料，我們會先更新本政策。

## 15. 聯絡我們

如果你對本隱私權政策有任何疑問，請聯絡：

- 電子郵件：lpjustdoit@163.com

---

## 其他語言

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
