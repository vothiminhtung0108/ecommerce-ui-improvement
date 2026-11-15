# AI Usage Log

## 1. Công cụ AI

- **Tên công cụ:** Gemini (Google AI)

## 2. Mục đích sử dụng

Phân tích giao diện website thương mại điện tử, đề xuất phương án thiết kế lại trang chi tiết sản phẩm (PDP), giải thích cấu trúc HTML/CSS ngữ nghĩa, hỗ trợ tạo mã nguồn responsive và chẩn đoán, sửa lỗi đường dẫn/định dạng hình ảnh.

## 3. Prompt đã sử dụng

1. *“Bạn là chuyên gia phân tích nghiệp vụ và thiết kế trải nghiệm người dùng cho website thương mại điện tử. Tôi đang khảo sát website: Cellphones https://cellphones.com.vn/. Hãy giúp tôi lập bảng phân tích các khu vực: 1. Trang chủ 2. Danh mục sản phẩm 3. Chi tiết sản phẩm 4. Tìm kiếm 5. Giỏ hàng...”*
2. *“Quy trình thực hiện bài tập là một chuỗi logic liền mạch... Giờ nên cải tiến gì?”*
3. *“Tôi đang thực hiện bài tập phát triển giao diện website thương mại điện tử bằng HTML5 và CSS3. Tôi muốn cải tiến khu vực: Chi tiết sản phẩm. Đối tượng sử dụng: khách hàng mua sắm trực tuyến tại Việt Nam. Hãy đề xuất: 1. Bố cục giao diện 2. Các thành phần HTML cần sử dụng 3. Cách tổ chức CSS 4. Cách hiển thị trên máy tính và điện thoại 5. Những điểm cần kiểm tra về khả năng sử dụng...”*
4. *“Dựa trên phương án đã thống nhất, hãy tạo một trang giao diện thương mại điện tử bằng HTML5 và CSS3...”*
5. *“Giữ nguyên code file Html và Css chỉ sửa lại tên hình cho link với file images trong hình.”*
6. *“Check lại code xem trỏ đúng chưa? Hay có lỗi tên hình không [kèm hình ảnh cây thư mục VS Code].”*
7. *“Dòng pin sạc dự phòng không hiển thị hình”*

## 4. Kết quả AI đề xuất

- Bảng đánh giá phân tích nghiệp vụ và trải nghiệm người dùng đối với năm khu vực trên website CellphoneS.
- Bản đề xuất cấu trúc bố cục, danh sách thẻ ngữ nghĩa HTML5 và phương án responsive CSS cho trang chi tiết sản phẩm iPhone 16 Pro Max.
- Mã nguồn file `index.html` và `style.css`.
- Chẩn đoán nguyên nhân ảnh không hiển thị dựa trên cây thư mục VS Code: sai phần mở rộng file (`.png` thay vì `.webp`/`.jpg`), sai tên file AirPods có dấu gạch dưới kép và tên file pin sạc dự phòng dài bị hệ thống cắt ngắn.

## 5. Kiểm tra và điều chỉnh

- **Điểm đã kiểm tra:** Kiểm tra cây thư mục thực tế trong VS Code và rà soát từng thuộc tính `src` trong các thẻ `<img>`.
- **Điểm đã sửa đổi:**
  - Sửa các đường dẫn ảnh trong `index.html` từ `.png` sang `.webp` để phù hợp với định dạng file thực tế.
  - Đổi tên file ảnh `images.png` thành `images.jpg` cho sản phẩm củ sạc Apple.
  - Đổi tên file ảnh pin sạc dự phòng trên ổ đĩa thành `pin-sac-du-phong.webp` và cập nhật lại mã HTML.
  - Sửa lỗi tên ảnh AirPods Pro 2 có hai dấu gạch dưới trong `_8__2_1_1`.
- **Điểm không sử dụng:** Không dùng JavaScript hay thư viện CSS bên ngoài (Bootstrap/Tailwind), nhằm tuân thủ yêu cầu sử dụng HTML5/CSS3 thuần.

## 6. Phần tôi hiểu và có thể giải thích

### Các thành phần HTML5 quan trọng

- Thẻ `<article class="product-hero">` bao bọc khối thông tin sản phẩm chính.
- Thẻ `<figure>` kết hợp với `<img>` quản lý vùng hiển thị hình ảnh sản phẩm và nhãn giảm giá.
- Thẻ `<fieldset>` và `<legend>` nhóm các lựa chọn màu sắc, dung lượng trong biểu mẫu.
- Thẻ `<aside class="sticky-bottom-bar">` tạo thanh mua hàng cố định ở đáy màn hình di động.

### Cách tổ chức CSS3 quan trọng

- Khai báo biến toàn cục trong `:root` (ví dụ `--primary-color`, `--border-color`) để quản lý màu sắc tập trung.
- Sử dụng `display: grid` để chia bố cục thành hai cột theo tỷ lệ `5fr 7fr` trên máy tính và hiển thị bốn sản phẩm phụ kiện trên một hàng.
- Dùng `display: flex` để căn chỉnh các thành phần giao diện như nút chọn phiên bản, mức giá và breadcrumb.
- Áp dụng `@media (min-width: 992px)` để điều chỉnh giao diện cho màn hình máy tính so với thiết bị di động.
