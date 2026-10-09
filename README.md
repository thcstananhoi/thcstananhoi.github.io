# Phòng truyền thống 3D

Mô hình Phòng truyền thống Trường THCS Tân An Hội, dựng từ ảnh tư liệu. Tường chính có 11 bằng khen đã nắn thẳng từ ảnh chụp. Tượng Bác dùng mô hình President Ho Chi Minh Statue của Mr. Mushi, đã nhập từ bộ tải chính thức do người dùng cung cấp. Tường bên trái có bảng Ban giám hiệu qua các thời kỳ (11 ảnh chân dung kèm nhiệm kỳ, 8 ảnh hoạt động nổi bật) và bảng Ban chấp hành Công đoàn qua các thời kỳ (17 ảnh chân dung xếp 5–6–6, 9 ảnh hoạt động nổi bật). Tường sau có 18 ảnh hoạt động giáo viên, xếp theo thứ tự 1–18 bên dưới bốn lá cờ và dòng Một số hoạt động nổi bật. Tường bên phải có poster Truyền thống nhà trường (từ bản thiết kế PDF) và bảng Thành tích tiêu biểu của Chi bộ với 9 giấy khen xếp 5 hàng (1–2–2–2–2), theo mã hàng–cột của tên file trong thư mục `7-Giấy khen (2)`; ảnh 11.jpg ở giữa hàng đầu.

Trang web: **https://thcstananhoi.github.io/**

Mở trang là mô hình tự tải. Chọn **Bảng chuyên môn**, rồi nhấp vào một trong 8 ảnh để xem ảnh gốc; chọn **Bằng khen**, rồi nhấp vào một trong 11 bằng khen để xem lớn; chọn **Ban giám hiệu** hoặc **Công đoàn**, rồi nhấp vào một ảnh chân dung hoặc ảnh hoạt động nổi bật để xem ảnh gốc; chọn **Truyền thống**, rồi nhấp vào poster hoặc một giấy khen để xem lớn. Dùng nút trước/sau hoặc phím mũi tên để chuyển ảnh, và **Esc** để đóng. Trong cửa sổ xem lớn, bấm vào ảnh (hoặc nút **+**) để phóng to và đọc chi tiết, cuộn hoặc kéo để di chuyển, bấm lần nữa để xem lại cả ảnh.

- Kéo chuột trái để xoay (khi đứng trong phòng: quay nhìn quanh tại chỗ, cảnh đi theo con trỏ); cuộn để thu phóng; kéo chuột phải để di chuyển.
- Giữ **Shift** và lăn chuột: camera tự về giữa phòng rồi quay tại chỗ, lăn tiếp để nhìn quanh toàn bộ phòng.
- Trên điện thoại: kéo một ngón tay để xoay, dùng hai ngón tay để thu phóng và di chuyển.
- Có các góc Tổng thể, Trong phòng, Nhìn từ trên, Bảng chuyên môn, Bằng khen, Ban giám hiệu, Công đoàn, Tường sau, Truyền thống; có thể bật trần hoặc mở mặt cắt. Chọn Tường sau rồi bấm ảnh để xem bản gốc và chuyển qua đủ 18 ảnh.
- Bảng điều khiển và hướng dẫn thao tác được thu gọn khi mở trang: nhấp nút **☰** (góc trên) hoặc nút hình con chuột (giữa cạnh dưới) để hiện, nút **×** để thu gọn lại.

Kích thước và tỷ lệ phòng được ước lượng từ ảnh, chưa được đo thực tế.

Điện thoại, iPad và Safari tự tải mô hình nhẹ `model-mobile.glb`. Hình học và UV của tượng giữ nguyên; ảnh vật liệu trong mô hình được giảm kích thước để giảm bộ nhớ texture ước tính từ khoảng 1.372 MiB xuống 150 MiB. Chế độ này cũng giảm độ phân giải render và tắt khử răng cưa MSAA. Ảnh tư liệu khi mở xem lớn vẫn dùng bản gốc. Máy tính với trình duyệt khác tiếp tục tải mô hình đầy đủ. Số liệu và kiểm tra bảo toàn hình học nằm trong `mobile_optimization.json`.

