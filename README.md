### 1. MÔ TẢ ĐỀ TÀI
- Tên đề tài: Phân tích và khắc phục lỗi Broken Authentication
- Hệ thống demo: Assignment Manager hệ thống quản lý bài tập sinh viên

Mục tiêu:
- Hiểu các lỗi xác thực phổ biến
- Phân tích nguyên nhân và hậu quả
- Đề xuất và triển khai giải pháp khắc phục

Các lỗi được demo:
- Không giới hạn số lần đăng nhập sai
- Logout không hủy session
- Không có session timeout

### 2. CÔNG CỤ SỬ DỤNG
Công cụ	Mục đích
- HTML/CSS/JavaScript: Xây dựng giao diện và xử lý logic
LocalStorage: Lưu trữ session trên trình duyệt
Fetch API: Đọc dữ liệu người dùng từ file JSON
Live Server: Chạy web server để demo

### 3. CÁCH CHẠY DEMO
Bước 1: Đảm bảo có 3 file trong cùng thư mục:
- BrokenAuthentication.html (bản lỗi)
- SecureAuthentication.html (bản vá)
- users.json (dữ liệu tài khoản)
Bước 2: Chạy web server (không thể mở trực tiếp file HTML do CORS):
- Dùng Live Server (VS Code):*
- Chuột phải vào file HTML → Open with Live Server

### 4. TÀI KHOẢN GIẢ LẬP

Dữ liệu được lấy từ file `users.json` với cấu trúc:

| Username | Password | Vai trò |
|----------|----------|---------|
| student | 123123 | Học sinh |
| teacher | 123456 | Giáo viên |
| admin | admin123@ | Quản trị viên |

> **Lưu ý:** Hệ thống bắt buộc phải có file `users.json`, không có dữ liệu mặc định.
