# FORM CONTROLS

## 1.1.1 Các control phổ biến

**Control nhập văn bản**

Một trong những công việc phổ biến nhất khi người dùng làm việc với web form là nhập thông tin dạng văn bản. 
Người dùng có thể nhập thông tin trong một hàng hoặc nhiều hàng.

**Nhập thông tin trong một hàng**

Để người dùng có thể nhập thông tin trong một hàng, chúng ta sử dụng control có tên là input với thuộc tính type=“text”, 
đây là thuộc tính mặc định cho control input, nghĩa là nếu bỏ qua thuộc tính type=“text” thì control input sẽ cho phép 
người dùng nhập thông tin trong một hàng.

VD:

```html
<label>Tỉnh/Thành phố: <input type="text" name="city" id="form-city"

value="Đà Lạt" maxlength="50"></label>
```

- name: là thuộc tính bắt buộc phải có, chứa tên của biến (city)
- value: là thuộc tính chứa nội dung văn bản sẽ được thiết lập mặc định khi form được hiển thị, hoặc sau khi reset form (Đà Lạt)
- maxlength: mặc định, control này cho phép người dùng nhập số kí tự không giới hạn, tuy nhiên, lập trình viên có thế giới hạn
số lượng kí tự được phép nhập bằng thuộc tính maxlength(50).
- Phần tử label: khi bọc input bằng phần tử label, người dùng chỉ cần bấm chuột vào nội dung của phần tử label
là trường nhập liệu của input sẽ được kích hoạt/có dấu nháy chuột, sẵn sàng để người dùng nhập dữ liệu.

**Nhập thông tin gồm nhiều hàng**

Nếu người dùng cần nhập thông tin gồm nhiều hàng dữ liệu, thì chúng ta sử dụng control textarea. Khác với phần tử input, 
phần tử textarea cho phép đặt nội dung giữa thẻ mở và thẻ đóng, phần nội dung này sẽ được hiển thị trong trường nhập văn bản 
và được gửi về web server nếu người dùng gửi form (submit), vì vậy nên cẩn thận về điều này. Thực tế, các lập trình viên 
thường để trống phần nội dung, và chỉ hiển thị thông tin gợi ý bằng thuộc tính title hoặc placeholder.

VD: control textarea có nội dung giữa thẻ mở và thẻ đóng

```html
<form action="" method="get">

    <p><label>Nhận xét của bạn về cuốn sách:<br>

      <em>Cho chúng tôi biết cảm nhận của bạn về cuốn sách này, đây sẽ là những thông tin rất có ích đối với Nhà xuất bản, tác giả và các độc giả khác</em><br>

      <textarea name="nhan-xet" cols="30" rows="10">Cuốn sách rất có ích cho sinh viên</textarea></label></p>

</form>
```

VD: control textarea có sử dụng thuộc tính placeholder

```html
<form action="" method="get">

      <p><label>Nhận xét của bạn về cuốn sách:<br>

      <em>Cho chúng tôi biết cảm nhận của bạn về cuốn sách này, đây sẽ là những thông tin rất có ích đối với Nhà xuất bản, tác giả và các độc giả khác</em><br>

      <textarea name="nhan-xet" cols="30" rows="10" placeholder="Nhận xét không quá 50 từ"></textarea></label></p>

</form>
```

Hai thuộc tính rows và cols được sử dụng để xác định kích thước cho trường nhập văn bản, rows là số hàng, cols là độ rộng. 
Thực tế, chúng ta nên sử dụng CSS để thiết lập các thuộc tính này.

| **Thuộc tính disabled và readonly** |
|---------------------------------|
| Đây là hai thuộc tính có thể thêm vào mọi control, mục đích là không cho người dùng thao tác với control đó. |
| Với thuộc tính disabled, người dùng không thể chọn control, thường thì control sẽ có màu xám (có thể thay đổi bằng CSS). Có thể thay đổi giá trị của thuộc tính này bằng đoạn mã (script). Thuộc tính này rất hữu dụng khi muốn hạn chế người dùng truy cập một số control tùy vào lựa chọn trước đó của họ. |
| Thuộc tính readonly không cho phép người dùng thay đổi giá trị hiện có của control (mặc dù người dùng vẫn chọn được). Thuộc tính này rất hữu dụng khi muốn sử dụng đoạn mã để tự động thiết lập giá trị cho control dựa trên các lựa chọn trước đó của họ. |

