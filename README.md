# E-commerce UI Improvement
## 1. Giới thiệu
Dự án thuộc bài tập cá nhân Chương 1 môn Phát triển ứng dụng TMĐT: Khảo sát cấu trúc thực tế của một website thương mại điện tử lớn tại Việt Nam, phân tích các điểm hạn chế về trải nghiệm người dùng (UX) và xây dựng phiên bản cải tiến giao diện khu vực **Danh mục sản phẩm** bằng HTML5 và CSS3 chuẩn ngữ nghĩa, tối ưu khả năng tương thích trên thiết bị di động.
## 2. Website tham khảo
- Tên website: Tiki
- URL: https://tiki.vn
- Nhóm sản phẩm: Đa ngành hàng (Sách, Thiết bị số - Phụ kiện, Điện thoại - Máy tính bảng, Điện gia dụng, Làm đẹp - Sức khỏe, Bách hóa...)
- Khách hàng mục tiêu: Học sinh, sinh viên, nhân viên văn phòng và người tiêu dùng trực tuyến tại Việt Nam có nhu cầu mua sắm nhanh chóng, tiện lợi.
- Các chức năng mua sắm chính: Tìm kiếm bằng thanh gợi ý thông minh, duyệt danh mục ngành hàng, xem chi tiết và cấu hình sản phẩm, giỏ hàng tự động tính toán voucher, đặt hàng và theo dõi vận chuyển.
- Khu vực đã khảo sát: Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng.

### Bảng khảo sát 5 khu vực thực tế:
| Khu vực | Chức năng đang cung cấp | Điểm hợp lý trong thiết kế | Điểm có thể cải thiện | Đề xuất cải tiến & Lý do |
| :--- | :--- | :--- | :--- | :--- |
| **Trang chủ** | - Hiển thị thanh cam kết (100% hàng thật, Freeship, Hoàn 200%, Đổi trả 30 ngày).<br>- Banner sự kiện lớn ("Yêu thương bản thân", "Xả kho cuối tuần").<br>- Widget nút nổi góc phải: “Tải App nhận quà”, “Trợ lý”, “Tin mới”. | - Tông màu xanh dương đồng bộ, cam kết thương hiệu rõ ràng tạo độ tin cậy cao.<br>- Phân cấp rõ nét giữa banner chính và lưới tiện ích bên dưới. | Thanh công cụ nổi bên góc phải (“Trợ lý”, "Tin mới") chiếm diện tích cố định, dễ đè lên nội dung sản phẩm khi cuộn trang. | Cho phép người dùng thu gọn nút trợ lý thành biểu tượng nhỏ để giải phóng không gian hiển thị sản phẩm. |
| **Danh mục sản phẩm** | - Hiển thị dạng cột dọc danh sách ngành hàng kèm icon trực quan (Nhà sách, Điện gia dụng, Làm đẹp...).<br>- Hiệu ứng highlight xám bo góc khi người dùng di chuột hoặc chọn ngành hàng ("Điện Thoại - Máy Tính Bảng"). | - Icon minh họa rõ ràng, kích thước chữ vừa vặn, bố cục dọc bên trái gọn gàng giúp định hướng danh mục nhanh. | Danh mục chỉ hiển thị cấp 1 ở menu ngoài, chưa mở rộng menu phụ cấp 2 dạng bay ngay khi rê chuột để chọn nhanh nhóm hàng con. | Thêm menu đa cấp bay ngang khi rê chuột để khách hàng truy cập thẳng vào danh mục con mà không cần bấm chuyển trang nhiều lần. |
| **Chi tiết sản phẩm** | - Thanh breadcrumb điều hướng cấp bậc chi tiết.<br>- Khung ảnh sản phẩm kèm ảnh thu nhỏ (thumbnail) bên dưới.<br>- Cột phải cố định hiển thị: Nhà bán "Tiki Trading", chọn số lượng, nút "Mua ngay", "Thêm vào giỏ" và "Mua trước trả sau". | - Khối mua hàng bên phải rất tập trung: nút "Mua ngay" màu đỏ nổi bật nhất trang, hiển thị tạm tính rõ ràng.<br>- Có đầy đủ thông tin thời gian giao hàng và địa chỉ nhận hàng. | Phần giá bán thể hiện mức giảm (-48%) bên cạnh giá gốc gạch ngang nhưng cỡ chữ giá gốc khá nhỏ và mờ nhạt nếu nhìn lướt. | Tăng độ tương phản cho giá gốc và làm nổi bật badge giảm giá màu đỏ để khách hàng dễ so sánh mức độ hời của sản phẩm. |
| **Tìm kiếm** | - Thanh input tìm kiếm trên header có gợi ý sẵn (“Freeship đơn từ 45k”).<br>- Dropdown mở rộng hiển thị: Lịch sử tìm kiếm gần nhất, mục "Tìm Kiếm Phổ Biến", và lưới “Danh Mục Nổi Bật” có hình tròn minh họa. | - Dropdown phân chia 3 tầng nội dung rất khoa học, hình ảnh danh mục nổi bật trực quan giúp giữ chân người dùng khi chưa biết mua gì. | Mục "Tìm Kiếm Phổ Biến" và lịch sử tìm kiếm xếp chung trong một khung dài khiến người dùng dễ ấn nhầm vào từ khóa gợi ý thay vì lịch sử của mình. | Tách rõ phần "Lịch sử tìm kiếm của bạn" có nút "Xóa tất cả" riêng biệt ở trên cùng để người dùng dễ quản lý quyền riêng tư. |
| **Giỏ hàng** | - Checkbox chọn tất cả hoặc chọn theo từng gian hàng ("Tiki Trading").<br>- Bộ đếm số lượng (+/-), nút xóa (thùng rác), thông báo số lượng tồn ("Còn 4 sản phẩm").<br>- Khung phải hiển thị danh sách voucher ("Giảm 8%", "Giảm 50K") và bảng tổng tiền chi tiết. | - Tự động áp dụng và tính toán tiền giảm giá trực tiếp (-36.500đ, -12.120đ) rất minh bạch.<br>- Cảnh báo số lượng tồn kho giúp người mua chủ động chốt đơn sớm. | Khối voucher khuyến mãi bên phải có nhiều nút "Bỏ chọn" / "Chọn" với màu xanh khá giống nhau, dễ gây nhầm lẫn voucher nào đang có hiệu lực. | Sử dụng viền xanh lá hoặc icon tích xanh rõ nét hơn cho voucher đang được áp dụng để người mua yên tâm về mức giá cuối cùng. |
## 3. Chức năng
- **Bộ lọc tab nhanh:** Cho phép người dùng chuyển nhanh giữa các nhóm nhu cầu (Tất cả, Thiết bị công nghệ, Đời sống, Sức khỏe, Sách...).
- **Lưới danh mục sản phẩm:** Hiển thị các khối ngành hàng trực quan với icon kích thước lớn, tiêu đề rõ ràng, số lượng sản phẩm ước tính và nhãn ưu đãi nổi bật (“Flash Sale”, “Chính hãng 100%”, “Freeship”).
- **Liên kết khám phá:** Nút điều hướng trực tiếp vào từng danh mục con.
- **Đáp ứng đa kích thước màn hình:** 
  - Máy tính: Hiển thị lưới 3 cột cân đối.
  - Máy tính bảng: Tự động co giãn thành 2 cột.
  - Điện thoại: Chuyển thành 1 cột duy nhất; thanh bộ lọc hỗ trợ vuốt cuộn ngang mượt mà (`overflow-x: auto`).

