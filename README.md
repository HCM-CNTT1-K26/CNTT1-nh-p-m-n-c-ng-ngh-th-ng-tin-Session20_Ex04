# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session20_Ex04
### 1. Bảng so sánh bảo mật

| Tiêu chí | Lưu trực tiếp trên Chrome | Cài đặt Bitwarden |
| --- | --- | --- |
| **Chống Infostealer** | **Yếu:** Mã độc quét dễ dàng trích xuất file `Login Data` lưu cục bộ trên máy và giải mã nhanh chóng. | **Tốt:** Dữ liệu mã hóa đầu cuối (E2EE), mã độc lấy file cũng chỉ thấy chuỗi mã hóa vô nghĩa nếu thiếu Master Password. |
| **Zero-Knowledge Architecture** | **Không:** Dữ liệu đồng bộ qua tài khoản Google, về mặt kỹ thuật phía server vẫn có thể can thiệp nếu không bật mã hóa riêng. | **Có:** Mã hóa/giải mã hoàn toàn tại thiết bị người dùng. Phía Bitwarden không lưu và không biết Master Password. |
| **Đồng bộ chéo nền tảng** | **Hạn chế:** Tối ưu tốt nhất trên Chrome/Android, dùng qua trình duyệt khác rất bất tiện. | **Linh hoạt:** Chạy mượt trên mọi OS (Windows, Mac, Linux, iOS, Android) và mọi trình duyệt qua extension. |

---

### 2. Lý do Bitwarden thắng thế dù tốn công nhập Master Password

* **Tách biệt khỏi rủi ro trình duyệt:** Trình duyệt là mục tiêu hàng đầu của mã độc Infostealer. Bitwarden lưu trữ độc lập, giải mã tạm thời trên RAM và tự khóa lại, giúp chặn đứng việc thu thập mật khẩu tự động.
* **Chuẩn bảo mật Zero-Knowledge:** Dù server Bitwarden có bị hack hay rò rỉ dữ liệu, kẻ tấn công cũng không thể giải mã được mật khẩu vì chìa khóa duy nhất nằm ở Master Password của nhân viên.
* **Kiểm soát an toàn cho công ty:** Giúp IT bắt buộc các chính sách mật khẩu mạnh, bật 2FA/MFA và chia sẻ tài khoản trong nhóm an toàn, tránh việc nhân viên lưu lộn xộn vào tài khoản Google cá nhân.
