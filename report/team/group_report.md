# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Huuduyen
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Thiết lập hệ thống nhận diện tình trạng buồn ngủ của tài xế và cảnh báo sớm.
- Quyết định cuối: Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | Lê Hải Lân | Khi tài xế rời vào trạng thái mệt mỏi, buồn ngủ vì cơ thể suy kiệt khi lái xe đường dài | Tài xế | Làm sao để nhận diện được giấc ngủ trắng do giấc ngủ trắng không thể hiện ở việc nhắm mắt | Nguyễn Bá Quang Huy |
| 5 | Nguyễn Bảo Duy | Thu thập dữ liệu, tích hợp dữ liệu xây dựng hệ thống AI hỗ trợ ôn thi cho sinh viên | Sinh viên | Có thể dùng cái AI hiện hành, cấy dữ liệu vào để xây dựng chat bot trả lời | Nguyễn Bá Quang Huy |
| 6 | Nguyễn Bá Quang Huy | Xây dựng hệ thống hỗ trợ chấm bài cho giáo viên | Giáo viên | Trên thị trường đã có nhiều công cụ sẵn có và đã hỗ trợ rất tốt | Nguyễn Bá Quang Huy |
| 7 |Nguyễn Bảo Duy |Tra cứu mốc thời gian trong Video bài giảng |Sinh viên |Tốn thời gian để tìm kiếm nội dung trong video | |
| 8 |Nguyễn Bảo Duy |Tự động hóa tạo bộ Flashcard ôn thi từ nhiều tài liệu|Sinh viên |Mất thời gian đọc từng tài liệu và tổng hợp kiến thức đưa vào flashcard | |
| 9 |Nguyễn Bảo Duy |Trợ lý so sánh giá và tóm tắt review TMĐT |Người tiêu dùng |Tìm kiếm thủ công, tra cứu giá của các sản phẩm trên từng sàn thương mại điện tử  | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Tài xế đường dài thực sự gặp tình trạng buồn ngủ trong quá trình lái xe và đây là vấn đề đáng quan tâm | Value | 5 | 2 | ✅ |
| 2 | Tài xế thường không nhận biết đủ sớm mức độ buồn ngủ của bản thân để chủ động nghỉ ngơi | Value | 5 | 1 | ✅ |
| 3 | Mô hình có thể duy trì độ chính xác trong các điều kiện khác nhau như ban ngày, ban đêm, đeo kính và thay đổi góc camera | Feasibility | 5 | 1 | ✅ |
| 4 | Kết hợp nhiều dấu hiệu theo thời gian giúp phân biệt buồn ngủ với hành vi bình thường tốt hơn một tín hiệu đơn lẻ | Feasibility | 5 | 2 | ✅ |
| 5 | Việc thu thập và xử lý video khuôn mặt tài xế có thể đáp ứng yêu cầu về quyền riêng tư và chính sách dữ liệu | Viability | 5 | 1 | ✅ |
| 6 | Tài xế và doanh nghiệp vận tải sẵn sàng sử dụng hệ thống cảnh báo trong quá trình vận hành thực tế | Viability | 4 | 1 | ✅ |

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi | L.V.K, 36 tuổi, tài xế container đường dài, có 5 năm kinh nghiệm. |
| Câu nói đáng nhớ nhất (nguyên văn) | "Khó khăn lớn nhất và hiểm nguy nhất của cánh tài xế là buồn ngủ." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Chuyến chở chuối từ Trảng Bom, Đồng Nai đến cửa khẩu Hữu Nghị, Lạng Sơn, khởi hành lúc 21h. Bài viết mô tả hành trình và tình trạng buồn ngủ vào khoảng 2h sáng. |
| Hiện đang xử lý bằng cách nào (workaround)? | Uống trà đặc, cà phê, nước tăng lực; bật nhạc sôi động; rửa mặt bằng nước; cố chạy đến điểm nghỉ rồi ngủ khoảng 3 tiếng. |
| Mất bao lâu, bao lần? | Hành trình khoảng 2.000 km, yêu cầu chạy 45–50 tiếng. Khoảng 2h sáng xuất hiện cơn buồn ngủ mạnh. Tổng thời gian ngủ trên hành trình được anh chia sẻ khoảng 6 tiếng. |
| Insight / opportunity rút ra | Tài xế đường dài phải cân bằng giữa thời gian giao hàng và nhu cầu nghỉ ngơi. Những biện pháp chống buồn ngủ thông thường có thể không còn hiệu quả khi mệt mỏi kéo dài. |

**Interview 02 – T.V.C (Việt Nam)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | T.V.C, 34 tuổi, quê Lâm Đồng, tài xế xe tải đường dài. |
| Câu nói đáng nhớ nhất (nguyên văn) | Anh phải dùng nước đá dội lên đầu để chống lại cơn buồn ngủ khi lái xe. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Trong các chuyến xe chở hàng hơn 1.000 km từ TP.HCM ra Nam Định, tình trạng mệt mỏi và buồn ngủ xuất hiện trong hành trình. |
| Hiện đang xử lý bằng cách nào (workaround)? | Rửa mặt bằng nước đá, dội nước đá lên đầu, uống trà Bắc đặc; nếu không tỉnh táo thì dừng ở trạm xăng để chợp mắt. |
| Mất bao lâu, bao lần? | Không có số lần cụ thể. Có nhiều lần phải áp dụng các biện pháp chống buồn ngủ; thời gian chợp mắt không được định lượng. |
| Insight / opportunity rút ra | Tài xế đã phải sử dụng nhiều biện pháp thủ công để duy trì tỉnh táo. Ngoài nguy cơ tai nạn, việc tìm nơi nghỉ an toàn cũng là một rào cản. |

