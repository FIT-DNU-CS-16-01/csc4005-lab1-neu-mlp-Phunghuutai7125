# CSC4005 Lab 1 - Image Classification (MLP)

## 1. Giới thiệu

Bài toán phân loại ảnh sử dụng mô hình MLP trên bộ dữ liệu NEU Surface Defect.

---

## 2. Cách chạy

### Cài đặt

```bash
conda activate csc4005-dl
pip install -r requirements.txt
```

### Train model

```bash
python -m src.train --data_dir "D:\DL\Tuan2\NEU-CLS.zip" --run_name baseline_adamw
```

---

## 3. Experiments

* baseline_adamw
* runB_more_epochs
* runC_larger_image (best)

---

## 4. Kết quả

| Config            | val_acc    | test_acc   |
| ----------------- | ---------- | ---------- |
| baseline_adamw    | 41.85%     | 38.15%     |
| runB_more_epochs  | 35.93%     | 33.33%     |
| runC_larger_image | **53.33%** | **52.59%** |

👉 Best model: **runC_larger_image**

---

## 5. Kết luận

Tăng kích thước ảnh từ 64 lên 128 giúp cải thiện đáng kể hiệu suất mô hình.

---

## 6. W&B Dashboard

https://wandb.ai/phunghuutai07122005-/csc4005-lab1-neu-mlp
