# Garden Manager V1.1.3 — Visual Garden · Render Complete

Bản sửa hoàn chỉnh từ nhánh V1.1.0 đầy đủ chức năng.

## Sửa lỗi chính
- Khôi phục đầy đủ các module bị thiếu trong V1.1.1/V1.1.2: Tổng quan, Sơ đồ, Cây trồng, Nhật ký, Lịch, Cài đặt, Sao lưu, Cơ sở dữ liệu và 4 mục Hướng dẫn.
- Sửa lỗi trang trắng do `render()` tham chiếu tới các hàm module đã bị thiếu khỏi source.
- Giữ giao diện Visual Garden và thư viện chậu/cây của V1.1.0.
- Quy ước cố định: **0 m = Tây / bên phải → 125 m = Đông / bên trái; Bắc hướng xuống**.
- Kéo/thả và tọa độ trên Sơ đồ cùng dùng quy ước này.
- Giữ nguyên khóa dữ liệu `garden-manager-v1.0`; không xóa dữ liệu cũ.
- Có lớp chuẩn hóa dữ liệu cũ và error boundary.
- Service Worker dùng cache V1.1.3 mới.

## Cập nhật GitHub Pages
1. Sao lưu JSON nếu app cũ vẫn mở được trên thiết bị khác.
2. Upload đè **toàn bộ file bên trong gói này** vào root repo hiện tại.
3. Commit.
4. Chờ GitHub Pages deploy xong.
5. Mở URL Pages với `?v=113` một lần, sau đó reload.
