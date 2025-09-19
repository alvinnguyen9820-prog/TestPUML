# Màn hình: Xem thông tin chi tiết sinh viên
Popup xem thông tin chi tiết sinh viên

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin, Sinh viên, Giảng viên.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-43659&t=wrQJFoVLqh8Cg2iN-0]

## Thành phần

### Thông tin chinh

<div style="overflow-x:auto">

| Trường thông tin | Control  | Field       | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả |
| :--------------- | :------- | :---------- | :--------- | :------------- | :--------------- | :----------------- | :---- |
| Tên sinh viên    | text     | studentName | -          | -              |                  | N                  |       |
| Giới tính        | text     | gender      | -          | -              |                  | N                  |       |
| Ngày sinh        | datetime | dob         | -          | -              |                  | N                  |       |
| Trạng thái       | text     | status      | -          | -              |                  | N                  |       |

</div>


### Khác

<div style="overflow-x:auto">

| Tên          | Loại   | Mô tả                   |
| :----------- | :----- | :---------------------- |
| Biểu tượng x | Button | Click vào sẽ đóng popup |
| Đóng         | Button | Click vào đóng popup    |

</div>

