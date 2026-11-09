# Team — Kyori

> Bản phân công đề xuất để ba thành viên duyệt. Tên, MSSV và việc chọn vấn đề CV do Trần Minh Tân cung cấp. Các nhiệm vụ dưới đây chưa được coi là đóng góp đã thực hiện. Mỗi người tự xác nhận phần của mình trước khi nộp.

## Thông tin nhóm

- Tên nhóm: Kyori.
- Candidate problem nhóm chọn: Khi nhận nhiều CV cho một vị trí, HR mất thời gian đọc và đối chiếu thông tin trình bày không đồng nhất với yêu cầu công việc để chuẩn bị hồ sơ cho bước xét duyệt tiếp theo.
- Phạm vi dự thảo: hỗ trợ trích xuất bằng chứng, HR tự quyết shortlist; không tự xếp hạng/loại ứng viên.
- Quyết định cuối dự thảo: **Not Yet**, cần kiểm chứng người dùng và quyền dùng dữ liệu trước triển khai thực tế; nhóm chưa xác nhận kết luận này.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò đề xuất, chờ duyệt | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Thanh Toàn | 2A202603654 | Phụ trách bối cảnh tuyển dụng, kiểm chứng và rà tiêu chí JD | Chưa cung cấp |
| 2 | Trần Minh Tân | 2A202603688 | Điều phối tổng hợp, research, quy trình, đối chiếu báo cáo | minhtantran99 |
| 3 | Phạm Cát Tân | 2A202603678 | Phản biện phạm vi, kiểm chứng thứ hai, eval và rà rủi ro | Chưa cung cấp |

## Phân công theo checkpoint — đề xuất

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm cần tạo / rà |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Trần Minh Tân | Cả nhóm | Danh sách candidate, cluster, cây cơ hội, bảng điểm và biên bản thật |
| CP4 — Kiểm chứng | Vũ Thanh Toàn | Phạm Cát Tân | Mỗi người hỏi ít nhất một HR ngoài nhóm, ghi nguồn và thời điểm |
| CP4 — Research | Trần Minh Tân | Vũ Thanh Toàn | Rà 3 nguồn chính thức, xác nhận thông tin công cụ và khoảng trống |
| CP5 — Quy trình trước/sau | Trần Minh Tân | Vũ Thanh Toàn | Rà các bước, thời gian giả định, HITL và fallback |
| CP5 — Problem Statement v0 | Vũ Thanh Toàn | Trần Minh Tân | Duyệt actor, bước nghẽn, metric và boundary theo bằng chứng |
| CP6 — Mức can thiệp + v1 | Phạm Cát Tân | Cả nhóm | So sánh 4 mức, AI Canvas, PAIR và v1 |
| CP6 — Eval / rủi ro / quyết định | Phạm Cát Tân | Cả nhóm | Rà bộ 10 ca mẫu, 5 tiêu chí, 4 rủi ro, ngưỡng dừng và duyệt quyết định |

## Cá nhân

### VuThanhToan-2A202603654

**Thông tin đã nhận:** Trần Minh Tân chuyển danh sách ba chủ đề mang tên Vũ Thanh Toàn: sàng lọc CV, trả lời câu hỏi CSKH lặp lại, tổng hợp feedback.

**Phần việc phụ trách đề xuất:** bối cảnh HR, tiếp cận người phỏng vấn thứ nhất và rà các mục đối chiếu CV/JD.

**Đóng góp cụ thể:** đã có đầu vào ba chủ đề qua người đại diện; chưa có xác nhận phỏng vấn, đo lường hoặc sản phẩm nhóm do thành viên trực tiếp tạo.

**Bằng chứng đầu vào:**

