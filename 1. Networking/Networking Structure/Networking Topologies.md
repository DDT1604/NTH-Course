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

![Point-to-Point-Network-Topology-1024x593](https://github.com/DDT1604/NTH-Course/assets/101965134/96feb5f9-4643-42a5-a13d-06fd11bb34f0)

**B. Bus**
- Tất cả máy chủ được kết nối thông qua một phương tiện truyền dẫn trong cấu trúc liên kết bus
- Mọi máy chủ đều có quyền truy cập vào phương tiện truyền dẫn và các tín hiệu được truyền qua nó
- Vì phương tiện được chia sẻ với tất cả những người khác nên *chỉ có một máy chủ có thể gửi* và tất cả những người khác chỉ có thể nhận và đánh giá dữ liệu cũng như xem liệu nó có dành cho chính nó hay không <br />
**Chú ý*: Không có thành phần mạng trung tâm nào điều khiển các tiến trình trên đó

![istockphoto-1424073936-612x612](https://github.com/DDT1604/NTH-Course/assets/101965134/8a696992-031e-4c7e-b7e8-4f1f1a14257d)

**C. Star**
- Cấu trúc liên kết hình sao là một thành phần mạng duy trì kết nối với tất cả các máy chủ
- Mỗi máy chủ được kết nối với *thành phần mạng trung tâm* thông qua một kết nối riêng biệt. Đây thường là một router, hub hoặc switch. Chúng xử lý *chức năng chuyển tiếp* cho các gói dữ liệu
- Lưu lượng dữ liệu trên thành phần mạng trung tâm có thể rất cao vì tất cả dữ liệu và kết nối đều đi qua nó

![start-topology-type-network-600w-1977792497](https://github.com/DDT1604/NTH-Course/assets/101965134/3af6c48c-abbd-4f76-b14c-20bc8362f55e)

**D. Ring**
- Cấu trúc liên kết *vật lý* vòng sao cho mỗi máy chủ hoặc node được kết nối với vòng bằng 2 cáp: <br />
+) Một cho các tín hiệu đến <br />
+) Cái còn lại cho các tín hiệu ra
- Điều này có nghĩa là một cáp đến mỗi máy chủ và một cáp rời đi
- Cấu trúc liên kết vòng không cần thành phần mạng hoạt động
- Việc kiểm soát và truy cập vào các phương tiện truyền dẫn được điều chỉnh bởi một giao thức mà tất cả các trạm đều tuân theo
- Cấu trúc liên kết vòng *logic* dựa trên cấu trúc liên kết sao vật lý, trong đó bộ phân phối tại node mô phỏng vòng bằng cách chuyển tiếp từ cổng này sang cổng tiếp theo

![istockphoto-1428221851-1024x1024](https://github.com/DDT1604/NTH-Course/assets/101965134/9a398339-e8d6-40b8-9803-71f7df5b6ef4)

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
