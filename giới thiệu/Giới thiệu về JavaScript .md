Giới thiệu về JavaScript 

1. Là gì?
- JavaScript là ngôn ngữ lập trình mà cho phép bạn viết code trên webpage HTML, nó tự động được load và thực thi khi load webpage.
- JavaScript được cung cấp và thực thi như một plain text, nó không cần phải biên dịch trước khi thực thi. Về điểm này nó khác những ngôn ngữ lập trình khác.

2. Vì sao có tên là JavaScript?
- Ban đầu, JavaScript có tên là LiveScript, thời điểm đó Java đang rất phát triển phổ biến, đội phát triển muốn ngôn ngữ của mình như một người em của Java, sẽ được Java giúp đỡ để phát triển mạnh mẽ nên đối tên thành JavaScript, đến bây giờ JavaScript đã phát triển với tiêu chuẩn khác là ECMAScript và phổ biến rất rộng rãi và không còn liên quan gì đến Java nữa.

3. JavaScript hoạt động thế nào?
- JavaScript hoạt động trên Script Engine, các Script Engine được tích hợp trên Browser, trên các Browser khác nhau Script Engine sẽ có tên khác nhau, ví dụ như V8 của Chrome/Opera, SpiderMonkey trên Fifox, Chakra trên IE, ...
- Ngày nay, JavaScript không chỉ hoạt động trên Browser, nó có thể hoạt động trên máy tính, thiết bị khác mà có cài đặt Script Engine. Phổ biến là hoạt động trên NodeJS để làm việc như 1 máy chủ web.
- Dưới đây là các bước hoạt động của Script Engine:
	+ Script Engine tích hợp trong Browser sẽ được mã JavaScript
	+ Script Engine biên dịch JavaScript thành mã máy(Machine code) 
	+ Máy tính/Thiết bị sẽ thực thi mã máy(Machine code) đã được biên dịch.

4. JavaScript có thể làm được gì?
- Đầu tiên, cần hiểu là JavaScript ban đầu được thiết kế chỉ để hoạt động trên Script Engine của Browser, nó không được thiết kế để CPU, bộ nhớ máy tính - các thành phần mà yêu cầu quyền truy cập cấp thấp, lý do là các Browser không yêu cầu các quyền truy cập đó, nên nó được xem là ngôn ngữ an toàn.
- JavaScript phụ thuộc vào Script Engine mà nó chạy trên đó, ví dụ như trên NodeJS thì nó có các quyền xử lý file, làm việc với network, ...
- JavaScript chạy trên Script Engine của Browser thì có thể làm các việc dưới đây:
	+ JavaScript có thể thêm/sửa/xóa các mã HTML trong webpage. Nó làm thay đổi nội dung và style của webpage.
	+ JavaScript cho phép phản ứng nhanh với các hoạt động của người dùng trên webpage như click, rê chuột, ...
	+ JavaScript có thể gửi request đến Web Server để download/upload file, yêu cầu điều gì đó - Điển hình là AJAX, COMET nữa ...
	+ JavaScript cho phép set/get cookie ở Browser, hiển thị message thông báo, tạo form câu hỏi cho người dùng khi truy cập webpage
	+ JavaScript cho phép ghi nhớ/lưu trữ dữ liệu ở vùng lưu trữ local người dùng

5. JavaScript không thể làm được gì?
- JavaScript được thiết kế trên Script Engine của Browser bị giới hạn quyền hạn nhằm bảo vệ dữ liệu của người dùng. Mục đích là nhằm ngăn chặn các hoạt động xấu nhằm đánh cắp/thay đổi dữ liệu của người dùng.
- JavaScript trên Script Engine của Browser không thực hiện được các việc sau:
	+ JavaScript trên webpage không thể đọc/viết các file trên ổ cừng, không thể copy và thực thi nó. JavaScript không được cấp quyền để thực hiện trực tiếp các hoạt động của hệ điều hành.
	+ JavaScript ngày nay cũng có thể làm việc với file nhưng chỉ khi nó được người dùng đưa vào webpage thông qua thẻ <input>
	+ JavaScript cũng không có quyền truy cập các thiết bị khác như camera, phone, ...
	+ JavaScript trên các tab khác nhau sẽ hoạt động khác nhau, mặc dù JavaScript có thể mở thêm 1 tab mới nhưng đến khi đã mở xong thì chúng hoạt động độc lập và không biết gì về nhau. Điều này tuân thủ chính sách “Same Origin Policy”. Giới hạn này làm cho người dùng an toàn hơn, ví dụ người dùng có 2 tab trên một trình duyệt thì vì hoạt động độc lập nên nó an toàn.
	+ JavaScript dễ dàng làm việc với network, tuy nhiên buộc phải định nghĩa rõ ràng đến gửi và điểm nhận ở HTTP header, điều này làm cho việc truyền dữ liệu chính xác, điều này làm cho dữ liệu an toàn hơn.
	
6. JavaScript có gì đặc biệt?
- JavaScript sinh ra để hoạt động trên Browser và nó là duy nhất:
	+ Làm việc với HTML trên webpage
	+ JavaScript thiết kế để xử lý các việc đơn giản như tương tác với người dùng một cách nhanh chóng
	+ Hoạt động trên hầu hết các Browser
- Ngày nay, JavaScript còn hoạt động trên máy chủ Web và các thiết bị, miễn là có Script Engine được cài đặt để nó hoạt động trên đó.

7. JavaScript ngày nay?
- Để hỗ trợ cho việc phát triển các ứng dụng lớn với các chức năng phức tạp hơn, các biến thể khác của JavaScript được xây dựng, các biến thể này được biên dịch thành JavaScript thuần túy trước khi thực thi, việc này được thực hiện trong suốt nên chúng ta thường không nhìn thấy.
- Các biến thể có các cú pháp khác nhau, phù hợp với các nhóm phát triển khác nhau, về cơ bản cú pháp JavaScript không hoàn toàn phù hợp với tất cả mọi người mặc dù nó rất mạnh mẽ và phổ biến.
- Ví dụ các biến thể của JavaScript ngày nay:
	+ CoffeeScript - Làm cho JavaScript dễ viết, dễ hiểu, dễ dùng hơn
	+ TypeScript - Microsoft- Định nghĩa các quy chuẩn ràng buộc về việc phát triển bằng JavaScript, để dễ dàng tạo ra các ứng dụng lớn và phức tạp
	+ Flow - Facebook
	+ Dart - Google
- Dù là biến thể gì của JavaScript thì bạn cũng nên có hiểu biết về JavaScript để hiểu cách nó hoạt động
	
8. Tổng kết
- Ban đầu, JavaScript chỉ được thiết kế để hoạt động trên Browser, tuy nhiên ngày nay, JavaScript đã có thể hoạt động trên nhiều thiết bị khác nhau
- Cho đến hôm nay thì JavaScript vẫn là ngôn ngữ lập trình duy nhất dùng để xử lý HTML trên webpage để xây dựng nội dung và tương tác với người dùng trên webpage
- Có rất nhiều biến thể đã được xây dựng với nhiều tính năng hơn, tuy nhiên để hiểu và sử dụng thuần thục, vẫn nên hiểu về JavaScript
