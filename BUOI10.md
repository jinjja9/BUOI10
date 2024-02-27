 #  [JAVA] BUỔI 10: NHẬP XUẤT FILE, UNIT TEST
 
 ***
## 1. Xử lí File trong Java (Binary file, Text file)


>*Tài liệu tham khảo*:  [File](https://giasutinhoc.vn/lap-trinh/lap-trinh-java-co-ban/doc-va-ghi-file-trong-java-bai-5-2/)

\- Có 2 kiểu luồng trong Java
+ **Byte Stream**: Hỗ trợ nhập xuất dữ liệu trên byte -> Binary file
+ **Character Stream**: Hỗ trợ nhập xuất kiểu kí tự -> Text file


![alt text](image-25.png)
![alt text](image-28.png)

\- Kiến trúc Input Stream (Luồng nhập dữ liệu)

![alt text](image-26.png)

\- Kiến trúc Output Stream (Luồng xuất dữ liệu)

![alt text](image-27.png)


**Đọc và ghi file trong java – Các thao tác xử lý dữ liệu**
- Bước 1: Tạo đối tượng luồng và liên kết với nguồn dữ liệu.
- Bước 2: Thao tác dữ liệu (đọc hoặc ghi hoặc cả hai).
- Bước 3: Đóng luồng.

### 1.1: Binary file

>*Tài liệu tham khảo*:  [Binary file](https://gpcoder.com/3046-huong-dan-su-dung-luong-vao-ra-nhi-phan-trong-java/)

### 

## 2. Assertions

### 2.1: K/N

\- **Assertion trong  Java** cho phép chúng ta kiểm tra tính đúng đắn của bất kỳ giả định nào đã được thực hiện trong chương trình. Chúng ta có thể đạt được nó bằng cách sử dụng câu lệnh khẳng định trong Java. 
\- Trong khi thực hiện một xác nhận, chúng ta giả định nó là đúng. Nếu xác nhận không thành công, thì JVM sẽ ném ra lỗi AssertionError. 
\- Do đó, chúng tôi sử dụng nó cho mục đích thử nghiệm trong quá trình phát triển. Chúng ta có thể sử dụng câu lệnh khẳng định với biểu thức Boolean và có thể viết theo hai cách khác nhau như sau:

- Khẳng định biểu thức;
- Khẳng định biểu thức1: biểu thức2;

### 2.2: Tại sao lại cần sử dụng Assertion trong Java

>*Tài liệu tham khảo*:  [Assertion1](https://t3h.com.vn/tin-tuc/assertion-trong-java)

>*Tài liệu tham khảo*:  [Assertion2](https://websitehcm.com/assert-trong-java/)

\- **Assertion** được sử dụng bất kỳ khi nào kỹ sư phần mềm muốn kiểm tra tính đúng sai của một vấn đề trong lập trình Java.

- Để đảm bảo rằng một mã không thể truy cập thực sự không thể truy cập được
- Để đảm bảo rằng các giá trị giả định được viết trong các nhận xét là đúng
- Để đảm bảo rằng trường hợp chuyển đổi mặc định không được thực thi
- Kiểm tra trạng thái của đối tượng
- Sử dụng tại điểm, bắt đầu của phương thức
 
### 2.3: So sánh Java Assertion xử lý ngoại lệ thông thường

\- Chúng ta thường sử dụng Assertion để kiểm tra các tình huống bất khả thi về mặt logic. Ví dụ: Chúng ra có thể sử dụng chúng để kiểm tra trạng thái mà mã mong đợi trước khi nó bắt đầu chạy hoặc trạng thái sau khi chạy xong. Sự khác biệt giữa Assertion và ngoại lệ thông thường là các xác nhận thường bị vô hiệu hóa tại thời điểm chạy.

## 3. Unit test  

>*Tài liệu tham khảo*:  [Unit Test  1](https://gpcoder.com/5234-kiem-thu-voi-junit-trong-java/)


>*Tài liệu tham khảo*:  [Unit Test2](https://vn.got-it.ai/blog/unit-test-trong-java-tat-tan-tat-ve-junit)
\-  **Unit Test** có nghĩa là kiểm thử đơn vị, một bước trong kiểm thử phần mềm. Với Unit Test, chỉ có những đơn vị hay những thành phần riêng lẻ của phần mềm được kiểm thử. Mục đích là để xác định rằng mỗi đơn vị của phần mềm đều hoạt động đúng như kỳ vọng. 

\- **Unit Testing** được tiến hành trong quá trình phát triển (lập trình) một phần mềm. Unit Test cô biệt một phần của các mã code và đánh giá sự chính xác của chúng. Một đơn vị có thể là một hàm (function), một phương thức (method), một quy trình (procedure), một mô-đun hay một đối tượng. 

***Unit Test***
- Giúp sửa bug sớm trong chu trình phát triển sản phẩm và tiết kiệm chi phí
- Giúp các lập trình viên hiểu được nền tảng mã kiểm thử và cho phép họ đưa ra các thay đổi nhanh chóng
- Có thể được sử dụng như các ghi chép về dự án, nếu hiệu quả
- Tái sử dụng code. Kết hợp cả code của bạn và kiểm thử của bạn cho dự án mới. Thay đổi code cho đến khi kiểm thử chạy được

### 3.1: Một số khái niệm cần biết trong Unit Test

- **Unit Test case**: là 1 chuỗi code để đảm bảo rằng đoạn code được kiểm thử làm việc như mong đợi. Mỗi function sẽ có nhiều test case, ứng với mỗi trường hợp function chạy.
- **Setup**: Đây là hàm được chạy trước khi chạy các test case, thường dùng để chuẩn bị dữ liệu để chạy test.
- **Teardown**: Đây là hàm được chạy sau khi các test case chạy xong, thường dùng để xóa dữ liệu, giải phóng bộ nhớ.
- **Assert**: Mỗi test case sẽ có một hoặc nhiều câu lệnh Assert, để kiểm tra tính đúng đắn của hàm.
- **Mock**: là một đối tượng ảo, mô phỏng các tính chất và hành vi giống hệt như đối tượng thực được truyền vào bên trong khối mã đang vận hành nhằm kiểm tra tính đúng đắn của các hoạt động bên trong. Giả sử chương trình của chúng ta được chia làm 2 module: A và B. Module A đã code xong, B thì chưa. Để test module A, ta dùng mock để làm giả module B, không cần phải đợi tới khi module B code xong mới test được.
- **Test Suite** : Test suite là một tập các test case và nó cũng có thể bao gồm nhiều test suite khác, test suite chính là tổ hợp các test.

### 3.2: Các tính năng của JUnit
- JUnit là một khung kiểm tra nguồn mở, được sử dụng để viết và chạy test.
- Cung cấp annotation để định dạng các test method
- Cung cấp assertion để kiểm thử các kết quả mong đợi
- Cung cấp các trình chạy để chạy test
- Cho phép bạn viết code nhanh hơn, cải thiện chất lượng
- JUnit khá đơn giản. Nó ít phức tạp hơn và tốn ít thời gian hơn
- JUnit có thể được chạy tự động và tự kiểm tra kết quả, cung cấp phản hồi nhanh chóng. Không cần thiết phải xem xét thủ công các báo cáo về kết quả kiểm thử. 
- Các bài test JUnit có thể được tổ chức thành các bộ kiểm thử chứa các trường hợp kiểm thử, thậm chí là chứa các bộ kiểm thử khác. 
- JUnit thể hiện tiến độ kiểm thử trên một thanh. Nếu thanh có màu xanh, bài test đang chạy êm ả. Ngược lại, nếu thanh chuyển đỏ, tức là bài test thất bại.

## 4: Tầm quan trọng của việc viết Unit test
Đảm bảo tính chính xác của mã: Unit test giúp xác minh rằng mã của bạn hoạt động như mong đợi. Khi bạn thay đổi mã, các unit test giúp bạn đảm bảo rằng các tính năng hiện tại không bị ảnh hưởng.

Tự tin hơn khi refactor code: Khi bạn cần sửa đổi mã hoặc tái cấu trúc, unit test giúp đảm bảo rằng các tính năng vẫn hoạt động sau khi thay đổi.

Tăng tốc độ phát triển: Việc viết unit test từ ban đầu có thể tăng tốc độ phát triển vì bạn sẽ phát hiện và sửa lỗi sớm hơn trong quá trình phát triển thay vì phải tìm kiếm và sửa các lỗi sau này.

Tăng độ tin cậy của mã: Có unit test tạo ra một mức độ tin cậy trong mã của bạn. Nó cung cấp một cách tiếp cận khoa học để kiểm tra xem mã của bạn có đáp ứng các yêu cầu và kỳ vọng không.

Tài liệu sống (living documentation): Unit test có thể được coi như là tài liệu sống cho mã của bạn. Chúng mô tả cách các thành phần của mã nên hoạt động, cũng như cách sử dụng chúng.

Khuyến khích thiết kế linh hoạt và rõ ràng: Viết unit test thúc đẩy việc tạo ra mã dễ đọc, dễ bảo trì và dễ mở rộng. Khi viết unit test, bạn thường phải tách logic và tạo ra các hàm và lớp có khả năng tái sử dụng cao.

Hỗ trợ liên tục tích hợp (CI) và liên tục triển khai (CD): Unit test là một phần quan trọng trong quy trình CI/CD, giúp tự động hóa quy trình kiểm tra và triển khai mã.