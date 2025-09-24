# Use Case: Quản lý giảng viên

## User Story

Là một quản trị viên, tôi muốn có thể thực hiện quản lý giảng viên (thêm, sửa, xóa, tìm kiếm, xem chi tiết) để đảm bảo dữ liệu giảng viên luôn đầy đủ, chính xác

## Acceptance criteria
- Hệ thống cho phép quản trị viên thêm mới giảng viên.
- Hệ thống cho phép quản trị viên chỉnh sửa thông tin giảng viên đã tồn tại.
- Hệ thống cho phép quản trị viên xóa giảng viên và xác nhận trước khi xóa.
- Hệ thống cho phép quản trị viên tìm kiếm giảng viên theo tên giảng viên.
- Hệ thống cho phép quản trị viên xem chi tiết hồ sơ giảng viên với đầy đủ thông tin.
- Giao diện phải thông báo kết quả thao tác (thành công/thất bại) cho quản trị viên.

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
* Các use case chi tiết: UC_TeacherManager_Create, UC_TeacherManager_Update, UC_TeacherManager_Delete, UC_TeacherManager_Search, UC_TeacherManager_Detail
