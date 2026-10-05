# Garden Manager V1.0.1 — Mobile UI Test

Bản thử nghiệm này ưu tiên **sửa giao diện điện thoại trước**, đồng thời vẫn giữ nguyên **schema dữ liệu V1.0** và khóa localStorage `garden-manager-v1.0`. Vì vậy nếu cập nhật trên đúng URL GitHub Pages cũ, dữ liệu V1 đang có vẫn được đọc lại.

## Thay đổi giao diện chính

- Header mới: **menu trái → Garden Manager căn giữa → chuông thông báo**.
- Bỏ kích thước vườn khỏi header và bỏ nút `+ Thêm mới` ở header.
- Thanh dưới điện thoại có đúng 5 module, tự fit ngang màn hình:
  1. Tổng quan
  2. Sơ đồ
  3. Cây trồng
  4. Nhật ký
  5. Lịch
- **Cài đặt / Sao lưu & Khôi phục / Cơ sở dữ liệu** được chuyển vào menu trái.
- Menu trái có thêm nhóm **Thông tin & Hướng dẫn**:
  - Trồng · chăm sóc · thu hoạch theo cây
  - Hướng dẫn phân bón
  - Hướng dẫn thuốc BVTV
  - Nấm bệnh thông dụng

## Tổng quan

- Chạm thẻ diện tích để sửa ngay tên và kích thước vườn.
- Chạm thẻ Block hoặc Chưa đặt để chuyển sang Sơ đồ.
- Chạm từng Khu để sửa tên, mốc bắt đầu và kích thước khu.

## Sơ đồ

- Đổi tên `Bản đồ` thành **Sơ đồ**.
- Mặc định khung **5 m × 5 m**.
- Có thể chọn:
  - Khung 5 × 5 m
  - Toàn bộ vườn
  - Từng Khu đã nhập đủ mốc bắt đầu + dài + rộng
- Block dùng viền mảnh và nền nhạt hơn.
- Có thể chọn hiển thị **Tên cây** hoặc **Mã block**.
- Nếu block đã trồng cây, ưu tiên hiện tên cụ thể như `Đu đủ` thay vì nhóm `Cây ăn quả`.
- Chạm block có cây → hiện bảng thông tin nhanh.
- Chạm block trống → mở ngay form thêm cây vào block đó.
- Giữ và kéo block để thay đổi vị trí.

## Cây trồng

- Form thêm/sửa cây có ô **tìm kiếm loại cây/giống**.
- Chỉ giữ hai mốc ngày chính: **Ngày gieo** và **Ngày trồng**.
- Có nút **Xóa** để đưa ngày về trống.
- Bỏ nhập khoảng ngày, tháng/năm riêng và tuổi ước tính thủ công.
- Tuổi cây được tự tính từ ngày trồng; nếu chưa có ngày trồng thì dùng ngày gieo.

## Lịch

- Module Lịch mới thay vị trí Cài đặt ở thanh dưới.
- Chọn xem **Tuần / Tháng**.
- Chạm vào một ngày để thêm công việc/hoạt động cho ngày đó.
- Các hoạt động tương lai được xem là việc phải làm; hoạt động quá khứ là việc đã làm.
- Chuông trên header hiển thị số công việc trong 7 ngày tới.

## Hướng dẫn cập nhật

1. Trong app hiện tại, tải một bản sao lưu JSON.
2. Giải nén gói này.
3. Thay toàn bộ file ở root của repository GitHub Pages hiện tại bằng các file trong gói.
4. Commit/push.
5. Mở lại URL Garden khi có mạng và refresh một lần.
6. Nếu app cài trên màn hình chính vẫn giữ giao diện cũ, đóng hẳn app rồi mở lại sau khi trang web đã cập nhật.

Không đổi URL GitHub Pages nếu muốn tiếp tục dùng vùng localStorage hiện tại.

## File trong gói

- `index.html`
- `manifest.webmanifest`
- `service-worker.js`
- `garden-reference.png`
- `icon-192.png`
- `icon-512.png`
- `.nojekyll`
