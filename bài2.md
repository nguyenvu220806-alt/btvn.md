# Phần 1: Phân tích 
- **Input:** Văn bản thô hướng dẫn cài đặt cảm biến độ ẩm trang trại Lan, bao gồm các mô tả lệnh terminal, mã nguồn Python, thông số thiết bị và các bước kiểm tra.
- **Output:** Tài liệu Markdown hiển thị trực quan, phân định rõ ràng giữa lệnh Terminal (Inline Code), mã nguồn có màu, bảng so sánh thông số và danh sách việc cần làm (Task List).

# Phần 2: Source Code


```python
1. import time

def kiem_tra_do_am(do_am):
    if do_am < 40:
        print("Độ ẩm thấp! Bật máy bơm...")
    else:
        print("Độ ẩm ổn định.")

if __name__ == "__main__":
    kiem_tra_do_am(35)
2. So sánh cảm biến
|:Tiêu chí:|:Cảm biến cũ:|:Cảm biến mới:|
|:Độ chính xác:|:10%:|:2%:|
|:Kết nối:|:Có dây:|:Không dây:|
3. Task list kiểm tra thiết bị 
[x] Kiểm tra nguồn điện dây cáp nối 
[x] Cài đặt các thư viện python
[] Chạy thử nghiệm trương chình máy bơm
[] Bàn giao hệ thống cho chủ trang trại
```
