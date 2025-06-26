# 🧑‍💻 Thông tin sinh viên
- Họ tên: Nguyễn Phương Nam
- Mã SV: 23010028
- Lớp: K17_CNTT1
- link repo: https://github.com/NguyenNam2809/websitebanhang

# 📋 Mô tả dự án
Dự án "Jelly Boutique" là một ứng dụng web thương mại điện tử chuyên về kinh doanh thời trang , cho phép khách hàng mua sắm thời trang trực tuyến và quản trị viên quản lý sản phẩm, đơn hàng. Ứng dụng này cung cấp các tính năng như đăng ký, đăng nhập, quản lý sản phẩm, giỏ hàng, đặt hàng, thanh toán và xem lịch sử mua hàng.

## 📌 Mục tiêu dự án

- Tạo ra một nền tảng bán hàng trực tuyến thân thiện, tiện dụng.
- Hỗ trợ hoạt động quảng bá thương hiệu và tương tác khách hàng hiệu quả.
- Tích hợp các tính năng cần thiết như: tìm kiếm, đánh giá, giỏ hàng, thanh toán điện tử,...
- Phù hợp cho các cửa hàng vừa và nhỏ, hướng tới khả năng mở rộng trong tương lai.
---

## 🌟 Tính năng nổi bật

### Người dùng (khách hàng):
- Đăng ký / đăng nhập (hỗ trợ tài khoản Google, Facebook)
- Tìm kiếm, lọc, sắp xếp sản phẩm theo thương hiệu, giá, tên,...
- Xem thông tin chi tiết sản phẩm và bài viết liên quan
- Thêm sản phẩm vào giỏ hàng, sử dụng mã giảm giá
- Mua hàng và thanh toán (COD hoặc PayPal)
- Đánh giá sản phẩm, bình luận bài viết
- Xem lịch sử đơn hàng

### Quản trị viên:
- Quản lý danh mục sản phẩm, thương hiệu, sản phẩm
- Quản lý đơn hàng và trạng thái giao hàng
- Quản lý tài khoản người dùng, phân quyền
- Quản lý banner, bài viết, thẻ bài viết, bình luận
- Quản lý mã giảm giá, phí vận chuyển
- Thống kê doanh thu theo thời gian

---

## 🛠️ Công nghệ sử dụng

- **Back-end:** Laravel Framework (PHP 8.x), MySQL
- **Front-end:** Blade, HTML5, CSS3, JavaScript, jQuery
- **API tích hợp:**
  - Đăng nhập Google, Facebook
  - Thanh toán PayPal
  - Chat Facebook Messenger
- **Môi trường phát triển:** XAMPP (Apache, MySQL, PHP)
- **Mô hình kiến trúc:** MVC

---

## ⚙️ Cài đặt & triển khai

### 📦 Yêu cầu hệ thống

- PHP: >= 8.2
- Composer: >= 2.0
- Node.js: >= 18.0
- NPM: >= 9.0
- MySQL: >= 8.0 (hoặc PostgreSQL >= 13.0)
- Web Server: Apache/Nginx

### 🔧 Cài đặt

```bash
git clone https://github.com/your-username/jelly-boutique.git
cd jelly-boutique
cp .env.example .env
composer install
php artisan key:generate
php artisan migrate
npm install && npm run dev
php artisan serve

### Cấu hình DB trong file .env
DB_CONNECTION=mysql
 DB_HOST=127.0.0.1
 DB_PORT=3306
 DB_DATABASE=jelly_boutique
 DB_USERNAME=your_user
 DB_PASSWORD=your_pass
```

# 📁 Cấu trúc thư mục dự án Laravel
```bash
jelly-boutique/
├── app/                      # Chứa mã nguồn chính của ứng dụng
│   ├── Console/             # Các lệnh Artisan tùy chỉnh
│   ├── Exceptions/          # Xử lý ngoại lệ
│   ├── Http/                # Controller, Middleware, Request
│   │   ├── Controllers/     # Controller người dùng và admin
│   │   ├── Middleware/      # Middleware bảo vệ route
│   │   └── Requests/        # Validate dữ liệu đầu vào
│   ├── Models/              # Các model Eloquent (User, Product, Order, ...)
│   └── Providers/           # Service providers
│
├── bootstrap/               # Khởi tạo framework Laravel
│
├── config/                  # Các file cấu hình (database, mail, app, ...)
│
├── database/                # Cấu trúc và dữ liệu CSDL
│   ├── migrations/          # File tạo bảng
│   ├── seeders/             # Dữ liệu mẫu
│   └── factories/           # Tạo dữ liệu test
│
├── public/                  # Thư mục public (ảnh, js, css)
│   ├── assets/              # Tệp JS/CSS/IMG tĩnh
│   └── index.php            # Entry point chính của ứng dụng
│
├── resources/              
│   ├── views/               # Giao diện Blade (frontend & admin)
│   │   ├── layouts/         # Giao diện chung
│   │   ├── user/            # Giao diện người dùng
│   │   └── admin/           # Giao diện admin
│   ├── lang/                # Ngôn ngữ (đa ngôn ngữ nếu có)
│   └── sass/                # SCSS nếu dùng Laravel Mix
│
├── routes/                 
│   ├── web.php              # Route chính của website
│   └── api.php              # Route cho API nếu có
│
├── storage/                 # Lưu file tạm, log, cache, upload,...
│
├── tests/                   # Test tự động (Feature, Unit)
│
├── .env                     # Biến môi trường (DB, SMTP,...)
├── artisan                  # CLI tool của Laravel
├── composer.json            # Quản lý package PHP
└── package.json             # Quản lý JS/CSS (nếu dùng npm/yarn)
```
# 🧭 Sơ đồ và Biểu đồ Hệ Thống
### 📌 Biểu đồ trình tự chức năng đăng kí
![Image](https://github.com/user-attachments/assets/39baf549-d5a1-4f41-93b5-581603381a27)
### 📌 Biểu đồ trình tự chức năng đăng nhập
![Image](https://github.com/user-attachments/assets/ce19e1ca-57b4-47b2-b34d-4da6fce98a98)
### 📌 Biểu đồ trình tự chức năng Tìm kiếm sản phẩm
![Image](https://github.com/user-attachments/assets/497de78c-9f24-44e0-a95b-1bfbd066fb3a)
### 📌 Biểu đồ trình tự chức năng giỏ hàng
![Image](https://github.com/user-attachments/assets/6e3f9b32-4499-482f-aeef-b34238c73d19)
### 📌 Biểu đồ lớp phân tích chức năng quản lí bài viết
![Image](https://github.com/user-attachments/assets/7713bd58-59fc-4804-92f5-149dbd2c1fb9)
### 📌 Biểu đồ lớp phân tích chức năng quản lí sản phẩm
![Image](https://github.com/user-attachments/assets/b7715192-b9e7-4124-be8d-a08952731328)
### 📌 Biểu đồ lớp phân tích chức năng quản lí đơn hàng
![Image](https://github.com/user-attachments/assets/c27d0530-aecf-4266-ac9e-3ac5dd019e75)
