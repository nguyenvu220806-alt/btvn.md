# Phần 1 : Phân tích (I/O & Phần cứng)
- **Input:** Dữ liệu độ ẩm, nhiệt độ từ cảm biến IoT.
- **Process:** Vi điều khiển SoC xử lý và so sánh với ngưỡng cài đặt.
- **Output:** Kích hoạt máy bơm nước tự động khi đất thiếu ẩm.

---

# Phần 2 : Triển khai (README.md)

# 🚀 Smart-Farm

*Hệ thống tự động hóa tưới cây thông minh cho trang trại Lan.*

![Sơ đồ hệ thống Smart-Farm](https://greentech.vn/smart-farm-diagram.png)

## 1. Hướng dẫn cài đặt
```bash
pip install smartharm-sensor-iot
```
## 2. Tính năng hệ thống (Task List)
[x] Đọc dữ liệu từ cảm biến nhiệt độ và độ ẩm đất

[x] Xử lý logic tự động bật/tắt máy bơm

[ ] Đồng bộ dữ liệu thời gian thực lên Cloud Workspace

---

3. Bảng so sánh

| Thiết bị | Chức năng chính | Thông số kỹ thuật |
| :--------| :---------------| :-----------------|
| Cảm biến độ ẩm | Đo độ ẩm đất | Sai số 2% chuẩn IP67|
| Vi điều khiển SoC | Xử lý trung tâm | Chip IoT hiệu năng cao |

---

4. Nghiệp vụ: Chu kỳ Fetch–Decode–Execute

Quy trình xử lý của CPU:

Fetch (Lấy lệnh): Tải lệnh đọc cảm biến từ RAM.

Decode (Giải mã): Giải mã lệnh so sánh độ ẩm với ngưỡng an toàn (< 40%).

Execute (Thực thi): Kích hoạt rơ-le bật máy bơm nước

5. Mô hình DIKW
Data (Dữ liệu): 28.5°C

Information (Thông tin): Nhiệt độ đất đang cao hơn mức tiêu chuẩn

Knowledge (Tri thức): Hoa lan cần được tưới nước bổ sung

Wisdom (Trí tuệ): Tự động hóa chu trình tưới giúp tiết kiệm nước tối ưu

# Phần 3 : Kiểm thử 
Khi RAM bị đầy nhật ký hệ thống, tuyệt đối không tắt nguồn đột ngột. Hãy tiến hành xóa bộ nhớ đệm tạm thời hoặc xuất log cũ ra thẻ nhớ phụ để giải phóng không gian RAM