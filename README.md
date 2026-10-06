# Phòng truyền thống 3D

Mô hình Phòng truyền thống Trường THCS Tân An Hội, dựng từ ảnh tư liệu. Tường chính có 11 bằng khen đã nắn thẳng từ ảnh chụp và tượng Bác dạng khối 3D.

Trang web: **https://thcstananhoi.github.io/**

Mở trang là mô hình tự tải. Chọn **Bảng chuyên môn**, rồi nhấp vào một trong 8 ảnh để xem ảnh gốc; chọn **Bằng khen**, rồi nhấp vào một trong 11 bằng khen để xem lớn. Dùng nút trước/sau hoặc phím mũi tên để chuyển ảnh, và **Esc** để đóng.

- Kéo chuột trái để xoay; cuộn để thu phóng; kéo chuột phải để di chuyển.
- Giữ **Shift** và lăn chuột: camera tự về giữa phòng rồi quay tại chỗ, lăn tiếp để nhìn quanh toàn bộ phòng.
- Trên điện thoại: kéo một ngón tay để xoay, dùng hai ngón tay để thu phóng và di chuyển.
- Có các góc Tổng thể, Trong phòng, Nhìn từ trên, Bảng chuyên môn và Bằng khen; có thể bật trần hoặc mở mặt cắt.

Kích thước và tỷ lệ phòng được ước lượng từ ảnh, chưa được đo thực tế.

## Chạy và cập nhật

Đây là trang tĩnh, không cần cài đặt thư viện hay biên dịch. GitHub Pages phục vụ nhánh `main`, thư mục gốc `/`. File `.nojekyll` giữ nguyên các tài nguyên tĩnh.

Các file cần giữ cùng nhau:

- `index.html`: giao diện.
- `app.js`: trình xem 3D, đã đóng gói Three.js, không phụ thuộc CDN.
- `assets/model.glb`: mô hình và các texture.
- `gallery.json` và `assets/gallery/01.jpg` đến `08.jpg`: danh sách và ảnh gốc.
- `awards.json` và `assets/awards/01.jpg` đến `11.jpg`: danh sách và ảnh bằng khen.

Để xem tại máy, phục vụ thư mục này bằng một HTTP server, ví dụ `python -m http.server 8000`, rồi mở `http://localhost:8000/`.

Three.js được sử dụng theo giấy phép MIT trong `licenses/THREE-LICENSE.txt`. Giấy phép đó chỉ áp dụng cho thư viện Three.js.