**Nhập thông tin đặc thù**

Bên cạnh control cho phép nhập thông tin trên một hàng thông thường, với phần tử input và thuộc tính type=“text”, 
HTML còn cung cấp một số control cho phép nhập các thông tin có tính đặc thù, như: mật khẩu (password), từ khóa tìm kiếm 
(search terms), địa chỉ email (email addresses), số điện thoại (telephone number) và các URL.

- Nhập mật khẩu

```html <input type=“password”> ```

Trường nhập mật khẩu làm việc giống như một trường nhập văn bản thông thường, chỉ khác là nội dung nhập vào bị che 
bằng các kí tự thay thế như: dấu hoa thị (*) (asterisk), dấu đầu dòng (bulltet), hoặc một kí tự đại diện bất kỳ.

Tuy nhiên, cần để ý là: mặc dù người dùng không thể nhìn thấy các kí tự vừa nhập, nhưng nội dung nhập vào vẫn chưa được mã hóa,
chỉ cần mở mã nguồn là có thể thấy được mật khẩu vừa nhập. Vì vậy, cần phải thực hiện mã hóa mật khẩu để đảm bảo an toàn.

VD: 

```html
<label for="form-mat-khau">Mật khẩu:</label>

<input type="password" name="mat-khau" maxlength="8" id="form-mat-khau">
```

- Một số control đặc thù khác

Trước khi HTML5 ra đời, để nhập: từ khóa tìm kiếm, địa chỉ email, số điện thoại và các URL, chỉ có một cách là 
sử dụng control input với type=“text”, tuy nhiên, HTML5 đã cung cấp các công cụ có tính chuyên biệt, nhằm giúp cho việc 
lập trình được thuận tiện hơn. Các loại input này đều được hiển thị trên một hàng, đều có các thuộc tính giống như 
một input thông thường, như: name, maxlength, size, value.

Với mỗi loại input, trình duyệt sẽ cung cấp thêm chức năng kiểm tra dữ liệu, hoặc thêm các đặc tính riêng phù hợp 
với mỗi loại input. Ví dụ, với ô để nhập từ khóa tìm kiếm, khi người dùng nhập kí tự, sẽ tự động xuất hiện biểu tượng (x),
để xóa toàn bộ nội dung vừa nhập; hoặc bàn phím của điện thoại thông minh sẽ có thêm các nút, tùy theo input đang được 
kích hoạt.

Nếu các trình duyệt chưa hỗ trợ HTML5 thì các input này sẽ được tự động chuyển thành một input thông thường và 
mọi thứ vẫn hoạt động bình thường.

| **Tên control** | **Đặc điểm** |
|-----------------|--------------|
|``` <input type="search"> ``` | Dùng để nhập từ khóa để tìm kiếm. Bàn phím của điện thoại thông minh sẽ có thêm nút Search |
|``` <input type="email"> ``` | Dùng để nhập địa chỉ email. Bàn phím của điện thoại thông minh sẽ có thêm nút @ |
|``` <input type="tel"> ``` | Dùng để nhập số điện thoại. Bàn phím của điện thoại thông minh sẽ ở dạng bàn phím số |
|``` <input type="url"> ``` | Dùng để nhập url. Bàn phím của điện thoại thông minh sẽ có thêm phím “.com” |

**Phần tử datalist**

Phần tử datalist cho phép lập trình viên tạo ra một trình đơn xổ xuống gồm các giá trị đã được thiết lập sẵn,
người dùng chỉ việc lựa chọn giá trị phù hợp.

Tuy nhiên, nếu trong trình đơn không có giá trị phù hợp với người dùng thì sao? Giải pháp là kết hợp phần tử 
datalist và phần tử input với type=“text”. 

*Cách làm:*

- Tạo một input với type=“text”
- Tạo một datalist, trong datalist, mỗi mục chọn ứng với một phần tử option
- Trong input, thêm thuộc tính list trỏ tới id của datalist

