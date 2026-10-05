# Garden Manager V1.1.5 — Visual Garden · Full Audit Fix

Bản kiểm tra lại toàn bộ sau khi phát hiện repository GitHub đang chứa file trộn giữa V1.1.2 và V1.1.4.

## Sửa chính
- Đồng bộ `index.html`, `manifest.webmanifest`, `service-worker.js`, README về cùng V1.1.5.
- Tách lỗi ghi Local Storage khỏi lỗi render: lỗi giao diện không còn bị báo nhầm là lỗi lưu dữ liệu.
- Các form chính chỉ đóng sau khi ghi dữ liệu thành công; rollback khi lưu thất bại.
- Thay `structuredClone` bằng clone JSON tương thích rộng hơn cho dữ liệu app.
- Giữ đường kính/kích thước phủ bì và lòng chậu, chiều sâu lòng chậu, tỷ lệ đất lấp đầy, tính thể tích đất và gợi ý độ sâu.
- Giữ quy ước: **0 m = Tây / bên phải → 125 m = Đông / bên trái; Bắc hướng xuống dưới**.
- Service Worker dùng cache mới, điều hướng ưu tiên lấy bản mạng mới để tránh kẹt `index.html` cũ.

## Cập nhật GitHub Pages
Ghi đè **toàn bộ file root bằng đúng bộ V1.1.5 trong một commit**. Không xóa Local Storage của ứng dụng.

Sau deploy, mở URL GitHub Pages với `?v=115` và xác nhận header hiện `V1.1.5 · Visual Garden · Audit Fix`.
