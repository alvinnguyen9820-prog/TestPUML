# Màn hình: Danh sách lớp học
Nơi tập trung để xem và quản lý lớp học.

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[Đặt thiết kế figma tại đây]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin   | Control     | Field   | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                                       |
| :----------------- | :---------- | :------ | :--------- | :------------- | :--------------- | :----------------- | :------------------------------------------ |
| Tên lớp học        | textbox     | lopHoc  | 100        | Y              |                  | Y                  | Thông tin tên lớp học                       |
| Số lượng sinh viên | numericbox  | nam     | 6          | Y              | 50               | Y                  | Thông tin số lượng sinh viên trong lớp học. |
| Thời gian bắt đầu  | date picker | batDau  | -          | Y              | Ngày hiện tại    | Y                  | Thời gian bắt đầu lớp học                   |
| Thời gian kết thúc | date picker | ketThuc | -          | Y              |                  | Y                  | Thời gian kết thúc lớp học                  |



</div>

### Khác

<div style="overflow-x:auto">

| Tên                  | Loại   | Mô tả |
| :------------------- | :----- | :---- |
| Thêm mới             | Button |       |
| Sửa                  | Button |       |
| Xóa                  | Button |       |
| Phân công giảng viên | Button |       |
| Phân công sinh viên  | Button |       |

</div>

