# Mạch Mtiny ESP32 WROVER-IE (Arduino Compatible)

![](/image/32ie_01_front_of_product.jpg)

## Giới thiệu

Mạch Mtiny ESP32 WROVER-IE (Arduino Compatible) được nghiên cứu và và sản xuất bởi MakerLab.vn dựa trên module Wifi BLE SoC ESP32 ESP-WROVER-IE từ chính hãng Espressif, mạch có thiết kế nhỏ gọn tiện lắp đặt, dễ dàng kết nối và lập trình với phần mềm Arduino qua mạch nạp Mtiny Programmer với chuẩn nạp Mtiny Socket.

Mtiny là viết tắt của Maker Tiny là dự án tạo ra các mạch vi điều khiển với thiết kế nhỏ gọn sử dụng chuẩn chân cắm DIP 2.54mm, các mạch Mtiny sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

## Thông số kỹ thuật

<table><thead>
  <tr>
    <th>Model</th>
    <th>Mtiny ESP32 WROVER-IE (Arduino Compatible)</th>
  </tr></thead>
<tbody>
  <tr>
    <td>CPU and On­Chip Memory</td>
    <td>ESP32-D0WD-V3 embedded, Xtensa dual-core 32-bit LX6 microprocessor, up to 240 MHz<br>448 KB ROM<br>520 KB SRAM<br>16 KB SRAM in RTC</td>
  </tr>
  <tr>
    <td>Power Supply</td>
    <td>3.0 ~ 3.6VDC, Typical 3.3VDC, Current &gt; 500mA</td>
  </tr>
  <tr>
    <td>Interface</td>
    <td>SD card, UART, SPI, SDIO, I2C, LED PWM, Motor PWM, I2S, IR, pulse counter, GPIO, capacitive touch sensor, ADC, DAC, Two-Wire Automotive Interface (TWAI®, compatible with ISO11898-1)</td>
  </tr>
  <tr>
    <td>Wifi</td>
    <td>802.11b/g/n<br>Bit rate: 802.11n up to 150 Mbps<br>A-MPDU and A-MSDU aggregation<br>0.4 µs guard interval support<br>Center frequency range of operating channel: 2412 ~ 2484 MHz</td>
  </tr>
  <tr>
    <td>Bluetooth</td>
    <td>Bluetooth V4.2 BR/EDR and Bluetooth LE specification<br>Class-1, class-2 and class-3 transmitter<br>AFH<br>CVSD and SBC</td>
  </tr>
  <tr>
    <td>Integrated Components on Module</td>
    <td>40 MHz crystal oscillator<br>16MB (XX0H28) SPI Flash (mạch hiện chỉ có một phiên bản duy nhất với dung lượng bộ nhớ Flash là 16MB)<br>8MB external Pseudo Static RAM</td>
  </tr>
  <tr>
    <td>Antenna</td>
    <td>PCB</td>
  </tr>
  <tr>
    <td>Button</td>
    <td>EN (Enable) / IO0</td>
  </tr>
  <tr>
    <td>Led</td>
    <td>Power Led / D13</td>
  </tr>
  <tr>
    <td>Packet</td>
    <td>DIP30 (15x2) 2.54mm</td>
  </tr>
  <tr>
    <td>Programmer</td>
    <td><a href="https://makerlab.vn/mtprogrammer">Mạch Mtiny Programmer (Arduino Compatible)</a></td>
  </tr>
  <tr>
    <td>Programmer Connector</td>
    <td>Mtiny Socket - IDC 8-Pin (2x4)</td>
  </tr>
</tbody></table>

## Kích thước

![](/image/32ie_02_dimension.jpg)

## Các tính năng vượt trội

1) Thiết kế nhỏ gọn với chuẩn chân cắm DIP 2.54mm, tương thích với hầu hết các loại BreadBoard thông dụng.

2) Thuộc Series Mtiny nên sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

3) Bổ sung thêm các linh kiện giúp ổn định, chống nhiễu.

4) Sau khi đã nạp chương trình, có thể cấp nguồn linh hoạt cho mạch bằng mạch Mtiny Power (6 \~ 24VDC) hoặc cấp nguồn trực tiếp qua chân 3V3 (3 \~ 3.3VDC).

## Hình ảnh

![](/image/32ie_03_front_and_back.jpg)

## Hướng dẫn sử dụng

### Hướng dẫn hàn Mtiny Socket và kết nối với Mạch Mtiny Programmer cho Mạch Mtiny ESP32 WROVER-IE

Mạch Mtiny ESP32 WROVER-IE sử dụng mạch nạp Mtiny Programer với chuẩn nạp Mtiny Socket để nạp chương trình, cấp nguồn và giao tiếp với máy tính, hàn Mtiny Socket sử dụng rào đực đôi Header 2x4pins theo chiều hướng lên và kết nối như sau:

![](/image/32ie_04_.jpg)

