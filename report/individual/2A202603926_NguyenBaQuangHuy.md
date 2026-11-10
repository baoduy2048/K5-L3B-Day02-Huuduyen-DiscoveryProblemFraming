# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Bá Quang Huy
- MSSV: 2A202603926
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Huuduyen
- Link repo nhóm: https://github.com/baoduy2048/K5-L3B-Day02-Huuduyen-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | **Tốn thời gian** | Giáo viên khi chấm bài cho học sinh của mình sẽ cần phải xem đi xem lại từng bài làm của học sinh, kiểm tra bài làm của học sinh đã làm theo đúng nguyên tắc, quy tắc làm bài hay chưa. | Giáo viên | Trung bình việc chấm bài của học sinh đã tiêu tốn ít nhất khoảng 5 phút cho 1 bài tự luận của 1 học sinh, nhân 30 học sinh sẽ tốn khoảng 2 giờ, với bài trắc nghiệm sẽ nhanh hơn vì có hệ thống chấm điểm dựa trên kết quả có sẵn với làm online và chấm trắc nghiệm khoanh giấy cũng chỉ mất trung bình khoảng 2 phút cho 1 bạn.|
| 2 | **Pain từ người khác** | Khi học sinh đi học trên lớp nhưng học lực chênh lệch dẫn đến có những bạn không theo kịp được tiến độ của cả lớp  | Học sinh, Giáo viên | Học sinh bị bỏ lỡ kiến thức, về nhà không có điều kiện hỏi đáp với giáo viên những phần còn thắc mắc. |
| 3 | **Cần đọc, tổng hợp nhiều thông tin** | Giáo viên cần làm nhiều thủ tục hành chính ngoài việc giảng dạy và khi cần phải qua nhiều thao tác, nhiều bước mới lấy được dữ liệu mong muốn. Và giáo viên cũng phải cover nhiều việc phụ trợ cho công việc giảng dạy | Giáo viên | Giáo viên bị mất quá nhiều thời gian cho các thủ tục hành chính ngoài giảng dạy |
| 4 | **Tốn thời gian** | Khi giáo viên cần check bài về nhà cho học sinh trong lớp, phải lần lượt kiểm tra bài làm của học sinh và đưa ra nhận xét | Giáo viên, học sinh | Giáo viên bị mất nhiều thời gian cho việc chấm bài, chưa kể còn phải chuẩn bị kế hoạch giảng dạy cho ngày tiếp theo |
| 5 | **Tốn thời gian** | Khi muốn tổng hợp dữ liệu báo cơm bán trú của học sinh hàng ngày, giáo viên tổng hợp cần phải lấy dữ liệu excel từ nhiều nguồn từ giáo viên chủ nhiệm, và khi cần thống kê, ra soát học sinh trên excel cũng gặp nhiều khó khăn về trình độ kỹ thuật hoặc giới hạn quyền hạn truy xuất thông tin trong trường. | Giáo viên | Giáo viên tổng hợp bán trú sẽ cần phải qua nhiều công đoạn mới lấy được lượng dữ liệu mong muốn. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Gộp ý tưởng 4 vào 1 vì về cơ bản 2 ý tưởng này đều là hệ thống AI hỗ trợ chấm bài.
- Ý tưởng 5 chỉ cần tool, không có nêu dùng đến AI

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Giáo viên mất nhiều thời gian chấm bài cho học sinh | Đây là công việc hàng ngày của các giáo viên và cũng tốn rất nhiều thời gian, nên nếu giảm được áp lực chấm bài sẽ giảm tải bớt áp lực cho giáo viên.| Công nghệ AI đã đọc được tốt và chính xác chữ ghi trên giấy chưa, để đảm bảo tính đúng đắn của kết quả và trong quá trình đọc có bịa dữ liệu hay không |
| 2 | Giáo viên mất nhiều thời gian xử lý, tổng hợp dữ liệu từ nhiều nguồn để làm báo cáo | Giảm tải thời gian cho giáo viên sẽ giúp giáo viên có thêm thời gian để học tập và chăm lo cuộc sống cá nhân |  |
| 3 | Học sinh không đồng đều về lực học dẫn đến có những bạn không theo kịp cả lớp trong giờ học nhưng về nhà cũng không có điều kiện để thầy cô review hay hướng dẫn làm bài | Xây dựng hệ thống AI tự động hỗ trợ học sinh hỏi đáp và làm bài sẽ giúp học sinh có thêm nguồn tài liệu tự học | |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Giáo viên khi chấm bài cho học sinh của mình sẽ cần phải xem đi xem lại từng bài làm của học sinh, kiểm tra bài làm của học sinh đã làm theo đúng nguyên tắc, quy tắc làm bài hay chưa. |
| Actor | Giáo viên trực tiếp giảng dạy và chấm bài |
| Thời điểm / bối cảnh | Sau mỗi bài kiểm tra, bài tập về nhà hoặc bài luyện tập trên lớp. Đặc biệt khi giáo viên cần chấm bài tự luận cho một lớp có khoảng 30 học sinh. |
| Quy trình hiện tại (3–7 bước) | 1. Thu thập bài làm của học sinh (bản giấy hoặc bản online). 2. Đọc đề bài và xác định đáp án, tiêu chí chấm điểm. 3. Đọc và kiểm tra từng bài làm của học sinh. 4. Đối chiếu từng bước giải với đáp án, nguyên tắc và quy tắc làm bài. 5. Xác định lỗi sai, đánh giá mức độ hoàn thành và cho điểm. 6. Ghi nhận kết quả, nhận xét và tổng hợp điểm. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: Giáo viên phải đọc, kiểm tra và đối chiếu từng bài tự luận, trung bình ít nhất 5 phút/bài. Với lớp 30 học sinh, tổng thời gian tối thiểu khoảng 150 phút (2,5 giờ). Bài trắc nghiệm nhanh hơn, khoảng 2 phút/học sinh nếu chấm trên giấy; bài online có thể được hệ thống chấm tự động. |
| Impact (nếu không giải thì sao) | Giáo viên mất nhiều thời gian cho công việc chấm bài lặp đi lặp lại, giảm thời gian dành cho soạn giảng, chuẩn bị bài học và hỗ trợ học sinh. Khi số lượng bài kiểm tra tăng, áp lực công việc cũng tăng theo. |
| Success metric (baseline → target) | Thời gian chấm bài tự luận: từ ≥ 5 phút/bài xuống ≤ 2 phút/bài. Với lớp 30 học sinh: từ ≥ 150 phút xuống ≤ 60 phút. Đảm bảo độ chính xác chấm điểm và tính nhất quán với tiêu chí của giáo viên. |
| Phương án không dùng AI | Xây dựng đáp án và rubric chấm điểm chuẩn hóa. Sử dụng biểu mẫu chấm điểm có sẵn. Phân loại bài theo dạng câu hỏi để chấm theo từng câu thay vì từng bài. Sử dụng phần mềm quản lý bài kiểm tra và chấm trắc nghiệm tự động. |
| Giả thuyết về AI (nếu có) | Sử dụng AI để đọc nội dung bài làm (ảnh chụp hoặc văn bản), đối chiếu với đáp án và rubric do giáo viên cung cấp, nhận diện các bước giải đúng/sai, đề xuất điểm số và nhận xét. Giáo viên chỉ cần kiểm tra, điều chỉnh và xác nhận kết quả cuối cùng. |
| Cảm nhận nhanh | Workflow + Agent |