VD:

```html
<form action="" method="get">

      <label for="form-sach">

        Các cuốn sách bạn đã đọc khi là sinh viên:

        <input type="text" list="sach" id="form-sach">

        <datalist id="sach">

          <option value="Khuyến học"></option>

          <option value="Đúng việc"></option>

          <option value="Khởi hành"></option>

          <option value="Trên đường băng"></option>

          <option value="Nhà giả kim"></option>

        </datalist>

      </label>

  </form>
```

**Các nút**

Có thể chèn vào web form một số loại nút khác nhau, trong đó quan trọng nhất là nút submit. Submit có nghĩa là gửi đi 
hoặc đệ trình. Khi người dùng bấm hoặc chạm vào nút này, toàn bộ dữ liệu của form sẽ được gửi về web server để xử lý.

Nếu muốn thiết lập các control trở về trạng thái khởi tạo của nó thì sử dụng nút reset. Lưu ý, nút reset không phải 
là xóa hết dữ liệu của các control trên form, mà nó đặt lại giá trị mặc định của các control.

Hai nút submit và reset đều được tạo bằng control input, chỉ khác nhau giá trị của thuộc tính type. 
Vì là các nút chức năng nên không có dữ liệu đi kèm, nghĩa là không cần thuộc tính name, tất nhiên, vẫn có thể thêm 
thuộc tính name và giá trị đi kèm.

Cách sử dụng hai nút submit và reset khá đơn giản, chỉ việc đặt vào vị trí thích hợp trên form, tuy nhiên, 
thường hay được đặt ở cuối form. Mặc định, hai nút này sẽ có tên hiển thị là Submit và Reset tương ứng, có thể 
thay đổi tên này bằng thuộc tính value.

VD: hai nút với tên mặc định

```html
<input type="submit">

<input type="reset">
```

VD: hai nút với tên được thiết lập trong thuộc tính value

```html

 <input type="submit" value="Đăng nhập">

 <input type="reset" value="Làm lại">
```

**Lưu ý: **nút reset rất ít được sử dụng. Trong kĩ thuật xử lý form hiện nay, lập trình viên sẽ sử dụng JavaScript 
để kiểm tra tính hợp lệ của dữ liệu ngay khi người dùng nhập vào các control. Nếu có sai sót, người dùng sẽ được cảnh báo 
để sửa lại ngay, chứ không đợi đến khi nhập đầy đủ thông tin của form mới kiểm tra hoặc reset lại tất cả.

Ngoài hai nút trên, cũng có thể chèn vào form ba loại nút sau:

- Nút hình ảnh, nút này có chức năng tương tự như nút submit, chỉ khác là phần hiển thị của nút chính là một hình ảnh, cần thiết lập giá trị của thuộc tính alt cho phù hợp, phòng trường hợp không tải được hình ảnh.

VD: ```html <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">```

- Nút tùy biến, thiết lập thuộc tính của input là type=“button” để tạo ra một nút cho phép tùy biến bằng JavaScript, nút này chưa được thiết lập chức năng cụ thể.
 
VD: ```html   <input type="button" value="Nút bấm">```

- Phần tử button, đây là phần tử giúp tạo nút một cách linh hoạt tương tự như phần tử input, nội dung nằm giữa thẻ <button> và </button> (văn bản hoặc hình ảnh) sẽ được hiển thị trên nút.

VD: ```html <button>Nút bấm</button>```

**Nút Radio và checkbox**

Radio và checkbox là hai control giúp người dùng dễ dàng thực hiện các lựa chọn sẵn có, nó hoạt động giống như một 
công tắc hai trạng thái (chọn/không chọn). Cả hai đều được tạo bằng control input.

Sử dụng nút radio khi chỉ muốn chọn một trong một nhóm các mục chọn, các mục chọn có tính loại trừ (mutually exclusive), 
nghĩa là chọn mục này sẽ loại trừ các mục còn lại (ví dụ: yes hoặc no, có hoặc không, nam hoặc nữ).

Ngược lại với nút radio, nút checkbox được sử dụng để nhóm các mục chọn lại với nhau, nó cho phép người dùng chọn một hoặc
nhiều mục cùng lúc.






