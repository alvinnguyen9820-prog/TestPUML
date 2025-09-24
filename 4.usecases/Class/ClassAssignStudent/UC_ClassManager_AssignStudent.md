# Use Case: Phân công sinh viên

## User Story
- Là quản trị viên, tôi muốn có thể thực hiện phân công một hoặc nhiều sinh viên vào lớp học đã tạo, để có thể quản lý danh sách sinh viên trong lớp học

## Acceptance criteria
- Hệ thống hiển thị thành công form phân công sinh viên, trong form hiển thị danh sách sinh viên (tên) và checkbox lựa chọn sinh viên
- Người dùng tìm kiếm thành công sinh viên để thêm vào lớp
- Hệ thống hiển thị kết quả đánh dấu danh sách sinh viên của người dùng
- Sau khi bấm lưu, hệ thống cập nhật thành công danh sách sinh viên trong lớp học nếu các dữ liệu đều hợp lệ
- Nếu sinh viên bị trùng thời gian học hoặc sinh viên đã nghỉ học, hệ thống hiển thị cảnh báo lỗi "Sinh viên A đã được phân công vào lớp học khác hoặc sinh viên đã nghỉ học"

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