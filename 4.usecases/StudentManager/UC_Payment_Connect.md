# Use Case: Kết nối ngân hàng/ví điện tử

## Mục đích
Cho phép người dùng kết nối tài khoản ngân hàng hoặc ví điện tử vào hệ thống để thực hiện các giao dịch thanh toán.

## Tác nhân chính
- Người dùng

## Tiền điều kiện
- Người dùng đã đăng nhập hệ thống.

## Luồng chính
1. Người dùng chọn chức năng kết nối ngân hàng/ví điện tử.
2. Hệ thống hiển thị danh sách các kết nối đã có (**SCR_PaymentConnect**).
3. Hệ thống hiển thị danh sách các loại kết nối hỗ trợ cùng các lựa chọn (**SCR_PaymentConnect**).
4. Người dùng chọn loại kết nối (ngân hàng hoặc ví điện tử).
5. Người dùng thực hiện xác thực kết nối (bằng app ngân hàng, ví điện tử hoặc OTP).
6. Hệ thống kiểm tra xác thực:
   - Nếu xác thực thành công:
     - Lưu thông tin kết nối vào cơ sở dữ liệu (**ENT_PaymentMethod**).
     - Thông báo kết nối thành công.
     - Kết thúc use case.
   - Nếu xác thực thất bại:
     - Thông báo xác thực thất bại.
     - Cho phép người dùng thử lại hoặc hủy thao tác.

## Luồng phụ/ngoại lệ
- Người dùng hủy thao tác kết nối: Use case kết thúc, không lưu dữ liệu.
- Người dùng xác thực thất bại nhiều lần.

## Hậu điều kiện
- Nếu thành công: Thông tin kết nối ngân hàng/ví điện tử được lưu vào hệ thống và hiển thị trong danh sách.
- Nếu thất bại hoặc hủy: Không có thay đổi nào trong hệ thống.

## Liên kết
- Activity Diagram: [AD_Payment_Connect.puml](AD_Payment_Connect.puml)
- Form liên quan: **SCR_PaymentConnect**
- Entity liên quan: **ENT_PaymentMethod**