## Chạy và cập nhật

Đây là trang tĩnh, không cần cài đặt thư viện hay biên dịch. GitHub Pages phục vụ nhánh `main`, thư mục gốc `/`. File `.nojekyll` giữ nguyên các tài nguyên tĩnh.

Các file cần giữ cùng nhau:

- `index.html`: giao diện.
- `app.js`: trình xem 3D, đã đóng gói Three.js, không phụ thuộc CDN.
- `assets/model.glb`: mô hình và các texture.
- `assets/model-mobile.glb`: cùng hình học, texture tối ưu cho thiết bị di động và Safari.
- `gallery.json` và `assets/gallery/01.jpg` đến `08.jpg`: danh sách và ảnh gốc.
- `awards.json` và `assets/awards/01.jpg` đến `11.jpg`: danh sách và ảnh bằng khen.
- `management.json` và `assets/management/01.jpg` đến `11.jpg`: Ban giám hiệu, ảnh gốc, tên và nhiệm kỳ từ dữ liệu cung cấp.
- `union.json` và `assets/union/01.png`, `03.png` và `02.jpg` và các JPG từ `04.jpg` đến `17.jpg`: Ban chấp hành Công đoàn; cô Mai Thị Hoa ở hàng 1, cột 1, Chủ tịch Công đoàn, nhiệm kỳ 2000–2003; thầy Lê Chí Thành ở hàng 1, cột 3, Chủ tịch Công đoàn, nhiệm kỳ 2010–2017.
- `management_activities.json`, `union_activities.json` và `assets/management_activities/`, `assets/union_activities/`: ảnh gốc phần Các hoạt động nổi bật của hai bảng.
- `teacher_activities.json` và `assets/teacher_activities/`: 18 ảnh gốc JPG/PNG của tường sau.
- `archive_qr.json` và `assets/archive_qr/01.png`: mã QR cho bảng Kho tư liệu số Thị Trấn 2 bên trái tượng Bác; xoay tới bảng rồi bấm mã để xem lớn hoặc quét.
- `poster.json` và `assets/poster/poster.jpg`: poster Truyền thống nhà trường cỡ lớn.
- `party_awards.json`, `assets/party_awards/01.jpg` đến `05.jpg` và `06.png` đến `09.png`: 9 giấy khen của Chi bộ, bản quét gốc.

Để xem tại máy, phục vụ thư mục này bằng một HTTP server, ví dụ `python -m http.server 8000`, rồi mở `http://localhost:8000/`.

Mô hình tượng [President Ho Chi Minh Statue](https://sketchfab.com/3d-models/president-ho-chi-minh-statue-12577a979a2c4828ab065fc87a1e2e48) của [Mr. Mushi](https://sketchfab.com/mr.mushi) được sử dụng theo [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). Phần tượng được tách khỏi bệ và bảng thuyết minh của nơi trưng bày gốc; giữ nguyên khuôn mặt, đầu, cổ và ảnh vật liệu nguồn. Vai tại mép tách được khép lại, dùng bề mặt và tọa độ UV lấy từ vai đối diện của mô hình gốc. Phần đầu, mặt và cổ giữ nguyên; đáy được khép bằng vật liệu đồng. Tượng được căn hướng, thay đổi tỷ lệ đồng nhất và đặt lên bệ của phòng. Khi chia sẻ tài nguyên tượng, cần ghi công, kèm liên kết giấy phép, nêu thay đổi; sử dụng phi thương mại và chia sẻ phần chỉnh sửa của tượng theo cùng giấy phép. Phạm vi giấy phép này là mô hình tượng cùng vật liệu từ tác giả. Quyền sử dụng ảnh tư liệu của trường và tài nguyên khác được xác định theo từng nguồn.

Three.js được sử dụng theo giấy phép MIT trong `licenses/THREE-LICENSE.txt`. Giấy phép đó chỉ áp dụng cho thư viện Three.js.
