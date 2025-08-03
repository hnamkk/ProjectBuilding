# Hệ thống Quản lý Bất động sản
## Mô tả dự án
Đây là một ứng dụng web quản lý bất động sản với trọng tâm vào Backend, được xây dựng với framework Spring Boot. Dự án này cung cấp các chức năng cho cả quản trị viên và người dùng công khai. Hệ thống cho phép người dùng quản trị quản lý thông tin về các tòa nhà, khách hàng, và người dùng của hệ thống.
## Công nghệ sử dụng
### Backend
* Spring Boot: Framework chính để xây dựng ứng dụng độc lập, tự động cấu hình và quản lý các phụ thuộc.
* Spring Security: Cung cấp các dịch vụ xác thực và phân quyền truy cập, bảo vệ các tài nguyên của ứng dụng.
* Spring Data JPA & Hibernate: Spring Data JPA giúp đơn giản hóa việc truy cập dữ liệu, sử dụng Hibernate làm provider để ánh xạ các đối tượng Java với cơ sở dữ liệu.
* RESTful API: Các API được xây dựng để xử lý các yêu cầu từ phía client, đặc biệt là các thao tác CRUD.
* Maven: Công cụ quản lý dự án và các thư viện phụ thuộc.
* MySQL: Hệ quản trị cơ sở dữ liệu được sử dụng để lưu trữ dữ liệu của ứng dụng.
### Frontend
* JSP: Công nghệ view để tạo các trang web động.
* Bootstrap, HTML, CSS, JavaScript: Các công nghệ cơ bản để xây dựng giao diện và thêm tương tác cho người dùng.
* jQuery: Thư viện JavaScript để đơn giản hóa các thao tác DOM và xử lý AJAX.
* DisplayTag: Một thư viện thẻ tùy chỉnh của JSP để tạo các bảng dữ liệu có chức năng phân trang và sắp xếp.
## Cấu trúc thư mục chính
Dự án được tổ chức theo cấu trúc phân tầng chuẩn của Spring Boot, giúp dễ dàng bảo trì và mở rộng:
* src/main/java/com/javaweb/: Chứa mã nguồn Backend.
* src/main/webapp/: Chứa các tài nguyên Frontend, bao gồm các trang JSP và các file cấu hình giao diện.
* src/main/resources/: Chứa các file cấu hình ứng dụng (application.properties) và tài nguyên tĩnh.
## Tính năng chính
### Đăng nhập & Đăng xuất
### Quản lý Tòa nhà: 
* Xem danh sách các tòa nhà với các chức năng tìm kiếm động dựa trên nhiều tiêu chí.
* Thêm, sửa, xóa thông tin tòa nhà.
* Phân công nhân viên phụ trách các tòa nhà.
### Quản lý Khách hàng:
* Tìm kiếm, thêm, sửa, xóa thông tin khách hàng.
* Phân công nhân viên phụ trách khách hàng.
* Quản lý các giao dịch của khách hàng.
### Quản lý Người dùng:
* Thêm, sửa, xóa người dùng, bao gồm cả chức năng reset mật khẩu và cập nhật hồ sơ.
* Phân quyền người dùng dựa trên vai trò.
## Cài đặt và Chạy dự án
### Cơ sở dữ liệu
Tạo cơ sở dữ liệu MySQL với tên buildingprj và nhập dữ liệu từ file src/database/buildingprj.sql.
### Cấu hình
Cập nhật thông tin kết nối cơ sở dữ liệu trong src/main/resources/application.properties.
### Build
Sử dụng Maven để build dự án: 
* mvn clean install
### Chạy
Chạy ứng dụng thông qua Spring Boot
* mvn spring-boot:run
Hoặc chạy file SpringBootWebApplication.java từ IDE của bạn.
### Ứng dụng sẽ được khởi chạy tại: http://localhost:8081
