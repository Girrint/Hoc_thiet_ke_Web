## 1.1 URL, siêu liên kết và siêu văn bản:

Web là không gian thông tin toàn cầu. Không gian thông tin này được tạo bởi một mạng lưới gồm nhiều tài nguyên kết nối với nhau.
Mỗi một tài nguyên được định vị bằng một địa chỉ duy nhất, gọi là URL.

### 1.1.1 URL

URL(Uniform Resource Locator),  “bộ định vị tài nguyên thống nhất”, hiểu nôm na là “địa chỉ của một tài nguyên web”, hay địa chỉ web (web address).

URL là một tham chiếu tới tài nguyên web, 
cho biết một tài nguyên web nằm ở đâu trên hệ thống mạng 
và dùng giao thức (hay phương thức) gì để lấy (hay truy cập) được tài nguyên đó.

Một số giao thức có sử dụng URL như HTTP để truy cập web,
FTP để truyền tập tin, mailto để gửi email, JDBC để truy cập cơ sở dữ liệu.

URL cũng xuất hiện trong các thẻ của HTML, như các thẻ: <a href=URL>, <img src=URL>, <script src=URL>, <link href=URL>.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhRmzNxBTrylqOwoQnfI3GQ-dM5NVu8LpZnd2NVQySzKNnBrlVMNDPHqkQlyJ8WkGPe1y5B9nEcWjXcEq4EjfU_BD6ALUOG-Vg1l7YXuM2k-34NLKIH2Jr04M2SEKApIDj7BaLQmclTV38/w400-h84/Dinh+dang+cua+URL+1.jpg)

- Scheme là giao thức được sử dụng để trao đổi thông tin giữa client và server. 
Một số scheme phổ biến: http, https, ftp, file, mailto, data, irc. 
Scheme được ngăn cách với các thành phần phía sau bằng dấu “://”.

- Domain (hay domain name) là tên miền của máy server, cũng được gọi là hostname.  
Máy tính của người dùng sẽ đổi tên miền này thành địa chỉ IP để nó có thể tìm thấy và giao tiếp với máy server.

- Port là cổng, được sử dụng để giao tiếp giữa client và server.
Trong giao thức HTTP nếu không chỉ định rõ, thì giá trị của port sẽ được ngầm hiểu là 80, giao thức HTTPS là 443.

- Path là đường dẫn (đường dẫn thư mục, đường dẫn tuyệt đối) của tài nguyên web trên máy server.
Đường dẫn luôn bắt đầu bằng dấu xuyệt (slash) (/),
có nghĩa là thư mục gốc, mỗi thư mục ngăn cách nhau bằng một dấu “/”.

- URL cũng có thể chứa chuỗi truy vấn hoặc một định danh.
Chuỗi truy vấn (query string) là chuỗi chứa các cặp key=value, nằm ngay sau dấu ?,
 Định danh vùng nội dung (fragment_id) là một vị trí trên một trang web,
 được đánh dấu bằng một cái tên cụ thể, ví dụ một vùng trên trang web có tên là #noi-dung.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj5rhcl0AmAOB6JEIEfnA85OAJLR_X06W4EVdj4skbAwGxnTsrLTHdqrrjm7HSUjurIQ7TCRtkJBAbhImd75agr0_5lWuwujGws_RUVPFfZuOBGskVVnYf7qDegLgcIOmxY7lXFESPUrzQ/w400-h171/Vi+du+URL+2.jpg)

URL là tập con của URI, cộng đồng đang có xu hướng chuyển qua sử dụng URI thay cho URL. 
URI chính xác và tổng quát hơn URL. 
Tuy nhiên, nhiều người vẫn thích sử dụng khái niệm URL hơn. Bạn có thể sử dụng URL và URI thay thế cho nhau.

### 1.1.2 Giao thức File:
