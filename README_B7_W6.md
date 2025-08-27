# Web front-end (6)

## 1.1 Hiển thị văn bản

Để hiển thị văn bản, bạn cần biết cách sử dụng phần tử HTML phù hợp (đặc biệt là về mặt ngữ nghĩa của phần tử) 
để hiển thị các đoạn văn bản, các đề mục, các danh sách, các kí tự đặc biệt, tổ chức trang nội dung.

Việc sử dụng phần tử một cách hợp lý sẽ giúp trang web có thứ hạng cao trong kết quả của các trang tìm kiếm (ví dụ google),
được nhiều người biết đến, và các phần mềm phân tích nội dung có thể tự động phân tích trang web với độ chính xác cao.

**Phần này sẽ đề cập đến các nội dung:**

– Đoạn văn bản và đề mục

– Danh sách

– Một số phần tử hiển thị nội dung khác

### 1.1.1 Đoạn văn bản và đề mục

**Đoạn văn bản**

đoạn văn bản (gọi tắt là đoạn) là tập hợp của nhiều câu, toàn bộ văn bản chính là tập hợp của các đoạn. Trong HTML,
đoạn là một chuỗi các từ có chiều dài bất kì. Để tạo một đoạn, sử dụng phần tử p, đây là phần tử cơ bản nhất
trong việc hiển thị văn bản. Chữ p là viết tắt của paragraph.

**Lưu ý:** tất cả nội dung văn bản đều phải được bọc lại bằng các phần tử, nếu không, phần văn bản đó sẽ không có ngữ nghĩa và 
người lập trình sẽ không thể kiểm soát được việc hiển thị.

Ở chế độ mặc định, phần tử p được hiển thị theo kiểu khối (block). Nghĩa là, nó sẽ luôn được hiển thị ở một hàng mới và sẽ 
chiếm toàn bộ chiều rộng khả dụng.

Phần tử p ngoài việc chứa văn bản (text), nó còn có thể chứa hình ảnh, các phần tử nội tuyến (inline); tuy nhiên,
nó không thể chứa phần tử đề mục (heading), danh sách (list), phân vùng (sectioning), và các phần tử kiểu khối khác.

**Đề mục**

Một văn bản không chỉ có các đoạn, hình ảnh, mà còn có hệ thống đề mục (hay hệ thống tiêu đề).

Đề mục (heading) là một từ, cụm từ, hoặc kí hiệu, giúp người đọc có thể tìm kiếm và định vị được thông tin.

Hệ thống đề mục thường gồm nhiều cấp khác nhau, thể hiện cấu trúc, bố cục, hay bộ khung (outline) của một văn bản. 
Để dễ hiểu, hãy liên tưởng tới hệ thống heading trong Microsoft Word.

Để tạo đề mục, có thể sử dụng các phần tử: h1, h2, h3, h4, h5, h6. Đây là sáu loại đề mục khác nhau. 
Trong đó, phần tử h1 sẽ tạo ra đề mục mức cao nhất (heading level 1 – đề mục mức 1), h2 sẽ tạo ra đề mục mức 2, h3 
sẽ tạo ra đề mục mức 3…

Khi có các đề mục, trình duyệt sẽ sử dụng chúng để tạo ra bố cục cho văn bản.

Phần mềm đọc văn bản tự động (screen reader) sẽ dựa vào các đề mục để tóm tắt nội dung và dễ dàng duyệt qua toàn bộ văn bản.
Các công cụ tìm kiếm cũng sử dụng hệ thống đề mục trong thuật toán tìm kiếm của chúng, các đề mục mức cao hơn sẽ có trọng số lớn hơn.

**Đánh đấu kết thúc chủ đề**

Để đánh dấu kết thúc một chủ đề/ý tưởng và chuyển sang chủ đề/ý tưởng khác, sử dụng phần tử hr, phần tử này sẽ tạo một đường 
kẻ ngang (horizontal rule) giữa hai chủ đề/ý tưởng.

Nếu bạn chỉ muốn tạo một đường kẻ ngang trên trang web thì bạn sẽ dùng border trong CSS chứ không nên sử dụng phần tử hr.

