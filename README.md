# Phòng truyền thống 3D

Mô hình Phòng truyền thống Trường THCS Tân An Hội, dựng từ ảnh tư liệu. Tường chính có 11 bằng khen đã nắn thẳng từ ảnh chụp và tượng Bác dạng khối 3D. Tường bên trái có bảng Ban giám hiệu qua các thời kỳ (4 ảnh chân dung, 7 ảnh hoạt động nổi bật) và bảng Ban chấp hành Công đoàn qua các thời kỳ (15 ảnh chân dung, 8 ảnh hoạt động nổi bật). Tường bên phải có poster Truyền thống nhà trường (từ bản thiết kế PDF) và bảng Thành tích tiêu biểu của Chi bộ với 5 giấy khen.

Trang web: **https://thcstananhoi.github.io/**

Mở trang là mô hình tự tải. Chọn **Bảng chuyên môn**, rồi nhấp vào một trong 8 ảnh để xem ảnh gốc; chọn **Bằng khen**, rồi nhấp vào một trong 11 bằng khen để xem lớn; chọn **Ban giám hiệu** hoặc **Công đoàn**, rồi nhấp vào một ảnh chân dung hoặc ảnh hoạt động nổi bật để xem ảnh gốc; chọn **Truyền thống**, rồi nhấp vào poster hoặc một giấy khen để xem lớn. Dùng nút trước/sau hoặc phím mũi tên để chuyển ảnh, và **Esc** để đóng. Trong cửa sổ xem lớn, bấm vào ảnh (hoặc nút **+**) để phóng to và đọc chi tiết, cuộn hoặc kéo để di chuyển, bấm lần nữa để xem lại cả ảnh.

- Kéo chuột trái để xoay (khi đứng trong phòng: quay nhìn quanh tại chỗ, cảnh đi theo con trỏ); cuộn để thu phóng; kéo chuột phải để di chuyển.
- Giữ **Shift** và lăn chuột: camera tự về giữa phòng rồi quay tại chỗ, lăn tiếp để nhìn quanh toàn bộ phòng.
- Trên điện thoại: kéo một ngón tay để xoay, dùng hai ngón tay để thu phóng và di chuyển.
- Có các góc Tổng thể, Trong phòng, Nhìn từ trên, Bảng chuyên môn, Bằng khen, Ban giám hiệu, Công đoàn và Truyền thống; có thể bật trần hoặc mở mặt cắt.
- Bảng điều khiển và hướng dẫn thao tác được thu gọn khi mở trang: nhấp nút **☰** (góc trên) hoặc nút hình con chuột (giữa cạnh dưới) để hiện, nút **×** để thu gọn lại.

Kích thước và tỷ lệ phòng được ước lượng từ ảnh, chưa được đo thực tế.

## Chạy và cập nhật

Đây là trang tĩnh, không cần cài đặt thư viện hay biên dịch. GitHub Pages phục vụ nhánh `main`, thư mục gốc `/`. File `.nojekyll` giữ nguyên các tài nguyên tĩnh.

Các file cần giữ cùng nhau:

- `index.html`: giao diện.
- `app.js`: trình xem 3D, đã đóng gói Three.js, không phụ thuộc CDN.
- `assets/model.glb`: mô hình và các texture.
- `gallery.json` và `assets/gallery/01.jpg` đến `08.jpg`: danh sách và ảnh gốc.
- `awards.json` và `assets/awards/01.jpg` đến `11.jpg`: danh sách và ảnh bằng khen.
- `management.json` và `assets/management/01.jpg` đến `04.jpg`: Ban giám hiệu, ảnh gốc.
- `union.json` và `assets/union/01.jpg` đến `15.jpg`: Ban chấp hành Công đoàn, ảnh gốc.
- `management_activities.json`, `union_activities.json` và `assets/management_activities/`, `assets/union_activities/`: ảnh gốc phần Các hoạt động nổi bật của hai bảng.
- `poster.json` và `assets/poster/poster.jpg`: poster Truyền thống nhà trường cỡ lớn.
- `party_awards.json` và `assets/party_awards/01.jpg` đến `05.jpg`: giấy khen của Chi bộ, bản quét gốc.

Để xem tại máy, phục vụ thư mục này bằng một HTTP server, ví dụ `python -m http.server 8000`, rồi mở `http://localhost:8000/`.

Three.js được sử dụng theo giấy phép MIT trong `licenses/THREE-LICENSE.txt`. Giấy phép đó chỉ áp dụng cho thư viện Three.js.
