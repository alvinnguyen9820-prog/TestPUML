# Use Case: Quản lý sinh viên

## Mục đích

Cho phép người dùng thực hiện các thao tác quản lý sinh viên: thêm mới, chỉnh sửa, xóa, tìm kiếm, xem chi tiết

## Tác nhân chính

* Admin

## Tiền điều kiện

* Người dùng đã đăng nhập hệ thống và có quyền truy cập chức năng quản lý sinh viên.

## Luồng chính

1. Người dùng truy cập chức năng quản lý sinh viên.
2. Hệ thống kiểm tra quyền truy cập.
3. Người dùng chọn thao tác mong muốn:

   * Thêm mới: Thực hiện thêm mới sinh viên (chi tiết tại use case tương ứng).
   * Chỉnh sửa: Thực hiện chỉnh sửa sinh viên (chi tiết tại use case tương ứng).
   * Xóa: Thực hiện xóa sinh viên (chi tiết tại use case tương ứng).
   * Tìm kiếm: Thực hiện tìm kiếm sinh viên (chi tiết tại use case tương ứng).
   * Xem chi tiết: Hiển thị thông tin chi tiết sinh viên (chi tiết tại use case tương ứng). 

4. Hệ thống thực hiện thao tác tương ứng và thông báo kết quả.

## Luồng phụ/ngoại lệ

* Người dùng không có quyền truy cập: Hệ thống hiển thị thông báo lỗi và không cho phép thao tác.
* Người dùng hủy thao tác: Use case kết thúc, không thay đổi dữ liệu.

## Hậu điều kiện

* Nếu thành công: Thao tác quản lý sinh viên được thực hiện và cập nhật vào hệ thống.
* Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.

## Liên kết

* Activity Diagram: [AD_StudentManager.puml]
* Form liên quan: SCR_StudentManager
* Các use case chi tiết: AD_StudentManager_Create, AD_StudentManager_Update, AD_StudentManager_Delete, AD_StudentManager_Search, AD_StudentManager_Detail
