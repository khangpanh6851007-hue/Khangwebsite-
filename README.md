# 🔥 Hệ Thống Đặt Hàng Heo Quay Tự Động - Tùng Quay Heo 

Website giới thiệu thực đơn, dịch vụ gia công và hệ thống lên đơn hàng tự động, tối ưu điều hướng chuyển thẳng dữ liệu đơn về **Zalo** hoặc **Facebook Messenger** của chủ lò mà không cần sử dụng hệ thống máy chủ (Serverless).

---

## ⚡ Tính Năng Nổi Bật

*   **Giao diện chuẩn di động (Responsive):** Phát triển trên nền tảng Tailwind CSS, hiển thị mượt mà trên mọi kích thước màn hình từ điện thoại Android, iOS cho đến máy tính.
*   **Giỏ hàng động (Dynamic Cart):** Khách hàng có thể thêm món, tăng giảm số lượng, tính tổng tiền trực tiếp tức thì bằng JavaScript thuần.
*   **Bộ lọc danh mục thông minh:** Phân loại nhanh thực đơn (Heo nguyên con, heo miếng bán ký, dịch vụ gia công) giúp khách dễ dàng lựa chọn.
*   **Xử lý đơn hàng không cần Server:** Tự động gom thông tin khách hàng, thời gian giao nhận, quy cách chặt thịt và xuất thành chuỗi văn bản được mã hóa an toàn.
*   **Chuyển tiếp đa kênh tự động:** Cho phép khách hàng gửi duyệt đơn qua Zalo hoặc Messenger chỉ bằng một cú chạm (Auto-fill message).

---

## 🛠️ Hướng Dẫn Cấu Hình (Dành Cho Chủ Lò)

Để hệ thống gửi đơn về đúng tài khoản cá nhân của bạn, hãy mở file `index.html` và tìm đến dòng **từ 19 đến 22** để thay đổi thông tin cấu hình:

```javascript
// CẤU HÌNH THÔNG TIN LIÊN HỆ CỦA CHỦ LÒ
const CONFIG_ZALO_PHONE = "0900000000";    // Thay bằng Số điện thoại đăng ký Zalo nhận đơn (viết liền)
const CONFIG_FACEBOOK_PAGE = "HeoQuayTùng"; // Thay bằng Username (Tên định danh) của Trang/Messenger cá nhân