- [Báo cáo cá nhân](report/individual/2A202603654_VuThanhToan.md), mục 2 (CP1): scan 5 vấn đề gồm giáo án, lọc email, sàng lọc CV, tổng hợp feedback và CSKH trả lời câu hỏi lặp lại.
- Báo cáo cá nhân, mục 3 (CP2): bảng top 3 (CV, chatbot CSKH, feedback) và 3 Problem Card đầy đủ actor, quy trình, bottleneck, impact, phương án không dùng AI. Card muốn pitch nhất là #2, sàng lọc CV.
- Từ đầu vào cá nhân sang [báo cáo nhóm](report/team/group_report.md):
  - Mục 2.1, dòng 1–3, là ba card của Toàn. Candidate #1 (CV) là candidate nhóm chọn ở mục 2.4.
  - Bottleneck "đọc và đối chiếu CV với yêu cầu" (bước 3–4 của Card #2) là cơ sở cho bước nghẽn ở mục 4.1.
  - Phương án không dùng AI "form CV thống nhất + bảng Excel tiêu chí" được dùng cho dòng No AI ở mục 6.2.
  - Hai câu Toàn muốn nhóm phản biện ("ai đánh giá đúng năng lực ứng viên?", "bỏ sót ứng viên tiềm năng xử lý thế nào?") dẫn tới boundary "AI không chấm điểm/loại ứng viên" và phân tích bỏ sót ở mục 6.4.
  - Giả thuyết AI ban đầu trong Card #2 (chấm mức phù hợp, xếp nhóm ứng viên) được nhóm thu hẹp lại thành chỉ trích bằng chứng có nguồn (mục 3.2, 7).

**Điều học được từ phần nhóm:** cách hoạt động team, phân chia công việc tìm hiểu đề tài, hoàn thành nhiệm vụ được giao

### TranMinhTan-2A202603688

**Phần việc phụ trách đề xuất:** điều phối tổng hợp, research, quy trình và rà tính nhất quán.

**Đóng góp đã có trong phiên làm việc:** cung cấp thông tin cá nhân, nhóm, cách học trên LMS/Phoenix/Discord/Outlook; chuyển ba chủ đề của Vũ Thanh Toàn; thông báo nhóm chọn CV; yêu cầu AI dựng bản báo cáo để nhóm duyệt và số liệu minh họa. Chưa ghi nhận phỏng vấn, pitch hoặc tự chạy eval.

**Bằng chứng:** [báo cáo cá nhân](report/individual/2A202603688_TranMinhTan.md), [dự thảo nhóm](report/team/group_report.md), [bộ ca eval giả lập](report/assets/cp6-cv-eval-synthetic.md). Research chính thức và nội dung dự thảo do trợ lý hỗ trợ, cần nhóm mở kiểm tra và duyệt.

**Điều học được từ phần nhóm:** Trần Minh Tân tự bổ sung sau khi trao đổi, kiểm chứng và phản biện thật.

### PhamCatTan-2A202603678

**Thông tin đã nhận:** họ tên và MSSV; chưa có ba vấn đề cá nhân hoặc tài khoản GitHub.

**Phần việc phụ trách đề xuất:** phản biện phạm vi, phỏng vấn người thứ hai, rà eval và rủi ro.

**Đóng góp cụ thể:** chưa ghi nhận sản phẩm thực tế. Ba candidate trong báo cáo nhóm mục 2.1 dòng 7–9 do AI đề xuất để thành viên xem, không phải lịch sử pitch.

**Bằng chứng:** cần bổ sung ghi chú/file hoặc commit sau khi thực hiện nhiệm vụ.

**Điều học được từ phần nhóm:** .

## Duyệt và thông tin còn thiếu

- [ ] Vũ Thanh Toàn xác nhận GitHub, vai trò và đóng góp thực tế.
- [ ] Phạm Cát Tân xác nhận GitHub, ba candidate, vai trò và đóng góp thực tế.
- [ ] Trần Minh Tân xác nhận phần việc sau khi rà bản dự thảo.
- [ ] Cả nhóm duyệt Problem Statement, số liệu thiết kế, phân công và quyết định.
- [ ] Mỗi thành viên tự điền điều học được và commit phần cá nhân bằng danh tính của mình.
