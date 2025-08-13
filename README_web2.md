# Web front-end(2)
## Trình duyệt web là gì?
### Trình duyệt web là gì?
Trình duyệt web (web browser) là một phần mềm, được dùn để truy cập thông tin web. Mỗi một tài nguyên web đều có một URL tương ứng, trình duyệt sẽ dựa theo các URL này để tải nội dung về và hiển thị cho người dùng.<br>
Do web hoạt động theo kiến trúc client-server, nên thông tin web được đặt tại các server, trình duyệt sẽ yêu cầu thông tin từ một server cụ thể. Khi nhận được yêu cầu server sẽ xử lý yêu cầu và gửi lại kết quả để giển thị lên trình duyệt.<br>
Trình duyệt gồm nhiều thành phần như: User interface, Browser engine, Rendering engine, Networking, JavaScript Interpreter, UI Backend, Data Presistence.<br>
![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhGbsyU4i4beoEHqCJy0awFe9qXy8jWfJQVQppdGNY8mSHjvjhxZ_YTZQj1o91hv7ICAXbs_lVq_EZzaevB93XXgiF2XN1jyTH1GtFIWqmE57HtV_D0hezuCTVXSyGcei654Z8OIPsKpQY/w400-h291/Cac+thanh+phan+cua+browser.jpg)
<b>Trong đó:</b>
- User interface(UI): là toàn bộ giao diện của trình duyệt (menu, thanh địa chỉ, các nút, thanh trạng thái), trừ phần cửa sổ chứa nội dung trang web.<br>
- Rendering engine(RE): Phân tích mã HTML, CSS để hiển thị nội dung ra cửa sổ.<br>
- Browser engine(BE): ghép nối, điều phối hoạt động giữa UI và RE, BE nhận lệnh từ UI gửi cho RE thực thi.<br>
- Networking: thực hiện các giao tiếp mạng, truyền dữ liệu giữa trình duyệt và máy tính.<br>
- JavaScript Interpreter(JI): phân tích và thực thi mã JavaScript.<br>
- UI Backend: Thực hiện vẽ các đối tượng cơ bản.<br>
- Data Presistence: thực hiện các công việc liên quan đến lưu trữ dữ liệu trên đám mây cục bộ.<br>
### Xử dụng trình duyệt web để duyệt web
Trình duyệt gồm hai khu vực:
- Vùng 1: là giao diện của trình duyệt.
- Vùng 2: là giao diện của trang web hay ứng dụng web.
  ![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhKXGZHbx4eyWAAAUpNmxEWZ6gwpBeg3FssuapfCYqGHq4rYVpLWCOV-pRo3pjYuMJXkZwggvT6hbwwugubYj4s4oj5IzSj3gF1_cIJX4lPI2wD2oqwTlAZthHF60JPni_8bpd5-tDeqVY/w400-h230/3+Giao+dien+trinh+duyet.jpg)
### Giao diện của trình duyệt
- Giao diện thường bao gồm: các tab, thanh địa chỉ, các nút điều khiển, menu, thanh trạng thái, thanh cuộn.<br>
+ Người dùng thường có nhu cầu mở nhiều trang web, mỗi trang web sẽ nằm trên một tab.<br>
+ Sau khi mở tab mới, người dùng sẽ nhập địa chỉ trang web vào thanh địa chỉ.<br>
+ Thanh trạng thái(status bar): hiển thị URL khi người dùng rê chuột lên các liên kết của trang web, hoặc hiển thị thông báo khi trang web đang được tải về.<br>
+ Nút điều khiển, dùng để tải lại trang web hiện tại (reload), trở về trang mặc định (home page), trở về trang trước (go back), đi tới trang sau (go forward),...<br>
+ Menu: chứa chức năng cho phép người dùng thiết lập chế đô hiển thị, ngôn ngữ, bảo mật, cài thêm chức năng mở rộng, mở bộ công cụ cho lập trình viên,...<br>
+ Thanh cuộn: cho phép cuộn ngang/dọc để xem các phần thông tin chưa hiển thị hết trong khung.<br>
### Giao diện trang web
Giao diện của trang web, hay của ứng dụng web là phần nội dung được trình duyệt lấy từ server về và hiển thị cho người dùng. Nó chính là trang tin, trang thương mại điện tử hoặc các ứng dụng web khác, mà người sở hữu trang web muốn gửi tới người dùng và khách hàng của họ.<br>
### Sử dụng trình duyệt trong quá trình tạo ra trang web
Để tạo ra trang web, lập trình viên thường sử dụng các trình viết mã (text editor, code editor) hoặc môi trường phát triển tích hợp (IDE). Tuy nhiên, trong quá trình tạo ra trang web, lập trình viên cũng có thể kết hợp thêm một số tiện ích của trình duyệt để thiết kế giao diện, kiểm tra và sửa lỗi, xem trước kết quả.<br>
### Quá trình hiển thị trang web của trình duyệt
