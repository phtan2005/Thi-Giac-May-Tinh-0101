Bài thực hành: Xử lý ảnh với Pillow và OpenCV
Sinh viên thực hiện: Phạm Huỳnh Tấn

MSSV: 2374802013448

Môn học: Thị giác máy tính (TGMT)

📝 Tổng quan
Dự án này bao gồm các bài thực hành giới thiệu về xử lý ảnh kỹ thuật số sử dụng ngôn ngữ lập trình Python. Nội dung tập trung vào việc làm quen, thao tác cơ bản với ảnh thông qua hai thư viện phổ biến nhất hiện nay là Pillow (PIL) và OpenCV.

Người học sẽ hiểu được cách máy tính lưu trữ ảnh kỹ thuật số, cách đọc, hiển thị và thực hiện các thao tác cơ bản trên ảnh.

📂 Cấu trúc thư mục
1. Notebook: Pillow Library (PIL)
File: 2.1.1_TGMT_PhamHuynhTan_2374802013448 (2).ipynb

Nội dung chính:

Giới thiệu về thư viện Pillow (Python Imaging Library).

Cách tải và quản lý đường dẫn file ảnh.

Tải ảnh vào Python sử dụng module Image của PIL.

Hiển thị ảnh (Plotting).

Chuyển đổi ảnh sang ảnh xám (Gray Scale), lượng tử hóa (Quantization) và các kênh màu.

Chuyển đổi ảnh PIL sang mảng NumPy để xử lý.

Sử dụng hàm hỗ trợ get_concat_h để ghép ảnh.

2. Notebook: OpenCV Library
File: 2.1.2_TGMT_PhamHuynhTan_2374802013448.ipynb

Nội dung chính:

Giới thiệu về thư viện OpenCV (Open Source Computer Vision Library).

Sử dụng cv2.imread() để đọc ảnh.

Hiểu về sự khác biệt trong không gian màu: OpenCV sử dụng hệ màu BGR thay vì RGB mặc định như PIL.

Sử dụng matplotlib.pyplot để hiển thị ảnh trong môi trường Jupyter (thay thế cho cv2.imshow thường gặp lỗi trên notebook).

Thao tác với mảng NumPy (lấy kích thước shape, giá trị pixel lớn nhất/nhỏ nhất).

Hướng dẫn cài đặt & Sử dụng
pip install numpy matplotlib pillow opencv-python

Dữ liệu (Images)
Các notebook được thiết kế để tự động tải các ảnh mẫu cần thiết từ Internet thông qua lệnh wget. Các ảnh sử dụng bao gồm:

lenna.png

baboon.png

barbara.png

Cách chạy
1) Mở terminal hoặc command prompt.

2) Di chuyển đến thư mục chứa file notebook.

3) Khởi chạy Jupyter Notebook hoặc Jupyter Lab:
    jupyter notebook
4) Mở từng file .ipynb và chạy lần lượt các cell (Run All).