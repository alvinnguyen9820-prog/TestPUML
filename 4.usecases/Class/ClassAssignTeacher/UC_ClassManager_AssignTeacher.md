# Use Case: Phân công giảng viên

## User Story
- Là quản trị viên, tôi muốn có thể thực hiện phân công một hoặc nhiều giảng viên vào lớp học đã tạo, để có thể quản lý danh sách giảng viên trong lớp học

## Acceptance criteria
- Hệ thống hiển thị thành công form phân công giảng viên, trong form hiển thị danh sách giảng viên (tên) và checkbox lựa chọn giảng viên
- Người dùng tìm kiếm thành công giảng viên để thêm vào lớp
- Hệ thống hiển thị kết quả đánh dấu danh sách giảng viên của người dùng
- Sau khi bấm lưu, hệ thống cập nhật thành công danh sách giảng viên trong lớp học

## Tác nhân chính
⦁	Người dùng (có quyền phân công giảng viên vào lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền phân công giảng viên vào lớp học.
## Luồng chính
1.	Người dùng truy cập danh sách lớp học, nhấn nút "Phân công giảng viên" trên 1 bản ghi lớp học.
2.	Hệ thống hiển thị popup phân công giảng viên vào lớp học (SCR_AssignTeacher).
3.	Người dùng lựa chọn thao tác:
⦁	Nếu có thực hiện tìm kiếm:
⦁	Nhập họ tên hoặc mã giảng viên.
⦁	Hệ thống hiển thị danh sách giảng viên theo điều kiện tìm kiếm.
⦁	Nếu không thực hiện tìm kiếm:
⦁	Hệ thống hiển thị danh sách giảng viên mặc định
4.	Người dùng chọn 1 hoặc nhiều giảng viên trên danh sách giảng viên.
5.	Người dùng nhấn nút lưu, hệ thống kiểm tra tính hợp lệ của dữ liệu (trùng thời gian học của giảng viên/giảng viên đã nghỉ học):
⦁	Nếu dữ liệu hợp lệ:
⦁	Lưu dữ liệu phân công giảng dạy của giảng viên vào cơ sở dữ liệu (ENT_ClassTeacher).
⦁	Thông báo phân công giảng viên vào lớp học thành công.
⦁	Đóng popup phân công.
⦁	Kết thúc use case.
⦁	Nếu dữ liệu không hợp lệ:
⦁	Thông báo lỗi "giảng viên đã được phân công vào lớp học khác hoặc giảng viên đã nghỉ dạy học".
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác phân công giảng viên: Use case kết thúc, không lưu dữ liệu.
⦁	Lỗi hệ thống: Use case kết thúc, không lưu dữ liệu.
## Hậu điều kiện
⦁	Nếu thành công: phân công giảng viên vào lớp học được lưu vào hệ thống và hiển thị danh sách giảng viên đã được phân công trong form chi tiết lớp học.
⦁	Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_Classmanager_AssignTeacher.puml]
⦁	Form liên quan: SCR_AssignTeacher
⦁	Entity liên quan: ENT_ClassTeacher, ENT_Class, ENT_Teacher