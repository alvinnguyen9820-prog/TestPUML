# Màn hình: Chỉnh sửa lớp học
Popup chỉnh sửa lớp học, phân công sinh viên và giảng viên vào lớp học

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-36319&t=wrQJFoVLqh8Cg2iN-0]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin   | Control         | Field     | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                               |
| :----------------- | :-------------- | :-------- | :--------- | :------------- | :--------------- | :----------------- | :---------------------------------- |
| Tên lớp học        | text            | className | -          | Y              |                  | Y                  | Thông tin tên lớp học               |
| Thời gian bắt đầu  | dateime         | startDate | -          | Y              | Ngày hiện tại    | Y                  | Thời gian bắt đầu lớp học           |
| Thời gian kết thúc | dateime         | endDate   | -          | Y              |                  | Y                  | Thời gian kết thúc lớp học          |
| Sinh viên          | combobox search |           | -          | -              |                  | Y                  | Chọn sinh viên từ danh sách đã tạo  |
| Giảng viên         | combobox search |           | -          | -              |                  | Y                  | Chọn giảng viên từ danh sách đã tạo |


</div>

### Khác

<div style="overflow-x:auto">

| Tên          | Loại   | Mô tả                           |
| :----------- | :----- | :------------------------------ |
| Biểu tượng x | Button | Click vào sẽ đóng popup         |
| Đóng         | Button | Click vào đóng popup            |
| Lưu          | Button | Click vào thực hiện lưu bản ghi |

</div>

