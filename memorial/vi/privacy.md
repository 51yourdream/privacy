# Chính sách quyền riêng tư của Virtual Memorial Space

**Ngày có hiệu lực: 1 tháng 11 năm 2026**

## 1. Giới thiệu

Virtual Memorial Space ("Ứng dụng", "chúng tôi") là ứng dụng iOS để tạo không gian tưởng niệm riêng tư, thực hiện nghi thức tưởng nhớ và viết thư. Chính sách quyền riêng tư này giải thích Ứng dụng xử lý những thông tin nào, thông tin được lưu ở đâu và bạn có những lựa chọn nào.

Ứng dụng không yêu cầu tài khoản. Nội dung tưởng niệm của bạn chỉ nằm trên thiết bị của bạn. Máy chủ của chúng tôi chỉ được dùng cho Xu tưởng niệm, loại xu tùy chọn trong Ứng dụng dùng cho các kiểu lễ vật đặc biệt hơn.

Khi sử dụng Ứng dụng, bạn xác nhận rằng mình đã đọc và hiểu Chính sách quyền riêng tư này.

## 2. Thông tin chúng tôi không thu thập

Ứng dụng không thu thập và không yêu cầu:

- Tên, địa chỉ email, số điện thoại hoặc bất kỳ tài khoản đăng nhập nào của bạn
- Tên, ảnh, ngày tháng, phần giới thiệu, thư hoặc lời nhắn trong các không gian tưởng niệm của bạn
- Quyền truy cập toàn bộ thư viện ảnh, camera, micrô, danh bạ hoặc vị trí
- Thông tin thẻ thanh toán của bạn
- Mã định danh quảng cáo (IDFA). Ứng dụng không theo dõi bạn trên ứng dụng hoặc trang web của các công ty khác và không hiển thị yêu cầu Minh bạch theo dõi ứng dụng (ATT).
- Dữ liệu phân tích hoặc sự kiện sử dụng. Ứng dụng không có SDK phân tích và không có quảng cáo.

## 3. Nội dung tưởng niệm chỉ lưu trên thiết bị của bạn

Những nội dung sau được lưu trong bộ nhớ riêng của Ứng dụng trên iPhone hoặc iPad của bạn:

- Không gian tưởng niệm: tên, loại (ví dụ người thân yêu, người bạn đời, bạn bè hoặc thú cưng), phần giới thiệu, ngày sinh, ngày tưởng niệm, chủ đề và cài đặt nhắc nhở
- Ảnh bạn thêm vào không gian tưởng niệm
- Bản ghi nghi thức: nến, hoa hoặc lễ vật giấy đã dùng, số xu đã tiêu, thời gian và lời nhắn bạn thêm
- Thư bạn viết, kể cả bản nháp
- Tùy chọn: ngôn ngữ, giảm hiệu ứng, có hiển thị lễ vật giấy truyền thống hay không, đã hoàn tất phần giới thiệu hay chưa, dấu đánh dấu giao dịch đang chờ đồng bộ, và bộ đếm giới hạn số lần đề nghị đánh giá
- Số dư xu gần nhất nhận từ máy chủ của chúng tôi, chỉ dùng để hiển thị khi ngoại tuyến

Nội dung này không được tải lên máy chủ của chúng tôi, không dùng cho quảng cáo và không dùng cho bất kỳ tính năng hay việc huấn luyện trí tuệ nhân tạo (AI) nào. Nếu bạn bật Sao lưu iCloud, iOS có thể đưa dữ liệu này vào bản sao lưu thiết bị do Apple xử lý theo Apple ID của bạn. Ứng dụng không có tính năng đồng bộ đám mây riêng.

**Ảnh.** Bạn chọn ảnh bằng trình chọn ảnh của hệ thống. Ứng dụng chỉ nhận những ảnh bạn chọn và không truy cập toàn bộ thư viện ảnh. Mỗi ảnh được chọn sẽ được lưu một bản sao đã nén trong bộ nhớ của Ứng dụng.

## 4. Xu tưởng niệm và máy chủ của chúng tôi

Xu tưởng niệm là mục mua trong ứng dụng loại tiêu hao. Để số dư vẫn còn sau khi cài đặt lại Ứng dụng, số dư được lưu trên máy chủ của chúng tôi ("appapi"), chạy trên Vercel và lưu dữ liệu trong Vercel KV (Upstash Redis).

Máy chủ chỉ lưu:

