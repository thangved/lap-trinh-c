# Bài 3: Các cú pháp cơ bản

## Các token

Trong ngôn ngữ C, có rất nhiều token khác nhau như **từ khóa**, **định danh**, **hằng số**, **chuỗi** hoặc **kí tự**.

*Chúng ta sẽ từ từ tìm hiểu các khái niệm này trong những bài học tiếp theo*

## Dấu chấm phẩy trong C `;`

Trong ngôn ngữ lập trình C, mỗi câu lệnh phải kết thúc bằng dấu chấm phẩy.

```c
printf("Hello C!");
return 0;
```

Kết thúc mỗi câu lệnh, các bạn có thể xuống dòng hoặc không tùy thích. Nhưng việc viết quá nhiều lệnh trên 1 dòng là không nên chút nào!

## Comment trong C

Comment hiểu đơn giản nó là những ghi chú được ghi trực tiếp trong file C, tuy nhiên những nội dung đó sẽ không được biên dịch khi chương trình được chạy.

### Có 2 cách để comment trong C:

```c
// đây là cách comment thứ nhất

/*
Đây là cách comment thứ hai
*/
```

1. Đối với cách đầu tiên chúng ta chỉ có thể ghi chú trên 1 dòng.

2. Đối với cách comment thứ hai chúng ta có thể ghi chú trên nhiều dòng.

### Khi nào sử dụng comment

Bạn sẽ cần phải ghi chú lại để giải thích một số đoạn code mà bạn cho rằng nó khó hiểu cho người đọc.

### Không nên lạm dụng comment

Đúng vậy, mặc dù những ghi chú của bạn sẽ không được biên dịch, tuy nhiên máy tính vẫn phải chạy qua nó gây tốn thời gian biên dịch. Vì vậy, hãy comment khi cần thiết thôi nhé!

## Định danh

Một định danh trong C được sử dụng như tên biến, tên hàm, tên cấu trúc,...

Một định danh hợp lệ tuân thủ các quy tắc sau:

- Chứa các kí tự trong bảng chữ cái latin (a đến Z) và cái số từ 0 đến 9 và dấu _

- Không chứa các kí tự đặc biệt

- Không bắt đầu bằng số

### Ví dụ:

#### Định danh hợp lệ

```c
myName    Sum    _init    count    age    value1
```

#### Định danh không hợp lệ

```c
@@    1name    123
```

## Từ khóa trong C
