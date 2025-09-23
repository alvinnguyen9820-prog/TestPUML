# Use Case: Xóa lớp học
## Mục đích
Cho phép người dùng xóa lớp học.
## Tác nhân chính
⦁	Người dùng (có quyền xóa lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền xóa lớp học
## Luồng chính
1.	Người dùng chọn 1 bản ghi cần xóa trên danh sách lớp học.
2.	Hệ thống hiển thị popup xác nhận xóa lớp học (SCR_ClassDelete).
3.	Người dùng xác nhận xóa bản ghi
⦁	Nếu đủ điều kiện:
⦁	Thực hiện xóa bản ghi lớp học trên danh sách, không xóa trong CSDL (ENT_Class).
⦁	Thông báo xóa lớp học thành công.
⦁	Cập nhật lại danh sách lớp học (ENT_Class).
⦁	Kết thúc use case.
⦁	Nếu không đủ điều kiện xóa
⦁	Thông báo xóa lớp học thất bại..
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác xóa lớp học: Use case kết thúc, không thực hiện xóa dữ liệu.
⦁	Lỗi hệ thống: Use case kết thúc, không xóa dữ liệu.
## Hậu điều kiện
⦁	Nếu xóa thành công: lớp học được xóa và không hiển thị trên danh sách.
⦁	Nếu thất bại hoặc lỗi hệ thống: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_ClassManager_Delete.puml]
⦁	Form liên quan: SCR_ClassDelete
⦁	Entity liên quan: ENT_Class