# VTP
- **Virtual trunk protocal**

 - Tự động câp nhật tất cả các switch trong cùng 1 VLAN

 - Với cấu hình giao thức VTP chỉ cần thay đổi thông tin trên VTP server trong mạng. 

 - Đảm bảo việc tất cả các thay đổi được thực hiện cập nhật trên tất cả các switch.

## 1.1. VTP introduction

## 1.2. VTP version

## 1.3. VTP mode
- VTP Server mode
- VTP client mode
- VTP Transparent mode

### 1.3.1. VTP server mode
- Tất cả thông tin về VLAN được lưu trên NVRAM. 
- VTP Domain: 
 - Thông số được cấu hình trên các switch kết nối tới mạng.

 - Được dùng để xác định các switch sẽ cập nhật khi có sự thay đổi trong miền VTP domain.

### 1.3.2. VTP Client mode
- Lưu tất cả các thông tin về các VLAN trong RAM, vì vậy khi ** tắt nguồn sẽ mất thông tin **.

### 1.3.3. VTP Transparent mode
- Không tham gia vào miền VTP domain.
- Tạo, sửa, xóa VLAN trong nội bộ sw đó không ảnh hưởng đến sw khác.
- Chỉ chuyển tiếp qua cổng trunk mà không quảng bá thông tin của chính nó.

## 2. Cấu trúc bản tin VTP

- 4 phần
 - ** Summary advertisements **
 - ** Subnet advertisements **
 - ** Advertisements Request **
 - ** VTP join Messages **
