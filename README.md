# Garden Manager V1.1.7 — Zone & 0.5m Fix

Patch từ V1.1.6.

## Sửa chính
- Danh sách **Phạm vi Sơ đồ** nay hiển thị đồng bộ với danh sách **Khu vực** ở Tổng quan.
- Khu đã có kích thước nhưng chưa có **mốc bắt đầu** vẫn xuất hiện trong danh sách, có ghi rõ `thiếu mốc vị trí` và chưa cho chọn để tránh đặt sai tọa độ.
- Tổng quan phân biệt rõ: **Đã bố trí / Thiếu mốc / Chưa đo**.
- Sơ đồ hỗ trợ chính xác bước **0,5 m (50 cm)** thay vì làm tròn 1 m.
- Thanh chọn đoạn chạy theo bước 0,5 m; hai nút dịch chuyển cũng theo 0,5 m.
- Lưới Sơ đồ có vạch 0,5 m và nhãn 0,5 m; kích thước 4,5 m, 1,5 m... hiển thị nguyên giá trị, không làm tròn.
- Giữ nguyên quy ước phương hướng: **0 m = Tây / bên phải → 125 m = Đông / bên trái; Bắc hướng xuống**.
- Giữ nguyên sửa nhập **Tỷ lệ đất lấp đầy** của V1.1.6.

## Cập nhật GitHub
Upload đè 4 file này vào root repo hiện tại:
- `index.html`
- `service-worker.js`
- `manifest.webmanifest`
- `README.md`

Sau deploy mở `?v=117` để kiểm tra phiên bản.
