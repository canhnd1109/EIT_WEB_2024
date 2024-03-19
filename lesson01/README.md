# 1. Cài đặt IDE, Extension
- Cài đặt VS Code
- HTML CSS Support
- Live Server
- Auto Close Tag
- Auto Rename Tag
- HTML End Tag Labels

# 2. Giới thiệu Git, Github, cách sử dụng
- Git là một Version Control System giúp quản lý quá trình xây dựng dự án bằng việc lưu lại các phiên bản theo thời gian.
- Github là tên của 1 công ty cung cấp dịch vụ máy chủ repository, mỗi người có thể truy cập vào website này để tạo tài khoản trên đó và tạo ra kho chứa source của riêng mình khi làm việc
- Mô hình hoạt động của Git và Github
![Mô hình hoạt động của Git và Github](git-github.png)
- Tại sao nên sử dụng Git? <br>
Git mang đến nhiều lợi thế cho công việc lập trình
    - Quản lý source code dễ dàng hơn
    - Thuận tiện cho làm việc nhóm, tránh tình trạng xung đột 
    - Dễ dàng trong việc deployment sản phẩm, tạo ấn tượng với nhà tuyển dụng <br>
    ... <br>
- Các khái niệm quan trọng:
    - Repository - Repo:
        - Remote Repo: Nơi lưu trữ dự án ở trên môi trường online và ở đây sẽ là Github
        - Local Repo: Nơi lưu trữ quản lý dự án của Git ở trên máy tính bạn
    - Commit: Lưu trạng thái vào Git <br> 
        Sửa code, thêm file, xóa file, sửa file có thể hiểu là 1 một commit
    - Branch: Là một “nhánh” thông qua “nhánh” đó có thể quản lý nhiều người cùng đồng thời xây dựng một dự án.

- Các lệnh Git cơ bản
```
    git init
    git add
    git pull

    git add / git add .
    git commit -m "Desc"
    git push

    git log
    git status

    git clone [link]
    git branch ["name"] / tạo branch
    git checkout
    git merge
```
# 3. Giới thiệu HTML, CSS, Javascript
![HTML-CSS-Javascript](htmlcssjs.jpeg)

3 yếu tố cơ bản để tạo nên một trang web
- HTML: Cung cấp cấu trúc cho 1 trang web
- CSS: Sử dụng để định dạng, kiểm soát trình bày của trang web
- Javsscript: Kiểm soát hành vi của các yếu tố khác nhau

### 3.1. HTML
- HTML - HyperText Markup Language hay còn gọi là ngôn ngữ đánh dấu siêu văn bản được sử dụng trong việc phát triển các trang web
- HTML không phải ngôn ngữ lập trình vì nó chỉ là một cách xác định cấu trúc, ý nghĩa, mục đích của các phần tử trên trang trang web, như các phần tử văn bản, hình ảnh, liên kết,... bằng cách sử dụng các thẻ
- Nhiệm vụ chính của HTML là xây dựng cấu trúc siêu văn bản trên một trang web
### 3.2. CSS
CSS - Cascading Style Sheets, ngôn ngữ tạo phong cách của website, là ngôn ngữ thiết kế sử dụng để mô tả cách trình bày, bố cụ và phong cách của nội dung trên trang web
### 3.3. Javascript
- Javascript là một ngôn ngữ lập trình và là một phần quan trọng của các trang web
- Vai trò:
    - Biến những trang web tĩnh trở nên động, tạo ra sự tương tác trên trang web
    - Tăng cường các hành vi người dùng như xác nhận biểu mẫu, xác nhận hộp thoại
    - Kiểm soát mặc định của trình duyệt