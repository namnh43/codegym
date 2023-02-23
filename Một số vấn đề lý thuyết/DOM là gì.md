DOM là gì? 

Tìm hiểu và thao tác DOM trong Javascript

THam khảo: https://topdev.vn/blog/dom-la-gi/

DOM là gì?
DOM là tên gọi viết tắt của (Document Object Model – tạm dịch Mô hình Các Đối tượng Tài liệu). Là một chuẩn được định nghĩa bởi W3C (Tổ Chức Web Toàn Cầu – World Wide Web Consortium). DOM được dùng để truy xuất và thao tác trên các tài liệu có cấu trúc dạng HTML hay XML bằng các ngôn ngữ lập trình thông dụng như Javascript, PHP…

DOM là gì? Tìm hiểu và thao tác DOM trong Javascript
Trong mỗi thẻ HTML sẽ có những thuộc tính (Properties) và có phân cấp cha – con với các thẻ HTML khác. Sự phân cấp và các thuộc tính của thẻ HTML này ta gọi là selector và trong DOM sẽ có nhiệm vụ xử lý các vấn đề như đổi thuộc tính của thẻ, đổi cấu trúc HTML của thẻ.

Có thể thấy tất cả các thẻ HTML sẽ được quản lý trong đối tượng document. Thẻ cao nhất là thẻ html, tiếp theo là phân nhánh body và head. Bên trong head thì có những thẻ như style, title,… và bên trong body thì là vô số các thẻ HTML khác. Như vậy trong Javascript, để thao tác với các thẻ HTML ta phải thông qua đối tượng document.

HTML DOM là gì?
HTML DOM giúp thao tác dữ liệu theo mô hình hướng đối tượng. Các phần tử bên trong 1 tài liệu có cấu trúc được định nghĩa thành các đối tượng, phương thức và thuộc tính để có thể truy xuất dễ dàng mà vẫn đảm bảo tính cấu trúc.

Mỗi phần tử là một đối tượng, sở hữu các thuộc tính và các phương thức để làm việc với các thuộc tính đó như thêm, xóa, sửa, cập nhật. Bên cạnh đó, bạn cũng có thể thêm bớt các phần tử tùy thích, giúp cho nội dung và cấu trúc của trang web luôn cập nhật động. Nó định nghĩa sau đây:

HTML elements như là objects
properties của tất cả HTML elements
methods để truy cập đến tất cả HTML elements
events cho tất cả HTML elements
Cây cấu trúc DOM
Node
Đối với HTML DOM, mọi thành phần đều được xem là một node (nút), được biểu diễn trên 1 cây cấu trúc dạng cây gọi là DOM Tree. Các phần tử khác nhau sẽ được phân loại node khác nhau nhưng quan trọng nhất là 3 loại: node gốc (document node), node phần tử (element node), node văn bản (text node).

Node gốc: chính là tài liệu HTML, thường được biểu diễn bởi thẻ <html>.
Node phần tử: biểu diễn cho 1 phần tử HTML.
Node văn bản: mỗi đoạn kí tự trong tài liệu HTML, bên trong 1 thẻ HTML đều là 1 node văn bản. Đó có thể là tên trang web trong thẻ title, tên đề mục trong thẻ h1, hay một đoạn văn trong thẻ p.
Ngoài ra còn có node thuộc tính (attribute node) và node chú thích (comment node).
