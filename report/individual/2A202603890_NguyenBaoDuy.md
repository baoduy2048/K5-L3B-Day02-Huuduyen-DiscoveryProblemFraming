# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Bảo Duy
- MSSV: 2A202603890
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Huuduyen
- Link repo nhóm: https://github.com/baoduy2048/K5-L3B-Day02-Huuduyen-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian|Nghe lại toàn bộ file ghi hình bài giảng dài hàng tiếng đồng hồ để tìm lại các trọng tâm kiến thức giảng viên nhấn mạnh. | Sinh viên | Mất trung bình 2,5 đến 3,5 giờ để tua nghe lại file ghi hình dài 90 phút của mỗi buổi học |
| 2 |Tốn thời gian| Khi di chuyển vào mùa mưa bão, tôi muốn cập nhật trước các điểm ngập lụt sâu trên lộ trình, để chủ động chọn đường vòng tránh sự cố chết máy xe| Người đi xe máy, ô tô | Bị kẹt xe hoặc chết máy từ 30 đến 60 phút tại các điểm ngập|
| 3 |Lặp lại | Khi chuẩn bị bữa tối cho gia đình, tôi muốn kiểm kê tủ lạnh và lên thực đơn sẵn, để không phải mất 20 phút mỗi chiều loay hoay suy nghĩ hôm nay ăn gì|Người nấu ăn | Tốn khoảng 15–20 phút suy nghĩ mỗi ngày, lặp lại đều đặn 7 lần/tuần|
| 4 |Tốn thời gian | Khi cần mua sắm một món đồ trực tuyến, tôi muốn tổng hợp nhanh giá cả và đánh giá từ nhiều trang khác nhau, để không phải mở hàng chục tab trình duyệt và mất hàng giờ so sánh| Người mua sắm trực tuyến| Mất khoảng 30–45 phút cho mỗi lần tìm kiếm và so sánh giá trên 5–7 sàn thương mại điện tử|
| 5 |Lặp lại | Tự tay soạn bộ câu hỏi trắc nghiệm và thẻ ghi nhớ (flashcard) từ đầu cho mỗi môn học để luyện tập phương pháp Active Recall.|Sinh viên | Mất chính xác từ 4 đến 6 giờ thủ công để cắt dán tạo ra bộ khoảng 120 - 150 thẻ flashcard cho 1 môn học|
| 6 |Lặp lại |Khi bước vào mùa khô hoặc giai đoạn cây cần dưỡng chất, tôi muốn tính toán chính xác lịch trình và lượng nước tưới dựa trên độ ẩm đất thực tế, để không phải vận hành hệ thống tưới thủ công cảm tính gây lãng phí nước| Chủ trang trại, hộ nông dân | Kiểm tra và bật/tắt thủ công hệ thống tưới 2–3 lần/ngày, kéo dài suốt 3–4 tháng|
| 7 |Pain từ người khác |Khi phụ huynh liên tục nhắn tin hỏi về tình hình học tập và điểm số của con ngoài giờ làm việc, tôi muốn có sẵn các báo cáo tổng hợp trực quan để gửi đi, để không phải lục tìm sổ sách và trả lời dồn dập nhiều lần trong ngày | Giáo viên chủ nhiệm|Nhận từ 15 đến 20 tin nhắn hỏi về tình hình học tập của học sinh mỗi tuần từ phụ huynh |


## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tra cứu mốc thời gian trong Video bài giảng |một điều mà tool lớn (NotebookLM, YouTube) chưa làm tốt: video học nội bộ (LMS/Drive) không có phụ đề và nội dung nằm hoàn toàn trên slide. |- Tài nguyên xử lý: File video 90 phút rất nặng, hệ thống có bị quá tải (timeout) hoặc tốn nhiều chi phí API khi bóc tách ảnh/âm thanh không?
- Độ chính xác OCR: Ảnh slide giảng viên quay mờ/chất lượng thấp thì AI có đọc đúng công thức/chữ không?|
| 2 |Tự động hóa tạo bộ Flashcard ôn thi từ nhiều tài liệu |- Giải quyết Bottleneck khổng lồ (giảm từ 4-5 tiếng cắt dán thủ công xuống còn 10 phút)
- Rủi ro kỹ thuật thấp, dễ làm ra MVP hoạt động mượt mà vì xử lý Text RAG hiện nay đã rất phổ biến và rẻ |- Tính cạnh tranh: Hiện tại NotebookLM, Quizlet, Knowt đã làm chức năng này rất tốt. Sản phẩm tự build có gì thực sự khác biệt để sinh viên chọn dùng |
| 3 | Trợ lý so sánh giá và tóm tắt review TMĐT| Nhu cầu cực kỳ sát thực tế và diễn ra thường xuyên. Giải quyết tốt rủi ro mua hớ và nỗi đau "quá tải thông tin" khi phải đọc hàng ngàn review rác | - Khả năng lấy dữ liệu: Các sàn như Shopee, Lazada có cơ chế chống crawl (Anti-bot) cực mạnh, dễ bị chặn API
- Voucher động: Mã giảm giá thường phụ thuộc vào cấp độ tài khoản của từng user, AI rất khó tính ra "giá cuối cùng" chính xác nếu không có quyền đăng nhập|

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi ôn tập lại kiến thức từ video bài giảng trước kỳ thi, tôi muốn tìm ra chính xác phân đoạn giảng viên hướng dẫn bài tập hoặc giảng lý thuyết, để không phải mất hàng giờ tua đi tua lại tìm kiếm thủ công |
| Actor | Sinh viên đại học |
| Thời điểm / bối cảnh | Vào giai đoạn ôn thi cuối kỳ |
| Quy trình hiện tại (3–7 bước) | 
1. Mở file video bài giảng dung lượng lớn (90–120 phút) trên nền tảng lưu trữ

2. Di chuyển thanh trượt thời gian (seek bar) dọc theo tiến trình video để tìm kiếm phân đoạn nội dung cần thiết

3. Phát video kiểm tra từng phân đoạn, lặp lại thao tác tua đi tua lại khi chưa đúng nội dung

4. Ghi chép thủ công các mốc thời gian (timestamp) tương ứng ra tài liệu ghi chú cá nhân để tra cứu cho các lần tiếp theo

