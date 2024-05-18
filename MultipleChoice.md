Thì theo yêu cầu thì mình sẽ tải XAMPP:

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/a1381bbc-c21d-42f1-9eda-811c2891ed8e)

Mình sẽ dùng chmod và sudo ./ để tải file và ngồi đợi XAMPP tải xuống thui

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/a0f2c1ad-375b-4473-8034-336fa86d9d5e)

Và chỉ cần bấm Forward cho đến khi file tải xong là được

Do mình cần trang web có thể lưu trữ tên và password của user nên mình sẽ cần Khởi động database

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/cfa8f299-4192-4885-a200-1825f2ebabb0)

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/4a9678c6-260e-48fd-9499-a4bce5836e1a)

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/6bae02b4-61f2-4a3e-87c5-151337249ab0)

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/9fa900ed-5521-481b-a8fb-61354e1ca25f)

Tạo db theo yêu cầu đề bài (Khóa chính là id, nhập dải giá trị cho các cột và lưu lại

Sau khi lưu lại, ta sẽ có database. Tiếp theo, để tối ưu db thì mình có thể thêm chỉ mục cho 1 số cột sẽ cần truy vấn nhiều như: user_id, date, MSSV.

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/c5bcf517-8041-4be2-8f4b-5c0905d4f25c)

Tạo thư mục để chứa project:

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/0cc3b503-998a-4c06-867f-cd7c64b77acf)

Tiếp theo sẽ là kết nối với database sử dụng mysqli_connect:

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/c90d80d5-eb59-4667-b2cd-3c91a8a06776)

mysqli_connect sẽ trả về 1 object sau khi kết nối db thành công và mình có thể sử dụng object đó để tương tác với db. Ta sẽ dùng 1 câu lệnh if để kiểm tra kết nối.

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/14acdf08-6e4c-4d79-bfae-97b26637c5e0)

Mình sẽ tạo SESSION sử dụng biến super_global. SESSION là 1 biến dùng để chứa thông tin về 1 user, và có thể dùng để kiểm tra nếu user đó đã đăng nhập hay chưa trong 1 web application.
Mình sẽ include file connection khi nãy để sử dụng biến $con và file function để sử dụng hàm check_login do mình tạo để kiểm tra login của user.
![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/6d405130-e6eb-4a88-87b1-66827a064472)

Tiếp theo thì mình sẽ tạo file functions.php để tạo hàm check_login:

![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/23bdf596-cc2f-4fc5-8be9-940552e075fe)

Để nói chi tiết thì hàm này sẽ kiểm tra user_id đã có trong SESSION tức là kiểm tra user_id đã được set hay chưa. Nếu chưa có thì tương đương với user chưa đăng nhập, và nếu có rồi thì mình sẽ cần kiểm tra thêm 1 bước nữa là kiểm tra xem user đó có trong db hay chưa. Nếu user đã có trong db thì mình sẽ trả về dữ liệu người dùng đó.

Kế đến sẽ là file đăng ký.
![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/02dc0ce0-9514-4f75-8837-91ee1c8713d8)

Sau đó là file đăng nhập.
![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/66e32ac9-c993-4887-83e5-32ef374ae7f1)

File logout.
![image](https://github.com/Ash-Dust/Web_Project/assets/120457430/ab20f4b6-cd19-407d-9615-301167380d78)


