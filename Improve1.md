### Duplicated user
Để giải quyết vấn đề này thì mình sẽ sử dụng lệnh select để check username trong database nếu có thì báo lỗi cho user.

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/09aeba7b-ab05-4b4b-ba8e-1563ad5cd8e4)

Đồng thời thêm constraint UNIQUE cho cột user_name trong database.

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/17e2b78f-9f8d-489d-9e36-eb6d16655b4d)

*Hash Function
Ngoài ra thì ta sẽ hash password trước khi lưu về database để tăng tính bảo mật

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/4caf275c-9226-4743-ad6f-c41e8f09c873)

Sau khi thêm signup thì database sẽ có dữ liệu như hình dưới đây:

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/8f6b0d53-2126-4529-b895-99b669787be4)

## Modify Login Page
Ngoài ra ta cần phải thêm hàm password_verify để check hash_password trong database

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/8a580c0e-41c9-468d-ad7e-9252db042c90)

*password_verify là 1 hàm dùng để kiểm tra password trong php

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/3abc99f0-7753-4b6f-9284-b2eeca5205fa)


### Server Side Validation


### Add Category


### Take Unique Random questions from database


### Serverside Validation
