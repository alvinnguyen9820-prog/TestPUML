# Use Case: Phân công sinh viên
## Mục đích
Cho phép người dùng phân công sinh viên vào lớp học.
## Tác nhân chính
⦁	Người dùng (có quyền phân công sinh viên vào lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền phân công sinh viên vào lớp học.
## Luồng chính
1.	Người dùng truy cập danh sách lớp học, nhấn nút "Phân công sinh viên" trên 1 bản ghi lớp học.
2.	Hệ thống hiển thị popup phân công sinh viên vào lớp học (SCR_AssignStudent).
3.	Người dùng lựa chọn thao tác:
⦁	Nếu có thực hiện tìm kiếm:
⦁	Nhập họ tên hoặc mã sinh viên.
⦁	Hệ thống hiển thị danh sách sinh viên theo điều kiện tìm kiếm.
⦁	Nếu không thực hiện tìm kiếm:
⦁	Hệ thống hiển thị danh sách sinh viên mặc định
4.	Người dùng chọn 1 hoặc nhiều sinh viên trên danh sách sinh viên.
5.	Người dùng nhấn nút lưu, hệ thống kiểm tra tính hợp lệ của dữ liệu (trùng thời gian học của sinh viên/Sinh viên đã nghỉ học):
⦁	Nếu dữ liệu hợp lệ:
⦁	Lưu dữ liệu đăng ký lớp học của sinh viên vào cơ sở dữ liệu (ENT_Enrollment).
⦁	Thông báo phân công sinh viên vào lớp học thành công.
⦁	Đóng popup phân công.
⦁	Kết thúc use case.
⦁	Nếu dữ liệu không hợp lệ:
⦁	Thông báo lỗi "Sinh viên đã được phân công vào lớp học khác hoặc sinh viên đã nghỉ học".
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác phân công sinh viên: Use case kết thúc, không lưu dữ liệu.
⦁	Lỗi hệ thống: Use case kết thúc, không lưu dữ liệu.
## Hậu điều kiện
⦁	Nếu thành công: phân công sinh viên vào lớp học được lưu vào hệ thống và hiển thị danh sách sinh viên đã được phân công trong form chi tiết lớp học.
⦁	Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_Classmanager_AssignStudent.puml]
⦁	Form liên quan: SCR_AssignStudent
⦁	Entity liên quan: ENT_Enrollment, ENT_Class, ENT_Student