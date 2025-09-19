# Màn hình: Chỉnh sửa giảng viên
Popup chỉnh sửa giảng viên

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-25059&t=wrQJFoVLqh8Cg2iN-0]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin | Control  | Field       | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả |
| :--------------- | :------- | :---------- | :--------- | :------------- | :--------------- | :----------------- | :---- |
| Tên giảng viên   | text     | teacherName | -          | Y              |                  | Y                  |       |
| Giới tính        | dropdown | gender      | -          | Y              |                  | Y                  |       |
| Ngày sinh        | datetime | dob         | -          | Y              |                  | Y                  |       |
| Trạng thái       | dropdown | status      | -          | -              |                  | Y                  |       |


</div>

### Khác

<div style="overflow-x:auto">

| Tên          | Loại   | Mô tả                           |
| :----------- | :----- | :------------------------------ |
| Biểu tượng x | Button | Click vào sẽ đóng popup         |
| Đóng         | Button | Click vào đóng popup            |
| Lưu          | Button | Click vào thực hiện lưu bản ghi |

</div>

