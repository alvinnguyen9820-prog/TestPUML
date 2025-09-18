# Use Case: Tạo tờ khai thuế

## Mục đích
Cho phép người dùng tạo mới tờ khai thuế.

## Tác nhân chính
- Người dùng (có quyền tạo tờ khai thuế)

## Tiền điều kiện
- Người dùng đã đăng nhập hệ thống và có quyền tạo tờ khai thuế.

## Luồng chính
1. Người dùng bấm nút "Tạo tờ khai" trên giao diện.
2. Hệ thống hiển thị form tờ khai thuế (**SCR_TaxDeclarationForm**).
3. Người dùng nhập thông tin tờ khai:
   - Có thể nhập trực tiếp các trường thông tin.
   - Có thể hỏi đáp với AI để hỗ trợ điền thông tin.
   - Có thể chỉnh sửa lại thông tin đã nhập.
4. Người dùng nhấn "Lưu" để lưu tờ khai.
5. Hệ thống kiểm tra dữ liệu:
   - Nếu dữ liệu hợp lệ:
     - Lưu tờ khai vào cơ sở dữ liệu (**ENT_TaxDeclaration**).
     - Thông báo thành công.
     - Cập nhật lại danh sách tờ khai (**ENT_TaxDeclaration**).
     - Kết thúc use case.
   - Nếu dữ liệu không hợp lệ:
     - Hiển thị lỗi validation.
     - Quay lại bước nhập/chỉnh sửa thông tin.
6. Người dùng có thể tiếp tục chỉnh sửa và lặp lại các bước trên hoặc hủy thao tác để kết thúc.

## Luồng phụ/ngoại lệ
- Người dùng hủy thao tác tạo tờ khai: Use case kết thúc, không lưu dữ liệu.

## Hậu điều kiện
- Nếu thành công: Tờ khai thuế mới được lưu vào hệ thống và hiển thị trong danh sách.
- Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.

## Liên kết
- Activity Diagram: [AD_TaxDeclaration_Create.puml](AD_TaxDeclaration_Create.puml)
- Form liên quan: **SCR_TaxDeclarationForm**
- Entity liên quan: **ENT_TaxDeclaration**
