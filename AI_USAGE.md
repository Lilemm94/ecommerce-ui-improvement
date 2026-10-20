# AI Usage Log

## 1. Công cụ AI
- **Tên công cụ:** Google Gemini
- **Môi trường sử dụng:** Web browser, kết hợp môi trường lập trình Visual Studio Code

## 2. Mục đích sử dụng
- **Phân tích nghiệp vụ & UX:** Sử dụng AI để hỗ trợ khảo sát cấu trúc chức năng và trải nghiệm người dùng của 5 khu vực chính trên website thương mại điện tử Tiki.vn theo mẫu của đề bài.
- **Đề xuất giải pháp giao diện:** Nhờ AI tư vấn phương án thiết kế bố cục lưới danh mục sản phẩm  và thanh tab lọc nhanh bằng HTML5/CSS3 chuẩn ngữ nghĩa
- **Tạo mã nguồn khung ban đầu:** Hỗ trợ sinh đoạn mã HTML và CSS cấu trúc cơ bản trước khi sinh viên tự tay kiểm tra, chỉnh sửa và hoàn thiện].

---

## 3. Prompt đã sử dụng

### 3.1. Prompt 1 – Phân tích khảo sát website (Nhiệm vụ 2)
> "Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử.  
> Tôi đang khảo sát website: Tiki (https://tiki.vn)  
> Hãy giúp tôi lập bảng phân tích các khu vực:  
> 1. Trang chủ.  
> 2. Danh mục sản phẩm.  
> 3. Chi tiết sản phẩm.  
> 4. Tìm kiếm.  
> 5. Giỏ hàng.  
> Với mỗi khu vực, hãy nêu: mục đích của chức năng, thành phần giao diện cần có, điểm thuận tiện đối với khách hàng, một vấn đề có thể phát sinh, một đề xuất cải tiến[cite: 421].  
> Không khẳng định những tính năng chưa được kiểm chứng. Phân biệt rõ nhận xét dựa trên quan sát và đề xuất của AI."

### 3.2. Prompt 2 – Đề xuất phương án thiết kế giao diện (Nhiệm vụ 3 - Bước 2)
> "Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3.  
> Tôi muốn cải tiến khu vực: Danh mục sản phẩm
> Đối tượng sử dụng: Khách hàng mua sắm trực tuyến tại Việt Nam.  
> Hãy đề xuất:  
> 1. Bố cục giao diện.  
> 2. Các thành phần HTML cần sử dụng.  
> 3. Cách tổ chức CSS.  
> 4. Cách hiển thị trên máy tính và điện thoại. 
> 5. Những điểm cần kiểm tra về khả năng sử dụng.  
> Trước tiên, hãy giải thích phương án thiết kế. Chưa tạo toàn bộ mã nguồn cho đến khi tôi yêu cầu."

### 3.3. Prompt 3 – Sinh mã nguồn HTML/CSS (Nhiệm vụ 3 - Bước 3)
> "Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3."  
> Yêu cầu: Giao diện có tiêu đề và khu vực sản phẩm; có tối thiểu 4 sản phẩm/danh mục mẫu; mỗi khối có icon minh họa, tên, nhãn khuyến mãi và nút thao tác; bố cục phù hợp với màn hình máy tính và điện thoại; mã HTML có cấu trúc rõ ràng; CSS được tách thành file riêng; không sử dụng backend hoặc cơ sở dữ liệu; không đưa thư viện ngoài vào dự án.  
> Giải thích cách chạy trang web và những phần tôi cần kiểm tra."

---

## 4. Kết quả AI đề xuất
- **Về phân tích:** AI đã phân tích đầy đủ mục đích, cấu trúc thành phần và các điểm nghẽn UX tiềm ẩn của 5 khu vực trên Tiki.
- **Về giải pháp thiết kế:** AI đề xuất cấu trúc phân chia rõ ràng giữa Header, thanh Filter Tab ngang và lưới Card sản phẩm/danh mục.
- **Về mã nguồn:** AI cung cấp khung HTML5 sử dụng các thẻ ngữ nghĩa cơ bản (`header`, `main`, `section`, `article`, `footer`) và mã CSS sử dụng Flexbox cùng CSS Grid.

---

## 5. Kiểm tra và điều chỉnh (Sinh viên tự thực hiện)
Theo đúng yêu cầu không sao chép mù quáng từ AI[cite: 418, 421], sinh viên đã đối chiếu website thực tế và tự điều chỉnh các điểm sau:
1. **Loại bỏ nhận xét lý thuyết của AI:** AI từng giả định Tiki thiếu thanh tìm kiếm cố định và gợi ý voucher không tự động. Sinh viên đã kiểm tra giao diện Tiki thực tế và loại bỏ nhận định này vì thanh tìm kiếm Tiki có tính năng auto-complete rất tốt và giỏ hàng tự động trừ tiền khuyến mãi.
2. **Sửa đổi mã nguồn AI tạo ra:**
   - **Thay thế thư viện icon:** Ban đầu AI sử dụng thẻ `<i>` liên kết tới thư viện ngoài. Sinh viên đã chủ động gỡ bỏ thư viện theo đúng yêu cầu đề bài ("không đưa thư viện ngoài"), thay thế bằng hệ thống biểu tượng chuẩn UTF-8/Emoji kết hợp khung nền bo góc mềm mại.
   - **Tối ưu trải nghiệm cuộn ngang trên di động:** Sinh viên tự bổ sung thuộc tính `overflow-x: auto` và `white-space: nowrap` cho khối `.category-tabs` trong tệp `style.css` để thanh tab trên điện thoại có thể vuốt ngang mượt mà mà không bị tràn khung hay gãy dòng.
   - **Điều chỉnh màu sắc:** Tinh chỉnh mã màu chủ đạo của Header và nút bấm sang `#0b74e5` nhằm tái hiện đúng tông màu thương hiệu của Tiki.vn.
   - **Kiểm thử thực tế:** Tự mở trình duyệt Chrome, sử dụng Chrome DevTools (F12) để kiểm tra giao diện trên nhiều độ phân giải: Máy tính bàn (1200px), Tablet iPad (768px) và Điện thoại di động (375px - 414px).

---

## 6. Phần tôi hiểu và có thể giải thích
Sinh viên nắm vững và sẵn sàng giải thích các nội dung kỹ thuật sau khi giảng viên vấn đáp:
- **Ý nghĩa cấu trúc HTML5:** Hiểu rõ lý do sử dụng `<header>` cho phần đầu trang, `<nav>` cho thanh điều hướng/bộ lọc, `<main>` chứa nội dung trọng tâm, `<article>` cho từng thẻ card ngành hàng độc lập và `<footer>` cho thông tin bản quyền.
- **Cơ chế dàn trang bằng CSS Grid:** Giải thích được cách hoạt động của `display: grid` kết hợp `grid-template-columns: repeat(3, 1fr)` để chia 3 cột đều nhau trên màn hình lớn và khoảng cách `gap: 20px`.
- **Kỹ thuật Responsive với Media Query:** Nắm vững đoạn mã `@media (max-width: 576px)` để tự động gộp các cột về dạng `1fr` (1 cột duy nhất) trên điện thoại nhằm tối ưu diện tích chạm vuốt của ngón tay.
- **Tính toán khung hộp (Box Model):** Hiểu rõ việc sử dụng `* { box-sizing: border-box; }` ở đầu file CSS để chiều rộng của các phần tử luôn tính gộp cả padding và border, tránh bị vỡ bố cục khi co dãn màn hình.