**Interview 03 – Anh T (Việt Nam)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Anh T, quận 7, TP.HCM, có hơn 20 năm kinh nghiệm lái xe khách đường dài. |
| Câu nói đáng nhớ nhất (nguyên văn) | Anh từng giật mình tỉnh dậy khi đang lái xe và nhận ra mình suýt đâm vào phương tiện phía trước. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | 	Một lần lái xe ban đêm, đặc biệt trong khung giờ 4–5h sáng là thời điểm anh nhận thấy rất dễ buồn ngủ. Ngày cụ thể không được nêu. |
| Hiện đang xử lý bằng cách nào (workaround)? | Uống cà phê hoặc nước tăng lực trước khi lái; trò chuyện với người đi cùng; dừng xe ngủ một lát khi không thể cưỡng lại cơn buồn ngủ. |
| Mất bao lâu, bao lần? | Không có số lần hoặc thời lượng cụ thể. Anh xác nhận bản thân từng trải qua tình trạng này. |
| Insight / opportunity rút ra | Người lái có thể không kiểm soát được thời điểm xuất hiện cơn buồn ngủ. Việc tự đánh giá mức độ tỉnh táo đôi khi không đủ để ngăn chặn nguy cơ. |

**Interview 04 – Đ.V.H**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Đ.V.H, 47 tuổi, Đông Anh, Hà Nội, tài xế xe tải đường dài với hơn 20 năm kinh nghiệm. |
| Câu nói đáng nhớ nhất (nguyên văn) | Anh từng thiếp đi khoảng 1–2 giây khi đang lái xe. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Một chuyến chở hàng đi Tây Bắc. Do quá mệt, anh thiếp đi, đến khi nghe tiếng va chạm mới tỉnh lại và nhận ra bánh xe đã chạm ta-luy đường. |
| Hiện đang xử lý bằng cách nào (workaround)? | Bài viết không ghi rõ đầy đủ các biện pháp thường xuyên anh sử dụng. |
| Mất bao lâu, bao lần? | Anh cho biết từng vài lần rơi vào trạng thái thiếp đi 1–2 giây. |
| Insight / opportunity rút ra | Microsleep có thể xảy ra rất nhanh và tài xế chỉ nhận ra sau khi đã xuất hiện tình huống nguy hiểm. Kinh nghiệm lái xe lâu năm không đồng nghĩa với việc miễn nhiễm với buồn ngủ. |

