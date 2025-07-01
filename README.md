![image](https://github.com/user-attachments/assets/fb1422ac-b562-47c4-a40a-aca25fb14188)
![image](https://github.com/user-attachments/assets/a6e326b8-56f3-4889-a885-536efd024805)
![image](https://github.com/user-attachments/assets/6a5a54a1-e3bd-4cc1-875b-e3dc0188d443)
![image](https://github.com/user-attachments/assets/8575bac6-b213-4a66-b266-637b6a488424)
Đây là hệ thống mô phỏng quy trình gửi file an toàn, ký số và xác thực giữa hai bên thông qua server trung gian, với các công nghệ tiên tiến như RSA-2048, AES-GCM và Socket.IO đảm bảo tính bảo mật, toàn vẹn, và giao tiếp thời gian thực.

Hệ thống bao gồm 3 thành phần chính hiển thị trên giao diện:

1. Người Gửi
Cho phép gửi file .txt, .docx đã được mã hóa và ký số.

Các bước thực hiện:

Tạo cặp khóa RSA-2048.

Thực hiện bắt tay (Handshake) với người nhận.

Gửi khóa xác thực và file.

Giao diện có trạng thái kết nối, nhật ký hoạt động, tiến trình gửi file rõ ràng.

2. Server Trung gian - Real-time Monitor
Vai trò:

Chuyển tiếp thông điệp giữa người gửi và người nhận.

Ghi log chi tiết các giao dịch.

Giám sát số lượng kết nối, số giao dịch thành công.

Giao diện:

Thống kê số client kết nối, tin nhắn, giao dịch, tỷ lệ thành công.

Nhật ký giao dịch thời gian thực.

3. Người Nhận
Chức năng:

Tạo cặp khóa RSA-2048.

Chờ thông điệp bắt tay từ người gửi.

Nhận khóa xác thực và file.

Xác thực, giải mã file, kiểm tra toàn vẹn dữ liệu.

Giao diện thể hiện trạng thái kết nối, tiến trình nhận file, nhật ký hoạt động.
