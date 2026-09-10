| Test Case ID | Module | Test Scenario | Preconditions | Test Steps | Test Data | Expected Result | Priority |
|---|---|---|---|---|---|---|---|
| **TC-BOOK-001** | Book Cab | Kiểm tra chức năng hợp lệ | Người dùng có quyền truy cập | 1. Mở chức năng<br>2. Nhập dữ liệu hợp lệ<br>3. Nhấn xác nhận | Dữ liệu hợp lệ | Thực hiện thành công | **High** |
| **TC-BOOK-002** | Book Cab | Kiểm tra dữ liệu không hợp lệ | Hệ thống hoạt động | 1. Nhập dữ liệu sai<br>2. Xác nhận | Dữ liệu sai | Hiển thị thông báo lỗi | **High** |
| **TC-BOOK-003** | Book Cab | Kiểm tra trường bắt buộc rỗng | Ở màn hình chức năng | 1. Để trống trường bắt buộc<br>2. Xác nhận | Giá trị rỗng | Hiển thị lỗi Required | **High** |
| **TC-BOOK-004** | Book Cab | Kiểm tra ngoại lệ hệ thống | Mất kết nối hoặc tài nguyên không khả dụng | 1. Thực hiện thao tác | Exception data | Thông báo lỗi hệ thống, không crash | **Medium** |
| **TC-BOOK-005** | Book Cab | Kiểm tra Business Rule | Thỏa điều kiện biên | 1. Nhập dữ liệu biên<br>2. Xác nhận | Edge/Boundary | Đúng quy tắc nghiệp vụ | **Medium** |
