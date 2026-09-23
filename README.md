# Trái Tim 3D

Trang web tĩnh 3D, sẵn sàng triển khai bằng GitHub Pages.

## GitHub Pages

Xuất bản từ nhánh `main`, thư mục gốc `/`.

- Liên kết công khai mặc định ở chế độ chỉ xem.
- Chế độ quản trị giao diện dùng tham số `?mode=edit`.
- Mã QR tạo trong trang lưu màu, tốc độ, lời nhắn và nhạc Synth/link MP3 online hiện tại.
- MP3 tải trực tiếp từ máy chỉ có trong trình duyệt quản trị và không thể đóng gói vào QR.
- Nút Lưu Cấu Hình lưu cài đặt trên thiết bị quản trị và cập nhật link/QR mới.
- Có thể chọn thời điểm bắt đầu/kết thúc để phát lặp một đoạn của tệp hoặc link nhạc.
- Chế độ Người Xem chỉ giữ nút âm thanh và gợi ý thao tác; các nút chỉnh sửa và hiệu ứng được ẩn.
- Admin có thể dùng GitHub fine-grained token với quyền `Contents: Read and write` cho riêng repository này. Nút **Lưu & Cập Nhật Public** sẽ tải MP3 lên `assets/audio/current.mp3` và ghi toàn bộ trạng thái vào `config.json`.
- Token chỉ được giữ trong `sessionStorage` của tab Admin, không ghi vào repository, URL hay mã QR.
- Trang public không có tham số cấu hình sẽ tự đọc `config.json`; GitHub Pages thường cần khoảng 1–2 phút để phát hành thay đổi.
