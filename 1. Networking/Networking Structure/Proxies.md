# Proxies
- Proxy là khi một thiết bị hoặc dịch vụ nằm ở giữa kết nối và hoạt động như một trung gian hoà giải
- "*Người hoà giải*" là phần thông tin quan trọng vì nó có nghĩa là thiết bị ở giữa phải có khả năng kiểm tra nội dung của lưu lượng truy cập
- Nếu không có khả năng trở thành "*người hoà giải*", thiết bị về mặt kĩ thuật là một gateway, không phải proxy

**A. Dedicated Proxy/Forward Proxy**
- Forward proxy (proxy chuyển tiếp) là thứ mà hầu hết mọi người tưởng tượng về một proxy
- Proxy chuyển tiếp là khi client đưa ra request với máy tính và máy tính đó thực hiện request

![Forward-Proxy-01](https://github.com/DDT1604/NTH-Course/assets/101965134/f09a5d58-79c8-4fb4-8ba2-411e605740f2)

**B. Reverse Proxy**
- Như có thể đoán, một *reverse proxy* (proxy đảo ngược) là một phiên bản ngược lại của *forward proxy*
- Thay vì được thiết kế để lọc các request gửi đi, nó lọc các request gửi đến
- Mục tiêu phổ biến nhất với *proxy đảo ngược* là lắng nghe một địa chỉ và chuyển tiếp địa chỉ đó đến một mạng khép kín

![61ee501466af465f016c81b6_Proxy Servers vs  VPNs 3](https://github.com/DDT1604/NTH-Course/assets/101965134/b01bf399-10c5-4b42-a69f-5bd78ed4ac0d)