**Interview 05 – T.N.V**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | T.N.V, tài xế lâu năm, từng lái xe IFa W50 nhận khoán của công ty. |
| Câu nói đáng nhớ nhất (nguyên văn) | Anh cho biết không thể nhớ hết mình đã bao nhiêu lần ngủ gục và bao nhiêu lần thoát chết trong gang tấc. |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Bài viết hồi tưởng giai đoạn hơn 15 năm lái xe cả ngày lẫn đêm. Không nêu ngày xảy ra sự kiện gần nhất. |
| Hiện đang xử lý bằng cách nào (workaround)? | Không có biện pháp cụ thể được mô tả trong bài viết. |
| Mất bao lâu, bao lần? | Nhiều lần ngủ gục trong hơn 15 năm làm nghề, không có con số chính xác. |
| Insight / opportunity rút ra | Với một số tài xế, ngủ gật không phải sự kiện cá biệt mà có thể lặp lại nhiều lần trong suốt quá trình làm nghề. Điều kiện lao động và áp lực kinh tế là yếu tố đáng tìm hiểu. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| https://vnexpress.net/buon-ngu-ke-thu-cua-tai-xe-duong-dai-4577180.html | 1 | Buồn ngủ xuất hiện trong chuyến đi dài; phải dùng trà đặc, cà phê, nước tăng lực và rửa mặt để tỉnh táo. Có thời điểm buồn ngủ mạnh vào khoảng 2h sáng. | Tài xế đã có kinh nghiệm và chủ động bố trí thời gian nghỉ. Chưa có bằng chứng rằng hệ thống AI là giải pháp bắt buộc. |
| https://vietnamnet.vn/tai-xe-xe-duong-dai-ngay-doi-nuoc-da-len-dau-dem-khong-dam-ngu-sau-2230539.html | 1 | Phải dùng nước đá, trà đặc và dừng tại trạm xăng để chợp mắt khi buồn ngủ. Cho thấy các biện pháp tự xử lý hiện tại còn hạn chế. | Chưa có dữ liệu định lượng về tần suất buồn ngủ hoặc hiệu quả của từng biện pháp. |
| https://vietnamnet.vn/giac-ngu-trang-ap-den-khi-lai-xe-mot-giay-chop-mat-hiem-hoa-khon-luong-2467307.html | 1 | Từng nhiều lần thiếp đi 1–2 giây khi lái xe. Có trường hợp chỉ tỉnh lại khi nghe tiếng va chạm. Cho thấy nguy cơ microsleep thực tế. | Chưa có bằng chứng cho thấy camera AI có thể phát hiện sớm hơn cảm nhận của tài xế trong trường hợp này. |
| https://tuoitre.vn/tam-su-cua-tai-xe-tung-khong-nho-bao-nhieu-lan-ngu-guc-khi-lai-xe-choang-tinh-xe-nam-o-bai-co-20250114102229487.htm | 1 | Từng giật mình tỉnh dậy khi đang lái xe. Khung giờ 4–5h sáng dễ buồn ngủ. Đã sử dụng cà phê, nước tăng lực và dừng nghỉ để đối phó. | Tài xế đã nhận biết được một số khung giờ nguy hiểm và có biện pháp chủ động phòng tránh. |
| https://vnexpress.net/con-buon-ngu-sau-tay-lai-3873060.html | 1 | Buồn ngủ trong chuyến xe đêm sau khi làm việc liên tục. Áp lực giao hàng có thể khiến tài xế tiếp tục lái dù mệt mỏi. Đã xảy ra tai nạn nghiêm trọng. | Trường hợp này chưa chứng minh cảnh báo AI sẽ thay đổi hành vi nếu tài xế vẫn chịu áp lực phải hoàn thành chuyến hàng. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
|MediaPipe Face Mesh | https://vision.fe.uni-lj.si/cvww2016/proceedings/papers/05.pdf|Trích xuất tọa độ khuôn mặt & phân loại bằng công thức toán học | Siêu nhẹ, API cực tốt cho cả Python và C++. Chạy real-time mượt mà ngay cả trên CPU laptop thông thường|Không hoạt động tốt nếu thiếu sáng ban đêm, tài xế đeo kính râm đen, hoặc góc quay quá nghiêng. Không hiểu bối cảnh thời gian |Có thể tạo ra một prototype chạy được ngay trong 1-2 tuần đầu để test luồng (pipeline) của hệ thống |
|YOLOv8 / YOLOv11 |https://docs.ultralytics.com/integrations/tensorrt |Nhận diện đối tượng trên frame ảnh tĩnh & triển khai thực tế |Cân bằng giữa tốc độ và độ chính xác. Rất dễ chuyển đổi mô hình để chạy nhúng |Phải tự code thêm module quản lý trạng thái để xác định "buồn ngủ" thay vì chỉ 1 frame "nhắm mắt" |Có thể đưa mô hình lên các thiết bị IoT trên xe ô tô thực tế |
| Vision Transformer| https://github.com/lucidrains/vit-pytorch| Phân tích End-to-end: Đưa cả 1 đoạn video (chuỗi frame) vào, mô hình tự trả ra kết quả trạng thái tài xế| Hiểu được toàn bộ chuỗi hành vi lờ đờ, gật gù theo thời gian nhờ cơ chế Attention| Mô hình rất nặng, ngốn nhiều VRAM máy tính. Đòi hỏi GPU mạnh để huấn luyện. Khó tối ưu độ trễ khi chạy trên phần cứng yếu|Có thể ứng dụng nếu có server/GPU đủ mạnh |
|Phân tích Telematics | https://iieta.org/sites/default/files/pdf/2025-04/ts_42.02_38.pdf| Phân tích dữ liệu chuỗi thời gian 1D từ cảm biến của xe|Hoàn toàn miễn nhiễm với các vấn đề của Camera (chạy tốt ban đêm, không sợ tài xế đeo kính râm, che mặt, ngược sáng) |Thu thập dữ liệu thực tế cực kỳ khó. Hệ thống chỉ báo động khi xe đã có dấu hiệu lạng lách |Hướng đi nếu nhóm muốn áp dụng kiến thức Streaming |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

**Sơ đồ quy trình:**

```text
[1. Bắt đầu chuyến đi]
          ↓
[2. Lái xe liên tục]
          ↓
[3. Tự cảm nhận mức độ tỉnh táo]
          ↓
[4. Nhận biết dấu hiệu mệt mỏi/buồn ngủ]
          ↓
[5. Tự quyết định tiếp tục lái hoặc tìm nơi an toàn để nghỉ]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Tài xế | Lịch trình, phương tiện, tình trạng sức khỏe | Bắt đầu chuyến đi | Đầu mỗi chuyến | Chuẩn bị và kiểm tra trước khi lái |
| 2 | Tài xế | Tuyến đường, điều kiện giao thông | Tiếp tục điều khiển phương tiện | Liên tục trong chuyến đi | Có thể kéo dài nhiều giờ |
| 3 | Tài xế | Cảm giác cơ thể, mức độ tỉnh táo | Tự đánh giá tình trạng hiện tại | Không cố định | Phụ thuộc vào khả năng tự nhận biết |
| 4 | Tài xế | Dấu hiệu mỏi mắt, ngáp, nhắm mắt, mất tập trung | Nhận biết hoặc nghi ngờ bản thân đang buồn ngủ | Khi xuất hiện dấu hiệu | Có thể nhận biết muộn hoặc bỏ qua dấu hiệu |
| 5 | Tài xế | Cảm nhận về mức độ buồn ngủ, lịch trình | Quyết định tiếp tục lái hoặc dừng nghỉ | Khi cảm thấy cần thiết | Có thể tiếp tục lái do áp lực thời gian hoặc thiếu điểm nghỉ |

**Bottleneck chính:**

Bước 3–5: Tài xế phải tự nhận biết và đánh giá mức độ buồn ngủ. Tuy nhiên, khi tình trạng mệt mỏi tăng lên, khả năng tự đánh giá có thể không còn đáng tin cậy. Tài xế cũng có thể bỏ qua dấu hiệu cảnh báo hoặc cố tiếp tục lái vì áp lực lịch trình, dẫn đến phát hiện muộn và tăng nguy cơ mất kiểm soát phương tiện.

### 4.2. Quy trình tương lai

**Sơ đồ quy trình:**

```text
[1. Tài xế bắt đầu chuyến đi]
          ↓
