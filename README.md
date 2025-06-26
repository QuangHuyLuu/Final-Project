# 💎 Dự Án Cuối Kỳ: Dự Báo Giá Kim Cương

## 🎯 Mục Tiêu Dự Án

Mục tiêu của dự án là xây dựng các mô hình học máy để **dự đoán giá kim cương** dựa trên các đặc trưng vật lý và đánh giá chất lượng như trọng lượng, kích thước, độ trong, màu sắc và chất lượng cắt. Thông qua đó, dự án giúp người dùng hoặc doanh nghiệp có thể ước lượng giá trị của một viên kim cương trên thị trường.

## 📊 Dữ Liệu Sử Dụng

Dataset được sử dụng là **`diamonds.csv`** với hơn 50.000 mẫu kim cương, gồm các đặc trưng:

* `carat`: Trọng lượng của kim cương (carat)
* `cut`: Chất lượng cắt (Fair, Good, Very Good, Premium, Ideal)
* `color`: Màu sắc (D đến J, D là tốt nhất)
* `clarity`: Độ trong (I1 đến IF)
* `depth`, `table`: Các chỉ số hình học
* `x`, `y`, `z`: Kích thước chiều dài, chiều rộng, chiều cao (mm)
* `price`: Giá kim cương (USD)

## 🛠️ Công Cụ Sử Dụng

Dự án được thực hiện hoàn toàn bằng **Python**, sử dụng các thư viện phổ biến:

* `pandas`, `numpy`: Xử lý dữ liệu
* `matplotlib`, `seaborn`: Trực quan hóa
* `scikit-learn`: Xây dựng mô hình Linear Regression, Random Forest
* `xgboost`: Mô hình XGBoost
* `lightgbm`: Mô hình LightGBM
* `statsmodels`: Kiểm tra đa cộng tuyến (VIF), kiểm định mô hình

## 🤖 Mô Hình Áp Dụng

Dự án thử nghiệm và so sánh hiệu suất của các mô hình hồi quy sau:

* **Linear Regression**: Mô hình hồi quy tuyến tính đơn giản, làm baseline
* **Random Forest Regressor**: Mô hình ensemble mạnh mẽ, kháng nhiễu tốt
* **XGBoost**: Gradient Boosting tối ưu tốc độ và độ chính xác
* **LightGBM**: Mô hình boosting hiệu quả cho tập dữ liệu lớn

## 📈 Kết Quả & Nhận Xét

Hiệu suất các mô hình được đánh giá bằng các chỉ số:

* **R² (Hệ số xác định)**: Mức độ giải thích phương sai của mô hình
* **RMSE (Root Mean Squared Error)**: Sai số trung bình

