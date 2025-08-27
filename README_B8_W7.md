# Web front-end (7)

## 1.1 Bố cục một trang web

Cấu trúc cơ bản của một tài liệu HTML gồm các phần tử html, head, title và body. Trong đó, phần tử body chứa toàn bộ nội dung sẽ hiển thị ra màn hình, đó là phần nội dung các trang web. Trang web ở dạng mã nguồn được gọi là tài liệu HTML.

Nội dung của trang web rất đa dạng.

*Ví dụ:* có thể là một tờ báo, trang blog, trang thông tin của một công ty, giao diện game, các sản phẩm của một cửa hàng.

Phần này sẽ tập trung tìm hiểu cách tạo ra một trang web có bố cục cơ bản nhất. Dựa trên đó, bạn có thể tùy chỉnh cho từng trang web cụ thể.

### 1.1.1 Các phần tử tạo bố cục trang web

Trước khi HTML5 ra đời, để nhóm (grouping) các phần tử lại với nhau, nhằm tạo các vùng lớn hơn của một trang web, người ta thường sử dụng phần tử div.

Tuy nhiên, HTML5 đã cung cấp hàng loạt các phần tử, với ngữ nghĩa rõ ràng hơn, để chia (sectioning) nội dung thành các vùng (section) riêng biệt, phần này sẽ tìm hiểu các phần tử như: main, header, footer, section, article, nav, aside, address.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhvRI5MjxTNai5QbSWL9LygHK7iwmMjC2TCiqw9Aftd0GWhgXy_IEJB3E0dIDB8_eUS-o2XLx8tFXZB79dkq9O1f1sGveVGsxSSVTX5z8N4gR46we92H4acFeqH5UulKFPTAzmjO3VqaqJc3CeSCgkFBLdoihTQOM4xTYuIdEoKIZePDQMxBUNfv77L/w400-h289/Nhom_1.jpg)

Để dễ hiểu về các phần tử tạo bố cục trang web, phần này minh họa theo một bố cục hay cấu trúc (layout) của một trang web phổ biến. Trang web này được chia thành các vùng: Main content, Header, Sidebars, Footer.

![image](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEizFAgO9XDyiDeCFbkqffIdeXYXuKFaYnQEyfc1uLny5FX8oyr9mz4HrI839Dx-HN1PzT6zjBblem4ZCbnjkRriX1qR0egSNNu1dyw-Hmh1lW4fxwr6HH-Pg0BHsfYrHuciHjGILhOIxQWW-Qxosj2CnfCFkxFDmK4Jewif7cZQnZfkgkpXRX1KxnDX/w400-h353/Nhom2.jpg)

**Vùng nội dung chính (main content)**

Trong một website, nội dung các vùng tiêu đề (masthead, header), khung nội dung bổ trợ (sidebar), vùng quảng cáo (ads), và vùng cuối/chân trang (footer) thường xuất hiện nhiều lần, trong nhiều trang web (web page).

*Riêng vùng nội dung chính (main) chỉ xuất hiện một lần.*

Trong HTML, sử dụng phần tử main để tạo vùng Main.

Các phần tử header, sidebar, và các phần tử xuất hiện ở nhiều trang, thì không nên để trong phần tử main.

Phần tử main không nên lồng trong các phần tử article, aside, header, footer và nav.

**Phần đầu và phần chân (headers và footers)**

Đây là hai phần tử được đặt ở đầu và cuối của một vùng nội dung, nhằm tạo ra cấu trúc rõ ràng cho vùng nội dung đó.

**Phần đầu (headers)**

Phần tử header thường dùng để chứa nội dung giới thiệu, tuy nhiên, trong thực tế nó có thể chứa mọi thứ, miễn là liên quan đến mục đích giới thiệu.

*Ví dụ:* logo, tiêu đề, khẩu hiệu, thanh điều hướng. Phần tử này thường được đặt ở đầu của trang web, hoặc phía trên cùng của một vùng (section) hoặc một bài viết (article).

*Ví dụ:* sử dụng phần tử header để chứa logo, tiêu đề của trang web và thanh điều hướng.

```html
<header>
            <img src="/images/logo.png">
            <h1>Trang blog của Tèo</h1>
            <nav>
                        <ul>
                                    <li><a href="">Home</a></li>
                                    <li><a href="">Blog</a></li>
                                    <li><a href="">About</a></li>
                        </ul>
            </nav>
</header>
```

Trong một article, phần tử header thường được dùng để chứa: tiêu đề, tác giả, và ngày xuất bản của bài viết.

```html
<article>
            <header>
                        <h1>Tiêu đề bài viết</h1>
                        <p>người viết Nguyễn Văn Tèo</p>
                        <p>ngày xuất bản: 11/11/2022</p>
            </header>
            <p>...phần nội dung bài viết…</p>
</article>
```

**Phần chân (footers)**

Phần tử footer dùng để chứa các thông tin ở cuối một trang web, cuối một vùng (section) hoặc cuối một bài viết (article).

Phần tử footer thường chứa tên tác giả, thông tin bản quyền (copyright), các tài liệu liên quan, hoặc các điều hướng (navigation).

Phần tử footer đặt ở cuối trang thì sẽ là thông tin kết thúc của toàn trang.

Nó cũng có thể được đặt ở cuối một section, article, nav, hoặc aside và sẽ là thông tin kết thúc của chính phần tử chứa nó. 

*Ví dụ:* phần chân của một bài viết trên blog.

```html
<article>
            <header>
                        <h1>Tiêu đề bài viết</h1>
                        <p>người viết Nguyễn Văn Tèo</p>
                        <p>ngày xuất bản: 11/11/2018</p>
            </header>
            <p>...phần nội dung bài viết…</p>
            <footer>
                        <p><small>Copyright &copy;2018 Tèo.</small></p>
                        <nav>
                                    <ul>
                                                <li><a href="">Previous</a></li>
                                                <li><a href="">Next</a></li>
                                    </ul>
                        </nav>
            </footer>
</article>
```

**Phân vùng (section)**

Với một tài liệu dài, bạn nên chia nhỏ nó ra thành nhiều phần thì sẽ dễ hiển thị và dễ đọc hơn.

