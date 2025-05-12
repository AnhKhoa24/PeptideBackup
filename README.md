# 🔬 Dự đoán Peptide Kháng Khuẩn bằng LSTM kết hợp XAI

## 🧬 Giới thiệu

Dự án này tập trung xây dựng và đánh giá các mô hình học máy nhằm phân loại các chuỗi peptide thành **AMP (Antimicrobial Peptides)** và **nAMP (non-Antimicrobial Peptides)**. Đây là một hướng đi mới giúp hỗ trợ nhanh chóng trong quá trình phát hiện, thiết kế và phát triển thuốc kháng sinh mới – đặc biệt trong bối cảnh vấn nạn **kháng thuốc kháng sinh (AMR)** ngày càng trầm trọng.

Hai mô hình chính được phát triển:

- **Support Vector Machine (SVM)** sử dụng đặc trưng trích xuất từ chuỗi peptide (GPSD).
- **Long Short-Term Memory (LSTM)** xử lý trực tiếp chuỗi peptide dưới dạng tuần tự mà không cần trích xuất thủ công.

## 📂 Cấu trúc dự án

```
PEPTIDE_PROJECT_OFF/
├── Document		      # Tài liệu lý thuyết về dự án
├── Example                   # Các notebook được tham khảo
├── MyWork/                   # Thư mục làm việc chính
    ├── Crawl_data/	      # Công cụ về crwal dữ liệu
    ├── Harvest_data/	      # Datasets
    ├── MyNoteBook/	      # Thư mục làm việc phân tích và huấn luyện mô hình
    └── Reference/	      # Tài liệu tham khảo
```

## 📊 Mô hình và kết quả

| Mô hình | Accuracy | F1-Score | Sensitivity | Specificit |
| --------- | -------- | -------- | ----------- | ---------- |
| LSMT      |          |          |             |            |

### 🔍 Giải thích mô hình (XAI)

Dự án áp dụng **Explainable AI (XAI)** để:

- Phân tích ảnh hưởng của từng amino acid tới dự đoán.
- Hiển thị trực quan các chuỗi có độ ảnh hưởng cao đối với quyết định của mô hình.
- So sánh tính quan trọng của các đặc trưng trong SVM và các bước học tự động trong LSTM.

## 🔧 Cài đặt

```bash
git clone https://github.com/AnhKhoa24/Peptide-Final-semester-project-.git
cd PEPTIDE_PROJECT_OFF
pip install -r requirements.txt
```

## 🚀 Cách chạy mô hình

### Huấn luyện mô hình SVM:

```bash
python models/svm_model.py
```

### Huấn luyện mô hình LSTM:

```bash
python models/lstm_model.py
```

### Phân tích XAI:

```bash
python xai/visualize.py
```

## 🧠 Công nghệ sử dụng

- Python
- Scikit-learn
- Keras / Tensorflow
- BioPython
- Matplotlib / Seaborn
- SHAP (hoặc LIME) cho XAI

## 📚 Tài liệu tham khảo

- NCBI - National Center for Biotechnology Information
- Global Protein Sequence Descriptor (GPSD)
- Deep Learning for Bioinformatics

## ✅ Kết luận

Mô hình LSTM cho thấy khả năng vượt trội trong việc xử lý chuỗi peptide và dự đoán AMP so với SVM truyền thống. Bằng cách kết hợp học sâu và XAI, dự án không chỉ tăng độ chính xác mà còn giúp hiểu rõ hơn về cơ chế dự đoán, hỗ trợ cho việc phát triển các peptide kháng khuẩn tiềm năng trong tương lai.

---

**Người phát triển:** Huynh Anh Khoa |
**Liên hệ:** anhkhoa.24052003@gmail.com
