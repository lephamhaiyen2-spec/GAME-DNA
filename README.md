# 🧬 GAME-DNA — Phòng mô phỏng “Giải mã hệ thống”

Đã triển khai bản đầu tiên gồm:

- Màn hình mở đầu với DNA 3D xoay.
- Nhập tên đội.
- Đồng hồ 5 phút.
- Nhiệm vụ 1: ghép mạch bổ sung từ DNA `3' ATGCCTAGGCTTACAATTGGCTAT 5'`.
- Kiểm tra theo nguyên tắc A–T, G–C.
- Bắt buộc hoàn thành nhiệm vụ 1 mới mở khóa nhiệm vụ 2.
- Nhiệm vụ 2: phiên mã thành mRNA bằng A, U, G, C.
- Tính điểm theo nhiệm vụ, tốc độ và số lần sai.
- Ghi lịch sử lượt chơi.
- Teacher Dashboard tại `teacher.html`.
- QR tự sinh trên Teacher Dashboard để mở trang chơi.

## Kết quả chuẩn

Mạch bổ sung: `5' TACGGATCCGAATGTTAACCGATA 3'`

mRNA: `5' UACGGAUCCGAAUGUUAACCGAUA 3'`

## Quan trọng về dữ liệu

Bản hiện tại dùng localStorage để có thể chạy ngay trên GitHub Pages mà không cần đưa khóa API/database vào mã nguồn. Vì vậy dữ liệu được lưu trên từng trình duyệt/thiết bị, chưa phải cơ sở dữ liệu dùng chung giữa nhiều iPad.

Để dùng đúng mô hình lớp học nhiều thiết bị — tất cả đội quét QR, dữ liệu tập trung về một Teacher Dashboard và cập nhật theo thời gian thực — cần kết nối một backend như Firebase hoặc Supabase. Sau khi có cấu hình backend, có thể thay lớp lưu trữ localStorage bằng database dùng chung mà không thay đổi giao diện trò chơi.

## GitHub Pages

Trong GitHub: Settings → Pages → Deploy from branch → chọn `main` → `/ (root)`.

Sau khi Pages được bật, trang chơi sẽ có dạng:

`https://<username>.github.io/GAME-DNA/`

Dashboard:

`https://<username>.github.io/GAME-DNA/teacher.html`
