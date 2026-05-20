# 📘 Hướng Dẫn Lấy Personal Access Token (PAT) Của GitHub

Để ứng dụng **GiT UPLOAD** có thể thay mặt bạn tự động tạo kho lưu trữ (repository) và tải mã nguồn lên GitHub, bạn cần cung cấp một "chìa khóa" được gọi là **Personal Access Token (PAT)**.

Dưới đây là các bước rất đơn giản để tạo mã Token này.

---

## 🛠 Các bước thực hiện

### Bước 1: Truy cập vào trang quản lý Token của GitHub
1. Mở trình duyệt và đăng nhập vào tài khoản GitHub của bạn.
2. Bấm trực tiếp vào đường link sau để đi đến trang tạo Token:  
   👉 [https://github.com/settings/tokens](https://github.com/settings/tokens)

### Bước 2: Tạo Token Mới
1. Ở góc trên cùng bên phải, bấm vào nút **Generate new token**.
2. Khi menu xổ xuống, hãy chọn **Generate new token (classic)** *(Tạo token cổ điển)*.

> **Lưu ý:** Nếu hệ thống yêu cầu xác nhận mật khẩu hoặc mã xác thực (2FA), bạn hãy nhập vào để tiếp tục.

### Bước 3: Cấu hình Token (CỰC KỲ QUAN TRỌNG)
Trong trang tạo Token, bạn hãy điền các thông tin sau:
* **Note:** Nhập tên bất kỳ để bạn nhớ token này dùng cho việc gì (Ví dụ: `Git Upload App`).
* **Expiration:** Nên chọn `No expiration` (Không bao giờ hết hạn) để bạn không phải tạo lại token sau này.
* **Select scopes (Cấp quyền):** 
  * Hãy tìm đến dòng có chữ **`repo`** (thường nằm ngay đầu tiên).
  * **Tích chọn ✅ vào ô vuông chữ `repo`**. Hành động này sẽ tự động tích luôn các ô vuông con bên trong. (Điều này cho phép ứng dụng có quyền tạo và chỉnh sửa repository).

![Ảnh minh họa tích chọn ô repo](https://docs.github.com/ing/Screenshot 2026-05-21 023020.png)

### Bước 4: Hoàn tất và Copy
1. Cuộn xuống dưới cùng của trang và bấm nút xanh lá cây **Generate token**.
2. GitHub sẽ hiển thị một chuỗi ký tự dài bắt đầu bằng `ghp_...` (Ví dụ: `ghp_1234567890abcdefghijklmnopqrstuvwx`).
3. **Copy chuỗi này ngay lập tức** vì GitHub sẽ chỉ hiển thị nó 1 lần duy nhất!

---

## 🚀 Hoàn thành
Mở phần mềm **GiT UPLOAD** lên, dán mã Token bạn vừa copy vào ô **Personal Access Token (PAT)**. Giờ thì ứng dụng đã sẵn sàng hoạt động 100%!
