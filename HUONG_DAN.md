# Tạ Thanh Phúc — Thư viện e-book & thực hành AI

Website tĩnh HTML/CSS/JavaScript, không cần cài ứng dụng hoặc máy chủ riêng.
Phong cách tham khảo timkhoemoingay.github.io: xanh dương #1486ce, xanh lá #3aaa18, nền trắng, thẻ bo góc.

## 1. Xem trên máy

Giải nén gói, mở `index.html` bằng Chrome hoặc Edge. Các tệp cần nằm cùng cấu trúc sau khi giải nén. Có thể thử tìm kiếm, lọc sách, sao chép câu lệnh và trang danh mục ngay trên máy. Trình duyệt có thể hạn chế clipboard hoặc lưu cục bộ khi mở bằng file; bản HTTPS thuận tiện hơn.

## 2. Xuất bản tại tathanhphuc.github.io

Địa chỉ này phụ thuộc tài khoản hoặc tổ chức GitHub tên `tathanhphuc`; chưa xác minh tên này còn trống hoặc thuộc sở hữu của anh. Không đổi tên tài khoản `timkhoemoingay` đang dùng vì việc đó có thể ảnh hưởng trang sức khỏe. Nếu tên mong muốn không khả dụng, chọn tên khác và thay tên kho/địa chỉ tương ứng.

1. Đăng nhập tài khoản GitHub `tathanhphuc` mà anh sở hữu. Nếu chưa có, tạo tài khoản với tên này khi GitHub cho phép.
2. Chọn **New repository**; tên kho **tathanhphuc.github.io**, chọn **Public** rồi **Create repository**.
3. Chọn **uploading an existing file** (kho trống) hoặc **Add file → Upload files**. Tải nội dung thư mục giải nén vào gốc kho. Không tải nguyên tệp ZIP và không đặt `index.html` trong thư mục con `ta-thanh-phuc`.
4. Chọn **Commit changes**.
5. Vào **Settings → Pages → Build and deployment**. Chọn **Deploy from a branch**, nhánh **main**, thư mục **/(root)**, bấm **Save**.
6. Chờ GitHub triển khai. Mở **https://tathanhphuc.github.io/** khi GitHub báo trang đã xuất bản. GitHub cho biết cập nhật có thể mất tối đa khoảng 10 phút.
7. Nếu chưa thấy cập nhật, xem trạng thái **Actions**, kiểm tra Pages, rồi tải lại trang bằng Ctrl+F5.

Tài liệu chính thức: https://docs.github.com/en/pages/quickstart

## 3. Thêm một cuốn sách

1. Đặt tên tệp ngắn, không dấu, ví dụ `ai-cho-nguoi-moi.pdf`.
2. Trên GitHub mở thư mục `ebooks`, chọn **Add file → Upload files**, tải sách và ảnh bìa lên, rồi **Commit changes**. Nếu thư mục chưa xuất hiện, tạo `ebooks/README.md` trước.
3. Mở `quan-tri.html` trên trang hoặc trong bộ giải nén.
4. Nhập tên, chủ đề, giới thiệu, định dạng và ngày cập nhật.
5. Nhập đường dẫn sách `ebooks/ai-cho-nguoi-moi.pdf`. Đường dẫn bìa, ví dụ `ebooks/bia-ai.jpg`, có thể để trống. Có thể dùng URL HTTPS công khai cho tệp bên ngoài.
6. Bấm **Lưu vào danh mục đang soạn**, rồi **Tải books.js**.
7. Ở gốc kho, dùng **Add file → Upload files** để thay `books.js` bằng tệp mới tải. Bấm **Commit changes**.
8. Đợi triển khai xong; thử mở và tải sách trên máy tính, điện thoại. Kiểm tra cả quyền truy cập tệp nếu dùng link bên ngoài.

Lưu ý: Trang danh mục là công cụ tạo tệp cục bộ. Nó không tự tải sách, không tự đăng lên GitHub và không phải trang đăng nhập quản trị. Chỉ người có quyền ghi kho GitHub mới cập nhật trang công khai. Khi nhiều người cùng biên soạn, dùng danh mục mới nhất trước mỗi lần chỉnh để tránh ghi đè thay đổi.

## 4. Nội dung hiện có

- 4 đầu sách là danh mục dự kiến, đều ghi “Sắp phát hành”; chưa kèm tệp sách hoặc khẳng định sách đã được biên soạn.
- 3 bài thực hành có thể dùng ngay: soạn thông báo, kiểm tra bảng dữ liệu, biến kiến thức thành bài tập.
- Tìm kiếm không dấu/có dấu và lọc chủ đề.
- Nút đọc và tải chỉ xuất hiện khi đã nhập đường dẫn tệp. Liên kết bên ngoài mở nguồn, vì tải trực tiếp phụ thuộc máy chủ bên ngoài.
- Giao diện thích ứng điện thoại; menu di động; nhãn hỗ trợ truy cập bàn phím.

## 5. Kiểm tra trước khi chia sẻ

- Đường dẫn công khai vào được khi chưa đăng nhập.
- Các nút đọc/tải mở đúng sách, sách không yêu cầu quyền riêng tư.
- Không đăng dữ liệu cá nhân hoặc hồ sơ nghiệp vụ trong tài liệu.
- Sách thuộc quyền của anh hoặc được cho phép phát hành.
- Thông tin sách, ngày cập nhật và phiên bản đúng tệp đã tải.

## Cấu trúc

`index.html`: trang thư viện; `style.css`: giao diện; `books.js`: danh mục; `app.js`: tìm kiếm/lọc/nút copy; `quan-tri.html` + `admin.js`: công cụ thêm sách; `favicon.svg`: biểu tượng; `.nojekyll`: phục vụ website tĩnh; `ebooks/`: sách và bìa.

## Giới hạn kiểm tra bàn giao

Đã kiểm tra cú pháp JavaScript, dữ liệu danh mục, tìm kiếm, bộ lọc và xuất danh mục bằng kiểm tra kỹ thuật. Chưa kiểm tra giao diện bằng trình duyệt và chưa triển khai trên GitHub Pages tại địa chỉ mong muốn. Cần kiểm tra đường dẫn tệp thật sau khi bổ sung sách và kiểm tra vận hành sau xuất bản.
