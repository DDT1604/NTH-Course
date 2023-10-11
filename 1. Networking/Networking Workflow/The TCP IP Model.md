# The TCP/IP Model

- Mô hình *TCP/IP* cũng là một mô hình tham chiếu phân lớp, thường được gọi là *"bộ giao thức internet"*
- Thuật ngữ *TCP/IP* là viết tắt của 2 giao thức *Transmission Control Protocol (TCP)* và *Internet Protocol (IP)*
- *IP* nằm trong *lớp mạng (lớp 3)* và *TCP* nằm trong *lớp vận chuyển (lớp 4)* của mô hình lớp *OSI*

| Layer (Lớp)         | Function (Chức năng)                              |
|---------------------|---------------------------------------------------|
| 4. Application (Ứng dụng)| Lớp ứng dụng cho phép các ứng dụng truy cập các dịch vụ của các lớp khác và xác định các giao thức mà ứng dụng sử dụng để trao đổi dữ liệu|
| 3. Transport (Vận chuyển) | Tầng vận chuyển chịu trách nhiệm cung cấp các dịch vụ datagram và session cho tầng ứng dụng|
| 2. Internet | Lớp internet chịu trách nhiệm về địa chỉ máy chủ, đóng gói và các chức năng định tuyến|
| 1. Link (Liên kết) | Lớp liên kết chịu trách nhiệm đặt các gói TCP/IP trên phương tiện mạng và nhận các gói tương ứng từ phương tiện mạng|

- *IP* đảm bảo rằng dữ liệu đến đích và *TCP* kiểm soát việc truyền dữ liệu và đảm bảo kết nối giữa luồng dữ liệu và ứng dụng
- Sự khác biệt chính giữa *TCP/IP* và *OSI* là số lớp, một số lớp trong *OSI* đã được kết hợp lại để tạo thành các lớp trong *TCP/IP*
- Những nhiệm vụ quan trọng nhất của *TCP/IP* là:

| Task (Nhiệm vụ) | Protocol (Giao thức) | Description (Mô tả) |
|---|---|---|
| Logical Addressing | IP | Trong TCP/IP, IP tiếp quản địa chỉ logic của các mạng và node. Các gói dữ liệu chỉ đến được mạng nơi chúng cần đến. Các phương pháp để làm như vậy là network classes (lớp mạng), subnetting (mạng con) và CIDR
| Routing | IP | Đối với mỗi gói dữ liệu, node tiếp theo được xác định trong mỗi node trên đường từ người gửi đến người nhận. Bằng cách này, gói dữ liệu sẽ được định tuyến tới người nhận, ngay cả khi người gửi không biết vị trí của nó |
| Error & Control Flow | TCP | Người nhận và người gửi thường xuyên liên lạc qua kết nối ảo. Do đó, các thông báo điều khiển được gửi liên tục để kiểm tra xem kết nối có còn được thiết lập hay không |
| Application Support | TCP | Các cổng TCP và UDP tạo thành một bản tóm tắt phần mềm để phân biệt các ứng dụng cụ thể và các liên kết truyền thông của chúng |
| Name Resolution | DNS | DNS cung cấp khả năng phân giải tên thông qua Fully Qualified Domain Name (Tên miền đầy đủ) trong địa chỉ IP, cho phép tiếp cận máy chủ lưu trữ mong muốn với tên được chỉ định trên internet |
