# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
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
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

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

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

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
| **Actor** | Tài xế xe tải, xe khách hoặc tài xế đường dài. Người quản lý đội xe là bên có thể triển khai và theo dõi hiệu quả hệ thống|
| **Quy trình** |1. Bắt đầu chuyến đi - Tự đánh giá mức độ tỉnh táo - 3. Quan sát dấu hiệu buồn ngủ/mỏi mắt - 4. Tự quyết định lái tiếp hay nghỉ - 5. Camera ghi nhận khuôn mặt - 6. Hệ thống phát cảnh báo khi vượt ngưỡng - 7. Tài xế quyết định giảm tốc/nghỉ ngơi |
| **Bottleneck** |Bước 5–6: Việc nhận biết và phân biệt dấu hiệu buồn ngủ rất khó (nhắm mắt, ngáp riêng lẻ chưa chắc là buồn ngủ). Dựa vào một tín hiệu hoặc một khung hình tĩnh dễ dẫn đến cảnh báo sai hoặc bỏ sót |
| **Impact** |Cảnh báo sai thường xuyên làm tài xế mất niềm tin và bỏ qua cảnh báo thật; trong khi đó, cảnh báo muộn khiến tài xế không còn đủ thời gian phản ứng an toàn |
| **Success Metric** (baseline → target, cách đo) |1. Đạt Recall mục tiêu với các sự kiện buồn ngủ đã gán nhãn
2. Giảm số cảnh báo sai (false positive) trên mỗi giờ lái xe
3. Giảm độ trễ từ khi có dấu hiệu đến khi phát cảnh báo
4. Duy trì độ chính xác trong nhiều điều kiện ánh sáng và góc camera |
| **Boundary** | AI chỉ phân tích chuỗi tín hiệu để đánh giá rủi ro và phát cảnh báo. AI không trực tiếp can thiệp vào việc điều khiển xe (phanh, đánh lái), tài xế vẫn là người đưa ra quyết định cuối cùng|
| **AI intervention point** |Can thiệp ở bước 5-6: AI thực hiện phân tích chuỗi thời gian (temporal analysis) dựa trên trạng thái mắt, miệng, chuyển động đầu để đưa ra cảnh báo đáng tin cậy thay vì phản ứng với một dấu hiệu đơn lẻ |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** |Rủi ro: Cảnh báo sai làm phiền tài xế hoặc bỏ sót dấu hiệu nguy hiểm
Người kiểm tra: Tài xế trực tiếp đánh giá tính chính xác của cảnh báo trên xe và người quản lý đội xe theo dõi log dữ liệu để đánh giá hiệu quả tổng thể của hệ thống |

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