- Một mã người dùng được tạo ngẫu nhiên, không liên kết với tên, email hoặc Apple ID của bạn
- Bản tóm tắt (hash) của mã truy cập được cấp cho mã người dùng đó. Máy chủ không lưu chính mã truy cập.
- Số dư xu của bạn
- Bản ghi mua: mã sản phẩm, mã giao dịch Apple, số xu và thời gian
- Bản ghi chi tiêu: mã lễ vật (ví dụ một loại nến), số xu, khóa yêu cầu dùng để tránh trừ xu hai lần, số dư sau khi chi tiêu và thời gian
- Sổ ghi các lần cộng xu, tiêu xu và hoàn tiền, kèm số lượng và mã giao dịch hoặc mã chi tiêu liên quan

Mỗi yêu cầu gửi đến máy chủ còn kèm phiên bản Ứng dụng và một mã định danh thiết bị (identifierForVendor của iOS), dùng để xác minh chữ ký của yêu cầu. Như mọi dịch vụ web, nhà cung cấp lưu trữ của chúng tôi có thể xử lý địa chỉ IP của bạn trong nhật ký yêu cầu thông thường để cung cấp và bảo vệ dịch vụ.

Máy chủ không lưu tên, email của bạn, cũng không lưu bất cứ điều gì về người hoặc thú cưng mà bạn tưởng nhớ: không có tên, ảnh, thư hay lời nhắn tưởng niệm nào.

Mã người dùng và mã truy cập được lưu trong Chuỗi khóa iOS trên thiết bị của bạn. Chúng có thể được đồng bộ qua Chuỗi khóa iCloud, nhờ đó số dư vẫn dùng được sau khi cài đặt lại Ứng dụng hoặc trên thiết bị khác đăng nhập cùng Apple ID.

## 5. Mua hàng

- **Apple (App Store)** xử lý mọi khoản thanh toán qua Apple ID của bạn. Chúng tôi không bao giờ nhận thông tin thẻ thanh toán của bạn. Chính sách quyền riêng tư của Apple: https://www.apple.com/legal/privacy/
- **RevenueCat** xác thực giao dịch. RevenueCat nhận mã người dùng ngẫu nhiên nêu trên, thông tin giao dịch (như mã sản phẩm, mã giao dịch Apple và thời gian mua) cùng thông tin kỹ thuật cơ bản như phiên bản Ứng dụng, phiên bản hệ điều hành và quốc gia của App Store. Máy chủ của chúng tôi yêu cầu RevenueCat xác nhận giao dịch mua, và RevenueCat thông báo cho máy chủ của chúng tôi về giao dịch mua và hoàn tiền, để xu chỉ được cộng một lần và bị thu hồi sau khi hoàn tiền. Chính sách quyền riêng tư của RevenueCat: https://www.revenuecat.com/privacy

Xu tưởng niệm không có giá trị tiền tệ thực tế. Việc hoàn tiền do Apple xử lý theo quy định của Apple. Điều khoản sử dụng là thỏa thuận cấp phép tiêu chuẩn của Apple: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Thông báo (tùy chọn)

Nếu bạn bật nhắc nhở ngày tưởng niệm cho một không gian, Ứng dụng sẽ xin quyền gửi thông báo và lên lịch thông báo cục bộ trên thiết bị của bạn. Nhắc nhở không đi qua máy chủ của chúng tôi. Bạn có thể tắt trong Ứng dụng hoặc trong Cài đặt iOS.

## 7. Cách chúng tôi sử dụng thông tin

Chúng tôi chỉ dùng thông tin trên để:

- Hiển thị và lưu các không gian tưởng niệm, nghi thức và thư trên thiết bị của bạn
- Tạo ví xu của bạn, cộng xu đã mua đúng một lần cho mỗi giao dịch, trừ xu khi bạn chọn lễ vật cao cấp và thu hồi xu sau khi hoàn tiền
- Xác minh yêu cầu và ngăn gian lận hoặc cộng xu trùng lặp
- Trả lời các yêu cầu hỗ trợ của bạn

Chúng tôi không bán hoặc cho thuê thông tin cá nhân, không dùng thông tin cho quảng cáo và không xây dựng hồ sơ quảng cáo.

## 8. Chia sẻ thông tin

Chúng tôi chỉ chia sẻ thông tin với các nhà cung cấp dịch vụ cần thiết để vận hành Ứng dụng (Apple, RevenueCat và Vercel / Upstash cho lưu trữ máy chủ và dữ liệu), hoặc khi pháp luật hay một thủ tục pháp lý hợp lệ yêu cầu.

## 9. Xóa dữ liệu của bạn

