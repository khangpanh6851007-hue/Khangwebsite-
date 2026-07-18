# 📦 Tùng Quay Heo - Ứng Dụng Hợp Nhất 1-File HTML (v10.9)

Dự án này là một hệ thống đặt hàng, tương tác cộng đồng trực tuyến dành riêng cho cửa hàng heo quay. Toàn bộ mã nguồn bao gồm **Giao diện (HTML), Thẩm mỹ (Tailwind CSS), Icon (FontAwesome), Tính năng (JavaScript) và Kết nối dữ liệu (Firebase)** được gộp hoàn toàn vào **duy nhất một file `index.html`**.

---

## 📱 Hướng Dẫn Chạy File Duy Nhất

Để khởi chạy ứng dụng trực tiếp trên điện thoại Android bằng **Acode**, hãy làm theo các bước sau:

1. **Tạo File:** Mở ứng dụng **Acode**, tạo một tệp tin mới và đặt tên chính xác là `index.html`.
2. **Dán Code:** Sao chép toàn bộ mã nguồn hợp nhất của phiên bản **v10.9** và dán vào file vừa tạo.
3. **Lưu File:** Nhấn vào biểu tượng **Save (Hình đĩa mềm)** để lưu lại.
4. **Khởi Chạy:** Nhấn vào nút **Play (Mũi tên Run)** ở thanh công cụ phía trên. Acode sẽ tự động kích hoạt trình duyệt nội bộ (hoặc trình duyệt máy) để hiển thị giao diện cửa hàng heo quay ngay lập tức.

---

## 🛠️ Tùy Biến Hệ Thống Ngay Trong Tệp Code

Vì mọi thứ nằm trong 1 file duy nhất, khi cần chỉnh sửa thông tin cửa hàng, bạn chỉ cần mở file trong **Acode**, tìm đến thẻ `<script>` ở phần đầu file để sửa đổi các hằng số:

### 1. Thông tin nhận đơn hàng (Zalo / Messenger)
Hệ thống tự động đóng gói đơn hàng thành văn bản và chuyển tiếp thẳng sang ứng dụng nhắn tin:
```javascript
const CONFIG_ZALO_PHONE = "0900000000";       // SĐT Zalo nhận thông báo đơn hàng của bạn
const CONFIG_FACEBOOK_PAGE = "HeoQuayPhatDat"; // Tên định danh (Username) Fanpage Facebook của bạn
const firebaseConfig = {
    apiKey: "AIzaSyDXI8ThxMEnuzvVFuVgZXWOfRFlvr6WnzE",
    authDomain: "heo-quay-tung-cua-toi.firebaseapp.com",
    databaseURL: "[https://heo-quay-tung-cua-toi-default-rtdb.firebaseio.com](https://heo-quay-tung-cua-toi-default-rtdb.firebaseio.com)",
    projectId: "heo-quay-tung-cua-toi",
    storageBucket: "heo-quay-tung-cua-toi.firebasestorage.app",
};
