
# 🚀 Hướng dẫn tạo Project C++ mới trong Qt6 bằng Qt Creator

## ✅ Bước 1: Mở Qt Creator

Từ terminal:
```bash
~/Qt/Tools/QtCreator/bin/qtcreator
```

Hoặc mở từ menu ứng dụng nếu đã cài vào hệ thống.

---

## ✅ Bước 2: Tạo Project mới

- Chọn **File → New Project**
- Chọn loại project:
  - **Console Application**: cho chương trình C++ dòng lệnh
  - **Qt Widgets Application**: nếu cần giao diện người dùng
  - **Qt Quick Application**: dùng QML (cấp cao hơn)

---

## ✅ Bước 3: Đặt tên project và thư mục

Ví dụ:
- Tên: `MyFirstQtApp`
- Thư mục lưu: `/home/user/Projects/MyFirstQtApp`

---

## ✅ Bước 4: Chọn Kit và Qt Version

- Chọn kit có tên như: `Desktop Qt 6.x.x GCC 64-bit`
- Nếu chưa thấy kit:
  - Cài g++: `sudo apt install build-essential`
  - Vào: `Tools → Options → Kits` để thêm kit

![image](https://github.com/user-attachments/assets/4bd6a42d-2fee-4765-bf71-8409a1d80283)

---

## ✅ Bước 5: Finish

Qt Creator sẽ tự tạo các file cần thiết:
- Console: `main.cpp`, `.pro`
- GUI: `main.cpp`, `mainwindow.cpp/h`, `mainwindow.ui`, `.pro`

---

## ✅ Bước 6: Build & Run

- Nhấn nút ▶️ (hoặc `Ctrl + R`)
- Console sẽ hiện ra (nếu là console app)
- Cửa sổ GUI hiện lên (nếu là Qt Widgets)

---

## 📌 Ghi chú:

- Dự án Qt sử dụng file `.pro` (qmake) hoặc `CMakeLists.txt` (CMake)
- Bạn có thể thêm thư viện, chỉnh sửa giao diện, v.v. sau khi tạo

---

Happy coding with Qt! 🚀
