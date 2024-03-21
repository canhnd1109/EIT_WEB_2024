#### Cấu trúc 1 file đuôi .html

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <h1>The Main Heading</h1>
    <h2>A catchy subheading</h2>
    <p>First paragraph</p>
  </body>
</html>
```

- `<!DOCTYPE html>`: khai báo kiểu dữ liệu hiển thị
- `<html> và </html>`: cặp thẻ bắt buộc, element cấp cao nhất, có nhiệm vụ đóng gói tất cả nội dung của trang HTML
- `<head> và </head>`: khai báo các thông tin meta của trang web như: tiêu đề trang, charset
- `<title> và </title>`: cặp thẻ nằm bên trong thẻ `<head>`, dùng để khai báo tiêu đề của trang
- `<body> và </body>`: cặp thẻ dùng để đóng gói tất cả các nội dung sẽ hiển thị trên trang
- `<h1></h1>, <h2></h2>`: định dạng dữ liệu dạng heading. Thông thường có 6 cấp độ heading trong HTML, trải dài từ `<h1>` tới `<h6>`. Trong đó, `<h1>` là cấp độ heading cao nhất và `<h6>` là cấp độ heading thấp nhất.
- `<p> và </p>`: cặp thẻ chứa các đoạn văn bản của trang web

#### Các tag cơ bản thông dụng của HTML

1. HTML Headings

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

_Lưu ý: một page chỉ có một thẻ h1_

2. HTML Paragraphs

- p: Hiển thị đoạn văn bản
- hr: Là 1 tag rỗng, không có end tag, dùng để hiển thị 1 đoạn line ngăn cách
- br: Là 1 tag rỗng, không có end tag, dùng để xuống dòng trong cùng 1 đoạn văn bản mà không cần phải thêm nhiều tag.

3. HTML Text Formatting

```html
<b>Chữ này in đậm</b>
<i>Chữ này bị nghiên</i>
<p>Chữ này bị<sub>thụt xuống</sub> và <sup>thụt lên</sup></p>
<u>Chữ này gạch chân</u>
```

4. HTML Links

```html
<a href="url">Liên kết</a>
```

5. HTML Images

```html
<img src="https://picsum.photos/100/100" alt="Some random image" />
```

6. HTML Tables

```html
<table style="width:100%">
  <caption>
    Monthly savings
  </caption>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$50</td>
    </tr>
  </tbody>
  <tfoot>
    <tr style="background-color: #FFE4B5">
      <td><b>Total: </b></td>
      <td style="color: red"><b>$150</b></td>
    </tr>
  </tfoot>
</table>
```

![enter image description here](https://images.viblo.asia/1a460544-c9e6-4eba-a07c-935f5e6cbc90.png)

Ngoài các tags hay sử dụng trong table như: `<table>, <tr>, <th>, <td>, <thead>, <tbody>, <tfoot>` thì còn 3 tags nữa ít sử dụng hơn.

- `<caption>`: Hiển thị cation của table.
- `<colgroup>`: Được sử dụng để định dạng cho một nhóm cột trong <table>.
- `<col>`: Được sử dụng để xác định giá trị thuộc tính cho một hoặc nhiều cột trong `<table>`
- CSS **border-collapse**: Thuộc tính thu gọn lại border cho các cell trong table. Thường được set default là 0.
- CSS **border-spacing:** Thuộc tính dùng để set các khoảng cách giữa các cell trong table. Thường được set default là 0.
- Attr **colspan**: Gộp nhiều cột lại với nhau.
- Attr **rowspan**: Gộp nhiều dòng lại với nhau.
  <br>

7. HTML Lists

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

| **unordered `<ul>`** | **ordered `<ol>`** |
| -------------------- | ------------------ |
| list-style-type      | type               |
| disc                 | 1                  |
| circle               | A                  |
| square               | a                  |
| none                 | I                  |
|                      | i                  |

#### Semantic element là gì?

- Semantic element là những phần tử mô tả rõ ràng ý nghĩa về cấu trúc của phần tử đó nghĩa là chỉ cần đọc tên các element này là chúng ta có thể hiểu được nội dung bên trong element này nói về cái gì.

![enter image description here](https://images.viblo.asia/170fc35c-3c55-44ec-baca-286f16e463ed.gif)

- Element `<nav>`: Xác định một khu vực chứa các link điều hướng

```html
<nav>
  <a href="/html/">HTML</a> | <a href="/css/">CSS</a> |
  <a href="/js/">JavaScript</a> |
  <a href="/jquery/">jQuery</a>
</nav>
```

- Element `<section>`:gồm các nội dung có cùng chủ đề.

```html
<section>
  <h2>Giới thiệu Framgia</h2>
  <p>
    Được thành lập vào tháng 10/2012, tại Hà Nội đến nay Framgia đã có ba chi
    nhánh tại Hà Nội, Đà Nẵng và TP. HCM và có mặt tại 5 quốc gia tại châu Á với
    gần 1000 nhân viên từ nhiều quốc gia trên thế giới như: Nhật Bản,
    Bangladesh, Cambodia, Nigeria, Kazakstan. Đạt tốc độ phát triển vượt bậc, từ
    khởi đầu chỉ với 5 thành viên, sau 5 năm Framgia Inc. đã trở thành là tập
    đoàn Offshore IT của Nhật Bản lớn nhất tại Việt Nam.
  </p>
</section>

<section>
  <h2>Sứ mệnh của Framgia</h2>
  <p>
    Với lý tưởng chung tay xây dựng nên một tương lai tốt đẹp và tươi sáng, sứ
    mệnh của Framgia là luôn cố gắng tạo ra những trải nghiệm thú vị khiến người
    ta phải thốt lên rằng “Awesome!” (Thật tuyệt vời), hoặc “Wow” hay “Crazy”
    (Thật không thể tin được)
  </p>
</section>
```

-Element `<article>`:được sử dụng cho các nội dung độc lập

```html
<article>
  <h2>Google Chrome</h2>
  <p>
    Google Chrome is a web browser developed by Google, released in 2008. Chrome
    is the world's most popular web browser today!
  </p>
</article>

<article>
  <h2>Mozilla Firefox</h2>
  <p>
    Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox
    has been the second most popular web browser since January, 2018.
  </p>
</article>

<article>
  <h2>Microsoft Edge</h2>
  <p>
    Microsoft Edge is a web browser developed by Microsoft, released in 2015.
    Microsoft Edge replaced Internet Explorer.
  </p>
</article>
```

-Element `<aside>`: Xác định nội dung nằm bên cạnh nội dung của trang

```html
<p>
  My family and I visited The Epcot center this summer. The weather was nice,
  and Epcot was amazing! I had a great summer together with my family!
</p>

<aside>
  <h4>Epcot Center</h4>
  <p>
    Epcot is a theme park at Walt Disney World Resort featuring exciting
    attractions, international pavilions, award-winning fireworks and seasonal
    special events.
  </p>
</aside>
```
