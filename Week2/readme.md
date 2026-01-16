I Mục tiêu bài học
- Thông qua các tệp Notebook này, bạn sẽ học được:

- Cách tải và hiển thị hình ảnh từ URL hoặc tệp tin cục bộ.

- Hiểu về cách lưu trữ hình ảnh trong bộ nhớ và cách sao chép (Copying) ảnh đúng cách để tránh lỗi tham chiếu (aliasing).

- Thực hiện các thao tác biến đổi hình ảnh: Lật ảnh (Flipping) và Cắt ảnh (Cropping).

- Thao tác trực tiếp trên các điểm ảnh (pixels): Vẽ hình khối, viết văn bản và chèn ảnh đè lên nhau (superimpose).

II. Thư viện sử dụng
Để chạy được các tệp .ipynb, bạn cần cài đặt các thư viện sau:
- pip install pillow opencv-python matplotlib numpy
III. Nội dung chi tiết
1. Thao tác với Pillow (Tệp: 2_2_1_basic_image_manipulation_PIL.ipynb)
Tập trung vào sử dụng thư viện Pillow, một thư viện mạnh mẽ và dễ dùng cho các tác vụ xử lý ảnh thông thường.

Mở và Hiển thị: Sử dụng Image.open().

Sao chép ảnh: Sử dụng phương thức .copy() để tạo một đối tượng ảnh độc lập.

Biến đổi: * Lật ảnh theo chiều ngang, dọc bằng transpose().

Cắt một vùng cụ thể của ảnh bằng crop().

Vẽ và Viết chữ: Sử dụng module ImageDraw để thêm các hình học cơ bản và văn bản vào ảnh.

2. Thao tác với OpenCV (Tệp: 2.2.2_basic_image_manipulation_open_CV.ipynb)
Tập trung vào OpenCV, thư viện tiêu chuẩn cho thị giác máy tính, xử lý ảnh dựa trên mảng đa chiều của NumPy.

Đọc ảnh: Sử dụng cv2.imread(). Lưu ý OpenCV mặc định đọc ảnh dưới định dạng BGR, cần chuyển sang RGB để hiển thị đúng màu với matplotlib.

Quản lý bộ nhớ: Giải thích chi tiết về việc sử dụng .copy() trong NumPy để tránh việc thay đổi ảnh gốc khi thao tác trên biến phụ.

Thao tác mảng: * Sử dụng slicing của NumPy để thực hiện lật ảnh và cắt ảnh.

Thay đổi giá trị pixel trực tiếp thông qua chỉ số mảng.

Vẽ hình khối: Sử dụng các hàm cv2.line(), cv2.rectangle(), cv2.circle() và cv2.putText().

III. Hướng dẫn bắt đầu nhanh
Tải dữ liệu: Các bài thực hành sử dụng lệnh !wget để tải các ảnh mẫu như cat.png, lenna.png, baboon.png.

Chạy mã: Mở các tệp Notebook trên Google Colab hoặc Jupyter Notebook.

Lưu ý quan trọng: * Trong OpenCV, hãy luôn nhớ chuyển đổi không gian màu: image_rgb = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2RGB)

Khi sao chép ảnh để chỉnh sửa mà vẫn muốn giữ bản gốc, hãy dùng lệnh .copy().