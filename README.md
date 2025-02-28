# 🔒 Khóa Cửa Thông Minh - Arduino

## 📄 Giới Thiệu

Dự án **Khóa Cửa Thông Minh** sử dụng **Arduino** là một hệ thống bảo mật hiện đại, cho phép người dùng mở khóa cửa bằng nhiều phương thức như **mật khẩu, thẻ RFID và cảm biến vân tay**. Dự án này giúp nâng cao tính an toàn, tiện lợi và có thể ứng dụng thực tế trong gia đình, văn phòng hoặc các khu vực yêu cầu bảo mật cao.

---

## 📂 Cấu Trúc Dự Án

```
📦 KhoaCuaThongMinh_Arduino
┣ 📂 Code/                   # Mã nguồn Arduino
┣ 📂 Schematics/             # Sơ đồ mạch điện
┣ 📂 Documentation/          # Tài liệu hướng dẫn và thiết kế
┣ 📜 README.md               # Tài liệu hướng dẫn
```

---

## 🛠️ Yêu Cầu Hệ Thống

### Phần Cứng

- **Vi điều khiển:** Arduino Uno hoặc tương đương
- **Cảm biến:** Mô-đun cảm biến vân tay (nếu sử dụng)
- **RFID:** Mô-đun RFID RC522 (nếu sử dụng thẻ từ)
- **Bàn phím:** Bàn phím ma trận 4x4 (nếu sử dụng mật khẩu)
- **Màn hình LCD:** LCD 16x2 (tùy chọn)
- **Khóa điện tử:** Relay điều khiển khóa cửa
- **Linh kiện khác:** Nút nhấn, LED, điện trở, dây nối, nguồn 5V

### Phần Mềm

- [Arduino IDE](https://www.arduino.cc/en/software)
- [Thư viện MFRC522](https://github.com/miguelbalboa/rfid) (dành cho RFID)
- [Thư viện Adafruit Fingerprint Sensor](https://github.com/adafruit/Adafruit-Fingerprint-Sensor-Library) (dành cho cảm biến vân tay)

---

## 🔧 Cài Đặt

1. **Clone repository:**
   ```bash
   git clone https://github.com/N21DCVT030/KhoaCuaThongMinh_Arduino.git
   cd KhoaCuaThongMinh_Arduino
   ```

2. **Cài đặt Arduino IDE:**
   - Tải và cài đặt [Arduino IDE](https://www.arduino.cc/en/software).

3. **Cài đặt các thư viện cần thiết:**
   - Mở Arduino IDE.
   - Vào **Sketch** > **Include Library** > **Manage Libraries...**.
   - Tìm và cài đặt các thư viện:
     - `MFRC522`
     - `Adafruit Fingerprint Sensor`

4. **Nạp mã nguồn vào Arduino:**
   - Kết nối Arduino với máy tính qua cáp USB.
   - Mở tệp `.ino` trong thư mục `Code/` bằng Arduino IDE.
   - Chọn đúng board và cổng COM trong **Tools**.
   - Nhấn **Upload** để nạp chương trình vào Arduino.

---

## 💡 Hướng Dẫn Sử Dụng

1. **Kết nối phần cứng:** Xây dựng mạch theo sơ đồ trong thư mục `Schematics/`.
2. **Khởi động hệ thống:** Cấp nguồn cho Arduino, hệ thống sẽ sẵn sàng hoạt động.
3. **Mở khóa cửa:**
   - Nhập mật khẩu trên bàn phím.
   - Quét thẻ RFID nếu sử dụng mô-đun RFID.
   - Sử dụng cảm biến vân tay nếu có.
4. **Quản lý người dùng:**
   - Đăng ký hoặc xóa người dùng RFID/vân tay qua giao diện Arduino (nếu hỗ trợ).
   - Thay đổi mật khẩu trực tiếp trên hệ thống.

---

## 🌟 Tính Năng

- ✅ Hỗ trợ mở khóa bằng mật khẩu, RFID và vân tay.
- ✅ Hiển thị trạng thái trên màn hình LCD (nếu có).
- ✅ Cảnh báo khi nhập sai mật khẩu/quét sai nhiều lần.
- ✅ Dễ dàng mở rộng và nâng cấp.

---
💡 *Hy vọng tài liệu này giúp bạn dễ dàng sử dụng và phát triển dự án hơn!* 🚀

