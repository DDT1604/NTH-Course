# The OSI Model
- Mô hình *OSI* là một mô hình tham chiếu cho phép giao tiếp của các hệ thống kĩ thuật khác nhau thông qua các thiết bị và công nghệ khác nhau và cung cấp khả năng tương thích
- Mô hình *OSI* sử dụng *7* lớp khác nhau, được phân cấp dựa trên nhau để đạt được mục tiêu này
- Các lớp này đại diện cho các giai đoạn thiết lập mỗi kết nối mà qua đó các packet (gói) đã gửi qua

| Layer (Lớp)                   | Function (Chức năng)                                                       |
|-------------------------------|---------------------------------------------------------------------------|
|*7. Application (Ứng dụng)*|Trong số những thứ khác, lớp này kiểm soát đầu vào và đầu ra của dữ liệu và cung cấp các chức năng của ứng dụng|
|*6. Presentation (Thuyết trình)*|Nhiệm vụ của lớp này là trình bày dữ liệu phụ thuộc vào hệ thống thành một dạng độc lập với ứng dụng|
|*5. Session*|Kiểm soát kết nối logic giữa hai hệ thống và ngăn chặn các sự cố|
|*4. Transport (Vận chuyển)*|Được sử dụng để kiểm soát từ đầu đến cuối dữ liệu được truyền. Có thể phát hiện và tránh các tình huống tắc nghẽn và phân đoạn các luồng dữ liệu|
|*3. Network (Mạng)*|Trên lớp mạng, các kết nối được thiết lập trong mạng chuyển mạch kênh và các gói dữ liệu được chuyển tiếp trong mạng chuyển mạch gói. Dữ liệu được truyền trên toàn bộ mạng từ người gửi đến người nhận|
|*2. Data Link (Liên kết dữ liệu)*|Nhiệm vụ chính của lớp 2 là cho phép truyền dữ liệu một cách tin cậy và không có lỗi trên phương tiện tương ứng. Với mục đích này, các dòng bit từ lớp 1 được chia thành các block (khối) hoặc frame (khung)|
|*1. Physical (Vật lí)*|Các kĩ thuật truyền dẫn được sử dụng là tín hiệu điện, tín hiệu điện quang hoặc sóng điện từ. Thông qua lớp 1, việc truyền tải diễn ra trên đường truyền có dây hoặc không dây|

- Nếu 2 hệ thống giao tiếp với nhau, tất cả 7 lớp của mô hình *OSI* sẽ chạy qua ít nhất *hai* lần, vì cả hai bên gửi và bên nhận đều dùng đến mô hình lớp
- Do đó, một số lượng lớn các tác vụ khác nhau phải được thực hiện trong các lớp riêng lẻ để đảm bảo tính bảo mật, độ tin cậy và hiệu suất của thông tin liên lạc
- Khi một ứng dụng gửi một gói đến hệ thống khác, hệ thống sẽ thực hiện các lớp được hiển thị từ lớp *7* xuống lớp *1* và hệ thống nhận sẽ giải nén gói từ lớp *1* lên lớp *7*
