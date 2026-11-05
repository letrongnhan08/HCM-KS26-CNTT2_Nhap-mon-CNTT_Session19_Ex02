**Bài 2 : Chuỗi tấn công từ mật khẩu bị rò rỉ** 

**Giải thích cơ chế Hacker sử dụng mật khẩu rò rỉ từ web nhỏ để chiếm đoạt các tài khoản lớn (domino effect)**
- Bảo mật lỏng lẻo ở website nhỏ: Nhiều diễn đàn nhỏ lưu trữ dạng plaintext hoặc mã hóa yếu không có salt ký tự ngẫu nhiên , khiến hacker dễ dàng giải mã hoặc đọc trực tiếp.
    
- Bot tự động thu thập email,tài khoản,mật khẩu vừa trộm được để thử đăng nhập tự động hàng loạt lên các dịch vụ như Gmail, Facebook và GitHub.
    
- Dùng chung một mật khẩu duy nhất (123456) cho nhiều nền tảng,nếu bị rò rỉ mật khẩu chung từ trang web nhỏ thì các dịch vụ như Gmail, Facebook và GitHub đã bị hack, lộ dữ liệu hết.

- **Phân tích tại sao mật khẩu cảm tính lại dễ bị bẻ khóa hơn mật khẩu do máy tính sinh ra.**  
+ Mật khẩu cảm tính: đặt kiểu dễ nhớ, không chứa các ký tự đặc biệt,mật khẩu 123456 quá phổ biến và cực dễ đoán, hacker cũng chẳng cần chuyên môn nhiều là đã bẻ khóa xong.
+ Mật khẩu do máy tính sinh ra : sẽ có chữ hoa, chữ thường, có các ký tự đặc biệt thêm vào, có thêm số và đặt không theo thứ tự ,ví dụ: "qKmR$0?1zE#p2B1"
    
- **giải thích tại sao việc sử dụng AES-256 lưu mật khẩu trong Password Manager lại an toàn hơn ghi chép thủ công.**  
- ghi chép thủ công là plainText vừa dễ nhìn vừa không có gì phức tạp bảo mật ,dễ bị bot của hacker ăn cắp thông tin rất dễ
+ Lưu mật khẩu trong Password Manager có sẽ mã hóa Master Password với AES-256 mật khẩu người dùng thành những ký tự phức tạp,  còn web và Password manager chỉ là nơi lưu trữ và chính bản thân  web và Password manager không thể biết được mật khẩu người dùng vì Master Password chỉ ở trong máy người dùng, nếu Password manager có bị hack thì hacker chỉ lấy được các ký tự vô nghĩa mà mã AES-256 tạo ra vì Master Password chỉ ở trong máy người dùng và Hacker muốn đoán trúng được mật khẩu sẽ mất hàng triệu năm. 

