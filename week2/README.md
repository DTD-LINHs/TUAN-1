# Supervised Learning & Unsupervised Learning – Báo cáo tổng quan

## I. Supervised Learning

### 1. Supervised Learning là gì?
Supervised Learning (Học có giám sát) là phương pháp học máy mà dữ liệu huấn luyện **đã có nhãn (label)**.  
**Mục tiêu:**  
→ Học mối quan hệ giữa **input (X)** và **output (Y)** để **dự đoán nhãn cho dữ liệu mới**.

---

### 2. Quy trình tổng quát của Supervised Learning

#### 1) Thu thập & gán nhãn dữ liệu
- Thu thập data → con người hoặc hệ thống gán nhãn

#### 2) Tiền xử lý dữ liệu
- Chuẩn hóa (scaling)  
- Mã hóa (encoding)  
- Loại nhiễu & ngoại lai (outlier)  
- Xử lý missing values  

#### 3) Chia tập dữ liệu
- Train set  
- Validation set  
- Test set  

#### 4) Huấn luyện mô hình
- Fit mô hình bằng tập huấn luyện

#### 5) Đánh giá mô hình
- **Classification:** Accuracy, Precision, Recall, F1-score, Confusion Matrix  
- **Regression:** MAE, MSE, RMSE  

#### 6) Tối ưu mô hình (Hyperparameter Tuning)
- Grid Search  
- Random Search  
- Bayesian Optimization  

#### 7) Triển khai & giám sát mô hình
- Đưa vào sản phẩm  
- Theo dõi model drift  
- Cập nhật mô hình định kỳ  

---

### 3. Phân biệt Classification và Regression

| Tiêu chí | Classification | Regression |
|---------|----------------|------------|
| **Output** | Nhãn rời rạc (0/1, A/B/C) | Giá trị liên tục |
| **Ví dụ** | Dự đoán email spam, phân loại ảnh | Dự đoán giá nhà, dự đoán điểm |
| **Đánh giá** | Accuracy, F1-score | MSE, MAE |
| **Thuật toán tiêu biểu** | Logistic Regression, SVM, Random Forest | Linear Regression, SVR |

---

## II. Unsupervised Learning

### 1. Unsupervised Learning là gì?
Unsupervised Learning (Học không giám sát) là phương pháp học máy mà dữ liệu **không có nhãn**.  
**Mục tiêu:**  
→ Tìm **cấu trúc ẩn**, **pattern**, **nhóm điểm giống nhau**, hoặc **biểu diễn gọn hơn** của dữ liệu.

---

### 2. Mục tiêu & ứng dụng

#### 1) Mục tiêu
- Tìm nhóm (cluster) trong dữ liệu  
- Tìm cấu trúc ẩn  
- Giảm chiều dữ liệu để trực quan hóa  
- Phát hiện bất thường (anomaly detection)  

#### 2) Ứng dụng
- Phân nhóm khách hàng trong marketing  
- Gợi ý sản phẩm (recommendation)  
- Nhận dạng bất thường giao dịch  
- Nén dữ liệu, trực quan hóa dữ liệu 2D/3D  

---

### 3. Phân biệt Clustering và Dimensionality Reduction

| Tiêu chí | Clustering | Dimensionality Reduction |
|---------|------------|--------------------------|
| **Output** | Gom nhóm điểm giống nhau | Giảm số chiều nhưng giữ thông tin quan trọng |
| **Ví dụ** | Nhãn cluster | Dữ liệu mới (ít chiều hơn) |
| **Thuật toán tiêu biểu** | K-Means, DBSCAN | PCA, t-SNE |
| **Ứng dụng** | Phân nhóm khách | Trực quan hóa 2D |

---

## III. So sánh Supervised vs Unsupervised Learning

| Tiêu chí | Supervised Learning | Unsupervised Learning |
|---------|---------------------|------------------------|
| **Dữ liệu** | Có nhãn | Không có nhãn |
| **Mục tiêu** | Dự đoán nhãn cho dữ liệu mới | Tìm cấu trúc ẩn, phân nhóm |
| **Ví dụ bài toán** | Classification, Regression | Clustering, Giảm chiều |
| **Khó khăn chính** | Thu thập & gán nhãn tốn kém | Khó đánh giá vì không có ground truth |
| **Độ phức tạp** | Thường cao | Tùy thuật toán (thấp/cao) |
| **Thước đo đánh giá** | Accuracy, F1, MSE… | Silhouette Score, SSE… |

---

## IV. Thuật toán tiêu biểu

### 1. Supervised Learning
- **Linear Regression** – Mô hình tuyến tính dự đoán giá trị liên tục  
- **Logistic Regression** – Phân loại nhị phân  
- **Decision Tree** – Chia dữ liệu bằng cây quyết định  
- **Random Forest** – Ensemble của nhiều Decision Tree  
- **SVM** – Tìm siêu phẳng phân tách tối ưu  
- **KNN** – Dự đoán dựa trên hàng xóm gần nhất  

### 2. Unsupervised Learning
- **K-Means** – Gom nhóm theo centroid  
- **DBSCAN** – Gom nhóm theo mật độ, phát hiện outlier tốt  
- **Hierarchical Clustering** – Gom nhóm dạng phân cấp  
- **PCA** – Giảm chiều tuyến tính  
- **t-SNE** – Giảm chiều phi tuyến để trực quan hóa đẹp  

