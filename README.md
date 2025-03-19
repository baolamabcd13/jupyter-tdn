# Phân tích dữ liệu ô nhiễm không khí toàn cầu

Dự án này thực hiện phân tích, trực quan hóa và khai phá dữ liệu từ bộ dữ liệu ô nhiễm không khí toàn cầu. Đây là đề tài cá nhân cho môn học Kho dữ liệu và Khai phá dữ liệu.

## Nội dung

- Phân tích thống kê cơ bản
- Trực quan hóa dữ liệu
- Khai phá dữ liệu với phân cụm K-means và phân lớp Random Forest
- Đánh giá kết quả khai phá

## Yêu cầu hệ thống

- Python 3.8 trở lên
- Git

## Cách cài đặt

### 1. Clone repository

```bash
# Clone repository về máy tính của bạn
git clone https://github.com/baolamabcd13/jupyter-tdn.git

# Di chuyển vào thư mục dự án
cd jupyter-tdn
```

### 2. Thiết lập môi trường ảo

#### Sử dụng venv (Python tích hợp)

```bash
# Windows
python -m venv venv
venv\Scripts\activate
```

### 3. Cài đặt các thư viện

```bash
# Cài đặt từ file requirements.txt
pip install -r requirements.txt
```

## Cách chạy

### Sử dụng Jupyter Notebook

```bash
# Khởi động Jupyter Notebook
jupyter notebook
```

## Sườn báo cáo đề tài

### TRANG BÌA

- Tên trường, khoa
- Đề tài: PHÂN TÍCH VÀ KHAI PHÁ DỮ LIỆU Ô NHIỄM KHÔNG KHÍ TOÀN CẦU
- Môn học: Kho dữ liệu và Khai phá dữ liệu
- Họ tên sinh viên:
- MSSV:
- Lớp:
- Giảng viên hướng dẫn:
- Năm học:

### MỤC LỤC

### NHẬN XÉT CỦA GIẢNG VIÊN

### DANH MỤC HÌNH ẢNH

- Hình 1.1: Boxplot của 3 chỉ số ô nhiễm không khí
- Hình 1.2: Q-Q Plots của các chỉ số ô nhiễm
- Hình 1.3: Histograms của các chỉ số ô nhiễm
- Hình 1.4: Scatter plots giữa các chỉ số ô nhiễm
- Hình 2.1: Boxplot AQI Value theo phân loại ô nhiễm
- Hình 2.2: Histograms AQI Value theo mức độ ô nhiễm
- Hình 3.1: Ma trận tương quan giữa các thuộc tính số
- Hình 3.2: Độ đo Cosin giữa 4 dòng dữ liệu

### DANH MỤC BẢNG BIỂU

- Bảng 1.1: Thống kê cơ bản của bộ dữ liệu
- Bảng 1.2: Thống kê của các thuộc tính số
- Bảng 1.3: Phân bố mức độ ô nhiễm
- Bảng 2.1: Tổng hợp theo quốc gia
- Bảng 2.2: Tổng hợp theo mức độ ô nhiễm

### PHẦN 1: GIỚI THIỆU VỀ CSDL SỬ DỤNG CHO ĐỀ TÀI

#### 1.1. Tổng quan về CSDL

- Giới thiệu về bộ dữ liệu ô nhiễm không khí toàn cầu
- Nguồn gốc, ý nghĩa và tầm quan trọng của bộ dữ liệu
- Tổng quan về quy mô dữ liệu: số lượng records, số lượng thuộc tính
- Phạm vi địa lý: số lượng quốc gia, thành phố

#### 1.2. Giới thiệu từng thuộc tính (field)

- Các thuộc tính: Country, City, AQI Value, AQI Category, CO AQI Value, CO AQI Category, Ozone AQI Value, Ozone AQI Category, NO2 AQI Value, NO2 AQI Category, PM2.5 AQI Value, PM2.5 AQI Category
- Ý nghĩa, kiểu dữ liệu, giá trị null, unique, thống kê cơ bản cho từng thuộc tính

#### 1.3. Tiền xử lý dữ liệu

- Xử lý dữ liệu bị thiếu (missing values)
- Xử lý các giá trị ngoại lai (outliers)
- Chuẩn hóa dữ liệu số
- Mã hóa các thuộc tính phân loại

### PHẦN 2: PHÂN TÍCH – THỐNG KÊ THỦ CÔNG TRÊN CSDL ĐÃ CHỌN

#### 2.1. Tìm hiểu dữ liệu

##### 2.1.1. Vẽ biểu đồ cho 3 thuộc tính

- Boxplot, Q-Q Plot, Histogram, Scatter plot cho các thuộc tính
- Nhận xét về phân bố dữ liệu và mối quan hệ

##### 2.1.2. Nhóm dữ liệu theo thuộc tính danh nghĩa

- Phân tích và vẽ biểu đồ theo AQI Category và Country

##### 2.1.3. Đo lường sự tương đồng và khác biệt

- Ma trận tương quan và độ đo cosin
- So sánh kết quả của hai phương pháp

#### 2.2. Tiền xử lý dữ liệu

- Quy trình tiền xử lý chi tiết với code Python

#### 2.3. Tổng hợp dữ liệu

- Tổng hợp theo quốc gia, mức độ ô nhiễm
- Bảng pivot và chỉ số tổng hợp

#### 2.4. Trực quan hóa dữ liệu

- Các biểu đồ phân tích phân bố và tương quan

#### 2.5. Thực hiện khai thác dữ liệu

##### 2.5.1. Sử dụng phương pháp khai phá dữ liệu

- Phân cụm K-means
- Phân lớp Random Forest

##### 2.5.2. Đánh giá kết quả

- Đánh giá phân cụm: Silhouette Score, NMI, ARI
- Đánh giá phân lớp: Cross-Validation, ROC curves

### KẾT LUẬN VÀ KIẾN NGHỊ

- Tổng kết kết quả phân tích
- Ứng dụng thực tiễn và hướng phát triển

### TÀI LIỆU THAM KHẢO
