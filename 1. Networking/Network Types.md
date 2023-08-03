# Network Types  
- Mỗi mạng lưới được cấu trúc khác nhau và thiết lập riêng lẻ
- Vì lý do này, cái được gọi là *type* và *topologic* đã được phát triển có thể được sử dụng để phân loại mạng này

|            Network Type            |                     Định nghĩa                   |
|------------------------------------|--------------------------------------------------|
| Wide Area Network (WAN)            | Internet                                         |
| Local Area Network (LAN)           | Mạng nội bộ (VD: nhà hàng, trường học, ...)      |
| Wireless Local Area Network (WLAN) | Mạng nội bộ có thể truy câp qua Wi-Fi, Bluetooth |
| Virtual Private Network (VPN)      | Kết nối nhiều trang mạng với một LAN             |  

**A, WAN**  
- WAN (Wire Area Network) thường được gọi là internet
- Khi xử lý thiết bị mạng, chúng thường có địa chỉ WAN và địa chỉ LAN
- Mạng WAN là địa chỉ thường được internet truy cập. Điều đó đang được nói, nó không bao gồm internet; một mạng WAN chỉ là một số lượng lớn các mạng LAN được kết hợp với nhau
- Nhiều công ty lớn hoặc chính phủ sẽ có một "mạng WAN nội bộ"

**B, LAN/WLAN**  
- LAN (Local Area Network) và WLAN (Wireless Local Area Network) sẽ chỉ định địa chỉ IP được chỉ định để sử dụng cục bộ
- Không có gì khác biệt giữa LAN và WLAN ngoài việc WLAN truyền dữ liệu mà không cần cáp. Nó chủ yếu là một chỉ định bảo mật

**C, VPN**
- Có 3 loại VPN (Virtual Private Network) chính:
  1. Site-To-Site VPN: Cả client và server đều là thiết bị mạng, thường là *router* hoặc *firewall* và chia sẻ toàn bộ phạm vi mạng
  2. Remote Access VPN:
    - Remote access VPN còn được xem như là dạng User-to-LAN, cho phép người dùng ở xa dùng phần mềm VPN client kết nối với VPN server
    - VPN hoạt động nhờ vào sự kết hợp với các giao thức đóng gói PPTP, L2TP, IPSec, GRE, MPLS, SSL, TLS
  3. SSL VPN:
    - Đây thực chất là một VPN được thực hiện trên web browser và càng ngày trở nên phổ biến vì các web browser càng ngày có khả năng thực hiện mọi thứ
    - Thông thường, chúng sẽ truyền trực tuyến các ứng dụng hoặc toàn bộ session máy tính tới web browser
