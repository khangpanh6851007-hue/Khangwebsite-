# 🐖 TÙNG QUAY HEO - Hệ Thống Thực Đơn Đám Mây v11.0

Ứng dụng web đặt hàng heo quay da giòn và dịch vụ gia công lễ vật trực tuyến, hoạt động trên kiến trúc **Single Page Application (SPA)** hợp nhất trong **1 file HTML duy nhất**. Hệ thống tích hợp cơ sở dữ liệu đám mây Realtime Database để đồng bộ thực đơn, lưu trữ hình ảnh tải lên trực tiếp và chuyển tiếp đơn hàng tự động qua Zalo/Messenger.

---

## 🚀 Tính Năng Nổi Bật (Phiên Bản v11.0)

*   **Đồng Bộ Realtime Cloud:** Kết nối trực tiếp với Firebase giúp cập nhật món ăn, số lượt thích, đánh giá sao và bình luận ngay lập tức mà không cần tải lại trang.
*   **Lưu Trữ Ảnh Trực Tiếp (Upload to Cloud):** Tích hợp công nghệ nén ảnh tự động (xuống độ phân giải 480px, chất lượng 65% JPEG) giúp tối ưu dung lượng và lưu trữ chuỗi Base64 thẳng vào Realtime Database. Không cần hosting lưu ảnh riêng biệt.
*   **Bộ Lọc Danh Mục Thông Minh:** Phân loại thực đơn trực quan (Heo nguyên con, Heo miếng bán ký, Dịch vụ gia công) giúp khách hàng dễ dàng tìm kiếm.
*   **Hệ Thống Tương Tác:** Khách hàng có thể thả tim (Like), đánh giá chất lượng theo số sao (1-5★) và để lại bình luận công khai dưới mỗi món ăn.
*   **Giỏ Hàng & Form Đặt Hàng Toàn Diện:** Thu thập đầy đủ thông tin khách hàng (Tên, SĐT, Địa chỉ, Ngày/Giờ nhận hàng, Cách thức chặt heo/Gia công chuẩn lễ).
*   **Gửi Duyệt Đơn Tự Động:** Đóng gói toàn bộ thông tin đơn hàng và chuyển tiếp nội dung trực tiếp qua API chat của **Zalo** hoặc **Facebook Messenger** tới chủ cửa hàng.

---

## 🛠️ Hướng Dẫn Cấu Hình Hệ Thống Hạ Tầng

Để ứng dụng vận hành trơn tru trên GitHub Pages hoặc chạy local, bạn cần đảm bảo cấu hình phân quyền trên **Firebase Console** đã được mở khóa:

### 1. Cấu hình Quyền Đọc/Ghi (Rules)
Truy cập vào **Firebase Console** -> **Realtime Database** -> Chọn tab **Règles (Rules)** và thay đổi cấu hình thành `true` để cấp quyền cho ứng dụng:

```json
{
  "rules": {
    ".read": "true",
    ".write": "true"
  }
}
