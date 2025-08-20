# 1.HTML
## 1.1 Tạo một trang web đơn giản:
<b>HTML là gì?</b><br>
HTML(HyperText Markup Language) là ngôn ngữ đánh dấu siêu văn bản (không phải ngôn ngữ lập trình) dùng để tạo nội dung cho môi trường web.<br>
<b>Tài liệu HTNL là gì?</b><br>
HTML document là tập tin chứa mã HTML, là trang web ở dạng mã nguồn.<br>
### 1.1.1 Trang web tĩnh:
Trang web tĩnh (static web page, flag page, stationary page): 
là trang web chứa nội dung cố định, 
nội dung giống nhau với mọi người dùng,
mọi ngữ cảnh.<br>
Mã nguồn của trang web tĩnh thường là tài liệu HTML, 
lưu dưới dạng tập tin.<br>
Mã nguồn của trang web tĩnh có thể được lưu trong cơ sở dữ liệu,
thậm chí bao gồm các trang web được tạo ra bằng mẫu có sẵn (template) và được phân phối thông qua một server ứng dụng,
miễn là các trang kết quả không thể thay đổi.<br>
### 1.1.2 Chuẩn bị nội dung cho trang web:
<b>Những thứ trình duyệt bỏ qua khi hiển thị một văn bản</b><br>
Chuỗi khoảng trắng (spaces): 
khi gặp một chuỗi khoảng trắng,
trình duyệt chỉ ghi nhận khoảng trắng đầu tiên,
các khoảng trắng sau đó sẽ bị bỏ.<br>
Kí hiệu xuống hàng (line break, carriage return):
Khi gặp 1 hay nhiều kí tự xuống hàng liên tiếp,
trình duyệt sẽ chuyển thành một khoảng trắng.<br>
Các tab cũng được chuyển thành khoảng trắng.<br>
Vì đặc tính bỏ qua chuỗi khonagr trắng,
kí hiệu xuống hàng và tab,
nên phần văn bản hoặc các phần tử nội tuyến (inline element) khác sẽ được đặt cạnh nhau, liên tục, 
và chỉ bị ngắt dòng khi gặp một phần tử khối (block element).<br>
Các thẻ (tag) mà trình duyệt không hiểu cũng bị bỏ qua.
Tuy nhiên trình duyệt sẽ xem nội dung của các thẻ mà nó không nhận ra là dạng văn bản thông thường và trình duyệt sẽ hiển thị nội dung ra giao diện.<br>
Phần chú thích (comment) sẽ bị bỏ qua, không hiển thị.<br>
<b>Văn bản là gì?</b><br>
Văn bản (text) là những thứ có thể đọc được. Văn bản chính là tập hợp các kí tự (letter) hoặc các từ (word) có ngữ nghĩa.<br>
Trong thông tin và truyền thông, văn bản là từ, là câu, là đoạn, không bao gồm thông tin định dạng và được lưu dưới dạng mã ASCII (để máy tính có thể hiểu và xử lý được).<br>
Những thứ không phải là văn bản bao gồm: các đối tượng đồ họa (graphic), các số (không ở dạng ASCII), và mã chương trình (dạng nhị phân).<br>
### 1.1.3 Cấu trúc cơ bản của một tài liệu HTML
<b>Phần tử HTML</b><br>
Phần tử HTML (HTML element) là một thùng chứa (container), nó được sử dụng để chứa văn bản, và chứa các phần tử HTML khác.<br>
Thùng chứa được tạo ra bằng cách dùng các thẻ HTML. Tên của thẻ sẽ quy định nội dung chứa bên trong mang ý nghĩa gì khi hiển thị.<br>
<b>Thẻ HTML</b><br>
Thẻ HTML (HTML tag) là các từ khóa (keyword), được sử dụng để báo cho trình duyệt biết cách định dạng và hiển thị các nội dung.
Trình duyệt sẽ không hiển thị các từ khóa này ra ngoài giao diện.<br>
<i>Thẻ HTML thường gồm 2 phần:</i><br>
Phần mở thẻ gọi là thẻ mở (opening tag, start tag).<br>
Phần đóng thẻ gọi là thẻ đóng (closing tag, end tag).<br>
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg387_FiMuzl_43ZYdvKCcEjstmarc22ifjVBMwmp761lOsO-ESTVu6SKNpjFaTC5zCJPOvaX8xdfdYT-3rC7AWpnfuvWDJ6tYnRbPWkhPmDLjZvuBdmIMj9E8aDRfMyD9mmWxVk1lgYGs/s698/html1.jpg)<br>
Cũng có thể hiểu nôm na, HTML sẽ sử dụng các thẻ (tag) để “đánh dấu” chỗ này là tiêu đề, chỗ khác là một đoạn văn bản, chỗ này sẽ hiển thị hình ảnh, chỗ khác sẽ hiển thị một video. Đây chính là ý nghĩa của chữ “đánh dấu” (markup) trong khái niệm HTML.<br>
Dưới đây là cú pháp một phần tử HTML thông thường (gọi là phần tử HTML thông thường vì còn có các phần tử HTML đặc biệt).<br>
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgPxwmZ-9lpbVqko8FdwA4w8stYJJKBUCgCqDfGk4Epm5M-YoDVPPn-tzqV6YiOYG95arQDG8EZ0RCKa1_m4Vsqh3lEJ9YyFF99XzqmhssTkXmVgjYA_wTZEWNzdODGT8t4BuEclL_-xOo/w400-h140/html2.jpg)<br>
Như vậy, một phần tử HTML sẽ bắt đầu là thẻ mở, tới phần nội dung, và cuối cùng là thẻ đóng.<br>
Thẻ HTML (HTML tag) và phần tử HTML (HTML element) là hai khái niệm khác nhau.<br>
Tuy nhiên, thẻ HTML là thành phần để tạo ra phần tử HTML.<br>
![]
