# ANN_in_RS

# File gee
Trong quá trình code xảy ra lỗi:
Tile error: An internal error has occurred (request: dfee2b92-8fbf-4478-9bd1-b93819c57f89) (computation: "X6LD5JJT5NYOZTHG46IY6GXY")
Thì đây không phải lỗi do code mà do GEE gặp vấn đề trong tính toán và hiển thị dữ liệu lớn.
Chỉ cần thay đổi các tham số tính toán như .filterDate, .filterMetadata,...

Khi xuất tệp có chứa dữ liệu huấn luyện sang Google Dive thì cần lưu ý
Nếu tệp cần xuất chưa xuất hiện ở Drive thì sang GEE chọn tabs 'Tasks' bấm Run để xuất tệp.

# File google_colab
Nếu như chưa có API của gee thì cài đặt ngay trong google_colab chỉ cần bỏ '#'
Để trích path đúng hãy chạy đoạn mã drive.mount() để nạp dữ liệu Drive vào.
Sau đó hãy bấm vào biểu tượng thư mục bên trái, dưới biểu tượng chìa khóa.
Sau đó tìm đến tệp dữ liệu bấm copy path để lấy link path.
Dán vào file_path = '' để lấy được dữ liệu đã xuất bên GEE
