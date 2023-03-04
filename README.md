# TalkWithFriend
1 Tạo project ứng dụng android
Bước 1: Tải Android Studio phiên bản 11.0.13
Bước 2: Cài đặt SDK/API 33, Android OS: Tiramisu.
Bước 3: Tạo project Android.	
•	Các bước chi tiết tạo project:
•	Mở Android Studio.
•	Tạo Project, chọn Form của ứng dụng, chọn Next.
•	Điền tên của Project, vị trí lưu, ngôn ngữ viết, phiên bản SDK, chọn Finish.
3.2 Tạo máy ảo điện thoại android studio
Trong Device Manager, chọn Create Device:
•	Chọn kiểu điện thoại, ở đây chúng ta chọn Phone – Pixel 3XL -> Next.
•	Chọn phiên bản Android OS, sử dụng phiên bản phù hợp với API level mà khi tạo project đã chọn, ứng dụng đang phát triển sử dụng OS Tiramisu ( API 33).
•	Điền tên thiết bị ảo, chọn Finish để hoàn thành việc tạo máy ảo.
3.3 Tạo firebase và thêm vào ứng dụng
3.3.1 Tạo firebase
Firebase là dịch vụ cơ sở dữ liệu hoạt động trên nền tảng đám mây – cloud. Kèm theo đó là hệ thống máy chủ cực kỳ mạnh mẽ của Google. Chức năng chính là giúp người dùng lập trình ứng dụng bằng cách đơn giản hóa các thao tác với cơ sở dữ liệu.
Các bước tạo firebase: 
Truy cập địa chỉ https://firebase.google.com/.
•	Chọn Truy cập vào bảng điều khiển (Console), sau đó chọn dấu + (Add Project) để bắt đầu tạo mới một Project Data Firebase.
•	Đặt tên cho project, chọn Continue.
•	Chọn tài khoản Google Analystics (Default Account for Firebase). Sau đó chọn Create project.
•	Sau khi project được tạo thành công, chọn Continue.
•	Chọn thẻ Database, chọn Create Database, chọn Start in test mode
•	Chọn vùng của Server, chọn Done
•	Chọn Realtime Database (do ứng dụng cần dữ liệu được cập nhật liên tục)
•	Hoàn thành tạo firebase
2 Thêm firebase vào Android Studio
•	Tại console của Firebase, vào mục project overview sau đó ấn vào nút chọn tích hợp vào Android. Sau đó có một sửa sổ hiện thị để chúng ta nhập package name và project name. Nhập vào tên package và tên project giống như project vừa tạo ở Android Studio.
•	Tải file google-services.json và copy vào trong thư mục app ở Android Studio.
•	Thực hiện cấu hình thư viện trên Android Studio Trong Android Studio, mở file build.gradle (project) và thêm dòng sau:
buildscript {
dependencies {
// Add this line
classpath 'com.google.gms:google-services:3.1.0'
}
}
•	Trong file build.gradle (app) thêm dòng sau vào cuối:
dependencies {
    //Add this line
    compile 'com.google.firebase:firebase-database:11.8.0'
}
apply plugin: 'com.google.gms.google-services'
•	Tại phía góc trên bên phải của Android Studio ấn Sync Now -> hoàn thành cấu hình FireBase lên Android Studio.
Chúng ta đã hoàn thành khởi tạo project, sau đó bọn em thực hiện lập trình ứng dụng với các chức năng được giao

