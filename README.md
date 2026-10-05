# Garden Manager V1.1.1 — Visual Garden · Orientation Fix

Bản V1.1.1 giữ nguyên khóa dữ liệu `garden-manager-v1.0` để đọc tiếp dữ liệu của các bản V1 trước.

## Quy ước phương hướng chuẩn

- **0 m = Tây = bên phải sơ đồ**.
- **125 m = Đông = bên trái sơ đồ**.
- **Bắc = hướng xuống dưới**.
- Vì vậy trục X tăng từ **phải sang trái**: `0 m → 125 m` về mặt giá trị, nhưng khi nhìn trên màn hình sẽ thấy `125 m / Đông` ở bên trái và `0 m / Tây` ở bên phải.

## Điểm chính của Visual Garden

- Nhận diện xanh mới đồng bộ toàn app và logo mới.
- 5 module chính dùng chung hệ thẻ, màu, nút, biểu mẫu và điều hướng mobile.
- Sơ đồ phong cách bán thực tế: nền gạch theo khu, chậu có vành/thân/đất, bóng đổ và nhóm cây mô phỏng.
- Mỗi khu có thể chọn 1 trong 4 nền: xám sáng, be/xi măng, đất nung, xám đậm.
- Thư viện chậu chuẩn hóa gồm chậu tròn cao vân trắng, chậu tròn thấp, chậu vuông loe, chậu vuông nhựa, chậu vuông trắng/xám, chậu chữ nhật, máng dài, hộc sâu, khay thấp, luống gỗ, bồn bê tông và giàn leo.
- Chậu có thêm `chiều cao / độ sâu đất`; app ước tính dung tích đất và phân loại Nông / Trung bình / Sâu.
- Khi chọn mẫu và thay kích thước, preview chậu, dung tích và gợi ý cây cập nhật tức thời.
- Hiển thị cây theo 6 nhóm: đất trống, rau xanh, rau tím/đỏ, cải/bắp/súp lơ, cây ăn quả tán chung, cây leo chỉ lá/dây trên giàn.

## Cập nhật lên GitHub Pages

1. Trong app hiện tại, bấm **Sao lưu** và tải JSON dự phòng.
2. Giải nén gói V1.1.1.
3. Thay toàn bộ file ở thư mục gốc repository GitHub Pages bằng các file trong gói này.
4. Commit / push lên nhánh đang dùng cho Pages.
5. Mở URL GitHub Pages bằng trình duyệt và tải lại một lần khi có mạng.
6. Nếu điện thoại còn giao diện cũ, đóng app đã cài, mở lại URL GitHub Pages bằng Chrome/Safari rồi reload; service worker V1.1.1 sẽ thay cache cũ.

## Cài trên thiết bị mới

Nút **Cài app** chỉ xuất hiện khi mở từ `*.github.io` và app chưa chạy ở chế độ standalone. Android/Chrome có thể cài trực tiếp. iPhone dùng Safari → Chia sẻ → Thêm vào Màn hình chính.

## Chuyển dữ liệu tọa độ

- Dữ liệu các bản cũ vốn đã dùng **0 m ở bên phải** sẽ được giữ nguyên.
- Nếu dữ liệu đã từng được lưu bằng V1.1.0 theo quy ước sai **0 m = Tây / bên trái**, V1.1.1 sẽ tự đảo lại tọa độ X của chậu và vị trí khu đúng **một lần** để giữ nguyên vị trí trực quan.
- Cờ chuyển đổi: `prefs.coordWestRightV111Migrated`.
