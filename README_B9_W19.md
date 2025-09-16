# TỔNG QUAN VỀ FORM

## 1.1 Form

Form (biểu mẫu) chính là đối tượng được sử dụng để xử lý các tương tác giữa người dùng và trang web. Từ trang web tĩnh, 
nhờ có form, người lập trình có thể tạo ra trang web động hay ứng dụng web. HTML5 cung cấp rất nhiều các điều khiển (control), 
các thuộc tính mới, giúp người lập trình dễ dàng tạo ra các giao diện tương tác, và tạo thuận lợi cho người dùng trong việc 
nhập thông tin và thực hiện các giao dịch trên web.

### 1.1.1 Tổng quan về form

**Form làm việc thế nào?**

Hoạt động của form gồm hai phần: phần hiển thị và phần xử lý.

Phần hiển thị là những gì người dùng nhìn thấy ở trên giao diện trang web, phần này được tạo ra bằng các phần tử HTML.

- Form thường chứa các nút (button), các trường nhập liệu (input field), các mục xổ chọn (drop-down menu), 
gọi chung là các điều khiển (form control).
- Form sử dụng các điều khiển để lấy thông tin từ người dùng.
- Form cũng có thể chứa văn bản (text) và các phần tử khác.
- Trình duyệt có nhiệm vụ tập hợp các thông tin người dùng đã nhập, đóng gói và gửi về phía web server để xử lý.

Phần xử lý là một chương trình/ứng dụng hoặc đoạn mã xử lý (script) đặt tại máy web server, nó sẽ xử lý các thông tin thu được 
từ người dùng và trả về kết quả tương ứng. Phần này chúng ta sẽ tìm hiểu trong phần lập trình phía back-end.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEho50z1PB5vzXirF4r-F3kjFaqibpRi811x9hwcYthgcqS1oAcHC4_kB4OVTYJ9jx7QWh4-0RkiGlG11jBeo4hrxdVnBQlVlGOuqbzLz4S80dLb3mn-k87gOJO431jYXNw7xYwBGJ65Ygdliee79ZKmqeTo5NhqyNuDwzMjKslpV9towFANXMmn-LVE/w400-h255/formHTML.jpg)

| Mã hoá dữ liệu của form |
|-------------------------|
| Dữ liệu của form sẽ được mã hóa tương tự như mã hóa URL, nghĩa là các khoảng trắng và các kí tự không được phép gửi trực tiếp về server sẽ được chuyển sang dạng giá trị hệ 16 (hexadecimal) tương ứng. |
| Ví dụ, khoảng trắng sẽ được chuyển thành %20, dấu xuyệt (/) sẽ là %2F. Lập trình viên không cần quan tâm tới việc mã hóa này, vì trình duyệt sẽ thực hiện tự động. |

**Phần tử form**

Phần tử form chứa toàn bộ nội dung của form, bao gồm: các điều khiển (form control) như các ô nhập liệu, các nút; các phần tử khối (block element) như h1, p, danh sách. Phần tử form không thể chứa phần tử form khác, hay nói cách khác không được lồng form.

VD:
``html
<!DOCTYPE html>

<html>

 

<head>

            <meta charset="utf-8">

            <title>Đăng ký nhận tin</title>

</head>

 

<body>

  <h1>Đăng ký nhận tin</h1>

  <form action="/dang-ky.php" method="post">

    <fieldset>

      <legend>Gửi thông tin của bạn cho chúng tôi</legend>

      <p>Đăng ký để nhận được các thông tin định kì về giá nông sản</p>

      <ol>

        <li><label for="ho-ten">Tên:</label>

          <input type="text" name="ten" id="ho-ten"></li>

        <li><label for="email">Email:</label>

          <input type="text" name="email" id="email"></li>

      </ol>

      <input type="submit" value="Đăng ký">

    </fieldset>

  </form>

</body>

</html>
```


Ngoài vai trò là thùng chứa các control, để giao tiếp/làm việc với ứng dụng web tại server, form còn có thêm một số thuộc tính đi kèm.

**Thuộc tính action**

Thuộc tính action cho biết địa chỉ (URL) của ứng dụng/chương trình hoặc đoạn mã (tại máy web server) sẽ xử lý thông tin do form gửi về. 

Phần mở rộng của tập tin là .php cho biết: ứng dụng trên web server để xử lý form được viết bằng ngôn ngữ PHP. Người lập trình có thể sử dụng một trong các ngôn ngữ sau để viết các đoạn mã xử lý tại web server.

VD:
– PHP
– C#
– Python
– Golang
– JavaScript
– Java
– Ruby

