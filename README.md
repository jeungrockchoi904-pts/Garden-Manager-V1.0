# Garden Manager V1.1.4 — Dimension & Save Fix

Bản nâng cấp từ V1.1.3, giữ nguyên khóa dữ liệu `garden-manager-v1.0`.

## Sửa chính

- Sửa luồng **Lưu** khi chỉnh thông tin vườn, khu và chậu; chỉ đóng hộp thoại sau khi dữ liệu lưu thành công.
- Khi sửa kích thước chậu làm vị trí cũ không còn hợp lệ, app vẫn lưu thông tin và tự đưa chậu về **Chưa đặt** thay vì chặn toàn bộ thao tác lưu.
- Chậu tròn: nhập **đường kính ngoài/phủ bì** và **đường kính trong/lòng chậu**.
- Chậu vuông/chữ nhật: nhập **kích thước phủ bì** và **kích thước lòng chậu** riêng.
- Bổ sung **chiều cao phủ bì**, **chiều sâu lòng chậu** và **tỷ lệ đất lấp đầy (%)**.
- Thể tích đất được tính từ kích thước lòng chậu + chiều sâu lòng + tỷ lệ lấp đầy + hệ số hình dáng của mẫu chậu.
- Gợi ý cây dùng **độ sâu đất thực** thay vì chỉ dùng chiều cao chậu ngoài.
- Giữ đúng phương hướng: **0 m = Tây / bên phải → 125 m = Đông / bên trái; Bắc hướng xuống dưới**.

## Cập nhật GitHub Pages

Giải nén ZIP và upload đè toàn bộ file vào root repo hiện tại. Không tạo repo mới. Sau khi GitHub Pages deploy, mở URL với `?v=114` một lần để bỏ cache.
