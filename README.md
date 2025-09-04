# 📘 DSTC 2025 – Vòng 2 (Bảng Đại học)

## 🚀 Giới thiệu  
Repo này chứa toàn bộ code dự thi **Data Science Talent Competition 2025 – Vòng 2 (Bảng Đại học)**.  
Chúng tôi xây dựng chiến lược **lựa chọn cổ phiếu thông minh**, kết hợp **Phân tích cơ bản (FA)**, **Phân tích kỹ thuật (TA)**, **Feature Engineering** và **Machine Learning + Backtest** để tạo danh mục tối ưu.

---

## 📂 Cấu trúc repo  

- `Cào dữ liệu FA.ipynb` → Thu thập dữ liệu tài chính doanh nghiệp.  
- `Cào dữ liệu timestamp.ipynb` → Thu thập & đồng bộ dữ liệu theo mốc thời gian.  
- `FA_filter.ipynb` → Lọc sơ cấp theo tiêu chí: ROE > 0, D/E < 2.5, Net Revenue Growth YoY > 0.  
- `FA_Score.ipynb` → Tính điểm FA đa tiêu chí, chọn doanh nghiệp có nền tảng tốt.  
- `TA_calculate.ipynb` → Tính toán chỉ báo kỹ thuật, chọn top cổ phiếu theo ngành.  
- `ML_Backtest.ipynb` → Feature Engineering nâng cao, huấn luyện mô hình ML (XGBoost, LightGBM…), backtest danh mục, so sánh với VNIndex.  

---

## 🔑 Quy trình phân tích  

1. **Cào dữ liệu FA + TA** (báo cáo tài chính, giá, volume).  
2. **FA Filter** → loại bỏ cổ phiếu yếu, giữ ~964 mã.  
3. **FA Score** → chấm điểm đa tiêu chí, giữ ~449 mã.  
4. **TA Calculate + Sector Tagging** → chọn Top 10 mỗi ngành, còn 103 mã.  
5. **Feature Engineering + ML** → tạo thêm feature, huấn luyện mô hình ML tối ưu trọng số.  
6. **Backtest** → kiểm tra hiệu suất danh mục vs VNIndex.  

---

## ⚙️ Hướng dẫn chạy code  

Chạy lần lượt các notebook theo thứ tự:  

1. `Cào dữ liệu FA.ipynb`  
2. `Cào dữ liệu timestamp.ipynb`  
3. `FA_filter.ipynb`  
4. `FA_Score.ipynb`  
5. `TA_calculate.ipynb`  
6. `ML_Backtest.ipynb`  

---

## 📊 Kết quả nổi bật  

- Danh mục cuối cùng gồm **103 cổ phiếu** từ 11 ngành.  
- **Backtest**: danh mục vượt trội VNIndex cả về lợi nhuận và rủi ro  
  - Lợi nhuận cao hơn  
  - Sharpe Ratio tốt hơn  
  - Drawdown thấp hơn  
- **Insight**: FA giúp loại bỏ DN yếu, TA bắt xu hướng, ML tối ưu hóa trọng số → chiến lược thông minh và có khả năng mở rộng.  

---

## 👨‍💻 Nhóm thực hiện  

- Nhóm: Stock Crasher 
- Thành viên: Tạ Tuấn Thành, Bùi Quang Vinh, Phi Anh Khôi
