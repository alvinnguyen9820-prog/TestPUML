# Use Case: xem chi tiết lớp học

## User Story
- Là Quản trị viên, tôi muốn xem chi tiết thông tin lớp học, để có thể theo dõi chi tiết thông tin chung lớp học, danh sách sinh viên, danh sách giảng viên trong lớp

## Acceptance criteria
-  Khi quản trị viên chọn xem chi tiết lớp học, hệ thống hiển thị popup chi tiết thông tin lớp học với các trường:
    - Tên lớp 
    - Danh sách giảng viên đã phân công
    - Tổng số lượng giảng viên
    - Danh sách sinh viên đã phân công
    - Tổng số lượng sinh viên
    - Ngày bắt đầu 
    - Ngày kết thúc 
- Nếu lớp học chưa có sinh viên hoặc giảng viên, hệ thống hiển thị thông báo: "Chưa có sinh viên/giảng viên trong lớp này".

## Tác nhân chính
⦁	Người dùng (có quyền xem chi tiết lớp học)

## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền xem chi tiết lớp học.

## Luồng chính
1.	Người dùng truy cập danh sách lớp học, nhấn nút "Xem chi tiết" trên 1 bản ghi lớp học.
2.	Hệ thống hiển thị form chi tiết thông tin lớp học (SCR_ClassDetail) bao gồm các thông tin
    - Tên lớp 
    - Danh sách giảng viên đã phân công
    - Tổng số lượng giảng viên
    - Danh sách sinh viên đã phân công
    - Tổng số lượng sinh viên
    - Ngày bắt đầu 
    - Ngày kết thúc 
## Luồng phụ/ngoại lệ
⦁	Người dùng bấm nút đóng hoặc biểu tượng x: hệ thống đóng popup xem chi tiết thông tin
## Hậu điều kiện
⦁	Nếu thành công: Hiển thị chi tiết thông tin lớp học, danh sách sinh viên, giảng viên trong lớp.
⦁	Nếu lỗi hệ thống/Thất bại: Hiển thị thông báo lỗi và yêu cầu thử lại.

## Liên kết
⦁	Activity Diagram: [AD_ClassManager_Detail.puml]
⦁	Form liên quan: SCR_ClassDetail
⦁	Entity liên quan: ENT_Class, ENT_Student, ENT_Teacher, ENT_Enrollment, ENT_ClassTeacher