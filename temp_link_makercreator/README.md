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

![](/temp_link_makercreator/creator1.jpg)

## Kích thước sản phẩm

![](/temp_link_makercreator/creator2.jpg)

## Hướng dẫn sử dụng

### Các chức năng chính trên mạch

![](/temp_link_Vuno_shield/image/Vuno_shield5.jpg)

1. _**Nút nhấn Reset:**_ được nối với chân Reset (RST) của Arduino hoặc các bo mạch tương thích, sử dụng để khởi động lại (Reset) chương trình.
2. _**Cổng cấp nguồn Domino:**_ được nối với chân VIN của Arduino hoặc các bo mạch tương thích, sử dụng để cấp nguồn cho mạch hoạt động hoặc lấy áp từ chân VIN của Arduino cấp cho các mạch khác, lưu ý không cấp ngược nguồn âm (-) và dương (+) và không cấp quá điện áp quy định dưới đây:
    - Với các mạch Arduino sử dụng IC giảm áp LM1117 5VDC: điện áp VIN cấp từ 6~9VDC.
    - Với mạch Vietduino sử dụng nguồn xung giảm áp: điện áp VIN từ 6~24VDC.
3. _**Cổng giao tiếp I2C:**_ chuẩn cắm Conector XH2.54 4Pins (4 chân), được sử dụng để giao tiếp với cách bo mạch, module, cảm biến sử dụng giao tiếp I2C, thứ tự các chân tín hiệu: SCL-SDA-5V-GND, có tổng cộng 5 cổng I2C với các chân tín hiệu được nối song song (tương đương nhau).
4. _**Cổng Digital I/O đôi:**_ chuẩn cắm Conector XH2.54 4Pins (4 chân), được sử dụng để giao tiếp với các bo mạch, module, cảm biến với 2 chân Digital I/O là D12 và D13 như cảm biến siêu âm hoặc có thể sử dụng như cổng Software Serial UART, thứ tự các chân tín hiệu: D12-D13-5V-GND.
5. _**Cổng giao tiếp UART:**_ chuẩn cắm Conector XH2.54 4Pins (4 chân) được sử dụng để giao tiếp với cách bo mạch, module, cảm Biến sử dụng giao tiếp UART, thứ tự các chân tín hiệu: TX-RX-5V-GND.
6. _**Cổng Digital I/O đơn:**_ chuẩn cắm Conector XH2.54 3Pins (3 chân), được sử dụng để giao tiếp với các bo mạch, module, cảm biến sử dụng tín hiệu Digital, thứ tự các chân tín hiệu: Digital I/O-5V-GND, có tổng cộng 3 cổng Digital I/O đơn được nối với các chân tín hiệu là: D9, D10, D11, thứ tự các chân tín hiệu: Digital Signal-5V-GND.
7. _**Cổng cấp nguồn đầu ra bổ sung POWER+:**_ là cổng OUTPUT (đầu ra), được sử dụng để cấp nguồn cho các bo mạch, module, cảm biến cần sử dụng thêm các tín hiệu nguồn cấp bổ sung như: mạch relay, mạch điều khiển động cơ,..., thứ tự các chân tín hiệu: 3V3-5V-VIN-GND.
8. _**Cầu phân áp VIN:**_ là cầu phân áp được nối với chân VIN, đầu ra của cầu phân áp sẽ trả ra giá trị là VOUT = VIN/5.7 được nối vào chân tín hiệu Analog A0 trên mạch, được sử dụng để đo giá trị của VIN trong các trường hợp: xác định mức pin, báo hiệu hết pin,...
9. _**Cổng Analog Input:**_ chuẩn cắm Conector XH2.54 3Pins (3 chân), được sử dụng để giao tiếp với các bo mạch, module, cảm biến sử dụng tín hiệu Analog, thứ tự các chân tín hiệu: Analog Signal-5V-GND, có tổng cộng 3 cổng Analog Input được nối với các chân tín hiệu là: A1, A2, A3 (lưu ý đối với Arduino thì chân Analog còn có thể sử dụng như chân Digital nên cũng có thể sử dụng các cổng Analog Input này với chức năng như các cổng Digital I/O đơn).
10. _**Đèn báo nguồn:**_ đèn sẽ sáng báo hiệu khi mạch MakerEdu Shield for Vietduino đã được cấp nguồn.

### Cách kết nối

#### Kết nối MakerEdu Shield với Vietduino Uno

![](/temp_link_Vuno_shield/image/Vuno_shield6.jpg)

**Lưu ý khi kết nối:**

1. Cần cắm chặt và chính xác các chân kết nối của MakerEdu Shield với Vietduino.  
2. Đèn nguồn trên MakerEdu Shield sẽ phát sáng khi các chân được kết nối chặt, khớp và đúng thứ tự.

![](/temp_link_Vuno_shield/image/Vuno_shield7.jpg)

## Các thiết bị sử dụng trong bài

### Vietduino

- [Mạch Vietduino Uno (Arduino Uno Compatible)](https://www.makerlab.vn/vuno)
- [Cảm biến độ ẩm nhiệt độ MKE-S14 DHT11 Temperature and Humidity Sensor](https://www.makerlab.vn/mkes14)
- [Mạch màn hình MKE-M07 LCD1602 I2C Display Module](https://www.makerlab.vn/mkem07)
- [Cảm biến ánh sáng quang trở MKE-S02 LDR Light Sensor](https://www.makerlab.vn/mkem02)
- [Mạch còi báo MKE-M03 Buzzer Module](https://www.makerlab.vn/mkem03)
- [Cáp kết nối MakerEdu XH2.54 3Wires 20cm Cable](https://hshop.vn/cap-ket-noi-makeredu-xh2-54-3wires-20cm-cable)
- [Cáp kết nối MakerEdu XH2.54 4Wires 20cm Cable](https://hshop.vn/cap-ket-noi-makeredu-xh2-54-4wires-20cm-cable)

### Arduino

- [Mạch Uno (Arduino Uno Compatible)](https://hshop.vn/arduino-uno-r3)
- [Cảm Biến Độ Ẩm, Nhiệt Độ DHT11 Temperature Humidity Sensor ra chân](https://hshop.vn/cam-bien-do-am-nhiet-do-dht11-ra-chan)
- [Màn hình LCD text LCD1602 xanh dương](https://hshop.vn/lcd-text-lcd1602-xanh-duong)

## Hỗ trợ và liên hệ

- Website: [https://www.makerlab.vn/](https://www.makerlab.vn/)
- Facebook: [https://www.facebook.com/makerlabvn](https://www.facebook.com/makerlabvn)

## Nhà phân phối

- Các bạn có thể mua sản phẩm của MakerLab tại các [Nhà Phân Phối.](https://www.makerlab.vn/distributor/)
