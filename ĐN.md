ĐỊNH NGHĨA BÀI TOÁN
1. Tên bài toán:
Phân loại độ tin cậy của đánh giá sản phẩm trên các sàn thương mại điện tử bằng mô hình học máy.
2. Bối cảnh bài toán:
Trong môi trường thương mại điện tử, người tiêu dùng thường dựa vào các đánh giá sản phẩm (bao gồm số sao, nội dung văn bản và hình ảnh đính kèm) để đưa ra quyết định mua hàng. Tuy nhiên, một số đánh giá có thể không đáng tin cậy (giả mạo, spam, hoặc mang tính thao túng đánh giá). Việc phát hiện và phân loại các đánh giá không đáng tin cậy sẽ giúp nâng cao trải nghiệm người dùng và tính minh bạch của nền tảng.
3. Mục tiêu bài toán:
Xây dựng một mô hình học máy có khả năng phân loại các đánh giá thành 2 nhóm: "đáng tin cậy" hoặc "không đáng tin cậy", dựa trên các thông tin đầu vào như số sao, nội dung đánh giá văn bản và hình ảnh đính kèm (URL ảnh).
4. Đầu vào dữ liệu (Input):
- Số sao (từ 1 đến 5).
- Nội dung văn bản đánh giá.
- URL hình ảnh (nếu có).
- (Sau khi thu thập và tiền xử lý) gán nhãn thủ công cho mỗi đánh giá: 1 = đáng tin cậy, 0 = không đáng tin cậy.
5. Đầu ra (Output):
Một mô hình phân loại có thể dự đoán độ tin cậy của các đánh giá chưa được gán nhãn (test set).
6. Bản chất bài toán:
- Đây là bài toán phân loại nhị phân (binary classification) trong lĩnh vực học máy thống kê.
- Tập dữ liệu cần được xử lý kỹ lưỡng về:
   + Làm sạch văn bản (text cleaning).
   + Trích xuất đặc trưng (feature extraction: TF-IDF, embedding…).
   + Xử lý hình ảnh (nếu đưa vào mô hình đa modal).
- Có thể áp dụng các mô hình: Logistic Regression, SVM, Random Forest, hoặc Deep Learning (BERT, CNN cho ảnh).
