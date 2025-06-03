![image](https://github.com/user-attachments/assets/487be3b3-8008-4c88-a2c7-cd14180c348d)
1. Giới thiệu
Ứng dụng này là một công cụ web đơn giản giúp người dùng mã hóa và giải mã tệp tin bằng thuật toán DES (Data Encryption Standard). Ứng dụng hỗ trợ người dùng chọn tệp, nhập khóa và thực hiện một trong hai thao tác: mã hóa hoặc giải mã. Kết quả sẽ được tải về dưới dạng tệp đã được xử lý.

2. Chức năng cơ bản
Giao diện người dùng (Frontend):

Giao diện đẹp, hiện đại với hiệu ứng "glassmorphism".

Cho phép người dùng:

Tải lên tệp cần mã hóa/giải mã.

Nhập khóa DES đúng 8 ký tự.

Chọn thao tác "Encrypt" hoặc "Decrypt".

Nhận lại tệp đầu ra sau khi xử lý.

Xử lý phía máy chủ (Backend):

Nhận file và khóa từ người dùng.

Thực hiện mã hóa hoặc giải mã file bằng thư viện PyCryptodome với chế độ DES ECB.

Trả lại file đã xử lý để người dùng tải xuống.

Bảo vệ và xử lý lỗi:

Giới hạn kích thước tệp tải lên là 16MB.

Kiểm tra độ dài khóa DES (đúng 8 ký tự).

Hiển thị thông báo lỗi nếu khóa sai hoặc file hỏng.

3. Kỹ thuật và công nghệ sử dụng
   ![image](https://github.com/user-attachments/assets/2b2713d2-c8a1-41b4-b620-d0cf9ba9c1fc)