### 1.1.2 Danh sách

Trong khi trình bày một văn bản, bạn rất hay gặp phải tình huống cần phải liệt kê hàng loạt các đối tượng.

**HTML cung cấp ba loại danh sách:**

– Danh sách không có thứ tự (unordered list)

– Danh sách có thứ tự (ordered list)

– Danh sách mô tả (description list)

Mặc định, phần tử danh sách được hiển thị theo kiểu khối (block), tuy nhiên, có thể thay đổi kiểu hiển thị bằng CSS.

**Danh sách không có thứ tự**

Danh sách không có thứ tự là một dãy các mục (item), trong đó tính trước sau của mỗi mục là không quan trọng.

Mỗi mục thường được trình duyệt đánh dấu bằng một kí tự đầu dòng (dấu đầu dòng) (bullet). Trong thực tế, phần lớn các danh sách sẽ thuộc loại này.

Để tạo danh sách không có thứ tự, sử dụng phần tử ul, viết tắt của unordered list (danh sách không có thứ tự).

Để tạo mỗi mục của danh sách, sử dụng phần tử li, viết tắt của list item (mục của danh sách).

**Cú pháp là**
```html
<ul>

            <li>phần tử 1</li>

            <li>phần tử 2</li>

</ul>
```

Mặc định, mỗi mục sẽ được trình duyệt đánh dấu bằng dấu chấm tròn (trên mã nguồn thì không xuất hiện các dấu này), 
nếu muốn thay bằng dấu khác cần sử dụng CSS.

**Chú ý:** sau thẻ mở <ul> phải là một hoặc nhiều phần tử li, chứ không cho phép chèn văn bản hoặc các phần tử khác, 
tuy nhiên, trong phần tử li thì có thể chứa văn bản hoặc các phần tử bất kì. Ví dụ, đoạn mã dưới đây là không hợp lệ.

**danh sách có thứ tự**

Danh sách có thứ tự là một dãy các mục, trong đó tính trước sau của mỗi mục là quan trọng, 
ví dụ, danh sách các bước hướng dẫn để làm một công việc.

 Để thể hiện tính thứ tự của các mục, trình duyệt sẽ tự động sử dụng các số hoặc các chữ cái để gắn vào phía trước mỗi mục,
 giá trị của các số/chữ sẽ được tự động tăng cùng với các mục.

Để tạo danh sách có thứ tự, sử dụng phần tử ol, viết tắt của ordered list (danh sách có thứ tự).

Để tạo mỗi mục của danh sách, sử dụng phần tử li, viết tắt của list item (phần tử của danh sách).

**Cú pháp là**

<ol>

            <li>phần tử 1</li>

            <li>phần tử 2</li>

</ol>

Để ý là, mặc dù trong đoạn mã HTML không ghi các số 1, 2, 3, nhưng khi hiển thị ra màn hình lại thấy có các số. 
Như đã nói ở trên, trình duyệt đã tự đánh số thứ tự cho mỗi mục trong thẻ <ol>. Nếu không muốn đánh số thứ tự là 1, 2, 3,
mà muốn là a, b, c, hoặc I, II, III, thì sử dụng CSS.

Sau thẻ mở <ol> phải là một hoặc nhiều phần tử li, không cho phép chèn văn bản hoặc các phần tử khác, tuy nhiên,
trong phần tử li thì có thể chèn văn bản hoặc các phần tử bất kì trong đó.

Với danh sách có thứ tự, giá trị bắt đầu luôn là 1, I, i, A hoặc a. Để thay đổi giá trị bắt đầu, sử dụng thuộc tính start.

```html
<ol start="gia_tri_thay_doi">
```

| HTML   | Kết quả |
| -------- | ------- |
| ```html <ol type="i" start="4"> ```| Danh sách sẽ được đánh số bắt đầu từ iv   |
| ```html <ol type="I" start="4"> ```| Danh sách sẽ được đánh số bắt đầu từ IV   |
| ```html <ol type="A" start="4"> ```| Danh sách sẽ được đánh thứ tự từ chữ D    |
| ```html <ol type="a" start="4"> ```| Danh sách sẽ được đánh thứ tự từ chữ d    |

