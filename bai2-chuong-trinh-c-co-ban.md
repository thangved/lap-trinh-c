# Bài 2: Chương trình C cơ bản

## Tạo file C

Các bạn có thể tạo file C bằng cách ấn tổ hợp phím `Ctrl` + `N` và `Ctrl` + `S` để lưu nó với phần mở rộng là `.c` 

## Cấu trúc của một chương trình C

Cấu trúc của một chương trình C gồm các thành phần sau:

1. Các lệnh tiền xử lý

2. Các hàm

3. Các biến

4. Các lệnh và biểu thức

5. Các comment 

Trong các thành phần trên thì thành phần cơ bản nhất của một chương trình C là hàm `int main`, đây là hàm bắt buộc phải có và là hàm sẽ được thực thi khi chương trình được chạy.

```c
int main(){
    return 0;
}
```

## Chương trình *Hello C!*

Chúng ta sẽ cùng nhau thử viết một chương trình in ra màn hình dòng chữ *Hello C!*.

Như đã nêu ở phần trên, một chương trình C bắt buộc phải có ít nhất là hàm `int main`.

Ngoài ra, chúng ta cần phải import thư viện `stdio.h` để có thể sử dụng các hàm nhập xuất cơ bản.

*Cú pháp import thư viện:`#include<tenThuVien>`*

Để có thể in một chuỗi kí tự ra màn hình chúng ta sử dụng hàm `printf` với tham số là chuỗi cần in ra màn hình.

```c
#include<stdio.h>

int main(){
    printf("Hello C!");
    return 0;
}
```

Như vậy, chúng ta đã viết thành công một chương trình để in ra màn hình dòng chữ *Hello World*.

Bạn có thể chạy chương trình này bằng cách nhấn tổ hợp phím `Ctrl` + `Alt` + `N` trên **Visual Studio Code**.