Trong Cài đặt của Ứng dụng:

- **Xóa tất cả dữ liệu (Delete All Data)** xóa toàn bộ nội dung tưởng niệm trên thiết bị này: không gian tưởng niệm, ảnh, bản ghi nghi thức, thư và lời nhắn.
- **Xóa dữ liệu xu (Delete Token Data)** xóa ví của bạn trên máy chủ của chúng tôi: bản ghi mã người dùng, hash của mã truy cập, số dư, bản ghi mua và chi tiêu, và sổ ghi. Số dư trở về 0 và không thể khôi phục. Để tránh cùng một giao dịch mua được cộng xu lần nữa, chúng tôi chỉ giữ lại mã giao dịch Apple (kèm mã sản phẩm) đã bỏ mã người dùng. Sau đó, mã người dùng và mã truy cập cũng được xóa khỏi Chuỗi khóa của bạn.

Xóa Ứng dụng sẽ xóa nội dung cục bộ khỏi thiết bị, nhưng **không** xóa ví của bạn trên máy chủ của chúng tôi. Để xóa ví, hãy dùng "Xóa dữ liệu xu" trước khi xóa Ứng dụng, hoặc liên hệ với chúng tôi. Dữ liệu cục bộ đã xóa có thể vẫn còn trong các bản sao lưu iCloud trước đó của thiết bị cho đến khi Apple thay thế hoặc xóa chúng.

Bạn cũng có thể yêu cầu chúng tôi đề nghị RevenueCat xóa bản ghi giao dịch mua mà họ lưu giữ.

## 10. Bảo mật và thời gian lưu giữ

Kết nối tới máy chủ của chúng tôi, Apple và RevenueCat đều dùng HTTPS được mã hóa. Yêu cầu được ký, máy chủ chỉ lưu hash của mã truy cập, và danh tính của bạn được giữ trong Chuỗi khóa iOS. Không có phương thức lưu trữ hay truyền tải nào an toàn tuyệt đối.

- Nội dung cục bộ được giữ cho đến khi bạn xóa nó hoặc xóa Ứng dụng.
- Dữ liệu ví trên máy chủ được giữ cho đến khi bạn dùng "Xóa dữ liệu xu" hoặc yêu cầu chúng tôi xóa.
- Mã giao dịch Apple không kèm mã người dùng được giữ lại để tránh cộng xu trùng lặp.
- Apple và RevenueCat lưu giữ bản ghi mua theo chính sách và nghĩa vụ pháp lý của riêng họ.

## 11. Quyền riêng tư của trẻ em

Virtual Memorial Space không hướng đến trẻ em. Chúng tôi không cố ý thu thập thông tin cá nhân của trẻ em dưới 13 tuổi (hoặc dưới độ tuổi tối thiểu theo quy định tại quốc gia của bạn). Nếu bạn cho rằng một trẻ em đã cung cấp thông tin cá nhân cho chúng tôi, hãy liên hệ và chúng tôi sẽ xóa thông tin đó.

## 12. Xử lý dữ liệu ở nước ngoài

Các nhà cung cấp lưu trữ máy chủ và dữ liệu của chúng tôi cùng RevenueCat có thể xử lý dữ liệu tại Hoa Kỳ hoặc các quốc gia khác ngoài quốc gia của bạn. Chúng tôi dựa vào các biện pháp bảo vệ của những nhà cung cấp này cho việc xử lý đó.

## 13. Quyền của bạn

Tùy nơi bạn sinh sống, bạn có thể có quyền truy cập, chỉnh sửa, xóa hoặc hạn chế việc xử lý thông tin cá nhân của mình. Phần lớn dữ liệu nằm trên thiết bị và do bạn kiểm soát. Với dữ liệu trên máy chủ của chúng tôi, hãy dùng "Xóa dữ liệu xu" hoặc liên hệ với chúng tôi. Chúng tôi có thể đề nghị bạn cung cấp thông tin giúp tìm các bản ghi liên quan.

## 14. Thay đổi chính sách

Chúng tôi có thể cập nhật Chính sách quyền riêng tư này. Khi đó, ngày ở đầu trang sẽ thay đổi. Nếu Ứng dụng bắt đầu thu thập loại dữ liệu mới, chúng tôi sẽ cập nhật chính sách này trước.

## 15. Liên hệ

Nếu bạn có câu hỏi về Chính sách quyền riêng tư này, vui lòng liên hệ:

- Email: lpjustdoit@163.com

---

## Ngôn ngữ khác

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
