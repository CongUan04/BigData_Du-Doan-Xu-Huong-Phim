<h1 align="center">DỰ ĐOÁN XU HƯỚNG PHIM</h1>

<div align="center">

<p align="center">
  <img src="logo.png" alt="DaiNam University Logo" width="200"/>
</p>

[![Fit DNU](https://img.shields.io/badge/Fit%20DNU-green?style=for-the-badge)](https://fitdnu.net/)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-red?style=for-the-badge)](https://dainam.edu.vn)

</div>

<h2 align="center">DỰ ĐOÁN XU HƯỚNG PHIM</h2>

# 🎬 Dự Đoán Xu Hướng Phim

## 🚀 Giới Thiệu

Dự án này sử dụng **Python**, **PySpark**, và **Spark MLlib** để dự đoán xu hướng của các bộ phim dựa trên dữ liệu tài chính và thông tin phim. Mục tiêu chính của dự án:

- Tiền xử lý dữ liệu phim từ file CSV bằng **Pandas** và **PySpark**.
- Thực hiện imputation cho giá trị thiếu và tạo các đặc trưng mới như năm phát hành, tháng, và lợi nhuận (profit).
- Xây dựng pipeline dự đoán xu hướng phim sử dụng **Random Forest**.
- Áp dụng kỹ thuật oversampling để cân bằng dữ liệu giữa các lớp (trend = 0 và trend = 1).
- Đánh giá mô hình qua các chỉ số như Confusion Matrix, ROC Curve và Feature Importance.

---

## 🛠️ Công Nghệ Sử Dụng

### 📡 Phần mềm & Thư viện

[![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![PySpark](https://img.shields.io/badge/PySpark-3.x-orange?style=for-the-badge&logo=apache-spark)](https://spark.apache.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.x-green?style=for-the-badge&logo=pandas)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.x-yellow?style=for-the-badge&logo=scikit-learn)](https://scikit-learn.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-red?style=for-the-badge&logo=matplotlib)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.x-purple?style=for-the-badge&logo=seaborn)](https://seaborn.pydata.org/)

Dự án sử dụng các thư viện chính:
```bash
pip install pyspark pandas scikit-learn matplotlib seaborn
📦 Nhan-Dien-Giong_Noi
├── main_pyspark.py     # Pipeline dự đoán xu hướng phim sử dụng Spark MLlib
├── XulyDL.py    # Xử lý dữ liệu phim: làm sạch, imputation và tạo đặc trưng
├── movies_cleaned.csv       # Dữ liệu phim sau xử lý
├── Nhom7BIGDATA.docx        # Báo cáo chi tiết về dự án
├── README.md                # Tài liệu mô tả dự án (file này)

🎯 Mục Tiêu Dự Án
Dự đoán xu hướng phim: Phân loại phim thành xu hướng thành công (trend = 1) hoặc không thành công (trend = 0) dựa trên lợi nhuận và các đặc trưng liên quan.
Cân bằng dữ liệu: Áp dụng kỹ thuật oversampling cho lớp minority nhằm cải thiện hiệu quả dự đoán.
Hỗ trợ ra quyết định: Cung cấp thông tin dự báo hỗ trợ các nhà sản xuất và đầu tư đưa ra quyết định chiến lược trong ngành điện ảnh.