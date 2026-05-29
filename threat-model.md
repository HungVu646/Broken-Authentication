# Threat Model - Cyber Fortress
## 1. Asset - Tài sản cần bảo vệ
- Tài khoản người dùng
- Session đăng nhập
- Dữ liệu bài tập của sinh viên
- Thông tin cá nhân cơ bản của người dùng
## 2. Threat - Mối đe dọa
- Kẻ tấn công đoán mật khẩu bằng brute-force
- Người dùng cố truy cập trái phép vào tài khoản khác
- Bot/script tự động thử nhiều mật khẩu
- Người khác sử dụng lại session sau khi logout
## 3. Vulnerability - Lỗ hổng
Phiên bản đầu của hệ thống tồn tại các lỗ hổng:
- Không giới hạn số lần đăng nhập sai
- Không khóa tài khoản khi nhập sai nhiều lần
- Logout không hủy session
## 4. Impact - Tác động
- Kẻ tấn công có thể đoán đúng mật khẩu
- Người dùng bị mất tài khoản
- Người khác vẫn có thể dùng session cũ sau khi logout
## 5. Mitigation - Biện pháp giảm thiểu
Biện pháp kỹ thuật
- Giới hạn số lần đăng nhập sai
- Khóa tài khoản 20 giây sau 5 lần sai
- Thêm xác thực MFA bằng OTP demo
- Hủy session hoàn toàn khi logout
  
Biện pháp quy trình
- Ghi log đăng nhập thất bại
- Kiểm thử bảo mật định kỳ
 
Biện pháp nâng cao nhận thức
- Không chia sẻ tài khoản
- Không sử dụng cùng một mật khẩu cho nhiều hệ thống
