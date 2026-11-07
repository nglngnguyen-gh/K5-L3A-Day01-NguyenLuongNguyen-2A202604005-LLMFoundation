# Báo cáo cá nhân — Day 01: Lọc tin nhắn rác bằng ML, DL, Embedding và LLM

> Đổi tên file này thành `MSSV_HoTen.md` của bạn, ví dụ `2A20260000_NguyenVanAn.md`, rồi điền từng mục. Xoá các dòng hướng dẫn in nghiêng khi xong.

- **MSSV:** 2A202604005
- **Họ và tên:** Nguyễn Lương Nguyên
- **SEED** (in ở ô đầu notebook): 4115

## 1. Bằng chứng

| Tệp | Có? |
| --- | --- |
| [`day01_lab.ipynb`](day01_lab.ipynb) — notebook đã chạy, còn output | Có |
| [`lab1_report.json`](lab1_report.json) — do ô "Báo cáo cuối" sinh ra | Có |
| [`hand_calc.jpg`](hand_calc.jpg) — ảnh tính tay có các bước | Có |

## 2. Kết quả chính

                                  f1  f1_SUB
1. BoW + LogReg (tự code)        0.874   0.857
2. BoW + MLP (deep learning)     0.936   0.889
3a. Encoder (MiniLM) + kNN       0.895   0.923
3b. Encoder (MiniLM) + LogReg    0.923   0.947
3c. Encoder (MiniLM) + MLP head  0.953   0.947
4a. LLM nhỏ zero-shot            1.000   1.000
4b. LLM lớn zero-shot            1.000   1.000
4c. LLM nhỏ few-shot             1.000   1.000

## 3. Dự đoán và thực tế

  [16:39:04] ml_f1: F1 ~0.6, recall cao hơn vì số lượng positive cao hơn nhiều negative, model sẽ nghiêng về hướng negative, làm bỏ sót nhiều positive và làm recal cao
  [16:39:11] ml_lr: lr = 0.001 thì đường loss sẽ có dạng đường thẳng, lr=50 thì đường loss sẽ có hình gồ ghề
  [16:39:22] dl_curve: (1) Không giảm mãi (2) MLP có thể hơn Logistic Regression về F1

## 4. Phân tích 50 case khó

*Model nào tụt nhiều nhất, ở nhóm case nào? Nêu 2 case cụ thể và cơ chế khiến model sai.*

## 5. Thử thách cá nhân

*Đề theo SEED của bạn, cách làm, kết quả, giải thích.*

## 6. Phương án cho sản phẩm thật

*Với yêu cầu p95 < 50 ms/tin cho 10 triệu SMS/ngày: chọn phương án nào, dẫn số liệu nào, chấp nhận đánh đổi gì.*

## 7. AI log và điều đã học

*Mỗi lần dùng AI: hỏi gì, nhận gì, bạn sửa gì. Sau đó 2–3 câu: điều bạn hiểu ra hôm nay mà trước đó chưa hiểu.*
