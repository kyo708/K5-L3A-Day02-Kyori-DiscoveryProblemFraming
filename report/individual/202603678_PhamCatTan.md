# Báo cáo cá nhân — 202603678_PhamCatTan

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Cát Tân
- MSSV: 2A202603678
- Email trường (không bắt buộc, repo có thể để public): 26ai.tanpc@vinuni.edu.vn
- Tên nhóm: Kyori
- Link repo nhóm: https://github.com/kyo708/K5-L3A-Day02-Kyori-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi có nhiều deadline tới hạn tôi không control được các task và không biết bắt đầu nên hoàn thành task nào trước | PM, team | khoảng 2 tháng trước bị sếp phàn nàn vì trễ deadline |
| 2 | Tốn thời gian | Khi sếp giao 1 task về research và MVP trong 2 tuần nhưng mãi đọc paper và sử tìm cách implement paper đó cho task mà sếp giao là dùng Gen AI để sinh synthetic data ảnh để train mà thời gian gen 30 giây cho 1 ảnh nên đã không làm MVP kịp trong 2 tuần | team | sếp đã phàn nàn vấn đề này khoảng tháng 09/2026 |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận một yêu cầu phát triển tính năng, tôi muốn tổng hợp thông tin từ tài liệu SRS, Figma và Jira để hiểu đầy đủ nghiệp vụ | Developer, BA | Chọn 3–5 task, đếm số nguồn phải đọc, số lần hỏi lại và thời gian làm rõ yêu cầu |
| 4 | Pain từ người khác | Khi Frontend Developer sử dụng API, họ muốn biết chính xác cấu trúc request/response để không phải liên tục hỏi Backend Developer | FE, BE | Phỏng vấn 2–3 frontend dev, ghi nhận số lần API sai contract hoặc phải hỏi lại backend |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi hệ thống gặp lỗi production, tôi muốn nhanh chóng tổng hợp log từ nhiều service để xác định nguyên nhân và mức độ ảnh hưởng | BE, DevOps | Xem các incident gần đây, đo thời gian điều tra, số nguồn log và số người tham gia |
| 6 | Lặp lại | Khi hoàn thành API mới, tôi muốn tài liệu API được cập nhật đồng bộ để không phải sửa Swagger hoặc Postman thủ công nhiều lần | BE, FE | Kiểm tra 5–10 API gần nhất, đếm số API thiếu tài liệu hoặc có thông tin sai |
| 7 | Tốn thời gian | Khi tham gia một dự án đã phát triển lâu, tôi muốn hiểu nhanh cấu trúc source code và luồng nghiệp vụ để có thể bắt đầu nhận task | Developer | Phỏng vấn developer mới; đo số ngày từ lúc nhận source đến khi hoàn thành task đầu tiên |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Developer mới mất nhiều thời gian hiểu codebase | Dễ gặp trong dự án phần mềm, có thể đo thời gian onboarding | Bao nhiêu thời gian thực sự dành để tìm hiểu code? |
| 2 | Thông tin yêu cầu phân tán giữa SRS, Figma, Jira | Ảnh hưởng đến cả Developer, BA, Tester | Vấn đề do tài liệu phân tán hay yêu cầu chưa rõ? |
| 3 | Frontend và Backend gặp khó khăn khi tích hợp API | Có thể gây chậm tiến độ, dễ kiểm tra qua bug và task | Bao nhiêu lỗi thực sự xuất phát từ API contract? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi mới tham gia một dự án phần mềm đã tồn tại, tôi muốn nhanh chóng hiểu cấu trúc source code và các luồng nghiệp vụ chính để có thể bắt đầu phát triển tính năng mà không liên tục nhờ đồng nghiệp giải thích |
| Actor | Developer mới tham gia dự án |
| Thời điểm / bối cảnh | Khi Developer mới tham gia dự án đã có sẵn source code và được giao task đầu tiên, cần tìm hiểu cấu trúc hệ thống, các module liên quan và luồng xử lý nghiệp vụ trước khi bắt đầu lập trình. |
| Quy trình hiện tại (3–7 bước) | - 1. Đọc README và tài liệu dự án - 2. Cài đặt môi trường và chạy dự án - 3. Tìm hiểu cấu trúc thư mục, class, function - 4. Truy vết luồng nghiệp vụ qua nhiều file - 5. Hỏi đồng nghiệp để xác nhận cách hệ thống hoạt động |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước Truy vết luồng nghiệp vụ qua nhiều file: mất khoảng 60 phút để tìm các class, function, API và hiểu mối liên hệ giữa các thành phần trong hệ thống |
| Impact (nếu không giải thì sao) | Developer mất nhiều thời gian làm quen với dự án, chậm hoàn thành task đầu tiên, thường xuyên phải nhờ Senior Developer hỗ trợ, gây gián đoạn công việc của cả hai. Ngoài ra, việc chưa hiểu rõ luồng nghiệp vụ có thể dẫn đến sửa code sai hoặc phát sinh bug |
| Success metric (baseline → target) | Giảm thời gian tìm hiểu source code và luồng nghiệp vụ liên quan đến task đầu tiên từ 165 phút xuống ≤ 90 phút (giảm khoảng 45%). Đồng thời giảm số lần phải hỏi Senior Developer khi tìm hiểu luồng code |
| Phương án không dùng AI | Viết tài liệu onboarding, sơ đồ kiến trúc, danh sách module và các luồng nghiệp vụ quan trọng |
| Giả thuyết về AI (nếu có) | Công cụ có khả năng tìm kiếm và giải thích code theo ngữ cảnh, truy vết các hàm liên quan đến yêu cầu của developer |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 165 phút (ước lượng)

