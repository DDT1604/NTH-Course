# Networking Topologies
- Một cấu trúc liên kết mạng là cách sắp xếp *vật lý* hoặc *logic* của các thiết bị trong mạng
- Chúng cũng bao gồm các thiết bị mạng như *switch*, *bridge* và *router*
- Bố trí phương tiện truyền dẫn (*Transmission medium layout*) để kết nối các thiết bị là cấu trúc liên kết vật lý của mạng
- *Cấu trúc liên kết logic* là cách các tín hiệu hoạt động trên phương tiện mạng hoặc cách dữ liệu được truyền qua mạng từ một thiết bị đến kết nối vật lý của thiết bị
- Chúng ta có thể chia toàn bộ khu vực cấu trúc liên kết mạng thành ba khu vực:

**1. Connections**

| Wired connections (Kết nối có dây)| Wireless connections (Kết nối không dây)|
|-----------------------------------|-----------------------------------------|
| Cáp đồng trục                     | Wifi                                    |
| Cáp sợi thuỷ tinh                 | Di động (Cellular)                      |
| Cáp xoắn đôi                      | Vệ tinh                                 |

**2. Nodes - Networking Interface Controller (NICs)**

| Repeater | Hub | Bridge | Switch |
|:---|:---|:---|:---|
| **Router/Modem** | **Gateway** | **Firewall** |

- Các node mạng là điểm kết nối của *phương tiện truyền dẫn* (transmission medium) để phát và thu tín hiệu điện, quang hoặc vô tuyến trong môi trường
- Một node có thể được kết nối với máy tính, nhưng một số loại nhất định có thể chỉ có một bộ vi điều khiển trên một node hoặc có thể không có thiết bị lập trình nào cả

**3. Classifications**
- Cấu trúc liên kết mạng được chia làm 8 loại cơ bản như sau:

| Point-to-Point | Bus |
| :--- | :--- |
| **Star** | **Ring** |
| **Mesh** | **Tree** |
| **Hybrid** | **Daisy Chain** |

- Các mạng phức tạp hơn có thể được xây dựng dưới dạng kết hợp của hai hoặc nhiều cấu trúc liên kết cơ bản được đề cập ở trên

**A. Point-to-Point**
- Đây là cấu trúc liên kết mạng đơn giản nhất dành cho *2 máy chủ*
- Trong cấu trúc liên kết này, một liên kết vật lý trực tiếp và đơn giản chỉ tồn tại giữa *2 máy chủ*
- *Point-to-Point* là mô hình cơ bản của điện thoại truyền thống và không được nhầm lẫn với *P2P (Peer-to-Peer)*

