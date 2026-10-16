# Lab 27 — CS12: Đánh giá sản phẩm AI (bài tập buổi sáng 16/10/2026)

Bài thực hành đi kèm bộ slide "AI Evaluation" (66 trang). Mọi bài dùng chung một tình huống giả định: **trợ lý đổi trả "Mộc" của cửa hàng Mộc Store** (khoảng 300 tin nhắn đổi trả mỗi ngày, chuyên gia là chị Ngân, trưởng nhóm chăm sóc khách hàng).

## Thành viên nhóm H3201

| STT | Họ và tên | MSSV |
|---|---|---|
| 1 | Phan Duy Thành | 2A202602930 |
| 2 | Chử Trần Phương Nam | 2A202602675 |
| 3 | Phùng Gia Khánh | 2A202602585 |
| 4 | Bùi Hải Nam | 2A202602636 |
| 5 | Tô Anh Đức | 2A202602639 |

## Các file trong thư mục

| File | Là gì |
|---|---|
| `H3201_CS12.xlsx` | **Bài nộp** trên VLearn (Bài 1–5 và Xưởng đã điền) |

Chỉ điền các ô màu vàng, không sửa công thức. Các trang vẫn khoá như bản gốc.

## Bài 1–5 (cá nhân, không tính điểm)

| Bài | Nội dung | Kết quả tự kiểm tra |
|---|---|---|
| Bài 1 | Đọc báo cáo đánh giá và thu hẹp phạm vi | 9/9 |
| Bài 2 | Phủ ca và chọn tình huống | 14/14 |
| Bài 3 | Đọc vết thực thi, tìm bước sai đầu tiên | 9/9 |
| Bài 4 | Chọn cách chấm và ra kết luận | 15/15 |
| Bài 5 | Hiệu chỉnh giám khảo AI | 18/18 |

Một vài điểm đáng nhớ:
- **Bài 1:** v1.4 qua cổng tổng (84% ≥ 82%) nhưng nhóm Tra cứu đơn tụt 30 điểm (90% → 60%), nên chưa phát hành mà đọc 3 tin hồi quy trước. Muốn tin một khoảng chênh 3 điểm cần khoảng 1.000 ca.
- **Bài 4:** chọn **Lặp tiếp**: "Ghi nhận cảm xúc khách" tụt 8 điểm (84% → 76%), vượt mức cho phép 2 điểm. Đòn làm trước là sửa câu lệnh.
- **Bài 5:** TPR 87,5%, TNR 50%, kappa 0,40. Giám khảo chưa đạt vì TNR thấp (cho qua lỗi), cần siết định nghĩa Không đạt và thêm ví dụ trượt sát ranh.

## Xưởng (theo nhóm, 10 điểm)

| Phần | Nhóm đã làm | Tự kiểm tra |
|---|---|---|
| X1 · Đơn vị công việc AI | Đọc 1 tin nhắn đổi trả + kết quả `tra_cuu_don` → 1 câu trả lời theo CS-1 đến CS-6 kèm 1 bước tiếp theo, dưới 5 giây; hàng lỗi hoặc khách đòi gặp người thì gọi `chuyen_nhan_vien` | Đạt |
| X2 · Chiều và phễu | Ý định chính (3) × Thông tin đơn (3) × Tình trạng đơn (3) = 27 tổ hợp, loại 6 tổ hợp phi lý, chọn 15 tình huống × 3 cách diễn đạt = **45 đầu vào** | Đạt |
| X3 · 8 tình huống | 3 đại diện, 3 thử thách (thiếu mã đơn, 2 đơn trong 1 tin, tin không dấu báo hàng lỗi), 2 hồi quy nghiêm trọng (đòi hoàn tiền khi quá hạn, khách bực đòi gặp quản lý) | Đạt |
| X4 · 3 vết thực thi | W1: bước 3 · `missing_lookup`; W2: bước 2 · `wrong_intent`; W3: bước 4 · `missing_escalation` | 6/6 ô đúng |
| X5 · 4 tiêu chí nhị phân | Tra cứu trước khi hứa (mã lệnh, ≥ 95%) · Chuyển nhân viên khi hàng lỗi/đòi gặp người (mã lệnh + người kiểm mẫu 10%, ≥ 95%) · Không bịa mã đơn (mã lệnh, 100%) · Có bước tiếp theo (giám khảo AI, ≥ 90%) | Đạt |
| X6 · Hiệu chỉnh giám khảo | 4 ô: 12 / 2 / 0 / 6 → TPR 85,7% (dưới ngưỡng 90%), TNR 100% → kết luận **B** | 5/5 ô đúng |
| X7 · Kết luận có răng | **Phát hành** v1.4 (mọi tiêu chí đạt ngưỡng; Ghi nhận cảm xúc chỉ tụt 2 điểm = 1 tin trên 50, là nhiễu). Kế hoạch: lấy mẫu 5% tin thật mỗi ngày, 3 tín hiệu trôi có ngưỡng cảnh báo, chị Ngân quyết mỗi thứ Hai. Ba câu số liệu: 75% · 50 ca · 84% | 4/4 ô đúng |

Trang "Thang điểm" để trống cho giảng viên chấm.
