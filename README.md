# Garden Manager V1.0 — bản tối ưu điện thoại + bản đồ kéo thả

Bản này vẫn giữ **dữ liệu V1.0** và cùng khóa lưu `garden-manager-v1.0`, nên nếu anh cập nhật trên **đúng URL GitHub Pages cũ**, dữ liệu đang có trên điện thoại/trình duyệt vẫn được đọc lại bình thường.

## Điểm thay đổi chính

- Giao diện co gọn hơn trên điện thoại, hạn chế tràn ngang toàn trang.
- Module **Bản đồ** được thiết kế lại theo hướng bố trí trực quan.
- Có nút **Bố trí ngang** để dùng gần toàn màn hình khi xoay điện thoại ngang.
- Hướng bản đồ giống sơ đồ gốc: **0 m nằm bên phải**, số mét tăng dần về bên trái.
- Chia vườn dài 125 m thành các khung 5 m / 10 m / 15 m để thao tác dễ trên điện thoại.
- Block đã đặt có thể **chạm giữ và kéo trực tiếp**; thả ra là lưu vị trí.
- Có thể chọn bước căn khi kéo: 1 cm / 5 cm / 10 cm.
- Chậu tròn chỉ cần nhập **đường kính**.
- Chậu vuông chỉ cần nhập **cạnh**.
- Luống/chậu chữ nhật nhập **dài × rộng**.
- Mọi tọa độ X/Y đều được quy ước tại **tâm vật thể**. Không dùng góc chậu làm mốc.
- Tọa độ số được đưa vào mục **Nâng cao**, không bắt buộc khi bố trí bằng kéo thả.
- Block mới có thể tự đặt vào đoạn vườn đang xem; nếu chưa có chỗ thì nằm trong khay **Chưa đặt**.
- Ảnh sơ đồ vườn gốc được giữ trong app ở mục **Ảnh sơ đồ vườn gốc để đối chiếu**.
- Các “nhóm tham chiếu” từ ảnh cũ không còn bị tính như block thực tế trên Tổng quan/Bản đồ.

## Quy ước tọa độ

- **X tâm**: khoảng cách từ mốc **0 m** ở mép phải sơ đồ, chạy dọc theo chiều dài 125 m.
- **Y tâm**: khoảng cách từ mép trên của bản đồ xuống theo chiều rộng 5 m.
- Chậu tròn Ø50 cm: nếu tâm X = 1 cm thì chậu sẽ vượt biên vì bán kính là 25 cm. Tâm phải cách mép tối thiểu 25 cm. Bản mới báo rõ lý do này thay vì chỉ báo “vượt ranh giới”.

## Cập nhật lên GitHub Pages cũ

1. Trong repository Garden đang dùng, sao lưu dữ liệu JSON từ app hiện tại trước.
2. Thay toàn bộ các file ở root bằng nội dung của gói này.
3. Commit/push lên nhánh đang dùng cho GitHub Pages.
4. Mở URL app bằng Chrome/Safari khi có mạng và tải lại một lần.
5. Service worker của gói này dùng cache mới nên sẽ thay bộ nhớ offline cũ sau khi kích hoạt.

Không đổi URL GitHub Pages nếu muốn tiếp tục dùng dữ liệu localStorage hiện tại trên cùng thiết bị/trình duyệt.

## Cài mới

- Android: mở URL GitHub Pages bằng Chrome → **Cài app / Thêm vào màn hình chính**.
- iPhone: Safari → **Chia sẻ → Thêm vào Màn hình chính**.
- App chạy tĩnh, không cần npm, server riêng hay API key.

## File trong gói

- `index.html` — ứng dụng V1.0 đã chỉnh.
- `manifest.webmanifest` — cho phép xoay ngang/dọc (`orientation: any`).
- `service-worker.js` — cache offline mới.
- `garden-reference.png` — ảnh sơ đồ vườn anh cung cấp.
- `icon-192.png`, `icon-512.png` — icon app.
- `.nojekyll` — dùng cho GitHub Pages.
