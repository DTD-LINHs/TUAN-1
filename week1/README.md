# Tuần 1 – Tổng Quan Nội Dung

Tuần này tập trung tìm hiểu các kiến thức nền tảng về AI, Machine Learning, các thư viện phổ biến trong Python và làm quen với Notebooks cũng như nguồn dữ liệu. Dưới đây là tóm tắt toàn bộ nội dung đã hoàn thành.

---

## 1. Giới thiệu về AI

### **AI là gì?**
- Trí tuệ nhân tạo (Artificial Intelligence) là lĩnh vực nghiên cứu giúp máy móc có khả năng tư duy, học hỏi, suy luận và giải quyết vấn đề giống con người.

### **Các lĩnh vực của AI**
- Machine Learning
- Deep Learning
- Xử lý ngôn ngữ tự nhiên (NLP)
- Thị giác máy tính (Computer Vision)
- Robotics
- Expert Systems
- Speech Recognition

### **Ứng dụng AI trong thực tế**
- Chatbot và trợ lý ảo
- Nhận diện khuôn mặt
- Tự động lái (self-driving cars)
- Hệ thống gợi ý (tiki, shopee, youtube,…)
- Phát hiện gian lận ngân hàng
- Y tế/chuẩn đoán hình ảnh y khoa

### **Dữ liệu là gì & vai trò của dữ liệu trong AI**
- Dữ liệu là tập hợp thông tin thu thập được từ thực tế.
- AI — đặc biệt là Machine Learning — cần dữ liệu để:
  - Học mô hình
  - Dự đoán
  - Cải thiện độ chính xác
  - Giảm sai lệch (bias)

### **3 loại bài toán chính trong Machine Learning**
| Loại bài toán | Mục tiêu | Ví dụ | Đầu ra |
|---------------|----------|-------|--------|
| **Supervised Learning** | Học từ dữ liệu có nhãn | phân loại spam, dự đoán giá nhà | số hoặc label |
| **Unsupervised Learning** | Tìm mẫu trong dữ liệu không nhãn | phân cụm khách hàng | nhóm (clusters) |
| **Reinforcement Learning** | Tác nhân học bằng cách thử–sai | AI chơi game, robot | chuỗi hành động tối ưu |

### **Một số thuật ngữ quan trọng**
- Dataset, Sample, Features
- Label/Target
- Model
- Training / Testing
- Loss function
- Overfitting / Underfitting
- Accuracy, Precision, Recall

---

## 2. Một số thư viện phổ biến trong Python

### **NumPy**
- **Khái niệm:** Thư viện xử lý mảng và phép tính toán khoa học.
- **Ra đời:** 2005 — Người tạo: Travis Oliphant.
- **Ưu điểm:** nhanh, tối ưu, hỗ trợ đại số tuyến tính tốt.
- **Nhược điểm:** không thân thiện với dữ liệu dạng bảng như Pandas.

### **Pandas**
- **Khái niệm:** Thư viện thao tác dữ liệu dạng bảng (DataFrame).
- **Ra đời:** 2008 — Wes McKinney.
- **Ưu điểm:** dễ làm sạch, xử lý dữ liệu, mạnh mẽ.
- **Nhược điểm:** tốc độ chậm hơn NumPy khi xử lý mảng lớn.

### **Matplotlib**
- **Khái niệm:** Thư viện trực quan hóa dữ liệu.
- **Ra đời:** 2003 — John Hunter.
- **Ưu điểm:** mạnh, nhiều biểu đồ.
- **Nhược điểm:** cú pháp dài, hơi khó dùng cho người mới.

### **PyTorch**
- **Khái niệm:** Framework Deep Learning.
- **Ra đời:** 2016 — Facebook AI Research.
- **Ưu điểm:** dễ dùng, dynamic graph, phổ biến trong nghiên cứu.
- **Nhược điểm:** tài liệu nhiều nhưng chưa thống nhất như TensorFlow.

---

## 3. Tìm hiểu về Notebook và nguồn dữ liệu

### **a. Notebook (Jupyter / Colab / Kaggle)**
- Đã chạy thử notebook với python ví dụ:
```python
print("hello world")
# **b. Nguồn dữ liệu**

## **1. Kaggle**
- Kaggle là nền tảng thi đấu Machine Learning và chia sẻ dataset có cộng đồng lớn nhất thế giới.
- Người dùng có thể:
  - Tải dataset
  - Dùng Kaggle Notebook
  - Tham gia thi đấu AI/ML
  - Học hỏi qua code của cộng đồng

### **Dataset phổ biến trên Kaggle**
- Titanic – Machine Learning from Disaster  
- House Prices – Advanced Regression  
- MNIST Digit Classification  
- CIFAR-10 Image Dataset  
- Dogs vs Cats  
- Credit Card Fraud Detection  

---

## **2. Hugging Face**
- Hugging Face là nền tảng chia sẻ mô hình Machine Learning/Deep Learning lớn nhất hiện nay.
- Hỗ trợ NLP, Computer Vision, Audio, Multimodal…

### **Hugging Face gồm có:**
- **Models:** Kho mô hình khổng lồ (BERT, T5, GPT, Whisper, CLIP…).  
- **Datasets:** Hơn 100k+ dataset.  
- **Spaces:** Nơi tạo demo web AI bằng Gradio/Streamlit.  

---

# **4. Exploratory Data Analysis (EDA)**

## **EDA là gì?**
EDA (Exploratory Data Analysis) là bước phân tích dữ liệu sơ bộ để hiểu rõ dataset trước khi xây dựng mô hình.  
Mục tiêu là phát hiện cấu trúc, xu hướng, bất thường và hiểu dữ liệu đủ sâu để ra quyết định tiếp theo.

---

## **1. Data Understanding**
- Kiểm tra số dòng, số cột.
- Xem danh sách các thuộc tính.
- Kiểu dữ liệu (int, float, object, datetime…).
- Kiểm tra giá trị thiếu (missing values).
- Kiểm tra dữ liệu trùng lặp (duplicates).
- Xác định outliers (giá trị ngoại lai).

---

## **2. Data Analysis**
- Phân bố dữ liệu (distribution).
- Mối quan hệ giữa các biến.
- Tương quan (correlation matrix).
- Thống kê mô tả:
  - Mean (giá trị trung bình)
  - Median (trung vị)
  - Std (độ lệch chuẩn)
  - Min/Max
  - Quartiles

---

## **3. Data Visualization**
- **Histogram:** trực quan phân bố dữ liệu.
- **Scatter Plot:** mối quan hệ giữa 2 biến số.
- **Boxplot:** phát hiện outliers.
- **Heatmap:** ma trận tương quan.
- **Biểu đồ bar/category:** phân tích thuộc tính dạng phân loại.

---

