# Network Layer
- *Lớp mạng (lớp 3)* của *OSI* kiểm soát việc trao đổi các gói dữ liệu, vì chúng không thể được định tuyến trực tiếp đến người nhận và do đó phải được cung cấp các node định tuyến
- Các gói dữ liệu sau đó được chuyển từ node này sang node khác cho đến khi chúng đến đích
- Để thực hiện điều này, *lớp mạng* xác định các node mạng riêng lẻ, thiết lập và xoá các kênh kết nối, đồng thời đảm nhiệm nhận việc định tuyến và kiểm soát luồng dữ liệu
- Khi gửi các gói, địa chỉ được đánh giá và dữ liệu được định tuyến qua mạng từ node này sang node khác
- Nói tóm lại, nó chịu trách nhiệm cho các chức năng sau: <br />
+) *Logical Addressing* <br />
+) *Routing (định tuyến)*
- Các giao thức đại diện cho một tập hợp các quy tắc giao tiếp trong lớp tương ứng
- Chúng vô hình đối với các lớp bên trên hoặc bên dưới
- Một số giao thức hoàn thành nhiệm vụ của một số lớp và mở rộng trên hai hoặc nhiều lớp
- Các giao thức được sử dụng trong lớp này là: <br />
+) *IPv4 / IPv6* <br />
+) *IPsec* <br />
+) *ICMP* <br />
+) *IGMP* <br />
+) *RIP* <br />
+) *OSPF* <br />
- Nó đảm bảo việc định tuyến các gói từ nguồn đến đích trong hoặc ngoài mạng con. Hai mạng con này có thể có sơ đồ địa chỉ khác nhau hoặc kiểu địa chỉ không tương thích
- Trong cả hai trường hợp, việc truyền dữ liệu trong mỗi trường hợp đều đi qua toàn bộ mạng truyền thông và bao gồm việc định tuyến giữa các node mạng
- Vì giao tiếp trực tiếp giữa người gửi và người nhận không phải lúc nào cũng có thể do các mạng con khác nhau, các gói phải được chuyển tiếp từ các node (router) ở trên đường
- Các gói được chuyển tiếp không đến được các lớp cao hơn nhưng được chỉ định một trung gian mới và được gửi đến node tiếp theo