5. Lặp lại chu trình thao tác này đối với hệ thống video bài giảng của các môn học khác|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & 3 tua video thủ công ngốn từ 30 đến 45 phút để tra cứu thông tin|
| Impact (nếu không giải thì sao) | Mất 30 đến 45 phút cho việc tìm kiếm thông tin của một 1 môn học. Một kỳ thi nhiều môn học sẽ tốn nhiều giờ đồng hồ cho việc tìm kiếm |
| Success metric (baseline → target) | Rút ngắn thời gian tìm đúng đoạn video cần học từ 30 phút tua thủ công xuống dưới 30 giây|
| Phương án không dùng AI | sử dụng tính năng tìm kiếm phụ đề trên youtube, nhưng phần lớn nội dung bài học được lưu trữ trên hệ thống lms, hoặc google drive nên không thể tra cứu |
| Giả thuyết về AI (nếu có) |AI tự động chuyển đổi âm thanh thành văn bản kết hợp trích xuất khung hình slide, cho phép sinh viên chat truy vấn trực tiếp để hệ thống trả về đường link video gắn sẵn mốc thời gian chính xác đến từng giây |
| Cảm nhận nhanh | Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút
[1 Mở video trên nền tảng lưu trữ: 2'] → [2 Di chuyển thanh trượt tìm kiếm: 15'] → [3 Phát video kiểm tra (thử - sai): 20'] ← BOTTLENECK
→ [4 Ghi chép thủ công timestamp: 5'] → [5 Lưu trữ và chuyển video/môn khác: 3']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần ghi nhớ hàng trăm khái niệm và định nghĩa rải rác trong tài liệu trước kỳ thi, sinh viên muốn gom nhóm và hệ thống hóa nội dung thành các thẻ câu hỏi - đáp án ngắn gọn, để ôn tập dễ dàng hơn|
| Actor |Sinh viên đại học |
| Thời điểm / bối cảnh | Vào 2 tuần cao điểm trước kỳ thi cuối kỳ|
| Quy trình hiện tại (3–7 bước) |1. Mở 4–6 file tài liệu (slide, PDF, ghi chú)
2. Đọc lướt từng chương tìm định nghĩa, công thức quan trọng
3. Copy đoạn văn bản chứa khái niệm cốt lõi
4. Viết thủ công câu hỏi vào mặt trước thẻ Flashcard
5. Viết đáp án/giải thích vào mặt sau
6. Lặp lại thao tác cắt dán cho 120–150 thẻ/môn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, 4, 5 — Chọn lọc khái niệm và viết thủ công từng thẻ flashcard, mất khoảng 4 đến 5 giờ cho mỗi môn học|
| Impact (nếu không giải thì sao) | Mất nhiều thời gian làm thủ công gây mệt mỏi, dễ nản chí và bỏ cuộc trước khi kịp ôn tập; thiếu thời gian cho các môn học khác|
| Success metric (baseline → target) |Giảm tổng thời gian tạo bộ 150 flashcard từ 5 giờ xuống dưới 10 phút |
| Phương án không dùng AI | Dùng file mẫu Excel kết hợp tính năng import của Anki, nhưng sinh viên vẫn phải tự đọc tài liệu và gõ thủ công toàn bộ nội dung từng thẻ|
| Giả thuyết về AI (nếu có) |AI tự động phân tích tài liệu, trích xuất ý cốt lõi và sinh ra các cặp câu hỏi - đáp án (Front/Back) chuẩn định dạng JSON |
| Cảm nhận nhanh |Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 300 phút

[1 Mở 4–6 file tài liệu: 10'] → [2 Đọc lướt tìm định nghĩa, công thức: 40']
→ [3 Copy đoạn văn bản cốt lõi: 50'] ← BOTTLENECK
→ [4 Viết thủ công câu hỏi mặt trước: 90'] ← BOTTLENECK
→ [5 Viết giải thích/đáp án mặt sau: 100'] ← BOTTLENECK
→ [6 Kiểm tra và hoàn thiện bộ thẻ: 10']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story |Khi cần mua sắm một món đồ trực tuyến, tôi muốn tổng hợp nhanh giá cả và đánh giá từ nhiều trang khác nhau, để không phải mở hàng chục tab trình duyệt và mất hàng giờ so sánh.|
| Actor |Người mua sắm trực tuyến |
| Thời điểm / bối cảnh |Khi phát sinh nhu cầu mua các sản phẩm có giá trị hoặc trong các dịp sale lớn cần ra quyết định mua nhanh |
| Quy trình hiện tại (3–7 bước) |1. Xác định tên sản phẩm hoặc mã model cụ thể cần mua.
2. Mở ứng dụng hoặc trang web của 3–5 sàn thương mại điện tử khác nhau (Shopee, Lazada, Tiki, TikTok Shop...).
3. Tìm kiếm từ khóa trên từng sàn, lọc kết quả theo mức giá và số lượt bán.
4. Mở 5–10 tab chi tiết sản phẩm, đọc thủ công hàng chục bình luận để lọc đánh giá ảo (seeding) và xem ảnh chụp thực tế.
5. Thêm sản phẩm vào giỏ hàng ở từng sàn, thử áp dụng các mã giảm giá và phí vận chuyển để tính ra số tiền thanh toán cuối cùng.
6. So sánh chéo kết quả giữa các sàn để chốt đơn hàng có giá tốt và độ uy tín cao nhất. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 & 5 — Việc đọc đối chiếu bình luận thủ công và thử áp mã giảm giá ở từng nền tảng tiêu tốn từ 30 đến 45 phút|
| Impact (nếu không giải thì sao) |Tiêu tốn nhiều thời gian vô ích, dễ bị quá tải thông tin, dễ gây quyết định sai lầm |
| Success metric (baseline → target) | Giảm tổng thời gian khảo sát giá, đọc tóm tắt review và tìm ra link mua rẻ nhất từ 45 phút xuống dưới 2 phút|
| Phương án không dùng AI |Sử dụng các trang web/công cụ so sánh giá truyền thống. Tuy nhiên, các nền tảng này thường chỉ crawl được giá niêm yết tĩnh, không tính toán được mức giá cuối cùng sau khi áp voucher/phí ship, và hoàn toàn không có khả năng đọc hiểu, tổng hợp hàng nghìn review |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh |Workflow|

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút

[1 Xác định tên/mã sản phẩm: 2'] → [2 Mở 3–5 trang/app TMĐT: 3'] → [3 Tìm kiếm & lọc kết quả: 5']
→ [4 Đọc thủ công bình luận & xem ảnh: 20'] ← BOTTLENECK
→ [5 Thử áp mã giảm giá & tính phí ship cuối: 10'] ← BOTTLENECK
→ [6 So sánh chéo & chốt đơn hàng: 5']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: vì đây là vấn đề tôi đã từng gặp phải, và mong muốn đưa ra một giải pháp để giúp sinh viên ôn tập tốt hơn
- Câu hỏi muốn nhóm phản biện: thời gian thực tế có thể rút ngắn là bao nhiêu 



## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi đã trình bày 3 problem chính của mình| giúp nhóm hiểu rõ các problem mà mình đưa ra|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:liệu AI có cần thiết cho vấn đề này không | giúp nhóm quyết định xem lại sự cần thiết của AI cho tửng problem|
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST |Nhóm các problem cùng bản chất, như giáo dục, đời sống |dễ dàng đánh giá các problems |
| Chọn candidate problem |Tham gia đánh giá problems dựa trên các tiêu chí cốt lõi như cost, lattency, mức độ can thiệp, điểm khác biệt,... |Lựa chọn ra được 1 problem tốt nhất là nhận diện tài xê buồn ngủ khi đi xe đường dài |
| Kiểm chứng / research |research 1 số công nghệ sẵn có để ứng dụng cho problem |tìm ra được một số hướng đi, tìm ra một số căn cứ chứng minh tính khả thi của dự án |
| Quy trình nhóm |phân tích quy trình sau khi có giải pháp |cải thiện, khắc phục bottleneck |
| Problem Statement |Tham gia xác định actor, nhu cầu và vấn đề cốt lõi | Hoàn thiện Problem Statementv1|
| Mức can thiệp AI | đánh giá mức độ sử dụng AI| lựa chọn workflow để can thiệp|
| Quyết định | Tham gia thảo luận quyết định tiếp tục, điều chỉnh hoặc loại bỏ problem|Thống nhất hướng triển khai của nhóm |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | gợi ý thêm đề tài tương tự|đưa ra rất nhiều đề tài tương tự |tuy nhiên các đề tài tương đối trừu tượng hoặc không thực tế | đi sâu vào một số problem, thu hẹp user|
| CP2 Problem Card |đánh giá problem card |đánh giá theo format mẫu, chỉ ra những bước thiếu ở quy trình | bổ sung một số quy trình vô nghĩa| bổ sung một số bước thực sự quan trọng cho quy trình|
| CP4 Research | tìm kiếm các bài báo liên quan|tìm kiếm rất nhanh và đầy đủ các bài báo liên quan | đưa ra một số link không có thật| tiến hành kiểm chứng các đường link url và nội dung bài báo, github để tiến hành đưa vào report|
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Các thành viên đều có các ý tưởng trong các vấn đề khác nhau, một số problem khá thiết thực hướng đến lượng user lớn như trường học. Bên cạnh đó cũng có các đề tài hướng đến nhóm đối tượng nhỏ hơn như người nông dân, tài xế đường dài.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Nhóm xử lý tương đối tốt , phân tích chi tiết từng problem
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- tôi đã thay đổi ý tưởng về problem của mình, từ một ứng dụng hướng đến nhóm đối tượng nhỏ và ứng dụng chỉ trong 1 vấn đề duy nhất mở rộng ra nhóm đối tượng rộng hơn và bổ sung thêm các tính năng để hoàn thiện
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- kết quả kiểm chứng khá giống với những thông tin đã được đưa ra ở problem card
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- khó khăn khi xác định quy trình đầy đủ, chi tiết nhưng không bị dài dòng và phải chỉ ra chính xác bottleneck
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Nếu làm lại tôi sẽ xem xét lại problem của bản thân, xác định rõ nhóm người dùng phù hợp và các tính năng mong muốn
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
- problem của nhóm là phát hiện tài xế đường dài có hiện tượng ngủ gật khi đang tham gia giao thông, quy trình hiện tại tương đối phụ thuộc vào người tài xế. Nhóm sử dụng các metric chính để đánh giá bao gồm phát hiện đúng, tỷ lệ cảnh báo sai, thời gian phát hiện tài xế buồn ngủ. Ai chỉ có khả năng cảnh báo tài xế còn các quyết định trên đường đều do tài xế đưa ra cuối cùng. Mức can thiệp đó là CV + Temporal Analysis và các cơ chế cảnh báo theo quy tắc vì cần nhận diện và xác định khi nào đủ điều kiện cảnh báo qua thời gian thực. Nhóm quyết định theo đuổi hướng xây dựng hệ thống theo thời gian thực đồng thời kiểm thử, đánh giá độ tin cậy và hạn chế cảnh báo sai.
---

## 7. Tài liệu tham khảo

-
