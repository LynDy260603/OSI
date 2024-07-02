# MÔ HÌNH OSI 7-LAYER MODEL
**1. Layer 1- Physical (Lớp vật lý)**

- Đảm bảo các yêu cầu truyền/nhận các chuỗi bít qua các phương tiện vật lý ( là các dây cáp ).
  
**2. Layer 2- Data Link (Lớp liên kết dữ liệu)**

- Tạo/gỡ bỏ khung thông tin (Frames), kiểm soát luồng và kiểm soát lỗi. Giao thức sử dụng phổ biến cho lớp này là Ethernet, PPPoE, HDLC,...
Ví dụ cụ thể là card mạng trong máy tính đanng sử dụng giao thức Ethernet. 

**3. Layer 3- Network (Lớp mạng)**

- Thực hiện định tuyến gói tin, chọn đường đi tối ưu, quy định cấu trúc và định dạng của địa chỉ IP. Giao thức: IPv4, IPv6, IPX,...

**4. Layer 4- Transport (Lớp vận chuyển)**

- Vận chuyển thông tin giữa các máy chủ (End to End), kiểm soát lỗi và luồng dữ liệu. Sử dụng 2 giao thức chính là UDP và TCP- cả 3 giao thức đều chia các gói tin lớn thành nhỏ.
  
- Sự khác nhau của 2 giao thức UDP và TCP: 
  
  - UDP không có khả năng phục hồi statement khi mất đi và gửi các statement này một cách ồ ạt mà không cần máy đích phản hồi.
  - TCP thì chia nhỏ gói tin và đánh số gói tin khi truyền statement đi thì giao thức luôn chờ sự phản hồi từ máy đích về lại sau đó mới gửi tiếp statement khác.
Khi có một statement bị lạc thì bên máy chủ gửi không nhận tin phản hồi sẽ chủ động gửi lại statement đó mà chờ đến khi máy đích phản hồi đã nhận thì mới gửi đi các gói tin khác.

**5. Layer 5- Session (Lớp phiên)**

- Quản lý các cuộc liên lạc giữa các thực thể bằng cách thiết lập, duy trì, đồng bộ hoá và huỷ bỏ các phiên truyền thông giữa các ứng dụng.
- Nhờ lớp này mà ta có thể mở nhiều ứng dụng mạng cùng một lúc, nó chia tài nguyên card mạng của máy tính ra thành nhiều slot thời gian mà mỗi slot là cho một cái ứng dụng mạng truy cập 
đường truyền nhơ đó các ứng dụng có thể truy cập vào mạng một cách bình đẳng. 

**6. Layer 6- Presentation (Lớp trình bày)**

- Đảm bảo định dạng giữa thiết bị này khi truyền dữ liệu sang thiết bị khác hoàn toàn có thể đọc và hiểu.
  
- Chuyển đổi cú pháp dữ liệu để đáp ứng yêu cầu truyền thông của các ứng dụng. Ví dụ: Nếu tải file hình ảnh về thì sẽ có đuôi PNG,JPG thì máy tính sẽ biết dùng chương trình nào hợp lí
  để đọc và biên dịch được file ảnh đó.

**7. Layer 7- Application (Lớp ứng dụng)**

- Giao tiếp người và môi trường mạng. Thường thấy sẽ tiếp xúc với lớp này ở các ứng dụng như Email (Microsoft Outlook), File Transfer (Home FTP Client, Server),Website(Chrome, Firefox).



