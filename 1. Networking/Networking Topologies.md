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

- Các nút (node) mạng là điểm kết nối của *phương tiện truyền dẫn* (transmission medium) để phát và thu tín hiệu điện, quang hoặc vô tuyến trong môi trường
- Một nút có thể được kết nối với máy tính, nhưng một số loại nhất định có thể chỉ có một bộ vi điều khiển trên một nút hoặc có thể không có thiết bị lập trình nào cả

**3. Classifications**
- Cấu trúc liên kết mạng được chia làm 8 loại cơ bản như sau:

| Point-to-Point | Bus |
| :--- | :--- |
| **Star** | **Ring** |
| **Mesh** | **Tree** |
| **Hybrid** | **Daisy Chain** |

- Các mạng phức tạp hơn có thể được xây dựng dưới dạng kết hợp của hai hoặc nhiều cấu trúc liên kết cơ bản được đề cập ở trên

**A. Point-to-Point**
- Là cấu trúc liên kết mạng đơn giản nhất dành cho *2 máy chủ*
- Trong cấu trúc liên kết này, một liên kết vật lý trực tiếp và đơn giản chỉ tồn tại giữa *2 máy chủ*
- *Point-to-Point* là mô hình cơ bản của điẹn thoại truyền thống và không được nhầm lẫn với *P2P (Peer-to-Peer)*
![abc](https://github.com/DDT1604/NTH-Course/assets/101965134/03882c8c-be3f-4a00-8682-ad3415524a3f)