[2. Camera ghi nhận khuôn mặt liên tục]
          ↓
[3. Trích xuất đặc trưng mắt, miệng, chuyển động đầu]
          ← AI: Computer Vision / Facial Landmarks
          ↓
[4. Phân tích chuỗi tín hiệu theo thời gian]
          ← AI: Temporal Analysis
          ↓
[5. Phân loại trạng thái và đánh giá nguy cơ buồn ngủ]
          ← AI: Classification / Risk Scoring
          ↓
[6. Kiểm tra ngưỡng và quyết định phát cảnh báo]
          ← RULE + AI
          ↓
[7. Tài xế tiếp nhận cảnh báo, đánh giá tình trạng
    và chủ động dừng xe tại nơi an toàn để nghỉ]
          ← CON NGƯỜI
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Phương pháp |
|---:|---|---|---|---|---|
| 1 | Tài xế | Phương tiện, lịch trình | Bắt đầu chuyến đi | Đầu mỗi chuyến | Con người |
| 2 | Camera | Hình ảnh khuôn mặt tài xế | Video hoặc frame đầu vào | Liên tục | Rule / Thiết bị |
| 3 | Hệ thống AI | Frame hình ảnh | Đặc trưng mắt, miệng, chuyển động đầu | Liên tục | AI – Computer Vision, Facial Landmarks |
| 4 | Hệ thống AI | Chuỗi đặc trưng theo thời gian | Các mẫu hành vi và tín hiệu liên quan đến buồn ngủ | Liên tục | AI – Temporal Analysis |
| 5 | Hệ thống AI | Các tín hiệu đã trích xuất | Nhãn trạng thái hoặc điểm nguy cơ buồn ngủ | Theo từng cửa sổ thời gian | AI – Classification / Risk Scoring |
| 6 | Hệ thống cảnh báo | Điểm nguy cơ, ngưỡng cảnh báo, trạng thái hệ thống | Cảnh báo âm thanh hoặc hình ảnh | Khi đạt điều kiện cảnh báo | Rule + AI |
| 7 | Tài xế | Cảnh báo và tình trạng thực tế | Quyết định giảm tốc, dừng xe và nghỉ ngơi | Khi nhận cảnh báo | Con người |

**BOUNDARY:**

- AI chỉ hỗ trợ nhận diện dấu hiệu và đánh giá nguy cơ buồn ngủ, không khẳng định chắc chắn trạng thái sinh lý của tài xế.
- Không phát cảnh báo chỉ dựa trên một hành vi đơn lẻ như ngáp, nhắm mắt ngắn hoặc cúi đầu.
- AI không tự điều khiển phương tiện, không tự quyết định dừng xe và không thay thế trách nhiệm của tài xế.
- Video được ưu tiên xử lý trực tiếp trên thiết bị; không mặc định truyền lên cloud hoặc lưu trữ video khuôn mặt.
- Khi camera không nhận diện được khuôn mặt hoặc dữ liệu đầu vào không đủ chất lượng, hệ thống phải thông báo trạng thái không khả dụng thay vì kết luận tài xế tỉnh táo.

**PHƯƠNG ÁN QUAY VỀ:**

- Camera mất tín hiệu hoặc AI gặp lỗi → Thông báo hệ thống không khả dụng.
- Ánh sáng yếu, khuôn mặt bị che khuất hoặc góc camera không phù hợp → Thông báo hạn chế khả năng phát hiện.
- AI phát hiện sai hoặc cảnh báo bất thường → Tài xế đánh giá tình trạng thực tế, không phụ thuộc hoàn toàn vào kết quả AI.
- Hệ thống không thể hoạt động → Quay về quy trình tự giám sát và chủ động nghỉ ngơi theo lịch trình an toàn.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 7 | Bổ sung các bước giám sát, phân tích và cảnh báo tự động |
| Tổng thời gian | Không cố định | Giám sát liên tục, cảnh báo gần thời gian thực | Chưa có số liệu đo thực nghiệm |
| Số bước thủ công | 5/5 | 2/7 | Tài xế bắt đầu chuyến đi và xử lý cảnh báo; các bước còn lại được hệ thống hỗ trợ tự động |
| Bottleneck chính | Tài xế tự nhận biết và đánh giá mức độ buồn ngủ | AI phân biệt buồn ngủ với hành vi bình thường | Cần cân bằng Recall, false alarms/hour và độ trễ |
| Rủi ro mới phát sinh | Phát hiện muộn, bỏ qua dấu hiệu buồn ngủ | Cảnh báo sai, bỏ sót, lỗi camera hoặc điều kiện môi trường | Cần kiểm thử thực tế, boundary và phương án quay về |

