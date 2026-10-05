# Garden Manager V1.1.9 — Structured Pot Manager

Nâng cấp trực tiếp từ V1.1.8.

## V1.1.9
- Sơ đồ có 2 chế độ: **Sơ đồ trực quan ⇄ Quản lý chậu**.
- Quản lý 3 cấp: **Khu (LV1) → Mã chính (LV2) → Chậu con (LV3)**.
- ID hệ thống tách khỏi nhãn hiển thị; đổi nhãn nhóm không phá liên kết dữ liệu.
- Tự sinh số chậu con `.01`, `.02`, `.03`; có preview trước khi sắp xếp lại số.
- Bộ lọc Khu / Mã chậu / Loại cây / tìm kiếm; chip Có cây / Trống.
- Card LV2 thống kê số chậu, cơ cấu cây và tổng thể tích đất ước tính.
- Chạm chậu trên sơ đồ hoặc danh sách mở bottom sheet thao tác nhanh: Cây trồng / Chậu / Vị trí / Nhật ký / Sự vụ.
- Giữ dữ liệu V1.1.8 trong localStorage và tự bổ sung cấu trúc group khi mở bản mới.

## Deploy GitHub Pages
Upload/replace: `index.html`, `manifest.webmanifest`, `service-worker.js`, `icon-192.png`, `icon-512.png`, `garden-reference.png`, `.nojekyll`.


## V1.1.9 R2
- Sơ đồ mặc định mở Quản lý chậu LV1/LV2/LV3.
- Chạm chậu ở Sơ đồ trực quan mở bottom sheet, không còn thẻ CHẬU ĐANG CHỌN ở cạnh/bên dưới sơ đồ.
- Có nút chuyển Sơ đồ trực quan / Quản lý chậu.
