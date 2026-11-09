# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Vũ Thanh Toàn
- MSSV:2A202603654
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:Kyori
- Link repo nhóm:https://github.com/kyo708/K5-L3A-Day02-Kyori-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại | Mỗi ngày tôi đều phải đọc tài liệu và chuẩn bị giáo án cho ngày hôm sau để ngày mai có thể lên lớp | giáo viên  | mỗi ngày tốn 2 đến 4 giờ để chuẩn bị giáo án |
| 2 | Lặp lại | Lượng email gửi đến một ngày đang quá lớn việc ngồi đọc để lọc mail rác và tổng hợp thông tin quan trọng khiến tôi rất mất thời gian | KOC , quản lý | nhận 30-100 mail một ngày, thường xuyên phải đọc mail rác, mail cũ |
| 3 | Cần đọc, tổng hợp nhiều thông tin| là một nhà tuyển dụng khi đọc thủ công CV của quá nhiều ứng viên rất mất thời gian và dễ miss thông tin ứng viên tôi muốn thông tin ứng viên được tổng hợp và so sánh theo một tiêu chí để tiết kiệm thời gian  | HR, nhà tuyển dụng | hàng chục, hàng trăm CV mất thời gian sàng lọc thủ công |
| 4 |Cần đọc, Tổng hợp nhiều thông tin | Khi ra mắt một sản phẩm mới hoặc dự án mới thường có khá nhiều feedback được gửi về qua nhiều kênh thông tin khác nhau tôi muốn các thông tin feedback được tổng hợp và sàng lọc tìm ra các vấn đề phổ biến để tiếp tục phát triển sản phẩm | chủ doanh nghiệp, PM | phản hồi đến từ nhiều kênh fb,tiktok..., việc đọc và tổng hợp thông tin thường gặp khó khăn |
| 5 | Lặp Lại | Khi khách hàng liên tục hỏi các câu hỏi giống nhau tôi muốn có hệ thống tự động trả lời để tiết kiệm thời gian | nhân viên CSKH, chủ shop | liên tục phải trả lời các câu hỏi về giá, vận chuyển, bảo hành |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Sàng lọc CV tuyển dụng | Vấn đề thực tế, đối tượng sử dụng rõ ràng, quy trình lặp lại và AI có thể hỗ trợ đọc, phân loại, so sánh CV | AI đánh giá CV chính xác đến đâu? HR có sẵn sàng sử dụng không? |
| 2 | Chatbot trả lời câu hỏi lặp lại của khách hàng | Giảm thời gian CSKH trả lời các câu hỏi phổ biến về giá, vận chuyển, bảo hành | Chatbot có hiểu đúng câu hỏi và trả lời chính xác không? |
| 3 | Tổng hợp feedback sản phẩm | Giúp doanh nghiệp tổng hợp phản hồi từ nhiều kênh, nhanh chóng nhận diện vấn đề phổ biến | AI có phân loại chính xác feedback và xác định đúng vấn đề ưu tiên không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | hi ra mắt một sản phẩm mới hoặc dự án mới thường có khá nhiều feedback được gửi về qua nhiều kênh thông tin khác nhau tôi muốn các thông tin feedback được tổng hợp và sàng lọc tìm ra các vấn đề phổ biến để tiếp tục phát triển sản phẩm |
| Actor | chủ doanh nghiệp, PM |
| Thời điểm / bối cảnh | Khi vừa ra mắt sản phẩm hoặc triển khai một dự án mới |
| Quy trình hiện tại (3–7 bước) | 1. Ra mắt sản phẩm 2. Nhận được các feedback từ nhiều kênh 3. Vào từng kênh để đọc và tổng hợp 4. so sánh những vấn đề xem cái nào là phổ biến 5. Nâng cấp, phát triển sản phẩm |
| Bottleneck (bước nào, mất bao nhiêu phút) | bước 3 việc vào từng kênh đọc và tổng hợp thường tốn cả buổi |
| Impact (nếu không giải thì sao) | có thể tốn nhiều người và mất cả ngày để ngồi và tổng hợp  |
| Success metric (baseline → target) | giải phóng nhân lực để mn có thể làm những việc khác |
| Phương án không dùng AI | thay vì chờ từng fb đến và tổng hợp luôn sẽ có mốc thời gian cố định để tổng hợp  |
| Giả thuyết về AI (nếu có) | ai sẽ tự động tổng hợp và cập nhật theo thời gian thực để có thể phát hiện vấn đề sớm nhất |
| Cảm nhận nhanh | No AI / Rule / Workflow / Agent / Chưa biết | worklow

Quy trình nháp hiện tại:

```text

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi phải tuyển dụng và nhận được quá nhiều CV từ ứng viên, tôi muốn thông tin ứng viên được tự động tổng hợp, phân loại và so sánh theo các tiêu chí tuyển dụng để tiết kiệm thời gian sàng lọc và tránh bỏ sót ứng viên tiềm năng. |
| Actor | HR, nhà tuyển dụng, trưởng bộ phận tuyển dụng |
| Thời điểm / bối cảnh | Khi doanh nghiệp đăng tin tuyển dụng và nhận được số lượng lớn CV từ nhiều ứng viên. |
| Quy trình hiện tại (3–7 bước) | 1. Đăng tin tuyển dụng và đưa ra yêu cầu công việc 2. Nhận CV từ nhiều ứng viên qua email, website tuyển dụng hoặc nền tảng khác 3. Mở và đọc từng CV để tìm kiếm thông tin ứng viên 4. Đối chiếu kinh nghiệm, kỹ năng, trình độ với yêu cầu tuyển dụng 5. So sánh và phân loại ứng viên phù hợp, không phù hợp 6. Lập danh sách ứng viên tiềm năng để liên hệ phỏng vấn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và 4: Đọc từng CV, trích xuất thông tin và đối chiếu với tiêu chí tuyển dụng. Khi có hàng chục đến hàng trăm CV, công việc này có thể mất nhiều giờ hoặc cả ngày |
| Impact (nếu không giải thì sao) | Tốn nhiều nhân lực và thời gian cho việc sàng lọc thủ công. HR dễ bỏ sót ứng viên tiềm năng, đánh giá thiếu nhất quán hoặc mất nhiều thời gian mới tìm được người phù hợp |
| Success metric (baseline → target) | Giảm thời gian sàng lọc CV; giảm thời gian xử lý mỗi CV; giảm số giờ HR phải dành cho công việc đọc và phân loại CV thủ công |
| Phương án không dùng AI | Xây dựng một biểu mẫu CV thống nhất và bảng Excel chứa các tiêu chí tuyển dụng. HR sử dụng bộ lọc và công thức Excel để phân loại, so sánh ứng viên thay vì đọc và ghi chép hoàn toàn thủ công |
| Giả thuyết về AI (nếu có) | AI tự động đọc CV (PDF, DOCX), trích xuất thông tin như học vấn, kinh nghiệm, kỹ năng và dự án. Sau đó đối chiếu với JD, chấm mức độ phù hợp theo từng tiêu chí, tổng hợp và xếp nhóm ứng viên để HR dễ dàng đánh giá |
| Cảm nhận nhanh | Workflow

Quy trình nháp hiện tại:

```text

```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách hàng liên tục hỏi những câu hỏi giống nhau về sản phẩm và dịch vụ, tôi muốn có một hệ thống tự động tiếp nhận và trả lời các câu hỏi phổ biến để tiết kiệm thời gian, giảm khối lượng công việc và nâng cao hiệu quả chăm sóc khách hàng |
| Actor | 	Nhân viên CSKH, chủ shop, nhân viên bán hàng |
| Thời điểm / bối cảnh | Khi cửa hàng kinh doanh online hoặc doanh nghiệp có lượng lớn khách hàng liên hệ qua Facebook, Zalo, website và các nền tảng khác |
| Quy trình hiện tại (3–7 bước) | 1. Khách hàng gửi câu hỏi qua các kênh liên hệ 2. Nhân viên tiếp nhận và đọc tin nhắn 3. Xác định nội dung câu hỏi của khách hàng 4. Tìm kiếm thông tin về giá, vận chuyển, bảo hành hoặc sản phẩm 5. Soạn câu trả lời và gửi lại khách hàng 6. Tiếp tục xử lý những câu hỏi tương tự từ các khách hàng khác |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, 3, 4 và 5: Nhân viên phải liên tục đọc, phân loại câu hỏi, tìm thông tin và soạn câu trả lời. Mỗi câu hỏi có thể mất vài phút, đặc biệt khi phải xử lý nhiều khách hàng cùng lúc |
| Impact (nếu không giải thì sao) | Nhân viên CSKH phải dành nhiều thời gian cho các câu hỏi lặp lại, làm giảm thời gian xử lý những vấn đề phức tạp. Khách hàng có thể phải chờ lâu, dẫn đến trải nghiệm không tốt và bỏ lỡ cơ hội bán hàng |
| Success metric (baseline → target) | Giảm thời gian phản hồi trung bình; tăng tỷ lệ câu hỏi phổ biến được xử lý tự động; giảm số lượng câu hỏi nhân viên phải trả lời thủ công |
| Phương án không dùng AI | Xây dựng bộ câu trả lời mẫu cho các câu hỏi thường gặp, phân loại theo chủ đề như giá cả, vận chuyển, bảo hành. Nhân viên sử dụng câu trả lời có sẵn để phản hồi nhanh hơn |
| Giả thuyết về AI (nếu có) | AI có thể tự động phân tích nội dung tin nhắn, nhận diện ý định khách hàng và tìm kiếm câu trả lời từ dữ liệu sản phẩm, chính sách cửa hàng. Hệ thống tự động phản hồi các câu hỏi phổ biến và chuyển tiếp cho nhân viên khi gặp tình huống phức tạp hoặc không đủ thông tin |
| Cảm nhận nhanh | Workflow

Quy trình nháp hiện tại:

```text

```

### Card muốn pitch nhất

- Card số:2
- Vì sao: vì đây là vấn đề thực tế và hiệu quả có thể do lường cụ thể 
- Câu hỏi muốn nhóm phản biện: ai có thực sự đánh giá đúng năng lực ứng viên? việc bỏ sót ứng viên tiềm năng được giải quyết như nào?

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