![abc](https://github.com/DDT1604/NTH-Course/assets/101965134/03882c8c-be3f-4a00-8682-ad3415524a3f)

**B. Bus**
- Tất cả máy chủ được kết nối thông qua một phương tiện truyền dẫn trong cấu trúc liên kết bus
- Mọi máy chủ đều có quyền truy cập vào phương tiện truyền dẫn và các tín hiệu được truyền qua nó
- Vì phương tiện được chia sẻ với tất cả những người khác nên *chỉ có một máy chủ có thể gửi* và tất cả những người khác chỉ có thể nhận và đánh giá dữ liệu cũng như xem liệu nó có dành cho chính nó hay không <br />
**Chú ý*: Không có thành phần mạng trung tâm nào điều khiển các tiến trình trên đó

![lmao](https://github.com/DDT1604/NTH-Course/assets/101965134/8bf1d33f-e7d1-41d6-ba9f-79088a3ce972)

**C. Star**
- Cấu trúc liên kết hình sao là một thành phần mạng duy trì kết nối với tất cả các máy chủ
- Mỗi máy chủ được kết nối với *thành phần mạng trung tâm* thông qua một kết nối riêng biệt. Đây thường là một router, hub hoặc switch. Chúng xử lý *chức năng chuyển tiếp* cho các gói dữ liệu
- Lưu lượng dữ liệu trên thành phần mạng trung tâm có thể rất cao vì tất cả dữ liệu và kết nối đều đi qua nó

![what-is-star-topology1](https://github.com/DDT1604/NTH-Course/assets/101965134/97d39f98-cab0-4803-991b-e1fb76a59aeb)

**D. Ring**
- Cấu trúc liên kết *vật lý* vòng sao cho mỗi máy chủ hoặc node được kết nối với vòng bằng 2 cáp: <br />
+) Một cho các tín hiệu đến <br />
+) Cái còn lại cho các tín hiệu ra
- Điều này có nghĩa là một cáp đến mỗi máy chủ và một cáp rời đi
- Cấu trúc liên kết vòng không cần thành phần mạng hoạt động
- Việc kiểm soát và truy cập vào các phương tiện truyền dẫn được điều chỉnh bởi một giao thức mà tất cả các trạm đều tuân theo
- Cấu trúc liên kết vòng *logic* dựa trên cấu trúc liên kết sao vật lý, trong đó bộ phân phối tại node mô phỏng vòng bằng cách chuyển tiếp từ cổng này sang cổng tiếp theo

![ring](https://github.com/DDT1604/NTH-Course/assets/101965134/975923a9-192c-48ad-ac44-c295548937bd)

**E. Mesh**
- Nhiều node quyết định về các kết nối trên cấp độ *vật lý* và định tuyến (routing) trên cấp độ *logic* trong các mạng lưới
- Có hai cấu trúc cơ bản là "chia lưới hoàn toàn" và "chia lưới một phần"
- Mỗi máy chủ được kết nối với mọi máy chủ khác trong *cấu trúc chia lưới hoàn toàn*. Điều này có nghĩa là các máy chủ được chia lưới với nhau
- Kỹ thuật này chủ yếu được sử dụng trong *WAN* hoặc *MAN* để đảm bảo độ tin cậy và băng thông cao
- Trong thiết lập này, các node mạng quan trọng như router có thể được kết nối mạng với nhau
- Mỗi node có các chức năng định tuyến giống nhau và biết các node lân cận mà nó có thể giao tiếp gần với cổng mạng và tải lưu lượng
- Trong *cấu trúc chia lưới một phần*, các điểm cuối chỉ được kết nối bằng một kết nối
- Trong loại cấu trúc liên kết mạng này, các node cụ thể được kết nối với chính xác một node khác và một số node khác được kết nối với hai hoặc nhiều node khác bằng kết nối point-to-point

![topo_mesh](https://github.com/DDT1604/NTH-Course/assets/101965134/c136dfdf-15cc-4bc2-8ab4-25b5fef636ca)

**F. Tree**
- Cấu trúc liên kết cây là cấu trúc sao mở rộng mà các mạng cục bộ mở rộng hơn có trong cấu trúc này
- Có cả cấu trúc cây logic theo *cây bao trùm* và cây vật lý
- Các mạng hiện đại dạng module, dựa trên hệ thống cáp có cấu trúc với hệ thống phân cấp trung tâm, cũng có cấu trúc dạng cây

![Tree-Topology-1024x536](https://github.com/DDT1604/NTH-Course/assets/101965134/aa182676-4583-4ff3-af26-53e7c0e5d7fd)

**G. Hybrid**
- Cấu trúc liên kết lai là cấu trúc được kết hợp từ hai cấu trúc liên kết mạng cơ bản trở lên

![social-network-concept-hybrid-topology-network-social-network-concept-hybrid-topology-network-data-g](https://github.com/DDT1604/NTH-Course/assets/101965134/df92dfbe-67f0-430b-bde1-8dd2d924b9c4)

**H. Daisy Chain**
- Trong cấu trúc liên kết chuỗi daisy, nhiều máy chủ được kết nối bằng cách đặt cáp từ node này sang node khác

![daisy-chain-network-topology](https://github.com/DDT1604/NTH-Course/assets/101965134/0964fb3f-66d2-4fd6-8c83-33510f96b6e0)
