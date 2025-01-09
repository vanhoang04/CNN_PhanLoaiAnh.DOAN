# CNN_PhanLoaiAnh.DOAN
Kết quả sau khi huấn luyện trên 18.000 ảnh mèo và chó:
Số epochs = 15

Tỉ lệ chia dữ liệu huấn luyện / kiểm định = 80/20

MÔ HÌNH:

Các lớp tích chập (CONV) với bộ lọc 3x3 và chuẩn hóa batch norm - 32 x 64 x 96 x 96 x 64

Các lớp fully connected (Dense) với dropout 0.2 và 0.3 - 256 x 128 x 2

loss: 0.0638

accuracy: 0.9759

val_loss: 0.3255

val_accuracy: 0.9044

Mô hình được kiểm thử trên các ảnh trong thư mục test1. Hiệu suất của mô hình rất tốt, có khả năng dự đoán chính xác loài vật với độ chính xác từ 97-99%.

Các đồ thị biểu diễn độ chính xác và loss của mô hình như sau:

![alt text](./output/accuracy_5000images_15epochs.png?raw=true)

![alt text](./output/loss_5000images_15epochs.png?raw=true)

![alt text](./output/accuracy_18000images_15epochs.png?raw=true)

![alt text](./output/loss_18000images_15epochs.png?raw=true)

Phân loại ảnh:

![alt text](./output/cat_prediction1.PNG?raw=true)

![alt text](./output/cat_prediction2.PNG?raw=true)

![alt text](./output/dog_prediction1.PNG?raw=true)

![alt text](./output/dog_prediction2.PNG?raw=true)

Video kết quả dự đoán ảnh mèo và chó có thể xem tại đây.

Hướng dẫn chạy mã nguồn:
Bộ dữ liệu đầu vào

Di chuyển đến thư mục: cd Code/

Để bắt đầu quá trình huấn luyện, chạy lệnh:

$ python main.py