[Đọc README và tài liệu: 15']
→ [Cài đặt môi trường, chạy dự án: 30']
→ [Tìm hiểu cấu trúc source code: 40']
→ [Truy vết luồng nghiệp vụ: 60']
→ [Hỏi Senior Developer: 20']
→ [Sẵn sàng phát triển task đầu tiên]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận một task phát triển tính năng mới, tôi muốn nhanh chóng tổng hợp đầy đủ thông tin từ Jira, tài liệu SRS và Figma để hiểu chính xác yêu cầu nghiệp vụ, tránh bỏ sót thông tin hoặc phải hỏi lại BA nhiều lần |
| Actor | Frontend Developer hoặc Backend Developer được giao phát triển tính năng mới.  |
| Thời điểm / bối cảnh | Khi Developer nhận task mới từ Jira nhưng thông tin nghiệp vụ, giao diện và các yêu cầu kỹ thuật nằm ở nhiều nguồn khác nhau. Developer phải tìm kiếm, đọc và đối chiếu tài liệu trước khi bắt đầu lập trình. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc nội dung task trên Jira. 2. Tìm kiếm và đọc tài liệu SRS liên quan. 3. Kiểm tra thiết kế giao diện trên Figma. 4. Đối chiếu các tài liệu để xác định đầy đủ yêu cầu. 5. Trao đổi với BA để làm rõ những thông tin thiếu hoặc không thống nhất. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 Đối chiếu thông tin giữa nhiều tài liệu: ước tính mất khoảng 30 phút để tổng hợp yêu cầu và xác định các điểm chưa thống nhất giữa Jira, SRS và Figma |
| Impact (nếu không giải thì sao) | Developer mất nhiều thời gian tìm hiểu yêu cầu trước khi lập trình. Thông tin không đồng nhất có thể khiến Developer hiểu sai nghiệp vụ, triển khai sai chức năng hoặc phải sửa lại code. Ngoài ra, BA cũng thường xuyên bị gián đoạn để giải thích lại yêu cầu |
| Success metric (baseline → target) | Giảm thời gian tìm hiểu và tổng hợp yêu cầu cho một task từ 100 phút xuống ≤ 45 phút (giảm 55%). Đồng thời giảm số lần phải hỏi lại BA và số task cần sửa do hiểu sai yêu cầu |
| Phương án không dùng AI | Chuẩn hóa template Jira, bổ sung checklist nghiệp vụ và liên kết trực tiếp tài liệu SRS, Figma vào từng task. Quy định một nguồn thông tin chính thức để tránh mâu thuẫn giữa các tài liệu |
| Giả thuyết về AI (nếu có) | Công cụ AI có thể đọc và tổng hợp thông tin từ Jira, SRS và Figma, xác định các yêu cầu liên quan, phát hiện điểm không thống nhất và tạo bản tóm tắt nghiệp vụ để Developer kiểm tra trước khi lập trình |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 100 phút/task (ước lượng)

[Đọc task Jira: 10']
→ [Đọc tài liệu SRS: 25']
→ [Kiểm tra Figma: 20']
→ [Đối chiếu và tổng hợp yêu cầu: 30']
→ [Hỏi BA để làm rõ yêu cầu: 15']
→ [Bắt đầu phát triển tính năng]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tích hợp API từ Backend vào giao diện, tôi muốn có tài liệu API chính xác và cấu trúc request/response thống nhất để có thể triển khai chức năng nhanh chóng mà không phải mất nhiều thời gian debug hoặc trao đổi lại với Backend Developer |
| Actor | Frontend Developer chịu trách nhiệm tích hợp API vào giao diện ứng dụng. |
| Thời điểm / bối cảnh | Khi Backend đã phát triển API và Frontend bắt đầu tích hợp vào hệ thống. Trong quá trình tích hợp, cấu trúc dữ liệu thực tế có thể khác với tài liệu Swagger hoặc yêu cầu ban đầu, khiến Frontend phải kiểm tra và trao đổi lại với Backend |
| Quy trình hiện tại (3–7 bước) | 1. Đọc tài liệu API trên Swagger. 2. Kiểm tra cấu trúc request/response và các trường dữ liệu. 3. Viết code gọi API và xử lý dữ liệu trên giao diện. 4. Debug khi dữ liệu thực tế không khớp với tài liệu hoặc cấu trúc mong đợi. 5. Trao đổi với Backend Developer, điều chỉnh code và kiểm thử lại. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 Debug lỗi API contract: ước tính mất khoảng 30 phút để xác định nguyên nhân dữ liệu không khớp, kiểm tra request/response và tìm vị trí cần chỉnh sửa |
| Impact (nếu không giải thì sao) | Frontend Developer mất thêm thời gian debug và chờ phản hồi từ Backend. Việc tích hợp API bị chậm có thể ảnh hưởng đến tiến độ hoàn thành tính năng. Ngoài ra, sai lệch giữa tài liệu và API thực tế có thể gây lỗi giao diện hoặc phát sinh bug trong quá trình kiểm thử |
| Success metric (baseline → target) | Giảm thời gian tích hợp và xử lý vấn đề API contract cho một chức năng từ 115 phút xuống ≤ 70 phút (giảm khoảng 39%). Đồng thời giảm số lỗi request/response không khớp và số lần Frontend phải hỏi lại Backend. |
| Phương án không dùng AI | Chuẩn hóa API contract bằng OpenAPI/Swagger, tự động sinh TypeScript types, sử dụng mock API và contract testing để kiểm tra tính nhất quán giữa Backend và Frontend |
| Giả thuyết về AI (nếu có) | Công cụ AI có thể phân tích tài liệu API và source code Frontend, phát hiện sự khác biệt giữa request/response được khai báo và dữ liệu thực tế, đồng thời gợi ý cách điều chỉnh code tích hợp |
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 115 phút/chức năng (ước lượng)

[Đọc Swagger: 15']
→ [Kiểm tra request/response: 15']
→ [Viết code tích hợp API: 35']
→ [Debug lỗi dữ liệu không khớp: 30']
→ [Trao đổi Backend và kiểm thử lại: 20']
→ [Hoàn thành tích hợp API]
```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
