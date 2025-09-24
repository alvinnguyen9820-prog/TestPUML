# Use Case: Quản lý lớp học

## User Story

- Là một quản trị viên, tôi muốn quản lý lớp (thêm mới, chỉnh sửa, xóa, tìm kiếm, xem chi tiết, phân công giảng viên và sinh viên vào lớp) để đảm bảo thông tin lớp học luôn đầy đủ, chính xác và hỗ trợ hiệu quả cho công tác phân công giảng dạy, quản lý sinh viên.

## Acceptance Criteria
- Hệ thống cho phép quản trị viên thêm mới lớp học với đầy đủ thông tin bắt buộc.
- Hệ thống cho phép quản trị viên chỉnh sửa thông tin lớp học đã tồn tại.
- Hệ thống cho phép quản trị viên xóa lớp học và xác nhận trước khi xóa.
- Hệ thống cho phép quản trị viên tìm kiếm lớp học theo tên lớp.
- Hệ thống cho phép quản trị viên xem chi tiết thông tin lớp học với đầy đủ dữ liệu liên quan bao gồm thông tin lớp, danh sách giảng viên, danh sách sinh viên.
- Hệ thống cho phép quản trị viên phân công giảng viên vào lớp theo danh sách có sẵn.
- Hệ thống cho phép quản trị viên gán sinh viên vào lớp theo danh sách có sẵn.
- Hệ thống cho phép quản trị viên chỉnh sửa hoặc hủy phân công giảng viên/sinh viên khỏi lớp.
- Giao diện phải thông báo kết quả thao tác (thành công/thất bại) cho quản trị viên.

## Tác nhân chính

* Người dùng (có quyền quản lý lớp học, chi tiết theo từng tính năng)

## Tiền điều kiện

* Người dùng đã đăng nhập hệ thống và có quyền truy cập chức năng quản lý lớp học.

## Luồng chính

1. Người dùng truy cập chức năng quản lý lớp học.
2. Hệ thống kiểm tra quyền truy cập.
3. Người dùng chọn thao tác mong muốn:

   * Thêm mới: Thực hiện thêm mới lớp học (chi tiết tại use case tương ứng).
   * Chỉnh sửa: Thực hiện chỉnh sửa lớp học (chi tiết tại use case tương ứng).
   * Xóa: Thực hiện xóa lớp học (chi tiết tại use case tương ứng).
   * Tìm kiếm: Thực hiện tìm kiếm lớp học (chi tiết tại use case tương ứng).
   * Xem chi tiết: Hiển thị thông tin chi tiết lớp học (chi tiết tại use case tương ứng). 
   * Phân công giảng viên: Thực hiện phân công giảng viên vào lớp học (chi tiết tại use case tương ứng).
   * Phân công sinh viên: Thực hiện phân công sinh viên vào lớp học (chi tiết tại use case tương ứng).

4. Hệ thống thực hiện thao tác tương ứng và thông báo kết quả.

## Luồng phụ

## Ngoại lệ

* Người dùng không có quyền truy cập: Hệ thống hiển thị thông báo lỗi và không cho phép thao tác.
* Người dùng hủy thao tác: Use case kết thúc, không thay đổi dữ liệu.

## Hậu điều kiện

* Nếu thành công: Thao tác quản lý lớp học được thực hiện và cập nhật vào hệ thống.
* Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.

## Liên kết

* Activity Diagram: [AD_ClassManager.puml]
* Form liên quan: SCR_ClassManager
* Các use case chi tiết: UC_ClassManager_Create, UC_ClassManager_Update, UC_ClassManager_Delete, UC_ClassManager_Search, UC_ClassManager_Detail, UC_ClassManager_AssignTeacher, UCClassManager_AssignStudent
* Các entity liên quan: ENT_Class, ENT_Student, ENT_Teacher, ENT_Enrollment, ENT_ClassTeacher