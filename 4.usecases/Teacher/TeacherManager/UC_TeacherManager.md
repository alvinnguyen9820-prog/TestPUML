# Use Case: Quản lý giảng viên

## Mục đích

Cho phép người dùng thực hiện các thao tác quản lý giảng viên: thêm mới, chỉnh sửa, xóa, tìm kiếm, xem chi tiết

## Tác nhân chính

* Admin

## Tiền điều kiện

* Người dùng đã đăng nhập hệ thống và có quyền truy cập chức năng quản lý giảng viên.

## Luồng chính

1. Người dùng truy cập chức năng quản lý giảng viên.
2. Hệ thống kiểm tra quyền truy cập.
3. Người dùng chọn thao tác mong muốn:

   * Thêm mới: Thực hiện thêm mới giảng viên (chi tiết tại use case tương ứng).
   * Chỉnh sửa: Thực hiện chỉnh sửa giảng viên (chi tiết tại use case tương ứng).
   * Xóa: Thực hiện xóa giảng viên (chi tiết tại use case tương ứng).
   * Tìm kiếm: Thực hiện tìm kiếm giảng viên (chi tiết tại use case tương ứng).
   * Xem chi tiết: Hiển thị thông tin chi tiết giảng viên (chi tiết tại use case tương ứng). 

4. Hệ thống thực hiện thao tác tương ứng và thông báo kết quả.

## Luồng phụ/ngoại lệ

* Người dùng không có quyền truy cập: Hệ thống hiển thị thông báo lỗi và không cho phép thao tác.
* Người dùng hủy thao tác: Use case kết thúc, không thay đổi dữ liệu.

## Hậu điều kiện

* Nếu thành công: Thao tác quản lý giảng viên được thực hiện và cập nhật vào hệ thống.
* Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.

## Liên kết

* Activity Diagram: [AD_TeacherManager.puml]
* Form liên quan: SCR_TeacherManager
* Các use case chi tiết: AD_TeacherManager_Create, AD_TeacherManager_Update, AD_TeacherManager_Delete, AD_TeacherManager_Search, AD_TeacherManager_Detail
