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

- Card số: 1
- Vì sao: Actor rõ là developer mới, phạm vi có thể giới hạn vào luồng nghiệp vụ của task đầu tiên. Có thể đo thời gian tìm hiểu code và số lượt hỏi Senior Developer, đồng thời so sánh với phương án tài liệu onboarding hoặc sơ đồ kiến trúc trước khi chọn mức hỗ trợ AI.
- Câu hỏi muốn nhóm phản biện (đề xuất khi rà lại card): Tài liệu onboarding, sơ đồ luồng nghiệp vụ và tìm kiếm code có thể giải quyết được bao nhiêu khó khăn của developer mới? Cần bằng chứng gì để xác định phần còn lại cần AI hỗ trợ?

### AI đã phản biện card thế nào

Các nhận xét dưới đây được bổ sung khi rà lại ba card. Cột “Đồng ý?” ghi rõ những điểm tôi chưa xác nhận; các đề xuất chưa thực hiện được ghi là đề xuất.

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Cả ba card có mốc thời gian 165/100/115 phút nhưng các sơ đồ ghi là ước lượng; chưa đủ cơ sở gọi đây là baseline đã đo. | Chưa xác nhận số liệu bằng đo thực tế. | Giữ nhãn “ước lượng” trong các sơ đồ; chưa ghi các mức giảm thời gian thành kết quả đã đạt. Cần bổ sung cách đo trước/sau trên tác vụ tương đương. |
| Card #1 chọn Agent nhưng chưa chứng minh tài liệu onboarding, sơ đồ kiến trúc hoặc tìm kiếm code chưa đủ. | Chưa chốt lại mức can thiệp. | Đã bổ sung phương án đối chiếu và câu hỏi đề xuất trong mục “Card muốn pitch nhất”. Nhãn Agent trong card vẫn là cảm nhận ban đầu. |
| Card #2 chưa phân biệt rõ thời gian tìm tài liệu với thời gian xử lý yêu cầu mâu thuẫn; việc tổng hợp nhanh chưa bảo đảm hiểu đúng nghiệp vụ. | Chưa xác nhận bằng task thực tế. | Đề xuất ghi riêng thời gian tìm/đọc/đối chiếu và các điểm BA phải làm rõ. Chưa có số liệu hoặc kết quả áp dụng để ghi. |
| Card #3 có phương án OpenAPI, sinh types và contract testing; cần kiểm tra các cách này trước khi đề xuất thêm AI. | Chưa xác nhận phương án nào đủ dùng. | Giữ phương án không dùng AI đã có trong card. Đề xuất đối chiếu lỗi contract thực tế với từng cách xử lý; chưa có phép thử được thực hiện. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi đã trình bày miệng cả ba card: onboarding vào codebase, tổng hợp yêu cầu SRS/Figma/Jira và tích hợp API FE/BE. | Ba candidate được ghi tại dòng 7–9 của báo cáo nhóm. Tôi chưa cung cấp ngày pitch và không nhớ câu hỏi/phản hồi cụ thể. |
| Phản biện bài của bạn khác | Tôi không nhớ câu hỏi cụ thể đã đặt cho card của thành viên khác. | Chưa có nội dung để ghi một thay đổi do câu hỏi của tôi tạo ra. |
| Nhận phản biện | Tôi không nhớ câu hỏi hoặc phản hồi cụ thể nhóm đã đưa ra sau phần trình bày. | Chưa xác định được thay đổi nào bắt nguồn từ phản biện trong buổi pitch. |
| Gom cluster / cây OST | Tôi đề nghị cập nhật các candidate gán cho mình theo đúng ba card CP2 trong báo cáo cá nhân. | Candidate 7–9 đã được thay đúng; cluster được cập nhật trong bản nháp. Chưa xác nhận tôi cùng nhóm chốt cluster hoặc cây OST. |
| Chọn candidate problem | Tôi đã xem thông tin nhóm chọn bài toán chuẩn bị thông tin CV đối chiếu JD. | Chưa có ghi chép về ý kiến hoặc vai trò của tôi trong lần nhóm chọn candidate này. |
| Kiểm chứng / research | Tôi đã làm rõ nhiệm vụ hỏi HR về quy trình xử lý CV của bài toán nhóm. | Chưa cung cấp kết quả phỏng vấn HR hoặc survey; chưa có snapshot thực tế của tôi để bổ sung. |
| Quy trình nhóm | Tôi đã trao đổi để phân biệt thời gian giả định trong bản nhóm với số đo thực tế. | Các mốc 120 → 60 phút/lô CV được hiểu là mô hình và mục tiêu; chưa có kết quả đo do tôi cung cấp. |
| Problem Statement | Tôi đã nhờ AI xác định những phần v0/v1 còn cần dữ liệu hoặc xác nhận của nhóm. | Chưa ghi nhận việc tôi tự rà đầy đủ hoặc cùng nhóm duyệt phiên bản cuối. |
| Mức can thiệp AI | Tôi đã nhờ AI làm rõ phần việc liên quan đến đề xuất Workflow và các phương án No AI/Rule trong bản nhóm. | Chưa có phép thử do tôi thực hiện để xác nhận mức can thiệp phù hợp. |
| Eval / rủi ro / quyết định | Tôi đã nhờ AI rà trạng thái bộ eval và đề xuất Not Yet. | Bộ 10 ca vẫn chưa chạy; ghi chú rà soát được thêm vào bản nhóm. Chưa ghi nhận quyết định cuối được cả nhóm duyệt. |

