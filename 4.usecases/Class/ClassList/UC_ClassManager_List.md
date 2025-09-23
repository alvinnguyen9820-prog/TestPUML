# Use Case: Quản lý danh sách lớp học

## Mục đích

Cho phép người dùng xem danh sách lớp học

## Tác nhân chính

* Admin

## Tiền điều kiện

* Người dùng đã đăng nhập hệ thống và có quyền truy cập chức năng quản lý lớp học.

## Luồng chính

1. Người dùng truy cập chức năng quản lý lớp học.
2. Hệ thống kiểm tra quyền truy cập.
3. Hệ thống hiển thị danh sách lớp học

## Luồng phụ/ngoại lệ

* Người dùng không có quyền truy cập: Hệ thống hiển thị thông báo lỗi và không cho phép truy cập chức năng.

## Hậu điều kiện

## Liên kết

* Activity Diagram: [AD_ClassManager_List.puml]
* Form liên quan: SCR_ClassManager
* Entity liên quan: ENT_Class
