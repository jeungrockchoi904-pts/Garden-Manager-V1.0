# Garden Manager V1.1.8 — Exact Zone Layout

Patch từ V1.1.7.

## Sửa chính
- Sửa lỗi nhập **1,5 m** nhưng phần Sơ đồ vẫn nhìn như **2 m**.
- Với các khu có cùng bề rộng bằng toàn vườn, app tự phân bổ **liên tiếp theo đúng thứ tự danh sách**, lấy chính xác số cm đã nhập; không làm tròn mét.
- Ví dụ: khu dài 1,5 m = **150 cm** và chiếm đúng 3 ô lưới 0,5 m. Khu kế tiếp bắt đầu ngay tại 1,5 m, không còn khoảng hở 0,5 m do mốc cũ 2 m.
- Khi sửa chiều dài một khu, app tự tính lại `startCm` của các khu phía sau nếu đang ở chế độ phân đoạn liên tiếp.
- Vẽ thêm **ranh giới khu** và nhãn chiều dài trực tiếp trên Sơ đồ để kiểm tra bằng mắt.
- Dòng phương hướng không còn cố định 125 m; lấy đúng **chiều dài vườn hiện tại**. Ví dụ vườn 23 m sẽ hiện `23 m = Đông (bên trái) ← 0 m = Tây (bên phải)`.
- Giữ lưới 0,5 m, kéo block theo cm và toàn bộ sửa lỗi trước đó.

## Cập nhật GitHub
Upload đè 4 file vào root repo hiện tại:
- `index.html`
- `service-worker.js`
- `manifest.webmanifest`
- `README.md`

Sau deploy mở `?v=118` để kiểm tra. Header phải hiện **V1.1.8 · Visual Garden · Exact Zone Layout**.