### Câu hỏi phản biện đề xuất khi rà lại nội dung pitch

| Nội dung cần rà | Câu hỏi cụ thể đề xuất | Điểm cần kiểm chứng |
|---|---|---|
| Card #1 — onboarding developer | Với task đầu tiên gần nhất, phần nào mất nhiều thời gian nhất: cài môi trường, đọc cấu trúc code hay truy vết luồng nghiệp vụ? Mốc 165 phút trong card được đo hay ước lượng? | Xác định đúng bottleneck và nguồn của baseline. |
| Card #1 — mức hỗ trợ và chất lượng | Nếu đã có README, sơ đồ luồng nghiệp vụ và công cụ tìm kiếm code, developer còn vướng ở đâu? Làm thế nào kiểm tra người đó hiểu đúng luồng code trước khi sửa tính năng? | Xác định phần việc còn cần hỗ trợ và cách đánh giá ngoài tốc độ. |
| Card #2 — tổng hợp yêu cầu | Khi Jira, SRS và Figma không thống nhất, ai xác nhận yêu cầu cuối cùng? Thời gian chậm chủ yếu nằm ở tìm tài liệu hay chờ làm rõ yêu cầu? | Phân biệt vấn đề tìm thông tin với vấn đề yêu cầu chưa được chốt. |
| Card #3 — tích hợp API | Với một lỗi request/response không khớp đã xảy ra, OpenAPI, sinh types hoặc contract testing có phát hiện được lỗi đó không? Nếu chưa, phần nào còn cần người kiểm hoặc AI hỗ trợ? | Kiểm tra phương án đơn giản trước và làm rõ khoảng trống của cách hiện tại. |
| Bài toán CV của nhóm — câu tôi có thể hỏi khi thảo luận tiếp | Trong đợt tuyển gần nhất, HR mất nhiều thời gian nhất ở đọc và ghi thông tin CV, làm rõ JD hay kiểm lại dữ liệu? Nếu đã có ATS/parser, bằng chứng nào cho thấy công cụ bổ sung sẽ giảm tổng thời gian gồm cả kiểm và sửa? | Kiểm chứng vị trí bước nghẽn và nhu cầu của giải pháp bổ sung. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI đọc và rà cách diễn đạt Job Story, dấu hiệu và cách đo trong bảng scan đã có. | Phân biệt sự việc đã kể, số liệu ước lượng và kế hoạch đo thêm. | AI từng đánh đồng phần bằng chứng chưa cụ thể với việc tôi chưa hoàn thành CP1. | Tôi xác nhận CP1 đã được viết và yêu cầu làm rõ nhận xét; không bổ sung số liệu không có thật. |
| CP2 Problem Card | Nhờ AI rà ba card, bổ sung lý do chọn card #1 và một câu hỏi đề xuất để thảo luận. | Chỉ ra baseline chưa đo, phạm vi cần giới hạn và phương án đơn giản có thể thử trước. | Các gợi ý chưa thể chứng minh Agent cần thiết hoặc các mức giảm thời gian sẽ đạt được. | Tôi chọn card số 1. Câu hỏi mới được ghi là đề xuất khi rà lại card, không gán thành câu hỏi đã hỏi trong buổi pitch. Các điểm phản biện chưa xác nhận được ghi rõ trong bảng trên. |
| CP3 Ghi nhận tham gia / câu hỏi rà lại | Nhờ AI đối chiếu ba card với candidate 7–9, cập nhật ghi nhận về pitch và đề xuất câu hỏi cho lần trao đổi tiếp. | Sửa danh sách candidate khớp báo cáo cá nhân, ghi lại thông tin tôi xác nhận và chỉ ra các điểm cần kiểm chứng trong từng card. | AI ban đầu suy từ việc thiếu biên bản thành trạng thái chưa pitch; câu hỏi mới đề xuất không chứng minh các câu đó đã được hỏi trong buổi pitch. | Tôi xác nhận đã pitch miệng cả ba card và nói rõ không nhớ câu hỏi/phản hồi. Các câu mới được đặt riêng ở mục câu hỏi đề xuất sau pitch; chưa có câu trả lời hoặc thay đổi thực tế để ghi. |
| CP4 Chuẩn bị kiểm chứng | Hỏi AI để hiểu phần việc phỏng vấn HR thuộc bài toán CV của nhóm. | Làm rõ đối tượng và chủ đề cần kiểm chứng. | Hướng dẫn hoặc tình huống giả lập không tạo ra dữ liệu phỏng vấn người thật. | Chưa ghi tình huống giả lập thành snapshot hay kết quả phỏng vấn của tôi. |
| CP5 Quy trình / Problem Statement | Nhờ AI giải thích và rà trạng thái các mốc thời gian, metric và bản v0/v1 của nhóm. | Làm rõ thời gian đầu-cuối cần gồm cả kiểm/sửa, và số liệu nào còn là giả định. | AI không có số đo của HR để xác nhận baseline hoặc lợi ích. | Giữ rõ trạng thái dự thảo; chưa ghi các mốc thời gian là kết quả thực tế. |
| CP6 Eval / rủi ro / quyết định | Nhờ AI rà nhiệm vụ, bộ 10 ca giả lập và trạng thái đề xuất Not Yet. | Nhắc phân biệt tiêu chí đánh giá với kết quả chạy và đề xuất với quyết định đã duyệt. | Bộ ca chưa chạy và các nhận xét không thay thế kiểm chứng nhu cầu hoặc phê duyệt của nhóm. | Giữ trạng thái chưa chạy; chưa xác nhận thay nhóm rằng đã đạt ngưỡng eval hoặc đã chốt quyết định. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi đã trình bày miệng cả ba card của mình về onboarding developer, tổng hợp yêu cầu từ SRS/Figma/Jira và tích hợp API. Tôi chưa có ghi chép đủ để thuật lại phần trình bày của từng bạn. Khi đối chiếu danh sách candidate, các card của tôi thuộc công việc phát triển phần mềm, còn nhóm chọn bài toán CV. Vì vậy, phần việc tiếp theo của tôi cần bám vào quy trình của HR và dữ liệu của bài toán chung.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Trong card onboarding, tôi ghi cảm nhận ban đầu là Agent trong khi chưa có phép thử cho thấy tài liệu và tìm kiếm code chưa đủ. Đây là điểm cần phản biện về việc chọn giải pháp sớm. Bản nhóm hiện giới hạn AI vào trích xuất bằng chứng CV và giữ quyết định tuyển dụng ở con người. Tôi chưa có ghi chép về một cuộc thảo luận cụ thể đã dẫn tới giới hạn này, nên không gán nó thành kết quả phản biện của mình.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi không nhớ câu hỏi hoặc phản hồi cụ thể sau buổi pitch, nên chưa thể nêu một lần đổi ý do bạn trong nhóm phản biện. Việc điều chỉnh đã được ghi nhận là tôi yêu cầu đối chiếu các candidate mang tên mình với ba card CP2. Sau đó, candidate 7–9 được cập nhật cho khớp. Đây là thay đổi khi rà báo cáo; tôi chưa có căn cứ gọi đó là kết quả của buổi phản biện miệng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Tôi chưa cung cấp kết quả phỏng vấn HR hoặc survey, nên chưa có phản hồi người dùng để kể lại. Báo cáo nhóm có research về các công cụ đọc CV sẵn có. Phần này đặt ra việc cần kiểm tra phương án hiện tại của HR trước khi đề xuất thêm công cụ. Tôi cần tự rà các nguồn và hỏi về lần xử lý CV thực tế; thông tin tính năng của nhà cung cấp chưa chứng minh hiệu quả ở bối cảnh nhóm chọn.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điểm tôi cần làm rõ nhất khi rà Problem Statement là phân biệt baseline thực tế với mốc minh họa và mục tiêu. Bản nhóm dùng mô hình 120 phút/lô 20 CV và mục tiêu không quá 60 phút; đây chưa phải kết quả đo. Khi đánh giá, thời gian phải gồm chuẩn bị, kiểm, sửa và xử lý thủ công khi lỗi. Metric cũng cần đo độ đúng, độ đủ và nguồn dẫn để tránh chỉ tối ưu tốc độ.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ ghi câu hỏi, phản hồi và thay đổi ngay sau khi pitch để không mất thông tin. Với phần CV, tôi sẽ ưu tiên tiếp cận HR ngoài nhóm và ghi quy trình của lần tuyển gần nhất trước khi chọn mức AI. Tôi sẽ tập trung phản biện về lợi ích của checklist hoặc công cụ đang dùng, công kiểm sửa đầu ra và cách đo cùng phạm vi. Các kết luận cần được nhóm xác nhận và ghi lại.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Nhóm chọn vấn đề HR mất thời gian chuẩn bị thông tin CV để đối chiếu với JD cho một vị trí tuyển dụng. Quy trình hiện tại gồm tập hợp CV và JD, chốt checklist, đọc và ghi bằng chứng, kiểm lại rồi chuyển bảng cho người xét duyệt. Bước nghẽn giả định là đọc và ghi bằng chứng, chiếm 70 trong tổng 120 phút cho lô 20 CV, nhưng các mốc này chưa được đo thực tế. Mục tiêu đề xuất là không quá 60 phút/lô, độ đúng và độ đủ ít nhất 95%, cùng tỷ lệ dẫn nguồn đúng 100% trên bộ chuẩn được HR duyệt. Boundary yêu cầu AI không tự chấm điểm, xếp hạng hay loại ứng viên, không thêm thông tin thiếu nguồn và phải để HR kiểm mọi bảng. Workflow là hướng thử có điều kiện với một bước AI trích xuất, đồng thời so sánh với No AI và Rule để chọn mức đơn giản nhất đủ dùng. Bản dự thảo đề xuất Not Yet vì chưa có kiểm chứng HR, baseline đo thật và xác nhận quyền sử dụng dữ liệu; quyết định cuối vẫn cần cả nhóm duyệt.

---

## 7. Tài liệu tham khảo

-
