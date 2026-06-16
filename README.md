# Robot Controlled Car - IOT102 Project

## Giới thiệu
Đây là dự án xe robot thông minh được phát triển như một mô hình học tập cho môn học IOT102. 
Hệ thống nhận lệnh từ người dùng thông qua Bluetooth để điều khiển xe chạy thẳng, lùi, quẹo trái/phải và dừng lại. Ngoài ra, xe robot có khả năng đo nhiệt độ môi trường và đo khoảng cách để tránh vật cản phía trước.

## Thành viên nhóm (Group 2 - IA2001)
- Nguyễn Hoàng Quý (SE182666)
- Đỗ Trung Nguyên (SE193183) 

## Các linh kiện chính
- Controller: Arduino Uno R3
- Giao tiếp không dây: Bluetooth HC-05
- Cảm biến: Cảm biến siêu âm HC-SR04, Cảm biến nhiệt độ DHT11
- Cơ cấu chấp hành: L298N Motor Driver, 2x DC Motors, LED báo trạng thái

## Sơ đồ đấu nối chân (Pin Mapping)
- **HC-05:** TXD -> Pin 2 | RXD -> Pin 3
- **HC-SR04:** Trig -> Pin 4 | Echo -> Pin 5
- **DHT11:** DATA -> Pin 6
- **LED:** Anode -> Pin 7
- **L298N:** IN1->Pin 8 | IN2->Pin 9 | IN3->Pin 10 | IN4->Pin 11

## Cách sử dụng
1. Lắp ráp mạch theo sơ đồ chân phía trên.
2. Nạp file `SmartCar.ino` vào Arduino Uno thông qua Arduino IDE. Đảm bảo đã cài đặt thư viện `DHT.h` (phiên bản 1.4.6).
3. Kết nối nguồn 9V cho hệ thống.
4. Dùng điện thoại kết nối Bluetooth với HC-05 và sử dụng App điều khiển.
