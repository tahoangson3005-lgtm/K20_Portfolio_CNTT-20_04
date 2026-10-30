không hiện ảnh
không đúng đường dẫn
# AI Log - Báo cáo lỗi

Ngày kiểm tra: 30/10/2026

## Các lỗi phát hiện

1. **Không hiển thị hình ảnh (đã xác nhận ở mã nguồn, mức độ: trung bình)**
   - `index.html` không có thẻ `<img>`; `css/style.css` không khai báo `background-image`.
   - Dự án hiện không có tệp hình ảnh và thư mục `assets/` được liệt kê trong `README.md` cũng không tồn tại.
   - Kết quả: trang hiện không thể hiển thị ảnh hồ sơ hoặc ảnh dự án. Cần bổ sung ảnh và tham chiếu đúng đường dẫn tương đối nếu đây là nội dung mong muốn.

2. **Đường dẫn repository không thống nhất (đã xác nhận, mức độ: trung bình)**
   - `README.md:12-13` trỏ tới `phananhtai/portfolio-v7` và `phananhtai.github.io/portfolio-v7/`.
   - `index.html:49` lại trỏ tới `tahoangson/portfolio-v7`.
   - Kết quả: người xem có thể truy cập nhầm repository. Chưa xác minh URL nào là URL chính xác; cần chọn URL chính thức và đồng bộ các tài liệu/liên kết.

3. **Thông tin định danh không đồng nhất (đã xác nhận, mức độ: cao)**
   - Nội dung trang và README ghi Tạ Hoàng Sơn, MSSV `2071020164` (`index.html:23-24`, `README.md:1,4-5`).
   - Bình luận đầu `css/style.css` ghi Phan Anh Tài, MSSV `2071020166`; email tại `index.html:48` cũng chứa mã `2071020166`.
   - Kết quả: thông tin tác giả/MSSV trong sản phẩm có thể sai hoặc thuộc hai người khác nhau. Cần xác nhận thông tin đúng trước khi sửa.

## Phạm vi kiểm tra

- Đã kiểm tra tĩnh các tệp HTML, CSS và tài liệu trong thư mục dự án.
- Liên kết CSS `css/style.css` trong `index.html` trỏ tới tệp hiện có.
- Chưa kiểm tra HTTP/GitHub Pages hoặc xác nhận URL chính thức; các trạng thái triển khai trong README chưa được kiểm chứng độc lập.
