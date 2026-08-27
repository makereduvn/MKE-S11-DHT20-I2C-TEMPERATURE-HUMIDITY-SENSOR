# Cảm biến độ ẩm nhiệt độ MKE-S11 DHT20 I2C Temperature Humidity Sensor

**MKE-S11 DHT20 Temperature Humidity Sensor** là cảm biến đo **nhiệt độ và độ ẩm không khí** sử dụng giao tiếp **I2C**, chỉ cần hai chân tín hiệu `SDA` và `SCL`, giúp việc kết nối với vi điều khiển trở nên đơn giản và thuận tiện. DHT20 là phiên bản nâng cấp của dòng cảm biến DHT11, tích hợp phần tử đo nhiệt độ, độ ẩm và bộ xử lý tín hiệu cải tiến, cho khả năng đo **ổn định và chính xác hơn**. Giao tiếp I2C cũng cho phép kết nối nhiều thiết bị trên cùng một bus, giúp thuận tiện khi xây dựng các hệ thống cần nhiều cảm biến.

Sản phẩm phù hợp cho nhiều ứng dụng như **đo nhiệt độ – độ ẩm môi trường, vườn thông minh, hệ thống giám sát không khí, thiết bị IoT và các dự án STEM**. Mạch được thiết kế tối ưu về **độ ổn định tín hiệu và khả năng chống nhiễu**, đảm bảo hoạt động tin cậy trong cả môi trường học tập và ứng dụng thực tế.

**Cảm biến độ ẩm nhiệt độ MKE-S11 DHT20 Temperature Humidity Sensor** hỗ trợ điện áp giao tiếp **3.3V và 5VDC**, cho phép kết nối trực tiếp và an toàn với các bo mạch điều khiển phổ biến như **Arduino, Raspberry Pi, Jetson Nano, Micro:bit** và nhiều nền tảng khác. Sản phẩm đi kèm **cáp kết nối 4P XH2.54 – Dupont**, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

> **⚠️ Lưu ý:** Cảm biến chỉ nên được sử dụng để đo **độ ẩm không khí trong môi trường thông thường (hơi nước)**. Không sử dụng cảm biến trong các môi trường **ủ kín, có nhiều vi khuẩn, nấm mốc, hóa chất hoặc tác nhân ăn mòn** như **ủ tỏi đen, ủ yếm khí, môi trường có hơi muối**. Các tác nhân này có thể bám hoặc tác động lên bề mặt cảm biến, làm **giảm độ chính xác của phép đo** hoặc **gây hư hỏng cảm biến theo thời gian**.

## Thông số kỹ thuật

- Điện áp cấp nguồn: 5VDC
- Chuẩn tín hiệu điều khiển: I2C
- Điện áp giao tiếp: TTL 3.3 / 5VDC
- Cảm biến sử dụng: DHT20
- Dải đo độ ẩm: 0 ~ 100% RH
- Dải đo nhiệt độ: –40 ~ +80°C
- Độ chính xác độ ẩm: ±3% RH (tại 25°C)
- Độ chính xác nhiệt độ: ±0.5°C
- Độ lặp lại độ ẩm: ±0.1% RH / năm
- Độ lặp lại nhiệt độ: ±0.1°C / năm
- Độ phân giải độ ẩm: 0.024% RH
- Độ phân giải nhiệt độ: 0.01°C
- Thời gian đáp ứng độ ẩm: < 8 giây
- Thời gian đáp ứng nhiệt độ: 5 ~ 30 giây
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Ổn định, chống nhiễu
  - Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 4P XH2.54 – Dupont

## Các chân tín hiệu

| MKE-S11 | Ghi chú                   |
| :-------: | :------------------------- |
| `GND`     | Chân cấp nguồn âm 0VDC    |
| `5V`     | Chân cấp nguồn dương 5VDC |
| `SDA`   | Chân tín hiệu I2C Serial Data|
| `SCL`   | Chân tín hiệu I2C Serial Clock|


## Hướng dẫn sử dụng

### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân `GND` và `5V`
- Kết nối chân `SCL` của Module với chân I2C Clock của mạch điều khiển.
- Kết nối chân `SDA` của Module với chân I2C Data của mạch điều khiển.

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu tại **File / Examples / MKE_ONE / Sensor / MKE_S11_DHT20**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port*- của mạch và nhấn **Upload*- để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân `SDA` và `SCL` của cảm biến với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import*- chương trình theo đường link sau: `https://github.com/makereduvn/mke_s11_dht20_microbit/`
- Kết nối mạch Micro:bit và **Download*- chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân `SDA` và `SCL` của cảm biến với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT*- trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT*- sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-S11 DHT20](/extras/MKE-S11_1.jpg)

## Hình ảnh sản phẩm
![MKE-S11 DHT20](/extras/MKE-S11_2.png)
![MKE-S11 DHT20](/extras/MKE-S11_3.png)

## Miễn trừ trách nhiệm
Sản phẩm này là bo mạch phát triển được thiết kế phục vụ cho mục đích nghiên cứu, thử nghiệm và học tập, không phải là một thiết bị hoàn chỉnh. Trong trường hợp người dùng kết hợp mạch này với các linh kiện, thiết bị hoặc phần mềm khác để tạo thành một hệ thống hoặc sản phẩm hoàn chỉnh, mọi chức năng và tính phù hợp của sản phẩm sau cùng đều thuộc trách nhiệm của người dùng.
