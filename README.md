# 🚗 Smart Parking System (Hệ Thống Quản Lý Bãi Đỗ Xe Thông Minh)

> Dự án môn học **SWP391 (Software Development Project)** – Ứng dụng web quản lý bãi đỗ xe thông minh, hỗ trợ theo dõi vị trí trống theo thời gian thực, check-in/check-out bằng mã QR và thanh toán tự động qua cổng PayOS.

---

## 👥 Thành viên & Phân công công việc

| Thành viên | Vai trò | Nhiệm vụ chính |
| :--- | :--- | :--- |
| **Võ Hoàng Anh** | **Frontend Developer** | Thiết kế UI/UX, xây dựng giao diện Web App (ReactJS/Vite), xử lý định tuyến, tích hợp RESTful API, hiển thị sơ đồ bãi xe trực quan, luồng thanh toán QR và triển khai lên Cloudflare Pages. |
| **Nguyễn Bùi Tất Đạt** | **Backend Developer** | Thiết kế cơ sở dữ liệu (MySQL), xây dựng kiến trúc 3 lớp với Spring Boot (REST Controller, Service, Spring Data JPA), phân quyền người dùng, tích hợp cổng thanh toán PayOS và triển khai trên Microsoft Azure. |

---

## 🏗️ Kiến trúc hệ thống (System Architecture)

Hệ thống được xây dựng theo mô hình tách biệt Frontend – Backend (Client-Server) và kiến trúc phân lớp (Layered Architecture):
* **Frontend:** Single Page Application (SPA) xây dựng bằng ReactJS + Vite, triển khai trên Cloudflare Pages.
* **Backend:** Spring Boot Container chạy trên Microsoft Azure, gồm 3 lớp: *API Layer (REST Controller)* → *Business Logic (Service Layer)* → *Data Access (Repository Layer - Spring Data JPA)*.
* **Database & Payment:** Lưu trữ dữ liệu trên MySQL / Azure SQL và kết nối trực tiếp với cổng thanh toán PayOS.

---

## 🛠️ Công nghệ sử dụng

* **Frontend:** ReactJS, Vite, HTML5/CSS3
* **Backend:** Java, Spring Boot, Spring Data JPA, RESTful API
* **Database:** MySQL / Azure SQL
* **Payment Gateway:** PayOS
* **Cloud & Deployment:** Cloudflare Pages (Frontend), Microsoft Azure (Backend Container)

---

## ✨ Tính năng nổi bật

* **Phân quyền người dùng (RBAC):** Giao diện và chức năng tách biệt rõ ràng cho từng vai trò (Admin, Nhân viên bãi xe, Khách hàng).
* **Theo dõi bãi đỗ xe trực quan:** Cập nhật trạng thái từng ô đỗ (Trống / Đang sử dụng / Đã đặt trước) theo thời gian thực.
* **Check-in / Check-out bằng mã QR:** Tự động tạo và quét mã QR để ghi nhận thời gian xe ra vào, giảm thiểu thao tác thủ công.
* **Thanh toán tự động với PayOS:** Tự động tính cước phí gửi xe và tạo mã QR thanh toán trực tuyến.
* **Dashboard & Báo cáo thống kê:** Tổng hợp doanh thu và lưu lượng xe ra vào trực quan.

---

## 📸 Hình ảnh giao diện (Screenshots)

| Trang đăng nhập (Login) | Đặt chỗ / Sơ đồ bãi xe (Booking) | Dashboard thống kê |
| :---: | :---: | :---: |
| <img src="https://github.com/user-attachments/assets/179ea043-d22e-437d-a266-f04ea76ffdba" width="350" alt="Login" /> | <img src="https://github.com/user-attachments/assets/245a6ec2-350b-4ebb-8bf6-42c08c163121" width="350" alt="Booking" /> | <img src="https://github.com/user-attachments/assets/f65d100f-2297-43b8-85df-621523586f7a" width="350" alt="Dashboard" /> |

---

