## Scan rộng

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Tra cứu thông tin sản phẩm, chiến dịch bán hàng để trả lời câu hỏi của khác | CSKH, Khách hàng | Mất khoảng 5-10 phút/lần |
| 2 | Lặp lại | Tư vấn sản phẩm phù hợp theo nhu cầu khách | Sales | 10–20 phút/lần |
| 3 | Tốn thời gian | Viết mô tả sản phẩm chuẩn SEO từ catalogue của nhà sản xuất | Marketing | 20–40 phút/sản phẩm |
| 4 | Tốn thời gian | Tổng hợp các câu hỏi khách thường hỏi để cập nhật FAQ | CSKH | 1–2 giờ/tuần |
| 5 | AI có thể tốt hơn | Tóm tắt hàng trăm đánh giá của khách về một sản phẩm | Marketing, Product | Phân tích sentiment và các vấn đề nổi bật |
| 6 | AI có thể tốt hơn | Slack search tìm decision cũ rất khó | Cả team | 10-15 phút/lần tìm |
| 7 | Pain từ người khác | Designer phải hỏi lại vì spec từ PM mập mờ | Designer, PM | Hỏi lại 2-3 lần/spec |
| 8 | Pain từ người khác | CEO hỏi update nhưng report chưa sẵn | CEO, PM | Hay bị trễ deadline thứ Hai |
| 9 | Tốn thời gian | Tổng hợp monthly KPI từ nhiều dashboard | PM, manager | Lặp lại mỗi tháng |
| 10 | Lặp lại | Viết standup update mỗi sáng cùng format | PM | 5-10 phút/ngày |


## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Tra cứu thông tin sản phẩm, chiến dịch bán hàng để trả lời câu hỏi của khác | Workflow rõ ràng, lặp lại nhiều lần mỗi ngày, tốn thời gian tra cứu, dữ liệu (catalogue, FAQ, chính sách) thường đã có sẵn và dễ tích hợp cho AI. Có thể đo bằng thời gian phản hồi và tỷ lệ trả lời thành công. | AI cần trả lời đủ chính xác và đúng ngữ cảnh. Cần xác định thế nào là "câu trả lời đủ tốt" và tỷ lệ hallucination có chấp nhận được hay không. |
| 2 | Phân tích và tổng hợp đánh giá khách hàng | Doanh nghiệp thường có nhiều review nhưng khó đọc hết. AI có thể tóm tắt ý kiến, phân loại sentiment và phát hiện vấn đề lặp lại, giúp cải thiện sản phẩm nhanh hơn. | Khó chứng minh giá trị trực tiếp lên doanh thu. Cần xác định cách đo chất lượng bản tóm tắt và mức độ hữu ích với người dùng. |
| 3 | AI tư vấn và so sánh sản phẩm | Hỗ trợ khách chọn sản phẩm phù hợp, giảm thời gian tư vấn của sales và có tiềm năng tăng tỷ lệ chuyển đổi. Đây là nhu cầu phổ biến trên hầu hết website thương mại điện tử. | Cần dữ liệu sản phẩm đầy đủ và được chuẩn hóa. Phạm vi tư vấn có thể mở rộng quá nhanh (tương thích, tồn kho, giá, khuyến mãi...), khiến MVP khó kiểm soát. |

## Problem Card #1 — Weekly Report

**Problem 1 câu:**  
Mỗi khi khách hỏi về thông số kỹ thuật, chính sách hoặc chương trình khuyến mãi, nhân viên CSKH phải mất 5–10 phút tra cứu từ nhiều nguồn trước khi có thể trả lời.

**Actor:**  
Nhân viên CSKH hoặc Sales Online.

**Thời điểm / bối cảnh:**  
Trong quá trình chat trực tiếp với khách trên website, Facebook, Zalo hoặc các sàn thương mại điện tử.

**Current workflow:**

```text
1. Đọc câu hỏi của khách
2. Xác định khách đang hỏi về sản phẩm nào
3. Tra cứu catalogue hoặc trang sản phẩm
4. Tra cứu chính sách (bảo hành, vận chuyển, đổi trả...)
5. Kiểm tra chương trình khuyến mãi nếu có
6. Soạn câu trả lời
7. Gửi khách
```

**Bottleneck:**  
Bước 3–5: phải tra cứu nhiều tài liệu khác nhau, đặc biệt khi sản phẩm có nhiều phiên bản hoặc chính sách thay đổi thường xuyên.

**Impact:**  
Khoảng 5–10 phút cho mỗi câu hỏi. Với hàng chục đến hàng trăm câu hỏi mỗi ngày, tổng thời gian dành cho việc tra cứu là rất lớn, đồng thời khách phải chờ lâu hơn.

**Success metric:**  
Giảm thời gian trả lời từ 5–10 phút xuống dưới 1 phút.
≥90% câu hỏi được trả lời ngay mà không cần tra cứu thủ công.
Không làm tăng tỷ lệ phản hồi sai.

**Non-AI alternative:**  
Xây dựng FAQ, tài liệu nội bộ hoặc cải thiện chức năng tìm kiếm, nhưng nhân viên vẫn phải tự đọc và tổng hợp thông tin.

**AI hypothesis:**  
AI tìm kiếm trong tài liệu sản phẩm và chính sách, sau đó sinh câu trả lời kèm nguồn tham chiếu để nhân viên kiểm tra trước khi gửi.

**Quick gut:**  
Workflow.

### Draft current workflow

