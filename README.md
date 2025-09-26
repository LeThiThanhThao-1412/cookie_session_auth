Yêu cầu hệ thống
Node.js (phiên bản 18 trở lên)

MongoDB (chạy cục bộ trên cổng 27017)

Postman (để kiểm thử API)
Cài đặt
Clone repository

Cài đặt các dependencies: npm install
Đảm bảo MongoDB đang chạy trên mongodb://127.0.0.1:27017

Khởi động server: node app.js
Server sẽ chạy trên http://localhost:3000
1. Đăng ký tài khoản
POST http://localhost:3000/auth/register

Body (JSON):
{
  "username": "admin",
  "password": "12345"
}
![alt text](public/img/1.png)
![alt text](public/img/2.png)
2. Đăng nhập
POST http://localhost:3000/auth/login
![alt text](public/img/3.png)
![alt text](public/img/4.png)
3. Trang hồ sơ (bảo mật)
GET http://localhost:3000/auth/profile
![alt text](public/img/5.png)
4. Đăng xuất
GET http://localhost:3000/auth/logout
![alt text](public/img/6.png)
![alt text](public/img/7.png)