Quy trình nháp hiện tại:

```text
1. Giáo viên tạo bài kiểm tra: Nhập đề bài, đáp án chuẩn, thang điểm và rubric (tiêu chí chấm điểm) lên hệ thống.
2. Học sinh làm bài: Học sinh làm bài tự luận trên giấy theo format quy định.
3. Thu thập bài làm: Giáo viên chụp ảnh hoặc tải ảnh bài làm của học sinh lên hệ thống.
4. AI quét và đọc bài làm (OCR): AI nhận diện chữ viết tay, trích xuất nội dung bài làm từ hình ảnh và chuyển thành văn bản có cấu trúc.
5. AI phân tích bài làm: Đối chiếu nội dung học sinh với đáp án chuẩn, kiểm tra từng bước giải, công thức, nguyên tắc và quy tắc trình bày theo rubric.
6. AI đề xuất kết quả chấm: Tự động đề xuất điểm số cho từng câu, chỉ ra phần đúng, phần sai, lỗi sai và giải thích lý do trừ điểm.
7. Giáo viên kiểm duyệt: Giáo viên xem lại nội dung AI nhận diện, điểm số và nhận xét; điều chỉnh nếu cần thiết.
8. Xuất kết quả: Hệ thống tổng hợp điểm, nhận xét và lưu kết quả chấm bài của từng học sinh.
9. Trả kết quả: Giáo viên gửi điểm số và nhận xét cho học sinh.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi học sinh đi học trên lớp nhưng học lực chênh lệch dẫn đến có những bạn không theo kịp được tiến độ của cả lớp. |
| Actor | Học sinh, Giáo viên |
| Thời điểm / bối cảnh | Trong quá trình học tập trên lớp, đặc biệt khi giáo viên giảng bài mới, chuyển sang kiến thức nâng cao hoặc triển khai bài tập với tốc độ chung cho cả lớp. |
| Quy trình hiện tại (3–7 bước) | 1.Giáo viên chuẩn bị nội dung và kế hoạch bài giảng theo tiến độ chung. 2.Giáo viên giảng bài và hướng dẫn kiến thức cho cả lớp. 3.Học sinh tiếp thu kiến thức với tốc độ và khả năng khác nhau. 4.Một số học sinh không hiểu bài hoặc không theo kịp nội dung đang giảng. 5.Giáo viên tiếp tục bài giảng để đảm bảo tiến độ chương trình. 6.Học sinh chưa hiểu bài ghi nhớ thắc mắc hoặc bỏ qua phần kiến thức chưa nắm được. 7.Khi về nhà, học sinh tự ôn tập nhưng thiếu người hướng dẫn và giải đáp những phần chưa hiểu. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: Giáo viên khó theo dõi mức độ hiểu bài của từng học sinh trong một lớp đông và không thể dừng lại quá lâu để hỗ trợ riêng từng em. Bước 6–7: Học sinh không có điều kiện hỏi đáp trực tiếp với giáo viên sau giờ học, dẫn đến những lỗ hổng kiến thức chưa được giải quyết. Chưa có số liệu cụ thể về thời gian và tỷ lệ học sinh gặp vấn đề. |
| Impact (nếu không giải thì sao) | -Học sinh mất kiến thức nền tảng, khó tiếp thu các nội dung tiếp theo. -Chênh lệch học lực giữa các học sinh ngày càng lớn. -Học sinh dễ mất tự tin, giảm hứng thú và động lực học tập. -Giáo viên khó đảm bảo tất cả học sinh đạt được mục tiêu bài học. |
| Success metric (baseline → target) | -Tỷ lệ học sinh hiểu bài sau mỗi buổi học: đo baseline → mục tiêu tăng ít nhất 20%. -Tỷ lệ câu hỏi của học sinh được giải đáp: đo baseline → mục tiêu đạt trên 90%. -Thời gian học sinh phải chờ để được giải đáp thắc mắc: đo baseline → giảm đáng kể. |
| Phương án không dùng AI | -Tổ chức các nhóm học tập theo trình độ. -Giáo viên bố trí thời gian phụ đạo cho học sinh chưa theo kịp. -Cung cấp tài liệu ôn tập và bài tập phân cấp độ khó. -Tổ chức giờ hỏi đáp hoặc tư vấn ngoài giờ học. -Khuyến khích học sinh hỗ trợ và giải thích kiến thức cho nhau. |
| Giả thuyết về AI (nếu có) | Xây dựng trợ lý học tập AI cá nhân hóa theo từng học sinh. AI có thể dựa trên nội dung bài giảng, tài liệu giáo viên cung cấp và kết quả học tập để giải thích lại kiến thức theo cách dễ hiểu hơn, trả lời thắc mắc, đưa ra ví dụ và bài tập phù hợp với trình độ của từng học sinh. |
| Cảm nhận nhanh | Agent + Workflow |

Quy trình nháp hiện tại:

```text
1. Giáo viên chuẩn bị bài giảng
2. Học sinh học trên lớp
3. Phát hiện kiến thức chưa nắm vững
4. AI hỗ trợ học tập cá nhân
- Giải thích lại kiến thức chưa hiểu
- Trả lời câu hỏi theo tài liệu giáo viên
- Đưa ra ví dụ và bài tập theo trình độ
- Kiểm tra mức độ hiểu bài sau giải thích
5. Học sinh luyện tập và củng cố kiến thức
6. Giáo viên theo dõi tiến độ
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Giáo viên cần thực hiện nhiều thủ tục hành chính ngoài công việc giảng dạy. Khi cần tìm kiếm hoặc tổng hợp dữ liệu phục vụ công việc, giáo viên phải trải qua nhiều thao tác và nhiều bước mới lấy được thông tin mong muốn, đồng thời phải đảm nhiệm nhiều công việc phụ trợ khác. |
| Actor | Giáo viên |
| Thời điểm / bối cảnh | Trong quá trình công tác tại trường, ngoài giờ lên lớp hoặc khi phát sinh các yêu cầu hành chính, báo cáo, thống kê, tra cứu thông tin học sinh và phối hợp với các phòng ban. |
| Quy trình hiện tại (3–7 bước) | 1.Giáo viên tiếp nhận yêu cầu công việc hoặc thủ tục hành chính từ nhà trường và các phòng ban. 2.Xác định thông tin, biểu mẫu hoặc dữ liệu cần cung cấp. 3.Truy cập các hệ thống quản lý, file Excel, tài liệu hoặc nhóm trao đổi để tìm kiếm thông tin. 4.Thực hiện nhiều thao tác để lọc, đối chiếu và tổng hợp dữ liệu từ các nguồn khác nhau. 5.Nhập thông tin vào biểu mẫu hoặc lập báo cáo theo yêu cầu. 6.Gửi kết quả cho bộ phận liên quan và chỉnh sửa nếu có yêu cầu bổ sung. 7.Tiếp tục xử lý các công việc phụ trợ khác ngoài hoạt động giảng dạy. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: Giáo viên mất nhiều thời gian truy cập các hệ thống, tìm kiếm, đối chiếu và tổng hợp dữ liệu từ nhiều nguồn khác nhau. Một số thông tin phải nhập lại thủ công hoặc thực hiện nhiều thao tác mới truy xuất được. Chưa có số liệu cụ thể về thời gian trung bình cho từng thủ tục. |
| Impact (nếu không giải thì sao) | - Giảm thời gian dành cho soạn giảng, nghiên cứu và cải thiện chất lượng bài học. Tăng khối lượng công việc ngoài chuyên môn và áp lực hành chính. Dễ xảy ra sai sót khi nhập liệu, tổng hợp hoặc đối chiếu thông tin thủ công. Giảm hiệu suất làm việc và mức độ hài lòng của giáo viên. Khó cân bằng giữa công việc giảng dạy và các nhiệm vụ hành chính. |
| Success metric (baseline → target) | - Thời gian hoàn thành một thủ tục hành chính: đo baseline → mục tiêu giảm ít nhất 50%. Thời gian tìm kiếm và tổng hợp dữ liệu: đo baseline → mục tiêu giảm ít nhất 50%. Số thao tác để hoàn thành một yêu cầu: đo baseline → giảm ít nhất 30%. Tỷ lệ báo cáo phải chỉnh sửa do sai sót: đo baseline → giảm đáng kể. |
| Phương án không dùng AI | - Chuẩn hóa quy trình và biểu mẫu hành chính. Xây dựng hệ thống quản lý dữ liệu tập trung. Tạo các biểu mẫu nhập liệu và báo cáo tự động bằng Excel hoặc Google Sheets. Tích hợp các hệ thống quản lý để hạn chế nhập liệu nhiều lần. Phân công rõ trách nhiệm giữa giáo viên và các bộ phận hành chính. |
| Giả thuyết về AI (nếu có) | Xây dựng trợ lý AI dành cho giáo viên, có khả năng truy vấn dữ liệu từ các hệ thống được phân quyền, tìm kiếm thông tin bằng ngôn ngữ tự nhiên, tổng hợp dữ liệu và hỗ trợ tạo báo cáo, biểu mẫu hành chính. Ví dụ: giáo viên có thể yêu cầu "Thống kê danh sách học sinh nghỉ học trong tháng này" hoặc "Tổng hợp kết quả học tập của lớp 10A1" thay vì phải truy cập nhiều màn hình và lọc dữ liệu thủ công. |
| Cảm nhận nhanh | Workflow + Agent + RAG |

