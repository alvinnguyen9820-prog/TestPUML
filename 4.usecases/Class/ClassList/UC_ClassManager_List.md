# Use Case: Xem danh sách lớp học

## User Story

* Là một quản trị viên, tôi muốn xem danh sách lớp học để dễ dàng theo dõi và quản lý thông tin các lớp trong hệ thống.

## Acceptance criteria
* Hệ thống hiển thị danh sách tất cả lớp học.  
* Mỗi lớp trong danh sách phải hiển thị các thông tin cơ bản: mã lớp, tên lớp, thời gian bắt đầu, kết thúc, tổng số lượng sinh viên.  
* Nếu số lượng lớp vượt quá giới hạn hiển thị, hệ thống phải cung cấp phân trang (10 bản ghi 1 trang).
* Hệ thống cho phép tìm kiếm lớp học (chi tiết trong UC_ClassManager_Search).    
* Nếu không có lớp học nào trong hệ thống, hiển thị thông báo “Không có dữ liệu lớp học”.  
* Nếu có lỗi tải dữ liệu, hiển thị thông báo lỗi.  
* Danh sách lớp được hiển thị theo dạng bảng, thứ tự theo thời gian cập nhật từ mới tới cũ nhất.  

## Tác nhân chính

* Admin

## Tiền điều kiện

* Người dùng đã đăng nhập hệ thống và có quyền truy cập chức năng quản lý lớp học.

## Luồng chính

1. Người dùng truy cập chức năng quản lý lớp học.
2. Hệ thống kiểm tra quyền truy cập.
3. Nếu có quyền truy cập, hệ thống hiển thị danh sách lớp học theo thứ tự thời gian cập nhật từ mới tới cũ nhất
4. Nếu số lượng bản ghi lớn hơn 10, hệ thống thực hiện phân trang, 10 bản ghi mỗi trang
5. Người dùng thực hiện chuyển trang, hệ thống hiển thị danh sách bản ghi ở trang tương ứng
6. Người dùng thực hiện tìm kiếm (chi tiết trong UC_ClassManager_Search).
7. Hệ thống hiển thị danh sách theo kết quả tìm kiếm


## Luồng phụ

## Ngoại lệ

* Người dùng không có quyền truy cập: Hệ thống hiển thị thông báo lỗi và không cho phép truy cập chức năng.
* Nếu không có bản ghi nào, hệ thống hiển thị "Không có dữ liệu lớp học"
* Nếu có lỗi tải dữ liệu, hệ thống hiển thị thông báo lỗi.

## Hậu điều kiện
* Nếu thành công: Hệ thống hiển thị danh sách lớp học
* Nếu thất bại: Hệ thống hiển thị thông báo lỗi

## Liên kết

* Activity Diagram: [AD_ClassManager_List.puml]
* Form liên quan: SCR_ClassManager
* Các Entity liên quan: Class 
