# Ứng dụng Machine Learning trong dự đoán thời tiết

## Giới thiệu
Dự đoán thời tiết là bài toán quan trọng trong nông nghiệp, giao thông và phòng chống thiên tai. Dự án này xây dựng và so sánh các mô hình Machine Learning dựa trên dữ liệu khí tượng lịch sử nhằm dự đoán một đại lượng thời tiết (ví dụ: nhiệt độ).

## Mục tiêu
- Xây dựng pipeline xử lý dữ liệu khí tượng (làm sạch, chuẩn hóa, tạo đặc trưng).
- Huấn luyện và so sánh các mô hình hồi quy:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Đánh giá bằng MAE và RMSE để chọn mô hình phù hợp.

## Phương pháp
1. Thu thập dữ liệu khí tượng theo thời gian.
2. Tiền xử lý: xử lý giá trị thiếu, chuẩn hóa, tách train/test.
3. Huấn luyện mô hình và tinh chỉnh tham số cơ bản.
4. Đánh giá kết quả trên tập kiểm tra.

## Kết quả (minh họa)
Ví dụ kết quả:
- Linear Regression: MAE = 2.31, RMSE = 3.45
- Random Forest: MAE = 1.85, RMSE = 2.90
- Gradient Boosting: MAE = 2.60, RMSE = 3.80

> Lưu ý: Kết quả phụ thuộc bộ dữ liệu và cấu hình tiền xử lý.

## Cấu trúc thư mục
- `data/`: dữ liệu thô và dữ liệu đã xử lý
- `src/`: mã nguồn tiền xử lý, huấn luyện, đánh giá
- `docs/`: tài liệu (bài báo, poster)
- `results/`: kết quả, biểu đồ, metrics

## Cách chạy (gợi ý)
```bash
pip install -r requirements.txt
python src/preprocess.py
python src/train.py
python src/evaluate.py
