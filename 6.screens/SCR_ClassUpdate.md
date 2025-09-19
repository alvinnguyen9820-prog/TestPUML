# Màn hình: Chỉnh sửa thông tin lớp học
Popup chỉnh sửa thông tin lớp học, chỉnh sửa danh sách sinh viên và giảng viên trong lớp học

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-36319&t=C7PRvj1Utbi7VV69-1]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin   | Control         | Field     | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                               |
| :----------------- | :-------------- | :-------- | :--------- | :------------- | :--------------- | :----------------- | :---------------------------------- |
| Tên lớp học        | text            | className | -          | -              |                  | -                  | Thông tin tên lớp học               |
| Thời gian bắt đầu  | dateime         | startDate | -          | -              |                  | -                  | Thời gian bắt đầu lớp học           |
| Thời gian kết thúc | dateime         | endDate   | -          | -              |                  | -                  | Thời gian kết thúc lớp học          |
| Sinh viên          | combobox search |           | -          | -              |                  | -                  | Chọn sinh viên từ danh sách đã tạo  |
| Giảng viên         | combobox search |           | -          | -              |                  | -                  | Chọn giảng viên từ danh sách đã tạo |


</div>

### Khác

<div style="overflow-x:auto">

| Tên          | Loại   | Mô tả                           |
| :----------- | :----- | :------------------------------ |
| Biểu tượng x | Button | Click vào sẽ đóng popup         |
| Đóng         | Button | Click vào đóng popup            |
| Lưu          | Button | Click vào thực hiện lưu bản ghi |

</div>

