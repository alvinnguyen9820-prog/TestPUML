# Màn hình: Danh sách sinh viên
Nơi tập trung để xem và quản lý sinh viên.

## Điều kiện tiên quyết:

- Người dùng đã đăng nhập và là Admin.

## Nguyên mẫu
[https://www.figma.com/design/STv6BI8XR469xhObHjgCHs/Test-Puml?node-id=1-13684&t=wrQJFoVLqh8Cg2iN-0]

## Thành phần

### Bảng chính

<div style="overflow-x:auto">

| Trường thông tin | Control  | Field       | Max length | Bắt buộc (Y/N) | Giá trị mặc định | Cho phép sửa (Y/N) | Mô tả                                      |
| :--------------- | :------- | :---------- | :--------- | :------------- | :--------------- | :----------------- | :----------------------------------------- |
| Tên sinh viên    | text     | studentName | -          | -              |                  | N                  |                                            |
| Giới tính        | text     | gender      | -          | -              |                  | N                  |                                            |
| Ngày sinh        | datetime | dob         | -          | -              |                  | N                  |                                            |
| Trạng thái       | text     | status      | -          | -              |                  | N                  |                                            |
| Chức năng        | icon     | -           | -          | -              |                  | N                  | Click vao hien thi danh sách nut chuc nang |

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
| Tìm kiếm             | Input  | Điền thông tin tên sinh viên để tìm kiếm            |
| Reset                | button | Xóa thông tin đã nhập trên input tìm kiếm           |

</div>

