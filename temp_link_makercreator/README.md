# Mạch MakerEdu Creator

![](/temp_link_makercreator/creator1.jpg)

## Giới thiệu

MakerEdu Creator mà mạch điều khiển trung tâm trong hệ sinh thái phần cứng Robotics MakerEdu với 3 chức năng chính:

1. Chức năng lưu trữ và thực thi các lệnh lập trình qua Khối Vi Điều Khiển (Microcontroller Unit).
2. Chức năng cấp nguồn, giao tiếp và điều khiển các mạch module chức năng (MakerEdu Module), cảm biến (MakerEdu Sensor) qua các cổng kết nối chuẩn XH2.54.
3. Chức năng điều khiển 2 Động cơ DC, 2 Động cơ RC Servo qua Khối Công Suất (Power Unit).

Mạch MakerEdu Creator được thiết kế dựa trên nền tảng là mạch Arduino Uno nên hoàn toàn tương thích với các phần mềm:

## Thông số kỹ thuật

<table><thead>
  <tr>
    <th>Model</th>
    <th>MakerEdu Creator</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Vi điều khiển</td>
    <td>ATmega328P-PU</td>
  </tr>
  <tr>
    <td>Điện áp hoạt động</td>
    <td>5VDC từ cổng USB-C</td>
  </tr>
  <tr>
    <td>Digital Port</td>
    <td>D10, D11, D12, D3+D2</td>
  </tr>
  <tr>
    <td>Analog Port</td>
    <td>A1, A2, A3</td>
  </tr>
  <tr>
    <td>I2C Port</td>
    <td>3 x I2C (SDA: A4 / SCL: A5)</td>
  </tr>
  <tr>
    <td>Uart Port</td>
    <td>1 x UART (RX: D0 / TX: D1)</td>
  </tr>
  <tr>
    <td>RC Servo motor control Port</td>
    <td>D10, D11</td>
  </tr>
  <tr>
    <td rowspan="2">DC motor control port</td>
    <td>Motor_A (Speed: D6 / Direction: D8, D9)</td>
  </tr>
  <tr>
    <td>Motor_B (Speed: D5 / Direction: D4, D7)</td>
  </tr>
  <tr>
    <td>Dòng DC đầu ra các chân I/O</td>
    <td>Max 20mA</td>
  </tr>
  <tr>
    <td>Flash Memory</td>
    <td>32KB với 0.5 KB sử dụng cho bootloader</td>
  </tr>
  <tr>
    <td>SRAM</td>
    <td>2KB</td>
  </tr>
  <tr>
    <td>EEPROM</td>
    <td>1KB</td>
  </tr>
  <tr>
    <td>Clock Speed</td>
    <td>16MHz</td>
  </tr>
  <tr>
    <td>LED_BUILTIN</td>
    <td>D13</td>
  </tr>
  <tr>
    <td>IC nạp chương trình và giao tiếp UART</td>
    <td>CH340</td>
  </tr>
  <tr>
    <td>Cổng giao tiếp máy tính</td>
    <td>USB-C</td>
  </tr>
  <tr>
    <td>Tương tích hệ điều hành</td>
    <td>Windows / MacOS / Linux</td>
  </tr>
</tbody></table>

## Hình ảnh sản phẩm

![](/temp_link_makercreator/creator5.jpg)

## Kích thước sản phẩm

![](/temp_link_makercreator/creator2.jpg)

## Các tính năng vượt trội

![](/temp_link_makercreator/creator3.jpg)

1. Mạch MakerEdu Creator thuộc hệ sinh thái phần cứng Robotics MakerEdu với chuẩn kết nối connector XH2.54 chắc chắn, chống ngược và dễ dàng tháo lắp khi sử dụng với các mạch module chức năng (MakerEdu Module) và cảm biến (MakerEdu Sensor).
1. Cấp nguồn qua cổng USB-C dễ dàng và an toàn, có thể sử dụng pin dự phòng (Power Bank), nguồn sạc điện thoại hoặc nguồn từ cổng USB máy tính để cấp nguồn cho mạch MakerEdu Creator.
1. Tích hợp 2 cổng điều khiển 2 x Động cơ RC Servo.
1. Tích hợp Driver điều khiển 2 x Động cơ DC.
1. Vỏ Mica bảo vệ an toàn, tránh chập chạm.
1. Tương thích với hầu hết các hệ điều hành Windows / MacOS / Linux và các phần mềm lập trình phổ biến: Arduino, Mblock, PictoBlox,...

## Các lưu ý

![](/temp_link_makercreator/creator4.jpg)

### 1) Cấp nguồn

Mạch MakerEdu Creator sử dụng nguồn chính từ cổng USB-C để cấp nguồn 5VDC cho hệ thống hoạt động gồm bộ xử lý, cổng kết nối và động cơ. Các bạn có thể lựa chọn cấp nguồn từ cổng USB của máy tính, các loại nguồn cấp bằng cổng USB hoặc với các ứng dụng di động như robot có thể cấp nguồn bằng sạc dự phòng, loại sạc dự phòng khuyến nghị sử dụng:

- [Pin dự phòng USB-C 5VDC 2A 5000mAh Mini Power Bank](https://hshop.vn/pin-du-phong-usb-c-5vdc-2a-5000mah-mini-power-bank)

### 2) Động cơ DC

Động cơ DC sử dụng phải là loại có thể hoạt động ở điện áp 5VDC, với dòng điện tiêu thụ tối đa 800mA, các loại động cơ khuyến nghị sử dụng:

- [Động cơ DC giảm tốc V1 Dual Shaft Plastic Geared TT Motor + bánh xe](https://hshop.vn/dong-co-dc-giamtoc-v1-1-48)
- [Bộ động cơ DC giảm tốc GA12 N20 kèm gá bắt và bánh xe V1 34mm](https://hshop.vn/bo-dong-co-dc-giam-toc-ga12-n20-kem-ga-bat-va-banh-xe-v1-34mm)
- [Động cơ bơm chìm Mini Water Pump 5VDC](https://hshop.vn/dong-co-bom-chim-mini-5vdc) (lưu ý với động cơ bơm cần phải cấp đúng chiều + và - không sẽ làm hỏng cấu trúc động cơ).

### 3) Động cơ RC Servo

Động cơ RC Servo sử dụng phải là loại có thể hoạt động ở điện áp 5VDC, động cơ RC Servo sử dụng trực tiếp nguồn từ cổng USB-C của MakerEdu Creator nên khi sử dụng cần cấp nguồn với dòng điện đủ để động cơ có thể hoạt động bình thường, động cơ khuyến nghị sử dụng:

- [Động cơ RC Servo 9G](https://hshop.vn/dong-co-rc-servo-9g)
- [Động cơ RC Servo MG90S](https://hshop.vn/dong-co-rc-servo-mg90s)

## Hướng dẫn sử dụng với phần mềm Arduino

### Hướng dẫn sử dụng phần mềm Arduino cơ bản

1) Giới thiệu về Arduino

2) Ngôn ngữ lập trình Arduino

3) Cách cài đặt phần mềm Arduino IDE

4) Cách cài đặt Driver và nạp chương trình cho mạch Arduino / Arduino Compatible

5) Cách cài đặt các thư viện phần cứng Arduino Library

6) Cách sử dụng Serial Monitor & Serial Plotter trên phần mềm Arduino

### Hướng dẫn kết nối và nạp chương trình mẫu cho Mạch MakerEdu Creator trên phần mềm Arduino

1) Kết nối máy tính: Kết nối Mạch MakerEdu Creator với máy tính bằng cáp USB-C sẽ thấy Led nguồn PWR trên mạch phát sáng.

![](/temp_link_makercreator/creator6.jpg)

2) Cài đặt Driver: Mạch MakerEdu Creator là một mạch Arduino Uno Compatible (tương thích Arduino Uno) sử dụng IC nạp chương trình và giao tiếp máy tính CH340, các bạn có thể tham khảo Hướng dẫn cài đặt Driver cho các mạch sử dụng IC giao tiếp USB-UART CH34x - MakerLab Wiki.

3) Cấu hình mạch trên phần mềm Arduino: Để cấu hình mạch trên phần mềm Arduino chúng ta cần làm các bước sau:
    - Thiết lập Board tại Tools > Board > Arduino AVR Boards > Arduino Uno và Port (cổng kết nối) cho mạch, nếu không xác định được cổng kết nối có thể ngắt kết nối mạch và kết nối lại đồng thời kiểm tra phần Port để thấy cổng kết nối mới của mạch xuất hiện:

![](/temp_link_makercreator/creator7.jpg)

- Sau khi đã hoàn thành các thiết lập cơ bản bạn có thể nạp chương trình Blink sau vào mạch MakerEdu Creator trên phần mềm Arduino bằng cách nhấn vào nút Upload hoặc chọn Sketch > Upload sẽ thấy đèn Led L13 trên mạch chớp tắt 1 giây 1 lần:

```ino
/*
  Blink
  Turns an LED_BUILTIN on D13 of MakerEdu Creator for one second, then off for one second, repeatedly.
*/
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN on D13 as an output.
  pinMode(13, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(13, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(13, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

![](/temp_link_makercreator/creator8.jpg)

## Hướng dẫn sử dụng với phần mềm mBlock

### Hướng dẫn sử dụng phần mềm mBlock với mạch MakerEdu Creator

1) Giới thiệu và hướng dẫn cài đặt phần mềm mBlock

2) Giới thiệu mạch MakerEdu Creator

3) Cách cài đặt Driver và Device cho mạch MakerEdu Creator trên phần mềm mBlock

4) Các khối lệnh cơ bản của mạch MakerEdu Creator trên phần mềm mBlock

5) Cách cài đặt Extension và giới thiệu các khối lệnh cho phần cứng MakerEdu trên phần mềm mBlock

6) Cách sử dụng Extension Upload Mode Broadcast trên phần mềm mBlock

### Hướng dẫn kết nối và nạp chương trình cho Mạch MakerEdu Creator trên phần mềm Mblock

1) Kết nối máy tính: Kết nối Mạch MakerEdu Creator với máy tính bằng cáp USB-C sẽ thấy Led nguồn PWR trên mạch phát sáng như ở phần hướng dẫn Arduino.

2) Cài đặt Driver và Cấu hình Device: Cài đặt Driver và cấu hình Mạch MakerEdu Creator trên phần mềm Mblock theo hướng dẫn tại đây.

3) Nạp chương trình mẫu: Nạp chương trình chớp tắt đèn Led L13 trên mạch MakerEdu Creator với phần mềm Mblock để kiểm tra hoạt động:

![](/temp_link_makercreator/creator9.png)

## Hỗ trợ và liên hệ

- Website: [https://www.makerlab.vn/](https://www.makerlab.vn/)
- Facebook: [https://www.facebook.com/makerlabvn](https://www.facebook.com/makerlabvn)

## Nhà phân phối

- Các bạn có thể mua sản phẩm của MakerLab tại các [Nhà Phân Phối.](https://www.makerlab.vn/distributor/)
