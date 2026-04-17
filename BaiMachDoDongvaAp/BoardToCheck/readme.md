# Thực hành luyện tập layout PCB bài mạch đo dòng và áp có Ethernet

## Layer Impedence control stackup calculator

-   Thickness: 1.6mm
-   Outer cooper weight: 1oz
-   Inner cooper weight: 1oz
![alt text](image-1.png)

So sánh với setting trong ALtium Designer 

![alt text](image-2.png)     ![alt text](image-3.png)
 

- Bài luyện tập này dùng theo nhà sản xuất JLCPCB có mã là JLC041611-7628 Stackup
![alt text](image.png)

- Setting đã được áp dụng vào Altium Designer để tính toán độ trở kháng của đường truyền tín hiệu.
![alt text](image-4.png)

- Tính toán standard impedance của đường truyền tín hiệu là 50 Ohm. Kết quả tính toán được hiển thị trong bảng dưới đây:
![alt text](image-5.png)

- Từ đó cài đặt width của đường truyền tín hiệu là 0.3mm để đạt xấp xỉ (sai số nhỏ) được độ trở kháng chuẩn 50 Ohm.
  
## Tranmission line calculator
Có 2 dây differential pair (100 ohm) được thiết kế cho module Ethernet. Kết quả tính toán được hiển thị trong bảng dưới đây:

Cặp dây đúng với setting tự động tính toán của altium designer.

![alt text](image-7.png)

Đã được length matchinng để đảm bảo độ trễ của tín hiệu được đồng bộ giữa 2 dây trong cặp differential pair.

![alt text](image-8.png)

Cặp còn lại khi route thủ công đã tương đối bằng nhau nên không cần phải length matching nữa.

![alt text](image-9.png)

![alt text](image-6.png)