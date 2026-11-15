# E-commerce UI Improvement

## 1. Giới thiệu

Dự án tập trung khảo sát website thương mại điện tử bán lẻ thiết bị công nghệ và cải tiến giao diện người dùng (UI/UX) cho **trang chi tiết sản phẩm (Product Detail Page - PDP)** và **danh sách phụ kiện mua kèm**. Mục tiêu là phân tầng thông tin rõ ràng, giảm thao tác cuộn trang và tối ưu nút đặt mua trên cả máy tính lẫn thiết bị di động.

## 2. Website tham khảo

- **Tên website:** CellphoneS
- **URL:** [https://cellphones.com.vn/](https://cellphones.com.vn/)
- **Khu vực khảo sát:** Trang chủ, danh mục sản phẩm, chi tiết sản phẩm, tìm kiếm và giỏ hàng.

## 3. Chức năng

- Hiển thị thông tin chi tiết sản phẩm và giá bán.
- Hiển thị danh sách phụ kiện mua kèm.
- Bố cục đáp ứng nhiều kích thước màn hình.

## 4. Công nghệ

- HTML5
- CSS3

## 5. Cách chạy

Mở file `index.html` bằng trình duyệt. Không cần cài đặt thêm thư viện.

## 6. Cải tiến đã thực hiện

### Vấn đề

Khu vực mua hàng trên trang chi tiết sản phẩm có nhiều thông tin phụ như khuyến mãi, quà tặng và phụ kiện. Điều này có thể đẩy các nút thao tác chính xuống sâu hơn, gây phân tâm và tăng thao tác cuộn trang.

### Thay đổi

- Tái cấu trúc khu vực sản phẩm thành hai cột trên máy tính: thư viện ảnh ở cột trái; giá, phiên bản và nút mua hàng ở cột phải.
- Thu gọn chương trình ưu đãi thành danh sách.
- Đưa phụ kiện mua kèm xuống dưới khu vực mua hàng và hiển thị dạng lưới: một cột trên màn hình nhỏ, hai cột trên màn hình trung bình và bốn cột trên máy tính.
- Bổ sung thanh mua hàng cố định ở đáy màn hình di động để người dùng có thể truy cập nút **MUA NGAY** thuận tiện hơn.

## 7. Hỗ trợ từ AI

- **Phần AI hỗ trợ:** Phân tích UX/UI của năm khu vực chính trên website thương mại điện tử, đề xuất cải tiến bố cục PDP, cung cấp mã HTML5 ngữ nghĩa và xây dựng CSS Grid/Flexbox responsive.
- **Phần đã kiểm tra, điều chỉnh hoặc bổ sung:**
  - Kiểm tra đường dẫn ảnh trong `index.html` với các tệp thực tế trong thư mục `images/`.
  - Điều chỉnh phần mở rộng ảnh theo định dạng hiện có như `.webp` và `.jpg`.
  - Kiểm tra đường dẫn ảnh pin sạc dự phòng và ảnh AirPods, bao gồm tên tệp AirPods có ký tự gạch dưới kép.
