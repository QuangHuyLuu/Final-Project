# 💎 Dự Án Cuối Kỳ: Dự Báo Giá Kim Cương

## 🎯 Mục Tiêu Dự Án

Mục tiêu của dự án là xây dựng các mô hình học máy để **dự đoán giá kim cương** dựa trên các đặc trưng vật lý và đánh giá chất lượng như trọng lượng, kích thước, độ trong, màu sắc và chất lượng cắt. Thông qua đó, dự án giúp người dùng hoặc doanh nghiệp có thể ước lượng giá trị của một viên kim cương trên thị trường.

## 📊 Dữ Liệu Sử Dụng

Dữ liệu được lấy từ Kaggle: [Diamonds Price Dataset
](https://www.kaggle.com/datasets/amirhosseinmirzaie/diamonds-price-dataset/data)
Dataset gồm 50.000 mẫu, với các biến:

| Tên biến  | Mô tả                                                                                                               |
| --------- | ------------------------------------------------------------------------------------------------------------------- |
| `carat`   | **Trọng lượng kim cương** (tính bằng carat)                                                                         |
| `cut`     | **Chất lượng cắt** của viên kim cương (`Fair`, `Good`, `Very Good`, `Premium`, `Ideal`)                             |
| `color`   | **Màu sắc kim cương** — từ `J` (kém nhất) đến `D` (tốt nhất)                                                        |
| `clarity` | **Độ trong suốt của kim cương**, theo thứ tự từ kém đến tốt: `I1`, `SI2`, `SI1`, `VS2`, `VS1`, `VVS2`, `VVS1`, `IF` |
| `x`       | **Chiều dài** của kim cương (mm)                                                                                    |
| `y`       | **Chiều rộng** của kim cương (mm)                                                                                   |
| `z`       | **Độ sâu** của kim cương (mm)                                                                                       |
| `depth`   | **Tỷ lệ chiều sâu**, tính bằng công thức: `z / mean(x, y)`                                                          |
| `table`   | **Đường kính phần trên cùng rộng nhất** của kim cương (%)                                                           |
| `price`   | **Giá của kim cương** (USD) — *biến mục tiêu cần dự đoán*                                                           |

## 🔍 Các bước thực hiện:

1. Data Cleaning:
EDA (Phân tích dữ liệu khám phá):
Modeling:
Evaluation:

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

Các mô hình boosting (XGBoost, LightGBM) đạt kết quả dự đoán tốt nhất, cho thấy khả năng học phi tuyến và tối ưu hóa sai số vượt trội so với mô hình tuyến tính.