**Nhận định:**

Giá trị của quy trình tương lai không nằm ở việc giảm số bước hay giảm thời gian thao tác, mà ở việc chuyển từ tự giám sát hoàn toàn sang giám sát có AI hỗ trợ. Hệ thống hướng đến phát hiện dấu hiệu buồn ngủ sớm hơn, giảm phụ thuộc vào khả năng tự đánh giá của tài xế và cung cấp cảnh báo kịp thời để họ chủ động nghỉ ngơi. Đây là mục tiêu cần được kiểm chứng bằng thực nghiệm, không phải hiệu quả đã được chứng minh.
---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Tài xế điều khiển phương tiện, đặc biệt là tài xế phải lái xe liên tục trong thời gian dài. |
| **Quy trình** | Tài xế bắt đầu chuyến đi, tự theo dõi tình trạng tỉnh táo trong quá trình lái xe và chủ động quyết định nghỉ ngơi khi cảm thấy buồn ngủ hoặc mệt mỏi. |
| **Bottleneck** | Tài xế phải tự nhận biết và đánh giá mức độ buồn ngủ. Các dấu hiệu như chớp mắt chậm, nhắm mắt kéo dài, ngáp hoặc cúi đầu có thể xuất hiện nhưng không phải lúc nào tài xế cũng nhận ra hoặc đánh giá đúng mức độ nguy hiểm. |
| **Impact** | Phát hiện muộn hoặc bỏ qua dấu hiệu buồn ngủ có thể làm giảm khả năng tập trung, chậm phản ứng và tăng nguy cơ xảy ra tai nạn giao thông, gây thiệt hại về người và tài sản. |
| **Success Metric** (baseline → target, cách đo) | Baseline: Chưa có hệ thống giám sát tự động, khả năng phát hiện phụ thuộc vào tự đánh giá của tài xế và chưa có số liệu đo lường cụ thể. Target: Hệ thống phát hiện được các dấu hiệu buồn ngủ với Recall mục tiêu ≥ 90%, duy trì tỷ lệ cảnh báo sai ở mức thấp (ví dụ ≤ 1 false alarm/hour) và độ trễ cảnh báo mục tiêu ≤ 2 giây. Đo lường thông qua dữ liệu video được gán nhãn, so sánh kết quả dự đoán với nhãn thực tế, đồng thời thống kê số cảnh báo sai và độ trễ trong các tình huống kiểm thử. Đây là các mục tiêu đề xuất cần kiểm chứng thực nghiệm. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ nhận diện dấu hiệu và đánh giá nguy cơ buồn ngủ, không khẳng định chắc chắn trạng thái sinh lý của tài xế. Không đưa ra kết luận chỉ dựa trên một hành vi đơn lẻ. Không tự điều khiển phương tiện hoặc quyết định dừng xe. Tài xế phải tự đánh giá tình trạng thực tế và quyết định dừng xe tại nơi an toàn để nghỉ ngơi. Khi dữ liệu không đủ chất lượng, camera mất tín hiệu hoặc AI gặp lỗi, hệ thống phải thông báo không khả dụng thay vì kết luận tài xế tỉnh táo. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

1. Không nên coi hành vi ngáp hoặc nhắm mắt ngắn là bằng chứng chắc chắn của buồn ngủ: Hệ thống cần phân tích nhiều đặc trưng và chuỗi hành vi theo thời gian để hạn chế cảnh báo sai.
2. Không nên để AI tự quyết định điều khiển phương tiện hoặc dừng xe vì đây là quyết định có ảnh hưởng trực tiếp đến an toàn giao thông: AI chỉ đưa ra cảnh báo và đánh giá nguy cơ, tài xế chịu trách nhiệm xử lý.
---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: Độ mơ hồ cao × Độ phức tạp cao.

Vì sao: 
Độ mơ hồ cao: Biểu hiện buồn ngủ không hoàn toàn giống nhau giữa các tài xế. Một số hành vi như ngáp, chớp mắt hoặc cúi đầu có thể xuất hiện trong trạng thái bình thường, không nhất thiết đồng nghĩa với buồn ngủ.
Độ phức tạp cao: Hệ thống cần xử lý dữ liệu hình ảnh liên tục, nhận diện khuôn mặt, trích xuất đặc trưng mắt, miệng và chuyển động đầu, sau đó phân tích mối quan hệ giữa các tín hiệu theo thời gian.
Ngoài ra, hệ thống phải hoạt động trong nhiều điều kiện môi trường khác nhau như ánh sáng yếu, tài xế đeo kính, khuôn mặt bị che khuất hoặc thay đổi góc nhìn camera.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Quy định thời gian nghỉ giữa các chuyến, khuyến khích tài xế tự kiểm tra tình trạng tỉnh táo và nghỉ ngơi định kỳ. | Khi chỉ cần cải thiện ý thức và kỷ luật nghỉ ngơi của tài xế. | Phụ thuộc hoàn toàn vào ý thức và khả năng tự đánh giá; khó phát hiện dấu hiệu buồn ngủ bất thường. | Không |
| **Rule** | Sử dụng ngưỡng cố định để phát hiện các hành vi như nhắm mắt quá lâu, ngáp liên tục hoặc cúi đầu. | Khi môi trường hoạt động ổn định và các dấu hiệu cần phát hiện có thể mô tả bằng quy tắc rõ ràng. | Khó phân biệt hành vi bình thường và buồn ngủ; dễ báo nhầm hoặc bỏ sót. | Không |
| **Workflow** | Camera thu thập hình ảnh → AI nhận diện đặc trưng → phân tích theo thời gian → đánh giá nguy cơ → Rule kiểm tra ngưỡng → phát cảnh báo cho tài xế. | Khi cần kết hợp AI xử lý dữ liệu phức tạp với các quy tắc kiểm soát và quy trình xử lý rõ ràng. | Phụ thuộc vào chất lượng dữ liệu, mô hình AI và điều kiện môi trường; có thể xuất hiện cảnh báo sai hoặc bỏ sót. | Có |
| **Agent** | 	AI tự lập kế hoạch, chủ động thực hiện nhiều hành động hoặc phối hợp với các hệ thống khác để xử lý tình huống buồn ngủ. | Khi cần hệ thống tự chủ xử lý nhiều tác vụ và có quyền thực hiện hành động trong phạm vi được kiểm soát. | Tăng độ phức tạp, khó kiểm soát hành vi và không cần thiết đối với bài toán cảnh báo buồn ngủ. | Không |

