# Use Case: Chỉnh sửa lớp học

## User Story
- Là Quản trị viên, tôi muốn chỉnh sửa thông tin lớp học đã tồn tại, để có thể cập nhật hoặc bổ sung các thông tin

## Acceptance criteria
- Khi quản trị viên chọn Chỉnh sửa lớp học, hệ thống hiển thị form thông tin lớp học đã lưu sẵn. Các thông tin đã lưu được hiển thị trong form
- Hệ thống cho phép chỉnh sửa các trường:
    - Tên lớp (bắt buộc)
    - Ngày bắt đầu (bắt buộc)
    - Ngày kết thúc (bắt buộc)
- Nếu quản trị viên để trống trường bắt buộc, hệ thống hiển thị thông báo lỗi: "Vui lòng nhập đầy đủ thông tin bắt buộc"
- Nếu ngày bắt đầu >= ngày kết thúc, hệ thống hiển thị thông báo lỗi: "Ngày bắt đầu phải nhỏ hơn ngày kết thúc".
- Khi dữ liệu hợp lệ và nhấn Lưu, hệ thống cập nhật thông tin lớp học.
- Sau khi lưu thành công, hệ thống hiển thị thông báo: "Cập nhật thông tin lớp học thành công".
- Lớp học sau khi chỉnh sửa phải hiển thị đầy đủ thông tin cập nhật trong danh sách lớp học.

## Tác nhân chính
⦁	Người dùng (có quyền chỉnh sửa lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền chỉnh sửa lớp học.
## Luồng chính
1.	Người dùng bấm nút "Chỉnh sửa" 1 bản ghi trên giao diện danh sách quản lý lớp học.
2.	Hệ thống hiển thị form lớp học (SCR_ClassUpdate).
3.	Người dùng nhập thông tin lớp học:
⦁	Có thể nhập trực tiếp các trường thông tin.
⦁	Có thể chỉnh sửa lại thông tin đã nhập.
4.	Người dùng nhấn "Lưu" để lưu lớp học.
5.	Hệ thống kiểm tra dữ liệu:
⦁	Nếu dữ liệu hợp lệ:
⦁	Cập nhật thông tin lớp học vào cơ sở dữ liệu (ENT_Class).
⦁	Thông báo chỉnh sửa thành công.
⦁	Cập nhật lại danh sách lớp học (ENT_Class).
⦁	Kết thúc use case.
⦁	Nếu dữ liệu không hợp lệ
⦁	Hiển thị lỗi validation.
⦁	Quay lại bước nhập/chỉnh sửa thông tin.
6.	Người dùng có thể tiếp tục chỉnh sửa và lặp lại các bước trên hoặc hủy thao tác để kết thúc.
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác chỉnh sửa lớp học: Use case kết thúc, không cập nhật dữ liệu.
⦁	Lỗi hệ thống: Use case kết thúc, không cập nhật dữ liệu.
## Hậu điều kiện
⦁	Nếu thành công: thông tin lớp học được cập nhật vào hệ thống.
⦁	Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_ClassManager_Update.puml]
⦁	Form liên quan: SCR_ClassUpdate
⦁	Entity liên quan: ENT_Class