Quy trình nháp hiện tại:

```text
1. Giáo viên gửi yêu cầu bằng ngôn ngữ tự nhiên
Ví dụ: Tổng hợp danh sách học sinh nghỉ học tháng 10
2. AI phân tích yêu cầu
Xác định ý định, dữ liệu và nghiệp vụ cần xử lý3. Truy vấn dữ liệu từ hệ thống
RAG · Database Query · API Integration
4. AI tổng hợp và xử lý thông tin
Lọc dữ liệu · Thống kê · Tạo báo cáo
5. Giáo viên kiểm tra và xác nhận
Kiểm tra tính chính xác trước khi sử dụng
6. Xuất báo cáo hoặc thực hiện tác vụ
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Giải quyết được nỗi đau của giáo viên là mất quá nhiều thời gian cho việc chấm bài, khi có hệ thống chấm bài tự động giáo viên sẽ có thể bỏ qua các thao tác lặp đi lặp lại và dành thời gian review các phần bài tập đáng chú ý hơn.
- Câu hỏi muốn nhóm phản biện: 
1. Vấn đề xảy ra thường xuyên hay chỉ tăng cao vào các đợt kiểm tra giữa kỳ, cuối kỳ?
2. Đây có phải vấn đề lớn nhất của giáo viên khi chấm bài, hay còn vấn đề nghiêm trọng hơn như xây dựng rubric, nhập điểm và viết nhận xét?
3. Giáo viên thực sự mất ít nhất 5 phút cho mỗi bài tự luận, hay con số này chỉ đúng với một số môn học hoặc dạng bài nhất định?
### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có đủ bằng chứng xác thực cho con số trung bình 5 phút/bài. | Đồng ý | Xác định 5 phút/bài là số liệu ban đầu, cần phỏng vấn và đo thời gian thực tế từ nhiều giáo viên. |
| Giải pháp AI có thể đọc sai chữ viết tay, đặc biệt với ảnh mờ hoặc cách trình bày phức tạp. | Đồng ý | Bổ sung bước kiểm tra và chỉnh sửa kết quả OCR trước khi AI tiến hành chấm. |
| AI có thể đánh giá sai nếu học sinh có cách giải khác đáp án mẫu nhưng vẫn đúng. | Đồng ý | Sử dụng rubric và tiêu chí đánh giá theo từng bước; cho phép giáo viên điều chỉnh điểm AI đề xuất. |
| Chưa có cơ chế kiểm soát trách nhiệm khi AI chấm sai. | Đồng ý | Quy định AI chỉ đề xuất điểm và nhận xét; giáo viên là người quyết định điểm cuối cùng. |
| Chưa đánh giá các giải pháp không cần AI như chuẩn hóa rubric, biểu mẫu và quy trình chấm. | Đồng ý | Bổ sung phương án No AI để so sánh, chỉ sử dụng AI ở những công đoạn cần đọc hiểu và đánh giá nội dung bài làm. |
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
| CP1 Scan | Phân tích vấn đề ban đầu và xác định các khó khăn trong công việc chấm bài của giáo viên. | Giúp hệ thống hóa vấn đề, xác định Actor, nhu cầu và các dấu hiệu ban đầu. | Dễ suy diễn vấn đề và mức độ ảnh hưởng khi chưa có dữ liệu phỏng vấn thực tế. | Xác định giáo viên là Actor chính; giữ số liệu 5 phút/bài ở mức thông tin ban đầu, cần xác minh. |
| CP2 Problem Card | Xây dựng Problem Card theo cấu trúc Job Story, Context, Bottleneck, Impact và Success Metric. | Giúp chuẩn hóa cách mô tả vấn đề, xác định quy trình hiện tại và đề xuất ý tưởng mới. | Một số chỉ số như giảm thời gian từ 5 xuống 2 phút/bài chưa có cơ sở thực nghiệm. | Phân biệt số liệu hiện trạng với mục tiêu giả thuyết; bổ sung yêu cầu khảo sát giáo viên để xác minh. |
| CP4 Research | Hỗ trợ xác định hướng nghiên cứu, các câu hỏi phỏng vấn và thông tin cần thu thập. | Gợi ý các khía cạnh cần khảo sát như thời gian chấm, số lượng bài, phương pháp chấm và công cụ đang sử dụng. | Chưa có dữ liệu nghiên cứu thực tế đủ mạnh để kết luận vấn đề phổ biến hoặc mức độ nghiêm trọng. | Cần thu thập phỏng vấn thực tế, đo thời gian chấm và tìm hiểu sự khác biệt giữa môn học, dạng bài. |
| CP5 Quy trình | Phân tích quy trình hiện tại và đề xuất quy trình tương lai có tích hợp AI. | Giúp phân rã các bước OCR, phân tích bài làm, đối chiếu rubric, đề xuất điểm và nhận xét. | Chưa làm rõ đầy đủ các tình huống ngoại lệ như ảnh mờ, chữ viết khó đọc, cách giải khác đáp án mẫu. | Bổ sung bước kiểm tra OCR, cơ chế xử lý lỗi và bước giáo viên kiểm duyệt trước khi xác nhận điểm. |
| CP5–6 Problem Statement | Hỗ trợ tổng hợp Actor, quy trình, bottleneck, impact và success metric thành một phát biểu vấn đề rõ ràng. | Giúp kết nối vấn đề thực tế với nhu cầu cần giải quyết và kết quả mong đợi. | Có nguy cơ định hướng vấn đề theo giải pháp AI quá sớm, thay vì xuất phát từ nhu cầu thực tế của giáo viên. | Tập trung vào việc giảm thời gian và nâng cao tính nhất quán khi chấm bài; xem AI là một giả thuyết giải pháp cần kiểm chứng. |
| CP6 Mức can thiệp / quyết định | Đánh giá AI nên tự động hóa đến đâu và con người cần tham gia ở công đoạn nào. | Giúp xác định AI phù hợp với các tác vụ đọc, phân tích, đối chiếu và đề xuất kết quả. | AI có thể chấm sai, bỏ sót cách giải hợp lý hoặc đưa ra nhận xét thiếu chính xác; không nên giao toàn quyền quyết định điểm. | Chọn mô hình Human-in-the-loop: AI đề xuất điểm và giải thích, giáo viên kiểm tra, điều chỉnh và quyết định điểm cuối cùng. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Mỗi bạn sẽ có một ý tưởng và một hướng tư duy riêng cho sản phẩm, và khi lắng nghe, phản biện với các chủ đề của các thành viên, tôi đã hiểu hơn về thế nào là phân kỳ, thế nào là hội tụ, và sau một thời gian đánh giá, các ưu, nhược điểm sẽ bộc lộ và team có thể đánh giá tính khả thi của một dự án có tốt hay không.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Nhóm tôi đã có một chủ đề về ý tưởng rất hay là ứng dụng hệ thống AI dùng camera để hỗ trợ người nông dân chẩn đoán tình trạng cây trồng và đưa ra các cảnh báo và phương án cụ thể với những cây trồng đang bị bệnh. Tuy nhiên khi đi vào bàn bạc lại nảy sinh rất nhiều vấn đề về chi phí, về tính khả thi khi triển khai và cuối cùng cả team thống nhất là No-Go

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Khi bị phản biện, tôi đánh giá lại phản biện đó có đúng, có hợp lý không, sau đó nếu phản biện chưa hợp lý tôi lập tức trả lời và đặt lại câu hỏi để team xây dựng thêm nhiều thông tin mới. Ví dụ khi bàn bạc về dự án ứng dụng camera tích hợp hệ thống AI để tự động chẩn đoán và đưa ra quy trình xử lý bệnh cho cây trồng, tôi đặt quan điểm là thiết lập hệ thống camera để theo dõi cây trồng sẽ rất khó vì camera chỉ quét được 1 vùng, trường hợp cây trồng bị che chắn hay địa hình, thời tiết không thuận lợi đều gây ảnh hưởng đến kết quả báo cáo. Thành viên trong đội đã phản biện rằng đặt hệ thống camera lên hệ thống khung cao hơn cây trồng để theo dõi. Nhưng tôi lập tức phản biện rằng với trường hợp đó sẽ lại phát sinh vấn đề chi phí và độ phức tạp để xây dựng hệ thống sẽ tăng cao. Sau một hồi bàn bạc chúng tôi đã thống nhất các nhược điểm của hệ thống.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Kết quả kiểm chứng làm tôi một chút bất ngờ vì khi chúng tôi khảo sát các phỏng vấn liên quan đến hệ thống nhận diện và cảnh báo buồn ngủ cho tài xế, một số tài xế xem nhẹ việc ứng dụng AI cảnh báo và đề cao kinh nghiệm của bản thân, tuy nhiên khi team đánh giá, việc tài xế tự tin về kinh nghiệm hoặc cách xử lý của bản thân nhưng đây chỉ là phương án chủ quan, việc tích hợp một công cụ cảnh báo sẽ giúp tài xế tránh được các trường hợp lơ là, chủ quan dẫn đến tình huống không mong muốn.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất khi viết Problem Statement là tách bạch vấn đề gốc rễ khỏi giải pháp chủ quan, giữ đúng điểm cân bằng giữa vấn đề và giải pháp để tìm được điểm hội tụ. Nhiều người thường vội vàng nhảy thẳng vào cách giải quyết thay vì đào sâu tìm hiểu nguyên nhân thực sự đằng sau nỗi đau của người dùng 

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Tôi có ý tưởng về hệ thống hỗ trợ chấm bài, rà soát bài làm bằng AI hỗ trợ giáo viên, tuy nhiên hiện tại thị trường có những tool ứng dụng hiệu quả hơn và tôi chưa tìm ra phương án độc đáo nhất để vượt lên đối thủ. Tôi sẽ cần phải nghiên cứu rõ ràng thị trường hơn để đánh giá tính hiệu quả của dự án.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Theo tôi, vấn đề của nhóm mình là tài xế đường dài có thể không nhận ra hoặc đánh giá muộn dấu hiệu buồn ngủ, làm tăng nguy cơ mất tập trung và tai nạn. Hiện nay, tài xế tự theo dõi mức độ tỉnh táo rồi quyết định tiếp tục lái hay dừng nghỉ, nhưng cách này phụ thuộc nhiều vào khả năng tự nhận biết. Tôi đánh giá giải pháp bằng các mục tiêu cần kiểm chứng: Recall từ 90% trở lên, không quá 1 cảnh báo sai mỗi giờ và độ trễ cảnh báo không quá 2 giây. AI chỉ hỗ trợ nhận diện nguy cơ dựa trên nhiều dấu hiệu theo thời gian, không khẳng định chắc chắn tài xế buồn ngủ hay điều khiển phương tiện. Nếu dữ liệu không đủ chất lượng, hệ thống cần báo không khả dụng thay vì kết luận tài xế tỉnh táo. Vì vậy, nhóm tôi chọn mức can thiệp **Workflow**: AI phân tích và phát cảnh báo, còn tài xế tự đánh giá tình trạng và quyết định dừng nghỉ. Tôi cho rằng cần kiểm chứng bằng thực nghiệm trước khi kết luận giải pháp phù hợp để triển khai.

---

## 7. Tài liệu tham khảo

-