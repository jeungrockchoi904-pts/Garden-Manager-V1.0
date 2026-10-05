# Garden Manager V1.1.2 — Visual Garden · Render Fix

Bản sửa lỗi trang trắng sau khi nâng cấp từ các bản V1 cũ.

## Sửa chính
- Giữ nguyên khóa dữ liệu `garden-manager-v1.0`; không xóa dữ liệu đang lưu trên thiết bị.
- Bổ sung lớp tương thích khi dữ liệu V1 cũ thiếu trường/array mới.
- Có error boundary: nếu dữ liệu cũ gây lỗi render, app hiện nút **Khôi phục hiển thị** thay vì để trống toàn bộ nội dung.
- Giữ đúng phương hướng: **0 m = Tây / bên phải → 125 m = Đông / bên trái; Bắc hướng xuống**.
- Service Worker đổi cache sang V1.1.2 để tránh giữ `index.html` cũ.

## Cập nhật GitHub Pages
1. Không xóa Local Storage / dữ liệu trình duyệt.
2. Giải nén ZIP.
3. Upload đè toàn bộ file ở root repo hiện tại.
4. Commit.
5. Mở URL GitHub Pages bằng trình duyệt, refresh cứng 1 lần.
6. Nếu app đã cài trên điện thoại, đóng app rồi mở URL GitHub Pages trước để nhận V1.1.2, sau đó mở lại app.

Nếu vẫn thấy trang trắng, không xóa dữ liệu: V1.1.2 sẽ hiện thẻ lỗi và nút **Khôi phục hiển thị** để chuẩn hóa dữ liệu cũ.