## 4. Công nghệ
- **HTML5:** Sử dụng cấu trúc ngữ nghĩa tiêu chuẩn (`<header>`, `<main>`, `<nav>`, `<section>`, `<article>`, `<footer>`).
- **CSS3:** Tổ chức file riêng biệt (`css/style.css`), áp dụng kỹ thuật CSS Grid, Flexbox và Media Queries (`@media`). Không sử dụng thư viện ngoài hoặc mã nguồn bên thứ ba.

## 5. Cách chạy
- **Cách 1 (Chạy cục bộ):** Mở trực tiếp tệp `index.html` bằng các trình duyệt phổ biến (Google Chrome, Microsoft Edge, Mozilla Firefox).
- **Cách 2 (Xem trực tuyến):** Truy cập đường dẫn đã được triển khai qua GitHub Pages:
  `https://[USERNAME_CUA_BAN].github.io/ecommerce-ui-improvement/`

## 6. Cải tiến đã thực hiện
- **Vấn đề ban đầu:** 
  - Menu danh mục sản phẩm dọc trên các trang TMĐT truyền thống thường đơn điệu, chữ và icon nhỏ, chỉ liệt kê tên mà không có thông tin ưu đãi kích thích mua sắm.
  - Khi xem trên điện thoại, danh mục dọc chiếm diện tích cuộn rất dài hoặc bị giấu trong menu con khiến người dùng khó thao tác nhanh.
- **Thay đổi và giải pháp thực hiện:** 
  1. Chuyển đổi hoàn toàn từ danh sách dọc đơn điệu sang hệ thống lưới thẻ ngành hàng hiện đại, bổ sung icon lớn và bo góc mềm mại.
  2. Bổ sung thông tin số lượng sản phẩm ước tính và các tag khuyến mãi màu đỏ/hồng nổi bật (`.category-tag`) giúp người dùng nắm bắt nhanh các cơ hội giảm giá.
  3. "Bổ sung thanh tab lọc nhanh (.category-tabs) với thuộc tính overflow-x: auto kết hợp các nút bấm .tab-btn có white-space: nowrap cho phép cuộn ngang dễ dàng trên màn hình cảm ứng di động.
  4. Sử dụng `@media (max-width: 576px)` để tự động chuyển layout lưới về 1 cột trên điện thoại, đảm bảo các thẻ danh mục hiển thị to, rõ, dễ bấm.

## 7. Hỗ trợ từ AI
- **Những phần AI hỗ trợ:** 
  - Gợi ý khung prompt phân tích trải nghiệm người dùng (UX) theo tiêu chuẩn chuyên gia TMĐT.
  - Đề xuất bảng phân tích cấu trúc 5 khu vực website.
  - Gợi ý đoạn mã khung HTML5 ngữ nghĩa và cú pháp CSS Grid/Flexbox ban đầu cho giao diện danh mục.
- **Phần sinh viên kiểm tra, điều chỉnh và tự thực hiện:** 
  - Trực tiếp khảo sát, chụp ảnh màn hình và đối chiếu lại dữ liệu thực tế trên website Tiki.vn (loại bỏ các nhận định chưa được kiểm chứng của AI).
  - Tinh chỉnh mã màu chủ đạo `#0b74e5` theo đúng nhận diện thương hiệu của Tiki.
  - Tự thay thế các file ảnh ngoài bằng hệ thống icon emoji nhẹ, bổ sung thuộc tính cuộn ngang mượt mà cho thanh tab trên điện thoại.
  - Sử dụng Chrome DevTools (F12) để kiểm thử thực tế độ co giãn giao diện trên các kích thước màn hình: Desktop (1200px), iPad Mini (768px) và iPhone SE/12 Pro (375px - 576px).