**Mức chọn:** WORKFLOW

**Vì sao không chọn mức đơn giản hơn:**
Không chọn No AI: Vì việc tự giám sát của tài xế không đảm bảo phát hiện sớm các dấu hiệu buồn ngủ, đặc biệt khi tài xế không nhận thức được mức độ mệt mỏi của bản thân.
Không chọn Rule: Vì các dấu hiệu buồn ngủ có tính biến thiên, khó mô tả đầy đủ bằng những ngưỡng cố định. Cần AI để nhận diện đặc trưng hình ảnh và phân tích chuỗi hành vi theo thời gian.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Phân tích hình ảnh khuôn mặt và chuỗi hành vi theo thời gian để nhận diện các dấu hiệu liên quan đến buồn ngủ, từ đó phân loại trạng thái hoặc tạo điểm nguy cơ buồn ngủ. |
| **Judgment** — con người cân nhắc, quyết định gì? | Tài xế đánh giá tình trạng tỉnh táo thực tế của bản thân, cân nhắc mức độ nguy hiểm và quyết định có cần giảm tốc độ, dừng xe và nghỉ ngơi hay không. |
| **Action** — hành động cuối cùng là gì, ai làm? | Hệ thống AI phát cảnh báo bằng âm thanh hoặc hình ảnh khi đạt ngưỡng nguy cơ. Tài xế tiếp nhận cảnh báo và chủ động dừng phương tiện tại vị trí an toàn để nghỉ ngơi. |
| **Outcome** — đo kết quả bằng gì? | Recall, Precision, F1-score, số cảnh báo sai trên mỗi giờ (False Alarms/Hour), độ trễ cảnh báo và tỷ lệ phát hiện đúng trong các điều kiện môi trường khác nhau. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Video hoặc frame hình ảnh khuôn mặt tài xế từ camera, bao gồm đặc trưng mắt, miệng và chuyển động đầu. Dữ liệu được thu thập trực tiếp từ camera trong quá trình lái xe. Cần xây dựng tập dữ liệu có gán nhãn để huấn luyện và đánh giá mô hình. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Dữ liệu video đã được gán nhãn, kết quả kiểm thử thực tế, thống kê cảnh báo sai và phản hồi của tài xế. Các trường hợp nhận diện sai hoặc bỏ sót được sử dụng để bổ sung dữ liệu, điều chỉnh mô hình và ngưỡng cảnh báo. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
Người dùng muốn được hỗ trợ.
Bằng chứng:
-Tài xế vẫn trực tiếp điều khiển phương tiện và chịu trách nhiệm về an toàn chuyến đi.
-AI chỉ hỗ trợ phát hiện dấu hiệu buồn ngủ mà tài xế có thể không tự nhận ra.
-Khi nhận cảnh báo, tài xế tự đánh giá tình trạng thực tế và quyết định dừng xe nghỉ ngơi.
-AI không có quyền tự động điều khiển phương tiện hoặc đưa ra quyết định thay con người.

- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
Ai bỏ sót sẽ tệ hơn
Lý do:
-Nếu AI báo nhầm, tài xế có thể bị làm phiền hoặc phải kiểm tra lại tình trạng của mình, gây gián đoạn chuyến đi.
-Nếu AI bỏ sót dấu hiệu buồn ngủ, tài xế có thể tiếp tục lái xe trong trạng thái thiếu tỉnh táo mà không nhận được cảnh báo, làm tăng nguy cơ tai nạn.