### Hướng dẫn nạp chương trình với Arduino sử dụng mạch Mtiny Programmer

#### Hướng dẫn sử dụng phần mềm Arduino cơ bản

[Hướng dẫn cài đặt phần mềm, nạp chương trình, cài đặt bộ thư viện Arduino cơ bản.](https://github.com/makerlabvn/Arduino-Vietduino)

- Tải và cài đặt [phần mềm Arduino tại đây.](https://www.arduino.cc/en/software)

#### Hướng dẫn kết nối và nạp chương trình cho Mạch Mtiny ESP32 WROVER-IE trên phần mềm Arduino

1) Kết nối máy tính: Kết nối Mạch Mtiny ESP32 WROVER-IE với Mạch Mtiny Programmer bằng cáp IDC 2x4pins, kết nối Mạch Mtiny Programmer với máy tính bằng cáp USB-C sẽ thấy Led nguồn PWR trên mạch Mtiny Programmer và Mtiny ESP32 WROVER-IE phát sáng:

![](/image/32ie_05.jpg)

2) Cài đặt Driver: Mạch Mtiny Programmer sử dụng IC nạp chương trình và giao tiếp máy tính CH340, các bạn có thể tham khảo hướng dẫn cài đặt Driver tại đây cho hệ điều hành Windows, lưu ý hệ điều hành MacOS hoặc Linux sẽ tự nhận Driver mà không cần cài đặt.

3) Cấu hình mạch trên phần mềm Arduino: Để cấu hình mạch trên phần mềm Arduino chúng ta cần làm các bước sau:

Copy đường link sau và dán vào mục File > Preferences > Additional boards manager URLs (trên Windows) hoặc Arduino IDE > Settings > Additional boards manager URLs (trên MacOS) sau đó nhấn OK:
        
    <https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json>

![](/image/32ie_06.png)

Tiếp theo chọn Tools > Board > Boards Manager..., tìm từ khoá ESP32 sẽ thấy mục "esp32 by Espressif Systems", nhấn Install và chờ đợi cho đến khi cài đặt hoàn tất:

![](/image/32ie_07.png)

Sau khi cài đặt hoàn tất, tắt và khởi động lại phần mềm Arduino, sau đó thiết lập Board tại Tools > Board > esp32 > ESP32 Wrover Kit (all versions) và Port (cổng kết nối) cho mạch, nếu không xác định được cổng kết nối có thể ngắt kết nối mạch và kết nối lại đồng thời kiểm tra phần Port để thấy cổng kết nối mới của mạch xuất hiện:

![](/image/32ie_08.png)

Các thiết lập mặc định để nạp chương trình của mạch sẽ như hình dưới đây:
> Lưu ý quan trọng!!!:  
 Upload Speed với hệ điều hành Windows có thể chọn 912600, với MacOS hoặc các hệ điều hành khác nếu có báo lỗi khi nạp chương trình chọn 115200.  
 Flash Size nếu ký hiệu trên Module WROVER-IE là "XXN4" chọn 4MB, nếu ký hiệu là "XX0H28" chọn 16MB.

![](/image/32ie_09.png)

Sau khi đã hoàn thành các thiết lập cơ bản bạn có thể nạp chương trình Blink sau vào mạch để test bằng cách nhấn vào nút Upload hoặc chọn Sketch > Upload sẽ thấy Led được kết nối với chân IO2 trên mạch chớp tắt 1 giây 1 lần:

```ino
/*
  Blink
  Turns an LED_BUILTIN on IO2 of Mtiny ESP32 WROVER-IE for one second, then off for one second, repeatedly.
*/
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN on IO2 as an output.
  pinMode(2, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(2, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(2, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

![](/image/32ie_10.png)

### Hướng dẫn cấp nguồn sử dụng mạch Mtiny Power sau khi đã nạp chương trình

Trong các trường hợp đã nạp chương trình (không cần sử dụng đến mạch nạp), muốn cấp nguồn riêng cho các mạch Mtiny và các mạch khác trong hệ thống, các bạn có thể sử dụng mạch Mtiny Power kết nối với các chân 3V3-5V-GND trên Mtiny Socket như sau:

<table><thead>
  <tr>
    <td>Power Input</td>
    <td>USB-C: 5VDC (Support USB Power Bank)<br>Domino (VIN): 6~24VDC</td>
  </tr></thead>
<tbody>
  <tr>
    <td>Power Output</td>
    <td>5VDC - Max 500mA (USB-C Input)<br>5VDC - Max 1500mA (Domino Input)<br>3.3VDC - Max 700mA</td>
  </tr>
</tbody>
</table>

![](/image/32ie_11.jpg)

## Nhà phân phối

Có thể mua Mạch Mtiny ESP32 WROVER-IE (Arduino Compatible) tại các nhà phân phối sau:

- [Hshop.vn - Điện tử & Robot.](https://hshop.vn)
