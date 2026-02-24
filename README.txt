THIẾT KẾ MÔ HÌNH LAB VPN SITE TO SITE

Thiết kế hệ thống mạng cho doanh nghiệp

MÔ TẢ TOPOLOGY:

Doanh nghiệp các 3 chỉ nhánh Hanoi, HCM, Hải Phòng: Mỗi chi nhánh có các phòng ban: Ban GĐ, P. Nhân sự, P. Kế toán, P. Kỹ thuật, P. Server. Mỗi phòng ban có 30 host

1. Chi nhánh Hà Nội : chia subnet từ 192.168.1.0/24 cho các phòng ban của chi nhánh 
==> mỗi subnet /27 
192.168.1.0/27 (vlan 10 : G.doc)
192.168.1.32/27 (vlan 20 : Nhan su )
192.168.1.64/27 (vlan 30 : ke toan )
192.168.1.96/27 (vlan 40 : Ky thuat)
192.168.1.128/27 (vlan 50 : Server)

-cau hinh VTP , inter vlan 
- VPN IPsec : Có thể giao tiếp với Site HCM , HP thông qua VPN
- NAT : LAN nội bộ có thể NAT ra internet


2.Chi nhánh HCM : chia subnet từ 192.168.2.0/24 cho các phòng ban của chi nhánh

==> mỗi subnet /27 
192.168.2.0/27 (vlan 10 : G.doc)
192.168.2.32/27 (vlan 20 : Nhan su )
192.168.2.64/27 (vlan 30 : ke toan )
192.168.2.96/27 (vlan 40 : Ky thuat)
192.168.2.128/27 (vlan 50 : Server)

- cau hinh VTP , inter vlan 
- VPN IPsec : Có thể giao tiếp với Site HN , HP thông qua VPN
- NAT : LAN nội bộ có thể NAT ra internet


3.Chi nhánh Hà Nội : chia subnet từ 192.168.3.0/24 cho các phòng ban của chi nhánh

==> mỗi subnet /27 
192.168.3.0/27 (vlan 10 : G.doc)
192.168.3.32/27 (vlan 20 : Nhan su )
192.168.3.64/27 (vlan 30 : ke toan )
192.168.3.96/27 (vlan 40 : Ky thuat)
192.168.3.128/27 (vlan 50 : Server)

- cau hinh VTP , inter vlan 
- VPN IPsec : Có thể giao tiếp với Site HN , HCM thông qua VPN
- NAT : LAN nội bộ có thể NAT ra internet


-Thiết kế mô hình mạng, mô phỏng bằng phần mềm Packet tracer Cisco


-Server bên Hà Nội được cấu hình cấp địa chỉ IP động cho các Client; cấu hình WebServer; cấu hình MailServer