Cách thiết kế để hạn chế rủi ro:
-Ưu tiên Recall trong quá trình lựa chọn và đánh giá mô hình nhằm hạn chế bỏ sót các trường hợp buồn ngủ.
-Không dựa vào một hành vi đơn lẻ mà kết hợp nhiều đặc trưng mắt, miệng và chuyển động đầu theo thời gian.
-Sử dụng ngưỡng cảnh báo phù hợp để cân bằng giữa khả năng phát hiện và tỷ lệ cảnh báo sai.
-Khi dữ liệu đầu vào không đủ chất lượng, thông báo hệ thống không khả dụng thay vì kết luận tài xế tỉnh táo.
-Giữ tài xế trong vòng kiểm soát (Human-in-the-loop), không để AI tự quyết định hành động điều khiển phương tiện.
---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Tài xế điều khiển phương tiện (người dùng cuối trực tiếp) và người quản lý an toàn đội xe|
| **Quy trình** |Bắt đầu lái xe → Camera ghi hình liên tục → AI phân tích chuỗi hành vi → Đạt ngưỡng nguy hiểm → Phát cảnh báo → Tài xế quyết định giảm tốc/nghỉ ngơi |
| **Bottleneck** |Tài xế không thể tự nhận thức được khoảnh khắc ngủ gật chớp nhoáng hoặc sự suy giảm tập trung diễn ra từ từ. Đợi đến lúc tài xế tự nhận ra thì đã quá muộn |
| **Impact** |Nguy cơ tai nạn giao thông nghiêm trọng gây thiệt hại sinh mạng và tài sản. Tăng chi phí bảo hiểm và rủi ro pháp lý cho doanh nghiệp vận tải |
| **Success Metric** (baseline → target, cách đo) |Baseline: Hoàn toàn dựa vào cảm giác chủ quan của tài xế. Target: (1) Recall ≥ 90% (bắt đúng các ca buồn ngủ). (2) False Alarm ≤ 1 lần/giờ lái xe. (3) Độ trễ (Latency) ≤ 2 giây từ lúc có biểu hiện đến lúc hú còi. Cách đo: Lắp camera chạy thử nghiệm thực tế nghiệm. Quản lý đội xe đối chiếu video log với thời điểm AI phát cảnh báo để tính các chỉ số |
| **Boundary** | AI không can thiệp vào hệ thống lái/phanh của xe. AI không kết luận tài xế buồn ngủ chỉ qua 1 cú ngáp hay 1 cái chớp mắt đơn lẻ. Nếu camera bị che khuất hoặc thiếu sáng trầm trọng, AI phải báo "Hệ thống không khả dụng"|
| **AI intervention point** |Nằm ở bước số 4 và 5: AI can thiệp vào khâu phân tích dữ liệu video theo thời gian thực (ngay trên thiết bị trong cabin) và đối chiếu ngưỡng để kích hoạt cảnh báo, thay thế cho việc tài xế phải "tự cảm nhận" độ tỉnh táo của mình |
| **Mức chọn** | Workflow|
| **Rủi ro & người kiểm tra** |Rủi ro: Cảnh báo sai (False Positive) gây ức chế tâm lý khiến tài xế tắt thiết bị; hoặc bỏ sót (False Negative) gây tai nạn. Người kiểm tra: Tài xế kiểm tra chéo ngay lúc nhận cảnh báo + Quản lý đội xe hậu kiểm lại log video |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
|Actor |Chỉ có tài xế|Thêm "người quản lý an toàn đội xe" | Thực tế doanh nghiệp vận tải mới là người mua giải pháp và cần dashboard để theo dõi hành vi tài xế, tài xế chỉ là người sử dụng/tiếp nhận|
|Bottleneck |Tài xế tự đánh giá mức độ buồn ngủ|Nhấn mạnh vào khoảnh khắc ngủ gật chớp nhoáng và sự mất nhận thức tạm thời | Làm nổi bật lý do vì sao AI bắt buộc phải phân tích "chuỗi thời gian" thay vì chỉ nhìn 1 ảnh tĩnh tĩnh|

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 |Bắt đúng sự kiện |AI kích hoạt cảnh báo đúng vào các chuỗi sự kiện tài xế ngủ gật, gật gù liên tục khớp với dữ liệu đã gán nhãn thực tế | Bỏ sót các ca tài xế ngủ mở mắt (mắt lờ đờ, không tập trung) hoặc ngủ gật nhưng đầu vẫn giữ thẳng|
| 2 | Ít cảnh báo giả| AI phân biệt được và bỏ qua các hành vi bình thường: Nháy mắt sinh lý, ngáp do thiếu oxy nhẹ, liếc nhìn gương chiếu hậu. Tần suất báo sai ≤ 1 lần/giờ|Còi hú liên tục khi tài xế nheo mắt vì chói nắng mặt trời, hoặc khi tài xế đeo kính/chỉnh kính |
| 3 |Độ trễ thấp |Tính từ khoảnh khắc chuỗi đặc trưng vượt ngưỡng nguy hiểm, còi báo động phải kêu trong vòng ≤ 2 giây | Hệ thống giật lag, xử lý chậm, tài xế nhắm mắt 4-5 giây (xe đã lạng làn) thì AI mới bắt đầu báo động|
| 4 | Tính ổn định|Duy trì được khả năng nhận diện điểm neo khuôn mặt trong điều kiện thực tế khắc nghiệt: cabin tối (ban đêm), ánh sáng ngược chói, hoặc tài xế đeo kính/khẩu trang | Trạng thái mắt/miệng bị nhận diện sai lệch hoàn toàn khi góc camera rung lắc hoặc khi thay đổi điều kiện ánh sáng đột ngột|

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? |Thấp |Buồn ngủ là nguyên nhân top đầu gây tai nạn xe tải. Quản lý đội xe sẵn sàng đầu tư để giảm rủi ro đền bù và bảo vệ tài sản |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? |Trung bình |Đầu ra rất dễ hiểu (còi hú, đèn chớp). Tuy nhiên, nếu báo sai nhiều, tài xế sẽ ức chế. Cần thiết kế cơ chế (nút bấm vật lý) để tài xế báo cáo "AI nhận diện sai" giúp model học lại |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? |Trung bình |Việc huấn luyện AI nhận diện mặt không khó. Cái khó là tối ưu mô hình để chạy mượt mà chuỗi thời gian trên máy tính nhúng yếu (Edge AI) đặt trong xe mà không bị quá nhiệt hay giật lag |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? |Trung bình |Cần chi phí lắp đặt phần cứng (Camera hồng ngoại IR + Bộ vi xử lý) cho từng xe. Về pháp lý, cần thông báo rõ với tài xế về việc ghi hình để đảm bảo quyền riêng tư |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:** Vấn đề có giá trị cực kỳ lớn (cứu mạng người, tiết kiệm tài sản). Bài toán nằm trong khả năng giải quyết của Computer Vision hiện tại. Rủi ro về ranh giới an toàn đã được kiểm soát chặt chẽ bằng thiết kế Workflow

