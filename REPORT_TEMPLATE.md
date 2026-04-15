\# CSC4005 - Lab 1 Report



\## 1. Mục tiêu

Mục tiêu của bài lab là xây dựng mô hình phân loại ảnh sử dụng MLP trên bộ dữ liệu NEU.



\## 2. Cấu hình thí nghiệm

\- baseline\_adamw: AdamW, lr=0.001, dropout=0.3, img\_size=64, epochs=20

\- runB\_more\_epochs: AdamW, lr=0.001, dropout=0.3, img\_size=64, epochs=33

\- runC\_larger\_image: AdamW, lr=0.001, dropout=0.2, img\_size=128, epochs=50



\## 3. Kết quả

\- baseline\_adamw: val\_acc=41.85%, test\_acc=38.15%

\- runB\_more\_epochs: val\_acc=35.93%, test\_acc=33.33%

\- runC\_larger\_image: val\_acc=53.33%, test\_acc=52.59%



\### Learning Curves

!\[Learning Curves](outputs/runC\_larger\_image/curves.png)



\### Confusion Matrix

!\[Confusion Matrix](outputs/runC\_larger\_image/confusion\_matrix.png)



\## 4. Phân tích

Run C là cấu hình tốt nhất. Việc tăng kích thước ảnh từ 64 lên 128 giúp mô hình học được nhiều đặc trưng hơn, cải thiện đáng kể độ chính xác.



\## 5. Kết luận

Best model: runC\_larger\_image với val\_acc=53.33% và test\_acc=52.59%.

