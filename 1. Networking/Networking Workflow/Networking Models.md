# Networking Models
- Có hai mô hình mạng mô tả việc liên lạc và truyền dữ liệu từ máy chủ này sang máy chủ khác, được gọi là *ISO/OSI model* và *TCP/IP* model
- Đây là một đại diện đơn giản hoá của cái gọi là *layers* (lớp) đại diện cho các bit được truyền trong nội dung có thể đọc được

![osi-vs-tcp-ip2](https://github.com/DDT1604/NTH-Course/assets/101965134/7aca07d2-f253-4845-b935-d68fd98de7ed)

**A. OSI Model**
- Mô hình *OSI*, thường được gọi là mô hình lớp *ISO/OSI*, là một mô hình tham chiếu có thể được sử dụng để mô tả và xác định giao tiếp giữa các hệ thống
- Mô hình tham chiếu có *bảy* lớp riêng lẻ, mỗi lớp có các nhiệm vụ rõ ràng

**B. TCP/IP Model**
- *TCP/IP (Transmission Control Protocol/Internet Protocol)* là thuật ngữ chung cho nhiều giao thức mạng
- Các giao thức chịu trách nhiệm chuyển đổi và vận chuyển các gói dữ liệu trên internet
- Internet hoàn toàn dựa trên họ giao thức *TCP/IP*

***ISO/OSI vs. TCP/IP***
- *TCP/IP* là một giao thức truyền thông cho phép các máy chủ kết nối với internet
- Nó đề cập đến *transmission control protocol* (giao thức điều khiển truyền) được sử dụng trong và bởi các ứng dụng trên internet
- Trái ngược với *OSI*, nó cho phép giảm nhẹ các nguyên tắc phải tuân theo, miễn là các nguyên tắc chung được tuân theo
- Mặt khác *OSI* là một cổng giao tiếp giữa mạng và người dùng cuối
- Nó được biết đến với các hạn chế và giao thức nghiêm ngặt

**C. Packet Transfer**
- Trong một hệ thống phân lớp, các thiết bị trong một lớp trao đổi dữ liệu ở một định dạng khác được gọi là *protocol data unit (PDU)*
- Khi nhận được tín hiệu, các lớp ứng dụng xử lý từng công việc được giao mới mỗi lớp
- Dữ liệu sau đó được truyền qua lớp vật lý của mạng cho đến khi máy chủ đích hoặc thiết bị khác nhận được dữ liệu
- Trong quá trình truyền, mỗi lớp thêm một *header* vào *DPU* từ lớp trên, điều khiển và xác định gói tin. Quá trình này được gọi là encapsulation (đóng gói)
- Header và dữ liệu cùng nhau tạo thành DPU cho lớp tiếp theo
- Người nhận đảo ngược quá trình và giải nén dữ liệu trên mỗi lớp với thông tin của header
- Sau đó, ứng dụng cuối cùng sẽ sử dụng dữ liệu

![packet_transfer](https://github.com/DDT1604/NTH-Course/assets/101965134/148a36c8-c63b-4d65-a36c-1f167b452440)
