                                Dự án xây dựng hệ thống CAB System – Nền tảng đặt xe

B1:bussiness content
| Nội dung               | Mô tả                                                                                       |
| ---------------------- | ------------------------------------------------------------------------------------------- |
| **Business**           | Công ty ABC cung cấp dịch vụ đặt xe trực tuyến                                              |
| **Vấn đề hiện tại**    | Phân công tài xế thủ công, khó theo dõi chuyến, thanh toán chưa tập trung, khó mở rộng      |
| **Mục tiêu**           | Xây dựng nền tảng CAB có khả năng phục vụ nhiều khách hàng/tài xế và dễ mở rộng             |
| **Khách hàng**         | Đăng ký, đặt xe, theo dõi chuyến, thanh toán, xem lịch sử, đánh giá tài xế                  |
| **Tài xế**             | Quản lý hồ sơ/phương tiện, nhận/từ chối chuyến, cập nhật trạng thái, chia sẻ vị trí         |
| **Nhân viên vận hành** | Quản lý khách hàng, tài xế, phương tiện, chuyến đi, giao dịch và báo cáo                    |
| **Business goal**      | Tự động hóa điều phối, nâng cao trải nghiệm khách hàng, tăng khả năng mở rộng và độ ổn định |
| **Yêu cầu quan trọng** | Matching tài xế, thanh toán, thông báo, quản trị, bảo mật, logging, báo cáo                 |
| **Yêu cầu tương lai**  | Thêm dịch vụ, phương thức thanh toán, nhà cung cấp thông báo và thay đổi công nghệ dễ dàng  |




B2: tìm va xac nhan cac stack folder, ve ma tran vẽ trong cho biet tam anh huong quan trong cua stak trong he thong gom ten stack folder va vai tro cua no
| STT | Stack / Folder                     | Vai trò trong hệ thống CAB                                   | Mức độ quan trọng |
| --- | ---------------------------------- | ------------------------------------------------------------ | ----------------- |
| 1   | **Frontend / Client**              | Giao diện cho khách hàng, tài xế và nhân viên vận hành       | Cao               |
| 2   | **API / Backend**                  | Xử lý nghiệp vụ và kết nối các thành phần của hệ thống       | Rất cao           |
| 3   | **Authentication & Authorization** | Đăng nhập, xác thực và phân quyền người dùng                 | Rất cao           |
| 4   | **Ride Management**                | Tạo, quản lý và cập nhật trạng thái chuyến đi                | Rất cao           |
| 5   | **Driver Matching / Dispatch**     | Tìm kiếm và phân công tài xế phù hợp                         | Rất cao           |
| 6   | **Location / GPS**                 | Theo dõi vị trí tài xế và hỗ trợ tìm tài xế gần khách        | Cao               |
| 7   | **Pricing / Fare**                 | Tính cước chuyến đi                                          | Cao               |
| 8   | **Payment**                        | Xử lý thanh toán tiền mặt và điện tử                         | Rất cao           |
| 9   | **Notification**                   | Gửi thông báo cho khách hàng và tài xế                       | Cao               |
| 10  | **Database**                       | Lưu trữ tài khoản, chuyến đi, tài xế, phương tiện, giao dịch | Rất cao           |
| 11  | **Message Queue / Event Bus**      | Xử lý bất đồng bộ giữa các thành phần                        | Cao               |
| 12  | **Admin / Operation**              | Quản lý khách hàng, tài xế, chuyến đi và vận hành            | Cao               |
| 13  | **Reporting / Analytics**          | Thống kê chuyến, doanh thu và hiệu quả hoạt động             | Trung bình        |
| 14  | **Logging / Audit**                | Lưu vết thao tác và hỗ trợ kiểm tra sự cố                    | Cao               |
| 15  | **External Services**              | Tích hợp cổng thanh toán, bản đồ, SMS/Push Notification      | Cao              

<img width="946" height="684" alt="image" src="https://github.com/user-attachments/assets/2d871e55-ed68-4f56-8412-df2c724f3153" />


