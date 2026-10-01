# Bài 4: Cấu hình tường lửa bảo vệ máy chủ (UFW & Cloud Firewall Integration)

## 1. Các lệnh cấu hình UFW trên OS (Lớp 1)

Thực thi các lệnh sau trên Droplet Ubuntu:

```bash
# Thiết lập chính sách mặc định
sudo ufw default deny incoming
sudo ufw default allow outgoing

# Cho phép kết nối SSH (cổng 22) và HTTP (cổng 80)
sudo ufw allow 22/tcp
sudo ufw allow 80/tcp

# Kích hoạt UFW
sudo ufw enable


