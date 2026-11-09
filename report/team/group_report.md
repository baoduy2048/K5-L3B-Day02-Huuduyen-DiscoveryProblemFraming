# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Huuduyen
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
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
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| MediaPipe Face Mesh| https://vision.fe.uni-lj.si/cvww2016/proceedings/papers/05.pdf| Trích xuất tọa độ khuôn mặt và phân loại|Siêu nhẹ, API cực tốt cho cả Python và C++. Chạy real-time mượt mà ngay cả trên CPU laptop thông thường| Không hoạt động tốt nếu thiếu sáng ban đêm, tài xế đeo kính râm đen, hoặc góc quay quá nghiêng| Là công cụ để code ra một prototype chạy được ngay trong 1-2 tuần đầu để test luồng của hệ thống|
|YOLOv8 / YOLOv11 |https://docs.ultralytics.com/integrations/tensorrt | Nhận diện đối tượng trên frame ảnh tĩnh|Cân bằng tuyệt vời giữa Tốc độ và Độ chính xác. Rất dễ chuyển đổi mô hình để chạy nhúng | Phải tự code thêm module quản lý trạng thái để xác định "buồn ngủ" thay vì chỉ 1 frame "nhắm mắt"|Có thể đưa mô hình lên các thiết bị IoT trên xe ô tô thực tế |
|Vision Transformer |https://github.com/lucidrains/vit-pytorch |Phân tích End-to-end: Đưa cả 1 đoạn video vào, mô hình tự trả ra kết quả trạng thái tài xế |Hiểu được toàn bộ chuỗi hành vi lờ đờ, gật gù theo thời gian nhờ cơ chế Attention | Mô hình rất nặng, ngốn nhiều VRAM máy tính. Đòi hỏi GPU mạnh để huấn luyện. Khó tối ưu độ trễ|Có thể sử dụng nếu có server/GPU đủ mạnh để train |
|Phân tích Telematics | https://iieta.org/sites/default/files/pdf/2025-04/ts_42.02_38.pdf| Phân tích dữ liệu chuỗi thời gian 1D từ cảm biến của xe| Hoàn toàn miễn nhiễm với các vấn đề của Camera| Thu thập dữ liệu thực tế cực kỳ khó. Hệ thống chỉ báo động khi xe đã có dấu hiệu lạng lách| Có thể sử dụng nếu muốn áp dụng kiến trúc streaming|

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
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
