# Bài 1: Cài đặt IDE và môi trường lập trình

## IDE

Các bạn có thể sử dụng bất kì công cụ lập trình nào mà các bạn yêu thích. Ở đây mình đề xuất sử dụng **Visual Studio Code** vì nó có các điểm nổi bật như sau:

- Mã nguồn mở (Free)

- Nhiều extension hữu ích

- Cộng đồng hỗ trợ cực lớn

Để tải **Visual Studio Code** các bạn nhấp vào [Link này](https://code.visualstudio.com/) và lựa chọn phiên bản phù hợp với hệ điều hành và tải về.

![Hình chụp từ 2021-07-29 20-23-28.png](https://raw.githubusercontent.com/thangved/images/main/2021/07/29-20-23-35-H%C3%ACnh%20ch%E1%BB%A5p%20t%E1%BB%AB%202021-07-29%2020-23-28.png)

Sau khi cài xong Visual Studio Code các bạn cần cài đặt một extension có tên là code runner để có thể thực thi các đoạn mã trong vs code.

![Hình chụp từ 2021-07-29 20-27-54.png](https://raw.githubusercontent.com/thangved/images/main/2021/07/29-20-28-08-H%C3%ACnh%20ch%E1%BB%A5p%20t%E1%BB%AB%202021-07-29%2020-27-54.png)

## Môi trường lập trình

Để có thể lập trình C, các bạn cần có môi trường gcc để thực thi các đoạn mã, tùy theo từng hệ điều hành thì sẽ có các cách cài đặt khác nhau. Đối với các bạn sử dụng các IDE khác như Dev C/C++, Code::block,... thì không cần phải setup môi trường.

### Windows

#### Cài đặt gcc

Đối với những bạn sử dụng **Windows**, các bạn cài đặt **gcc** thông qua **minGW**.

*Tải minGW [tại đây](https://sourceforge.net/projects/mingw/)*

![Ảnh chụp màn hình (126).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-09-01-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(126).png)

Sau khi tải về, các bạn tiến hành cài đặt như các bước trong hình:

![Ảnh chụp màn hình (129).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-14-47-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(129).png)

![Ảnh chụp màn hình (130).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-14-54-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(130).png)

![Ảnh chụp màn hình (131).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-15-03-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(131).png)

Sau khi minGW đã tải xong tài nguyên, các bạn sẽ chọn các gói sau để cài đặt:

1. mingw32-gcc-ada

2. mingw32-gcc-fortran

3. mingw32-gcc-g++

4. mingw32-gcc-objc

![Ảnh chụp màn hình (132).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-16-36-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(132).png)

Sau khi lựa chọn xong các gói cài đặt, bạn nhấn vào phần installation và chọn Apply Changes. Sẽ có một cửa sổ hiện lên, bạn chọn Apply và đợi quá trình cài đặt hoàn tất.

![Ảnh chụp màn hình (133).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-16-52-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(133).png)

#### Thiết lập biến môi trường

Sau khi cài đặt xong gcc, các bạn cần phải thiết lập biến môi trường để máy tính có thể hiểu được lệnh `gcc`.

*Đầu tiên*, các bạn vào phần thông tin của hệ điều hành sau đó chọn `thiết lập chuyên sâu`.

*Tiếp theo*, tại cửa sổ hiện ra các bạn chọn vào `Enviroment Variables`.

![Ảnh chụp màn hình (136).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-25-11-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(136).png)

Chọn vào `path`.

![Ảnh chụp màn hình (137).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-25-15-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(137).png)

Chọn vào `New` để thêm một biến môi trường.

![Ảnh chụp màn hình (138).png](https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-25-22-A%CC%89nh%20chu%CC%A3p%20ma%CC%80n%20hi%CC%80nh%20(138).png)

Sau đó các bạn nhấn vào `Browser` và chọn thư mục `bin` theo đường dẫn `C:\MinGW\bin`.

*Cuối cùng*, bạn chỉ cần nhấn `OK` ở tất cả các cửa sổ là được.

*Để kiểm tra gcc đã được cài đặt thành công hay chưa, các bạn mở Termial (Hay bất cứ cái cmd nào mà bạn có) và gõ dòng lệnh sau:*

```
gcc --version
```

Nếu như nó không báo lỗi thì xin chúc mừng, bạn đã hoàn tất việc thiết lập môi trường để lập trình C.

Còn nếu chương trình báo lỗi thì có lẽ bạn đã thực hiện sai ở bước nào đó, hãy thử kiểm tra lại nhé.

<img src="https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-41-36-giphy.webp" title="" alt="giphy.webp" width="188">

### Linux

Đối với **Linux**, mọi chuyện thật đơn giản, bạn chỉ cần cài gcc thông qua apt.

```
sudo apt install gcc
```

<img src="https://raw.githubusercontent.com/thangved/images/main/2021/07/30-08-43-13-giphy%20(1).webp" title="" alt="giphy (1).webp" width="177">

### Mac OS

---
