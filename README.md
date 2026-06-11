# 🛡️ Ứng dụng Học Máy Phát Hiện Giao Dịch Gian Lận & Rủi Ro Mặc Định

Ứng dụng web được xây dựng dựa trên framework **Streamlit** mạnh mẽ kết hợp cùng thư viện Học máy chuyên sâu **Scikit-Learn**. 

## ✨ Tính năng chính
- **Cấu hình động**: Tùy chỉnh trực tiếp siêu tham số mô hình `RandomForestClassifier` ngay trên giao diện Sidebar.
- **Tổng quan Thống kê**: Tự động phân tích quy mô dữ liệu và mô tả các biến đặc trưng đầu vào mẫu.
- **Trực quan hóa Phân Phối**: Biểu đồ phân bổ dữ liệu trực quan dựa trên thư viện tương tác cao `Plotly`.
- **Đánh giá Chuyên Sâu**: Hiển thị tường minh các chỉ số kiểm tra mô hình bao gồm: *Accuracy, Precision, Recall, F1-Score, AUC*, cùng biểu đồ Ma trận nhầm lẫn (Confusion Matrix) và đường cong ROC.
- **Sử Dụng Linh Hoạt**:
  - Chế độ nhập liệu thủ công để kiểm tra rủi ro tức thì cho một giao dịch đơn lẻ.
  - Chế độ chấm điểm hàng loạt qua file danh sách Excel/CSV giúp tự động hóa vận hành.

## 📁 Cấu trúc dữ liệu yêu cầu
Mẫu dữ liệu huấn luyện hoặc chấm điểm cần tuân thủ cấu trúc định dạng cột sau:
- **Biến đặc trưng (X)**: Gồm chính xác 14 cột số mang tên từ `X_1` đến `X_14`.
- **Biến mục tiêu (y)**: Cột nhãn `default` chứa giá trị nhị phân (`0`: Bình thường, `1`: Rủi ro).

## ⚙️ Hướng dẫn Cài đặt & Khởi chạy

### Bước 1: Cài đặt các thư viện cần thiết
```bash
pip install -r requirements.txt
