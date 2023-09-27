# Build image test board bbb và thẻ nhớ
### Tải image trên test về bằng python và glown
```
sudo apt update
sudo apt install python3
pip install gdown
gdown --id 1NkpStgVo0f5SQhi_ZN22uY7wGDqrZtVa
```
Hoặc truy cập vào link sau để tải
https://drive.google.com/file/d/1NkpStgVo0f5SQhi_ZN22uY7wGDqrZtVa/view
### Nạp vào thẻ nhớ
Yêu cầu thẻ nhớ cần được xóa hết dữ liệu rồi 

```
sudo dd if=core-image-minimal-beaglebone-yocto.wic of=/dev/sdb bs=4M
sync
```

Rút thẻ nhớ và chạy thử ,đây là image rút gọn test

Bạn phải đăng nhập là root và không cần pass.