
# ✅ Hướng dẫn cài đặt Qt6 C++ (Community) trên Linux bằng Qt Online Installer

## 📦 Yêu cầu trước khi cài đặt:
Cài các gói công cụ cần thiết (trên Ubuntu/Debian):

```bash
sudo apt update
sudo apt install build-essential cmake libgl1-mesa-dev
```

## 📥 1. Tải trình cài đặt Qt
Tải file từ trang chính thức:

👉 https://www.qt.io/download-qt-installer

Chọn bản dành cho Linux:  
`qt-online-installer-linux-x64-4.9.0.run`

## 🔧 2. Cấp quyền thực thi cho file `.run`

```bash
chmod +x qt-online-installer-linux-x64-4.9.0.run
```

## 🚀 3. Chạy trình cài đặt

```bash
./qt-online-installer-linux-x64-4.9.0.run
```

> 💡 Nếu bạn đang sử dụng Wayland (Ubuntu 22.04 trở lên), hãy dùng lệnh này để tránh lỗi giao diện:
```bash
QT_QPA_PLATFORM=xcb ./qt-online-installer-linux-x64-4.9.0.run
```

## 👤 4. Đăng nhập tài khoản Qt

- Đăng nhập hoặc tạo tài khoản mới (miễn phí)
- Chọn **Open Source License**

## 🧩 5. Chọn thành phần cài đặt

Khi đến phần chọn **components**, hãy chọn:

- `Qt > Qt 6.x.x > Desktop gcc 64-bit`
- `Tools > Qt Creator` (nếu bạn muốn cài cả IDE Qt Creator)

## ⏳ 6. Hoàn tất cài đặt

Qt sẽ được cài vào thư mục `~/Qt/` theo mặc định.

## 🚀 7. Mở Qt Creator

Bạn có thể chạy Qt Creator từ terminal:

```bash
~/Qt/Tools/QtCreator/bin/qtcreator
```

Hoặc thêm vào `PATH` để gọi nhanh:

```bash
echo 'export PATH=$HOME/Qt/Tools/QtCreator/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
```

## 🧪 8. Kiểm tra cài đặt Qt

Trong Qt Creator:

- Chọn `File → New Project → Application → Qt Widgets Application` (hoặc `Console`)
- Build & Run thử

---

## 📌 Ghi chú thêm:

- Kiểm tra compiler:
```bash
g++ --version
```

- Có thể dùng Qt Creator với cả `.pro` hoặc `CMakeLists.txt`
- Nếu bạn chỉ build project không cần GUI, có thể chỉ cài `Qt` mà bỏ qua `Qt Creator`

---

Happy coding with Qt! 🚀