```text
CURRENT STATE — 8 phút

[1 Đọc câu hỏi: 30s]
→ [2 Xác định sản phẩm: 1']
→ [3 Tra catalogue: 3']
→ [4 Tra chính sách: 2']
→ [5 Soạn trả lời: 1']
→ [6 Kiểm tra: 30s]
```

### Draft future workflow

```text
FUTURE STATE — 1.5 phút

[1 Đọc câu hỏi: 30s]
→ [2 AI tìm tài liệu: 10s]
→ [3 AI draft câu trả lời: 10s]
→ [4 CSKH review: 30s]
→ [5 Gửi khách: 10s]

Fallback: AI không tìm thấy thông tin → CSKH tra cứu thủ công.
```


# Problem Card #2 — Phân tích và tổng hợp đánh giá khách hàng

**Problem 1 câu:**
Quản lý sản phẩm phải đọc hàng trăm đánh giá của khách để tìm các vấn đề phổ biến, gây mất nhiều thời gian và dễ bỏ sót insight.

**Actor:**
Product Manager, Marketing hoặc Quản lý bán hàng.

**Thời điểm / bối cảnh:**
Sau mỗi chiến dịch bán hàng hoặc khi đánh giá hiệu quả sản phẩm.

**Current workflow:**

```text
1. Xuất danh sách đánh giá
2. Đọc từng review
3. Đánh dấu review tích cực/tiêu cực
4. Gom nhóm các vấn đề
5. Viết báo cáo tổng hợp
6. Đề xuất cải thiện
```

**Bottleneck:**
Bước 2–4: đọc và phân loại hàng trăm review hoàn toàn thủ công.

**Impact:**
30–60 phút cho mỗi sản phẩm hoặc mỗi đợt phân tích. Những vấn đề lặp lại có thể bị phát hiện chậm.

**Success metric:**

* Giảm thời gian phân tích xuống dưới 10 phút.
* AI phát hiện đúng các chủ đề chính trong phần lớn review.
* Báo cáo vẫn đủ thông tin để hỗ trợ ra quyết định.

**Non-AI alternative:**
Lọc review theo số sao hoặc từ khóa, nhưng vẫn cần đọc thủ công để hiểu nguyên nhân.

**AI hypothesis:**
AI tự động phân loại sentiment, gom nhóm chủ đề và sinh báo cáo tóm tắt kèm các review đại diện.

**Quick gut:**
AI reasoning.

### Draft current workflow

```text
CURRENT STATE — 45 phút

[1 Export review: 5']
→ [2 Đọc review: 25']  <-- bottleneck
→ [3 Gom nhóm: 10']
→ [4 Viết báo cáo: 5']
```

### Draft future workflow

```text
FUTURE STATE — 8 phút

[1 Export review: 2']
→ [2 AI phân loại + tóm tắt: 1']
→ [3 AI đề xuất insight: 1']
→ [4 PM review: 4']

Fallback: PM đọc lại các review quan trọng nếu cần.
```

---

# Problem Card #3 — AI tư vấn và so sánh sản phẩm

**Problem 1 câu:**
Khi khách chưa biết nên chọn sản phẩm nào, nhân viên Sales phải đọc catalogue và so sánh nhiều sản phẩm trước khi đưa ra tư vấn phù hợp.

**Actor:**
Nhân viên Sales Online.

**Thời điểm / bối cảnh:**
Trong quá trình tư vấn trước khi khách quyết định mua hàng.

**Current workflow:**

```text
1. Hỏi nhu cầu khách
2. Xác định nhóm sản phẩm
3. Tra cứu catalogue
4. So sánh thông số
5. Đề xuất sản phẩm
6. Giải thích ưu và nhược điểm
7. Trả lời các câu hỏi tiếp theo
```

**Bottleneck:**
Bước 3–5: mất thời gian đọc catalogue và đối chiếu nhiều sản phẩm có thông số tương tự.

**Impact:**
10–20 phút cho một lượt tư vấn. Thời gian phản hồi lâu có thể khiến khách rời đi trước khi nhận được tư vấn.

**Success metric:**

* Giảm thời gian tư vấn xuống dưới 5 phút.
* Tăng tỷ lệ khách nhận được gợi ý ngay trong lần trao đổi đầu tiên.
* Không làm tăng tỷ lệ tư vấn sai sản phẩm.

**Non-AI alternative:**
Tạo bảng so sánh hoặc bộ lọc sản phẩm, nhưng khách vẫn phải tự đọc và nhân viên vẫn phải giải thích.

**AI hypothesis:**
AI hiểu nhu cầu của khách, lọc sản phẩm phù hợp, sinh bảng so sánh và giải thích lý do đề xuất để Sales chỉ cần xác nhận trước khi gửi.

**Quick gut:**
Workflow + AI reasoning.

### Draft current workflow

```text
CURRENT STATE — 15 phút

[1 Hỏi nhu cầu: 2']
→ [2 Tra catalogue: 5']
→ [3 So sánh sản phẩm: 5']  <-- bottleneck
→ [4 Giải thích: 2']
→ [5 Chốt tư vấn: 1']
```

### Draft future workflow

```text
FUTURE STATE — 4 phút

[1 Thu thập nhu cầu: 1']
→ [2 AI lọc sản phẩm: 20s]
→ [3 AI sinh bảng so sánh: 20s]
→ [4 Sales review + chỉnh sửa: 2']
→ [5 Gửi khách: 20s]

Fallback: Nếu khách có yêu cầu đặc biệt hoặc AI không đủ dữ liệu, Sales quay lại quy trình tư vấn thủ công.
```
