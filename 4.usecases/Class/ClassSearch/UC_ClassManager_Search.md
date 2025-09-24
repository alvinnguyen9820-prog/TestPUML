# Use Case: Tìm kiếm lớp học

## User Story
- Là Quản trị viên, tôi muốn tìm kiếm lớp học theo tên lớp học, để có thể truy xuất thông tin nhanh nhất.

## Acceptance criteria
- Khi quản trị viên truy cập danh sách lớp học, hệ thống hiển thị thanh tìm kiếm.
- Quản trị viên nhập thông tin tìm kiếm và nhấn Tìm kiếm hoặc gõ enter, hệ thống hiển thị danh sách lớp học theo tên lớp đã điền với kết quả gần đúng.
- Nếu không tìm thấy lớp học nào, hệ thống hiển thị thông báo: "Không tìm thấy lớp học phù hợp".

## Tác nhân chính
⦁	Người dùng (có quyền tìm kiếm lớp học)
## Tiền điều kiện
⦁	Người dùng đã đăng nhập hệ thống và có quyền tìm kiếm lớp học.
## Luồng chính
1.	Người dùng nhập từ khóa tìm kiếm theo tên lớp học, bấm nút "tìm kiếm" trên giao diện danh sách quản lý lớp học.
2.	Hệ thống kiểm tra tính hợp lệ của điều kiện tìm kiếm:
⦁	Nếu hợp lệ:
⦁	Thực hiện truy vấn theo điều kiện tìm kiếm
⦁	Nếu có kết quả:
⦁	Load lại trang danh sách và hiển thị danh sách kết quả tương ứng với điều kiện tìm kiếm (ENT_ClassManager).
⦁	Kết thúc use case.
⦁	Nếu không có kết quả:
⦁	Load lại trang danh sách không có bản ghi nào và hiển thị thông báo "Không có dữ liệu phù hợp với từ khóa tìm kiếm" (ENT_ClassManager).
⦁	Nếu dữ liệu không hợp lệ
⦁	Hiển thị thông báo lỗi "Điều kiện tìm kiếm không hợp lệ"
⦁	Quay lại bước tìm kiếm thông tin.
6.	Người dùng có thể tiếp tục tìm kiếm và lặp lại các bước trên hoặc hủy thao tác để kết thúc.
## Luồng phụ/ngoại lệ
⦁	Người dùng hủy thao tác tìm kiếm lớp học: Use case kết thúc, không cập nhật dữ liệu.
## Hậu điều kiện
⦁	Nếu thành công: thông tin lớp học được cập nhật vào hệ thống.
⦁	Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.
## Liên kết
⦁	Activity Diagram: [AD_ClassManager_Search.puml]
⦁	Form liên quan: SCR_ClassSearch
⦁	Entity liên quan: ENT_Class