B3. Mục tiêu nghiệp vụ (Business Goals)
| Mã       | Business Goal             | Mục tiêu                                                                                        |
| -------- | ------------------------- | ----------------------------------------------------------------------------------------------- |
| **BG01** | **Tự động tìm tài xế**    | Tự động xác định và phân công tài xế phù hợp, ưu tiên tài xế gần khách hàng.                    |
| **BG02** | **Quản lý đặt xe**        | Cho phép khách hàng tạo và quản lý yêu cầu đặt xe nhanh chóng, chính xác.                       |
| **BG03** | **Theo dõi chuyến đi**    | Cho phép khách hàng theo dõi trạng thái chuyến đi và vị trí tài xế theo thời gian thực.         |
| **BG04** | **Quản lý tài xế**        | Quản lý thông tin, phương tiện và trạng thái hoạt động của tài xế.                              |
| **BG05** | **Tính cước tự động**     | Tự động xác định số tiền khách hàng phải trả dựa trên thông tin chuyến đi và loại dịch vụ.      |
| **BG06** | **Quản lý thanh toán**    | Hỗ trợ thanh toán tiền mặt và thanh toán điện tử thông qua nhà cung cấp bên ngoài.              |
| **BG07** | **Gửi thông báo**         | Gửi thông báo kịp thời cho khách hàng và tài xế về các sự kiện của chuyến đi.                   |
| **BG08** | **Quản lý vận hành**      | Hỗ trợ nhân viên theo dõi, quản lý và xử lý các vấn đề phát sinh trong quá trình vận hành.      |
| **BG09** | **Bảo mật và phân quyền** | Bảo vệ dữ liệu và kiểm soát quyền truy cập của từng nhóm người dùng.                            |
| **BG10** | **Báo cáo và thống kê**   | Cung cấp báo cáo về số chuyến, doanh thu, tỷ lệ hoàn thành, hủy chuyến và hiệu quả tài xế.      |
| **BG11** | **Khả năng mở rộng**      | Cho phép hệ thống phục vụ số lượng lớn khách hàng, tài xế và mở rộng chức năng trong tương lai. |
| **BG12** | **Đảm bảo tính ổn định**  | Đảm bảo lỗi ở một thành phần như thanh toán hoặc thông báo không làm ngừng toàn bộ hệ thống.    |

 
 B4: xác định phạm vi yêu cầu phải làm,( vd: qlkh, ql tài xế) phải biết làm những gì, xác định các moldun cơ bản dưới hệ thống mdb, chỉ ra cái nào k nên làm
 | STT | Module                           | Phạm vi phải làm | Chức năng chính                                                              | Không làm / ngoài phạm vi                               |
| --- | -------------------------------- | ---------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------- |
| 1   | **QLKH – Quản lý khách hàng**    | **Phải làm**     | Đăng ký, đăng nhập, cập nhật thông tin, xem lịch sử chuyến, đánh giá tài xế  | Không quản lý thông tin ngoài dịch vụ CAB               |
| 2   | **QLTài xế – Quản lý tài xế**    | **Phải làm**     | Tạo tài khoản, cập nhật hồ sơ, quản lý trạng thái, thông tin phương tiện     | Không quản lý lương, hợp đồng lao động                  |
| 3   | **QLĐặt xe – Quản lý đặt xe**    | **Phải làm**     | Nhập điểm đón/điểm đến, chọn loại xe, tạo và hủy yêu cầu                     | Không hỗ trợ đặt các dịch vụ không liên quan đến CAB    |
| 4   | **Điều phối tài xế**             | **Phải làm**     | Tìm tài xế phù hợp, ưu tiên tài xế gần, xử lý từ chối/không phản hồi         | Không phân công thủ công là chức năng chính             |
| 5   | **QLChuyến đi – Quản lý chuyến** | **Phải làm**     | Theo dõi trạng thái, cập nhật trạng thái chuyến, lưu lịch sử chuyến          | Không quản lý hành trình ngoài hệ thống CAB             |
| 6   | **QLVị trí – GPS**               | **Phải làm**     | Theo dõi vị trí tài xế, hỗ trợ tìm tài xế và dự kiến thời gian đến           | Không xây dựng hệ thống bản đồ riêng                    |
| 7   | **QLCước – Tính cước**           | **Phải làm**     | Tính số tiền phải trả dựa trên loại dịch vụ và thông tin chuyến              | Chưa triển khai các chính sách giá chưa được thống nhất |
| 8   | **QLThanh toán**                 | **Phải làm**     | Thanh toán tiền mặt/điện tử, xử lý giao dịch thất bại, lưu lịch sử giao dịch | **Không lưu thông tin nhạy cảm của thẻ/tài khoản**      |
| 9   | **QLThông báo**                  | **Phải làm**     | Thông báo đặt xe, tài xế nhận chuyến, tài xế đến, hoàn thành, thanh toán     | Không tự xây dựng nhà mạng/SMS riêng                    |
| 10  | **QLVận hành/Admin**             | **Phải làm**     | Quản lý KH, tài xế, phương tiện, chuyến đi, xử lý sự cố, phân quyền          | Không cho nhân viên thường thực hiện thao tác nhạy cảm  |
| 11  | **Báo cáo – Thống kê**           | **Phải làm**     | Số chuyến, doanh thu, tỷ lệ hoàn thành/hủy, hiệu quả tài xế                  | Không xây dựng hệ thống BI phức tạp ở giai đoạn đầu     |
| 12  | **Bảo mật & Audit**              | **Phải làm**     | Xác thực, phân quyền, bảo vệ dữ liệu, lưu vết thao tác                       | Không lưu dữ liệu nhạy cảm không cần thiết              |
| 13  | **Mở rộng hệ thống**             | **Phải làm**     | Thiết kế để thêm dịch vụ, phương thức thanh toán, nhà cung cấp thông báo     | Không cần triển khai tất cả dịch vụ mới ngay từ đầu     |



