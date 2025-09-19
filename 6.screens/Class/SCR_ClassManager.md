# Màn hình: Danh sách lớp học
Nơi tập trung để xem và quản lý lớp học.

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-5217&t=C7PRvj1Utbi7VV69-1]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin   | Control  | Field        | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                                      |
| :----------------- | :------- | :----------- | :--------- | :------------- | :--------------- | :----------------- | :----------------------------------------- |
| Tên lớp học        | text     | className    | -          | -              |                  | -                  | Thông tin tên lớp học                      |
| Thời gian bắt đầu  | datetime | startDate    | -          | -              |                  | -                  | Thời gian bắt đầu lớp học                  |
| Thời gian kết thúc | datetime | endDate      | -          | -              |                  | -                  | Thời gian kết thúc lớp học                 |
| Số lượng sinh viên | number   | countStudent | -          | -              |                  | -                  | Tổng số lượng sinh viên                    |
| Chức năng          | icon     | -            | -          | -              |                  | -                  | Click vao hien thi danh sách nut chuc nang |


</div>

### Khác

<div style="overflow-x:auto">

| Tên                  | Loại   | Mô tả                                               |
| :------------------- | :----- | :-------------------------------------------------- |
| Tìm kiếm             | Button | Click vào thực hiện tìm kiếm theo thông tin đã nhập |
| Xem chi tiết         | Button | Bấm vào mở popup xem chi tiết                       |
| Thêm mới             | Button | Bấm vào mở popup thêm mới                           |
| Sửa                  | Button | Bấm vào mở popup chỉnh sửa                          |
| Xóa                  | Button | Bấm vào mở popup xác nhận                           |
| Phân công giảng viên | Button | Bấm vào mở popup phân công giảng viên               |
| Phân công sinh viên  | Button | Bấm vào mở popup phân công sinh viên                |
| Tìm kiếm             | Input  | Điền thông tin tên lớp học để tìm kiếm              |
| Reset                | button | Xóa thông tin đã nhập trên input tìm kiếm           |

</div>

