# AI Usage Log

## 1. Công cụ AI
- **Tên công cụ:** Google Gemini (hoặc ChatGPT).
- **Môi trường sử dụng:** Web browser, kết hợp môi trường lập trình Visual Studio Code[cite: 418].

## 2. Mục đích sử dụng
- **Phân tích nghiệp vụ & UX:** Sử dụng AI để hỗ trợ khảo sát cấu trúc chức năng và trải nghiệm người dùng của 5 khu vực chính trên website thương mại điện tử Tiki.vn theo mẫu của đề bài[cite: 419, 420, 426].
- **Đề xuất giải pháp giao diện:** Nhờ AI tư vấn phương án thiết kế bố cục lưới danh mục sản phẩm (Category Grid) và thanh tab lọc nhanh bằng HTML5/CSS3 chuẩn ngữ nghĩa[cite: 422, 426].
- **Tạo mã nguồn khung ban đầu:** Hỗ trợ sinh đoạn mã HTML và CSS cấu trúc cơ bản trước khi sinh viên tự tay kiểm tra, chỉnh sửa và hoàn thiện[cite: 423, 426].

---

## 3. Prompt đã sử dụng

### 3.1. Prompt 1 – Phân tích khảo sát website (Nhiệm vụ 2)
> "Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử.  
> Tôi đang khảo sát website: Tiki (https://tiki.vn)[cite: 420].  
> Hãy giúp tôi lập bảng phân tích các khu vực[cite: 420, 421]:  
> 1. Trang chủ[cite: 421].  
> 2. Danh mục sản phẩm[cite: 421].  
> 3. Chi tiết sản phẩm[cite: 421].  
> 4. Tìm kiếm[cite: 421].  
> 5. Giỏ hàng[cite: 421].  
> Với mỗi khu vực, hãy nêu: mục đích của chức năng, thành phần giao diện cần có, điểm thuận tiện đối với khách hàng, một vấn đề có thể phát sinh, một đề xuất cải tiến[cite: 421].  
> Không khẳng định những tính năng chưa được kiểm chứng[cite: 421]. Phân biệt rõ nhận xét dựa trên quan sát và đề xuất của AI[cite: 421]."

### 3.2. Prompt 2 – Đề xuất phương án thiết kế giao diện (Nhiệm vụ 3 - Bước 2)
> "Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3.  
> Tôi muốn cải tiến khu vực: Danh mục sản phẩm (Category Navigation/Grid)[cite: 421, 422].  
> Đối tượng sử dụng: Khách hàng mua sắm trực tuyến tại Việt Nam[cite: 422].  
> Hãy đề xuất[cite: 422, 423]:  
> 1. Bố cục giao diện[cite: 422].  
> 2. Các thành phần HTML cần sử dụng.  
> 3. Cách tổ chức CSS[cite: 423].  
> 4. Cách hiển thị trên máy tính và điện thoại[cite: 423].  
> 5. Những điểm cần kiểm tra về khả năng sử dụng[cite: 423].  
> Trước tiên, hãy giải thích phương án thiết kế[cite: 423]. Chưa tạo toàn bộ mã nguồn cho đến khi tôi yêu cầu[cite: 423]."

### 3.3. Prompt 3 – Sinh mã nguồn HTML/CSS (Nhiệm vụ 3 - Bước 3)
> "Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3[cite: 423].  
> Yêu cầu: Giao diện có tiêu đề và khu vực sản phẩm; có tối thiểu 4 sản phẩm/danh mục mẫu; mỗi khối có icon minh họa, tên, nhãn khuyến mãi và nút thao tác; bố cục phù hợp với màn hình máy tính và điện thoại; mã HTML có cấu trúc rõ ràng; CSS được tách thành file riêng; không sử dụng backend hoặc cơ sở dữ liệu; không đưa thư viện ngoài vào dự án[cite: 423].  
> Giải thích cách chạy trang web và những phần tôi cần kiểm tra[cite: 423]."

---

## 4. Kết quả AI đề xuất
- **Về phân tích:** AI đã phân tích đầy đủ mục đích, cấu trúc thành phần và các điểm nghẽn UX tiềm ẩn của 5 khu vực trên Tiki[cite: 420, 421].
- **Về giải pháp thiết kế:** AI đề xuất cấu trúc phân chia rõ ràng giữa Header, thanh Filter Tab ngang và lưới Card sản phẩm/danh mục[cite: 422, 423].
- **Về mã nguồn:** AI cung cấp khung HTML5 sử dụng các thẻ ngữ nghĩa cơ bản (`header`, `main`, `section`, `article`, `footer`) và mã CSS sử dụng Flexbox cùng CSS Grid[cite: 423].

---

## 5. Kiểm tra và điều chỉnh (Sinh viên tự thực hiện)
Theo đúng yêu cầu không sao chép mù quáng từ AI[cite: 418, 421], sinh viên đã đối chiếu website thực tế và tự điều chỉnh các điểm sau[cite: 421, 423]:
1. **Loại bỏ nhận xét lý thuyết của AI:** AI từng giả định Tiki thiếu thanh tìm kiếm cố định và gợi ý voucher không tự động. Sinh viên đã kiểm tra giao diện Tiki thực tế và loại bỏ nhận định này vì thanh tìm kiếm Tiki có tính năng auto-complete rất tốt và giỏ hàng tự động trừ tiền khuyến mãi[cite: 421].
2. **Sửa đổi mã nguồn AI tạo ra:**
   - **Thay thế thư viện icon:** Ban đầu AI sử dụng thẻ `<i>` liên kết tới thư viện ngoài (FontAwesome). Sinh viên đã chủ động gỡ bỏ thư viện theo đúng yêu cầu đề bài ("không đưa thư viện ngoài"), thay thế bằng hệ thống biểu tượng chuẩn UTF-8/Emoji kết hợp khung nền bo góc mềm mại[cite: 423].
   - **Tối ưu trải nghiệm cuộn ngang trên di động:** Sinh viên tự bổ sung thuộc tính `overflow-x: auto` và `white-space: nowrap` cho khối `.category-tabs` trong tệp `style.css` để thanh tab trên điện thoại có thể vuốt ngang mượt mà mà không bị tràn khung hay gãy dòng.
   - **Điều chỉnh màu sắc:** Tinh chỉnh mã màu chủ đạo của Header và nút bấm sang `#0b74e5` nhằm tái hiện đúng tông màu thương hiệu của Tiki.vn.
   - **Kiểm thử thực tế:** Tự mở trình duyệt Chrome, sử dụng Chrome DevTools (F12) để kiểm tra giao diện trên nhiều độ phân giải: Máy tính bàn (1200px), Tablet iPad (768px) và Điện thoại di động (375px - 414px)[cite: 423, 424].

---

## 6. Phần tôi hiểu và có thể giải thích
Sinh viên nắm vững và sẵn sàng giải thích các nội dung kỹ thuật sau khi giảng viên vấn đáp[cite: 418, 424, 426]:
- **Ý nghĩa cấu trúc HTML5:** Hiểu rõ lý do sử dụng `<header>` cho phần đầu trang, `<nav>` cho thanh điều hướng/bộ lọc, `<main>` chứa nội dung trọng tâm, `<article>` cho từng thẻ card ngành hàng độc lập và `<footer>` cho thông tin bản quyền[cite: 423].
- **Cơ chế dàn trang bằng CSS Grid:** Giải thích được cách hoạt động của `display: grid` kết hợp `grid-template-columns: repeat(3, 1fr)` để chia 3 cột đều nhau trên màn hình lớn và khoảng cách `gap: 20px`.
- **Kỹ thuật Responsive với Media Query:** Nắm vững đoạn mã `@media (max-width: 576px)` để tự động gộp các cột về dạng `1fr` (1 cột duy nhất) trên điện thoại nhằm tối ưu diện tích chạm vuốt của ngón tay.
- **Tính toán khung hộp (Box Model):** Hiểu rõ việc sử dụng `* { box-sizing: border-box; }` ở đầu file CSS để chiều rộng của các phần tử luôn tính gộp cả padding và border, tránh bị vỡ bố cục khi co dãn màn hình.