# Access_Control_Vulnerabilities
# Authorization
#### Lỗ hổng bảo mật người hack không cần phải biết code
#### Kiểm soát quyền truy cập
#### Để vào được Authorization thì phải vượt qua được Authentication(cookie, access token,.....)
#### Làm được những việc mà đáng nhẽ admin mới được phép làm (lên)
#### Làm được những việc mà tài khoản khác mới làm được cùng quyền hạn (ngang)
# Có rất nhiều viễn cảnh và loại lỗi Broken Access_Control
# IDOR (Insecure Direct Object Reference)
#### Chỉ đơn giản là bug nhận Untrusted Data rơi vào một mã định danh(Identifer) sau đó truy cập sql mà không kiểm tra quyền hạn gì cả
#### 99% Untrusted data chính là cái mã định danh
#### cho phép hacker truy cập trực tiếp tới các đối tượng thông qua untrusted data (vd ?postid=1,... thay 1 bằng 2 hacker xem được bài đăng 2)
