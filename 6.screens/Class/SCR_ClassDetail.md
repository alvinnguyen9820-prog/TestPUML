# Màn hình: Xem thông tin chi tiết lớp học
Popup xem thông tin chi tiết lớp học, xem danh sinh viên và giảng viên được phân công vào lớp học

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin, Sinh viên, Giảng viên.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-48553&t=C7PRvj1Utbi7VV69-1]

## Thành phần

### Thông tin chinh

<div style="overflow-x:auto">

| Trường thông tin   | Control  | Field     | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                      |
| :----------------- | :------- | :-------- | :--------- | :------------- | :--------------- | :----------------- | :------------------------- |
| Tên lớp học        | text     | className | -          | -              |                  | -                  | Thông tin tên lớp học      |
| Thời gian bắt đầu  | datetime | startDate | -          | -              |                  | -                  | Thời gian bắt đầu lớp học  |
| Thời gian kết thúc | datetime | endDate   | -          | -              |                  | -                  | Thời gian kết thúc lớp học |

</div>

### Danh sách sinh viên

<div style="overflow-x:auto">

| Trường thông tin | Control | Field       | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả         |
| :--------------- | :------ | :---------- | :--------- | :------------- | :--------------- | :----------------- | :------------ |
| STT              | text    | -           | -          | -              |                  | -                  | STT           |
| Tên sinh viên    | text    | studentName | -          | -              |                  | -                  | Tên sinh viên |

</div>

### Danh sách giảng viên

<div style="overflow-x:auto">

| Trường thông tin | Control | Field       | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả          |
| :--------------- | :------ | :---------- | :--------- | :------------- | :--------------- | :----------------- | :------------- |
| STT              | text    | -           | -          | -              |                  | -                  | STT            |
| Tên giảng viên   | text    | teacherName | -          | -              |                  | -                  | Tên giảng viên |

</div>

### Khác

<div style="overflow-x:auto">

| Tên          | Loại   | Mô tả                   |
| :----------- | :----- | :---------------------- |
| Biểu tượng x | Button | Click vào sẽ đóng popup |
| Đóng         | Button | Click vào đóng popup    |

</div>

