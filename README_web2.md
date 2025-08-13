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
