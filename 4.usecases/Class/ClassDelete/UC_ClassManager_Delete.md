# Use Case: Xóa lớp học

## User Story
* Là Quản trị viên, tôi muốn xóa lớp học, để có thể loại bỏ những lớp học không còn cần thiết hoặc đã bị tạo nhầm.

## Acceptance Criteria
- Khi quản trị viên chọn Xóa lớp học, hệ thống phải hiển thị hộp thoại xác nhận với nội dung: “Bạn có chắc chắn muốn xóa lớp học này không?”.
- Hệ thống phải cung cấp hai lựa chọn: Đồng ý/Xóa và Hủy.
- Nếu quản trị viên chọn Hủy, hệ thống đóng hộp thoại và lớp học không bị xóa.
- Nếu quản trị viên chọn Đồng ý/Xóa, hệ thống phải kiểm tra điều kiện trước khi xóa:
- Lớp học không có học viên đang theo học.
- Lớp học không ở trạng thái “Đang diễn ra”.
- Nếu vi phạm điều kiện, hệ thống phải hiển thị thông báo lỗi rõ ràng, ví dụ:
“Không thể xóa lớp học vì còn học viên đang theo học.”
“Không thể xóa lớp học đang diễn ra.”
- Nếu thỏa điều kiện, hệ thống phải xóa lớp học khỏi danh sách và cơ sở dữ liệu.
- Sau khi xóa thành công, hệ thống phải hiển thị thông báo: “Xóa lớp học thành công”.
- Hệ thống phải ghi nhận thông tin xóa lớp học vào nhật ký hệ thống bao gồm: người thao tác, thời gian, mã lớp học bị xóa.

## Tác nhân chính
* Quản trị viên

## Tiền điều kiện
*	Người dùng đã đăng nhập hệ thống và có quyền xóa lớp học

## Luồng chính
1.	Người dùng chọn 1 bản ghi cần xóa trên danh sách lớp học.
2.	Hệ thống hiển thị popup xác nhận xóa lớp học (SCR_ClassDelete).
3.	Người dùng xác nhận xóa bản ghi
*	Nếu đủ điều kiện:
*	Thực hiện xóa bản ghi lớp học trên danh sách, không xóa trong CSDL (ENT_Class).
*	Thông báo xóa lớp học thành công.
*	Cập nhật lại danh sách lớp học (ENT_Class).
*	Kết thúc use case.
*	Nếu không đủ điều kiện xóa
*	Thông báo xóa lớp học thất bại..

## Luồng phụ/ngoại lệ
*	Người dùng hủy thao tác xóa lớp học: Use case kết thúc, không thực hiện xóa dữ liệu.
*	Lỗi hệ thống: Use case kết thúc, không xóa dữ liệu.

## Hậu điều kiện
*	Nếu xóa thành công: lớp học được xóa và không hiển thị trên danh sách.
*	Nếu thất bại hoặc lỗi hệ thống: Không có thay đổi nào trong hệ thống.
## Liên kết
*	Activity Diagram: [AD_ClassManager_Delete.puml]
*	Form liên quan: SCR_ClassDelete
*	Entity liên quan: ENT_Class.