**Nếu Go — pilot nhỏ nhất:** 
Lắp đặt thiết bị trên 2-5 chiếc xe tải chạy tuyến đường dài (ca đêm) trong 2 tuần
Giai đoạn 1 (Shadow Mode - 1 tuần): AI chạy ngầm, ghi nhận log và video nhưng không phát ra tiếng còi để đánh giá âm thầm mức độ Recall và False Positive (tránh làm phiền tài xế khi model chưa hoàn thiện)

Giai đoạn 2 (Active Mode - 1 tuần): Bật cảnh báo âm thanh, thu thập feedback trực tiếp từ tài xế xem còi báo có đúng lúc và có gây ức chế không

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng**: Nếu sau 2 tuần Pilot mà tỉ lệ cảnh báo sai > 3 lần/giờ hoặc hệ thống liên tục bị sập do phần cứng quá nhiệt, thì quay về giai đoạn thu thập thêm dữ liệu gán nhãn (đặc biệt là dữ liệu ban đêm) và tối ưu lại trọng lượng mô hình trước khi đem ra test tiếp

---

## 9. Hạn chế và hướng tiếp theo
### 9.1. Hạn chế về dữ liệu và xác định "Ground Truth"
- Mất cân bằng dữ liệu: Trong thực tế, 99% thời gian lái xe là trạng thái bình thường, hành vi ngủ gật chỉ chiếm chưa tới 1%. Việc thu thập đủ dữ liệu đa dạng về các pha buồn ngủ thực tế trên xe tải là cực kỳ khó và tốn kém

- Tính chủ quan của nhãn: Camera chỉ ghi nhận được biểu hiện vật lý (nhắm mắt, ngáp). Ground truth tuyệt đối của giấc ngủ phải được đo bằng sóng não (EEG). Do đó, AI vẫn có sai số sinh học (ví dụ: tài xế lờ đờ nhưng mắt vẫn mở to, hoặc tài xế chớp mắt chậm do khô mắt chứ không phải buồn ngủ)
### 9.2. Hạn chế về môi trường và phần cứng
- Điểm mù ngoại cảnh: Hệ thống camera RGB thông thường sẽ bị suy giảm độ chính xác nghiêm trọng nếu tài xế đeo kính râm tối màu che khuất hoàn toàn đặc trưng mắt, hoặc khi cabin bị ngược sáng

- Xung đột giữa Độ trễ và Độ chính xác: Các mô hình phân tích chuỗi thời gian (như 3D-CNN hay Vision Transformer) cho độ chính xác rất cao nhưng lại quá nặng. Khi ép các mô hình này chạy trên thiết bị nhúng có tản nhiệt kém trong cabin xe, hệ thống dễ bị quá nhiệt, dẫn đến giật lag và làm tăng độ trễ cảnh báo
### 9.3. Hướng phát triển tiếp theo
- Cơ chế Feedback vật lý: Lắp đặt một nút bấm "Báo cáo sai" trên taplo. Mỗi khi hệ thống báo động nhầm, tài xế chỉ cần đập tay vào nút. Hệ thống sẽ tự động cắt 10 giây video trước đó, dán nhãn "False Positive" và gửi về server để model học lại
- Tích hợp dữ liệu Telematics (Mạng CAN bus): Không chỉ nhìn vào khuôn mặt, hệ thống sẽ kết hợp thêm dữ liệu từ chính chiếc xe (Góc đánh lái, vận tốc, phanh). Nếu mắt tài xế chớp chậm và xe bắt đầu có dấu hiệu lạng làn/đánh lái gắt, độ tin cậy của cảnh báo sẽ đạt mức gần như tuyệt đối
- Mỗi con người có một nhịp sinh học và tần suất chớp mắt bình thường khác nhau. Hướng đi tiên tiến nhất là AI tự học: Trong 15 phút đầu tiên của chuyến đi , hệ thống sẽ ngầm ghi nhận "Baseline" (ngưỡng bình thường) của riêng tài xế đó. Các cảnh báo sau này sẽ được đối chiếu với "Baseline" cá nhân hóa này thay vì dùng một quy tắc cứng nhắc cho tất cả mọi người
## 10. Tài liệu tham khảo

-
