# Use Case: Thêm mới lớp học

## User Story
- Là Quản trị viên, tôi muốn thêm mới lớp học, để có thể quản lý danh sách và thông tin trong hệ thống

## Acceptance criteria
-  Khi quản trị viên chọn Thêm mới lớp học, hệ thống hiển thị form nhập thông tin lớp học với các trường:
    - Tên lớp (bắt buộc)
    - Ngày bắt đầu (bắt buộc)
    - Ngày kết thúc (bắt buộc)
- Nếu để trống trường bắt buộc, hệ thống hiển thị thông báo lỗi: "Vui lòng nhập đầy đủ thông tin bắt buộc".
- Nếu ngày bắt đầu >= ngày kết thúc, hệ thống hiển thị thông báo lỗi: "Ngày bắt đầu phải nhỏ hơn ngày kết thúc".
- Khi dữ liệu hợp lệ và nhấn Lưu, hệ thống lưu lớp học mới và hiển thị trong danh sách
- Sau khi lưu thành công, hệ thống hiển thị thông báo: "Thêm mới lớp học thành công".

## Tác nhân chính
⦁	Người dùng (có quyền tạo mới lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền tạo lớp học.
## Luồng chính
1.	Người dùng bấm nút "Thêm mới" trên giao diện danh sách quản lý lớp học.
2.	Hệ thống hiển thị form lớp học (SCR_ClassCreate).
3.	Người dùng nhập thông tin lớp học:
⦁	Có thể nhập trực tiếp các trường thông tin.
⦁	Có thể chỉnh sửa lại thông tin đã nhập.
4.	Người dùng nhấn "Lưu" để lưu lớp học.
5.	Hệ thống kiểm tra dữ liệu:
⦁	Nếu dữ liệu hợp lệ:
⦁	Lưu lớp học vào cơ sở dữ liệu (ENT_Class).
⦁	Thông báo thành công.
⦁	Cập nhật lại danh sách lớp học (ENT_Class).
⦁	Kết thúc use case.
⦁	Nếu dữ liệu không hợp lệ
⦁	Hiển thị lỗi validation.
⦁	Quay lại bước nhập/chỉnh sửa thông tin.
6.	Người dùng có thể tiếp tục chỉnh sửa và lặp lại các bước trên hoặc hủy thao tác để kết thúc.
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác tạo lớp học: Use case kết thúc, không lưu dữ liệu.
⦁	Lỗi hệ thống: Use case kết thúc, không lưu dữ liệu.
## Hậu điều kiện
⦁	Nếu thành công: lớp học mới được lưu vào hệ thống và hiển thị trong danh sách.
⦁	Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_ClassManager_Create.puml]
⦁	Form liên quan: SCR_ClassCreate
⦁	Entity liên quan: ENT_Class