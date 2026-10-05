# Garden Manager V1.0 — GitHub Pages / PWA

Ứng dụng quản lý vườn chạy dạng web tĩnh, không cần npm, server riêng hay API key. Sau khi đưa lên GitHub Pages, có thể cài trên điện thoại như ứng dụng và dùng lại khi offline.

## Đưa lên GitHub Pages

1. Tạo repository mới trên GitHub, ví dụ `garden-manager`.
2. Giải nén gói này, đưa **toàn bộ nội dung bên trong thư mục** vào thư mục gốc của repository. `index.html` phải nằm ngay ở thư mục gốc.
3. Commit và push lên nhánh `main`.
4. Vào **Settings → Pages**; chọn **Deploy from a branch → main → /(root) → Save**.
5. Mở URL GitHub Pages được cấp. GitHub Pages chạy qua HTTPS; đợi biểu tượng lá xanh tải xong lần đầu để ứng dụng lưu bộ đệm offline.

Không cần chạy lệnh build. GitHub Pages phục vụ trực tiếp `index.html` và các tệp PWA đi kèm.

## Cài trên Android

Mở URL GitHub Pages bằng Chrome trên điện thoại, chọn **Cài app** trong ứng dụng hoặc menu Chrome **⋮ → Cài đặt ứng dụng / Thêm vào màn hình chính**. Sau khi cài, mở Garden từ biểu tượng mới tạo. Mở ứng dụng trực tuyến một lần để tải bộ nhớ offline.

## Cài trên iPhone

Mở URL bằng Safari → **Chia sẻ → Thêm vào Màn hình chính**. iOS có thể không hiển thị nút cài trong trang; dùng menu Chia sẻ của Safari.

## Lưu ý dữ liệu

- Dữ liệu được lưu trên thiết bị/trình duyệt nơi anh nhập; hiện V1.0 chưa đồng bộ giữa nhiều thiết bị.
- Dùng **Sao lưu** trong ứng dụng để tải JSON định kỳ. Trước khi xóa dữ liệu trình duyệt hoặc chuyển điện thoại, hãy sao lưu và khôi phục JSON.
- Giữ nguyên URL GitHub Pages để ứng dụng dùng cùng vùng lưu dữ liệu trên điện thoại.
- Mã HTML đã nhúng ảnh sơ đồ tham chiếu. Các nhóm trên sơ đồ chưa được coi là từng chậu/luống đã đo; tọa độ vẫn cần nhập thực tế.

## Quy ước cập nhật phiên bản

- Các bản sửa giao diện, sửa lỗi hoặc điều chỉnh nhỏ thuộc nhánh **V1**: thay `index.html`, giữ nguyên URL GitHub Pages. Mở ứng dụng khi có mạng một lần để tải bản mới; sau đó bản mới cũng được lưu để dùng offline.
- Các thay đổi lớn về chức năng bắt đầu ở **V2**, đóng gói thành bộ source mới và nâng số phiên bản rõ ràng.
- Trước mỗi lần cập nhật hoặc cài lại, tải bản sao lưu JSON từ ứng dụng.

## Nội dung gói

- `index.html` — ứng dụng Garden Manager V1.0.
- `manifest.webmanifest` — tên, biểu tượng và chế độ cài đặt PWA.
- `service-worker.js` — bộ nhớ đệm để mở ứng dụng offline sau lần tải đầu.
- `icon-192.png`, `icon-512.png` — biểu tượng Android/PWA.
- `.nojekyll` — bảo đảm GitHub Pages phục vụ nguyên các tệp tĩnh.
