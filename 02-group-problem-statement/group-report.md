# 02 — Group Problem Statement & Solution Framework

> **Bản nộp nhóm**  
> **Tên đề tài chốt:** Hệ thống AI Hỗ trợ Lập Kế hoạch & Tối ưu Lộ trình Học tập (Personalized Study Plan & Knowledge Gap Tracking)

---

## Thông tin nhóm

- **Danh sách thành viên (16 thành viên):**

| STT | Họ và tên         | Mã học viên | Vai trò trong nhóm |
| :-: | ----------------- | :---------: | ------------------ |
|  1  | Hồ Trung Tín      | 2A202601688 | Trưởng nhóm        |
|  2  | Nguyễn Huy Toàn   | 2A202601716 | Thành viên         |
|  3  | Hoàng Minh Quân   | 2A202601574 | Thành viên         |
|  4  | Đồng Phúc Lâm     | 2A202601902 | Thành viên         |
|  5  | Hoàng Bảo Huy     | 2A202601440 | Thành viên         |
|  6  | Nguyễn Xuân Hùng  | 2A202601640 | Thành viên         |
|  7  | Nguyễn Quốc Anh   | 2A202601100 | Thành viên         |
|  8  | Cáp Việt Anh      | 2A202601270 | Thành viên         |
|  9  | Trương Ái Linh    | 2A202601496 | Thành viên         |
| 10  | Nguyễn Mạnh Thắng | 2A202601944 | Thành viên         |
| 11  | Nguyễn Hải Yến    | 2A202601604 | Thành viên         |
| 12  | Phạm Thành Đạt    | 2A202601672 | Thành viên         |
| 13  | Lê Anh Quốc       | 2A202601740 | Thành viên         |
| 14  | Phạm Tuấn Anh     | 2A202601840 | Thành viên         |
| 15  | Nguyễn Duy Khương | 2A202601937 | Thành viên         |
| 16  | Bế Quốc Khánh     | 2A202601840 | Thành viên         |

---

## 1. Group Convergence (Nhật ký hội tụ)

Các thành viên đã tập hợp danh sách các bài toán từ 3 nguồn ý tưởng chính, thực hiện phân nhóm và gom trùng thành 3 cụm bài toán lớn:

| Cluster                                         | Candidate examples                                                     | Pattern chung                                                                                     |
| ----------------------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **A. Tối ưu học tập & Lên Kế hoạch Ôn thi**     | Học nhiều nhưng GPA thấp, ôn tập từ vựng, lab progress summary         | Gom thông tin từ nhiều nguồn rồi tự tổng hợp để kiểm tra lỗ hổng kiến thức và lập kế hoạch ôn tập |
| **B. Onboarding & Tư vấn Đời sống KĐT**         | Onboarding cư dân mới KĐT Vinhomes (chi phí, nội quy, VinBus, dịch vụ) | Lọc thông tin phân tán từ nhiều nguồn để lập cẩm nang/kế hoạch sinh hoạt cá nhân hóa              |
| **C. Onboarding Quy trình Nội bộ Doanh nghiệp** | Hướng dẫn thực tập sinh/nhân sự mới, giải đáp FAQ nội quy công ty      | Đọc tài liệu dài, trả lời các câu hỏi lặp đi lặp lại để tránh làm phiền/ngắt quãng quản lý        |

---

## 2. Shortlist và Scoring

Nhóm thực hiện chấm điểm từ 1–5 theo các tiêu chí bài lab cho 3 ứng viên đại diện từ 3 cụm bài toán:

| Candidate Problem                      | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain |   Tổng |
| -------------------------------------- | -------: | ----------: | ---------------: | -------------: | ------------: | -----------------: | ---------------: | -----: |
| **1. Kế hoạch & Tối ưu học tập (GPA)** |    **5** |       **5** |            **5** |          **5** |         **5** |              **5** |            **5** | **35** |
| 2. Onboarding Đời sống KĐT Vinhomes    |        4 |           5 |                4 |              4 |             4 |                  4 |                4 |     29 |
| 3. Onboarding Quy trình Doanh nghiệp   |        4 |           4 |                4 |              4 |             3 |                  4 |                4 |     27 |

- **Đề tài nhóm chọn:** **Hệ thống Lập Kế hoạch & Tối ưu Lộ trình Học tập (Giải bài toán Học nhiều nhưng GPA thấp)**.
- **Lý do chọn:**
  - **Domain hiểu rõ nhất:** 100% thành viên là sinh viên/học viên, trực tiếp trải qua cảm giác bị dồn bài sát kỳ thi (cramming) và học chưa tối ưu.
  - **Workflow & Metric rõ ràng:** Dễ dàng mô tả quy trình Trước/Sau, đo lường được chính xác số giờ chuẩn bị và tỉ lệ phủ lỗ hổng kiến thức.
  - **Tính khả thi trong bài Lab:** Phân định và so sánh rất rõ ràng giữa giải pháp Non-AI (Pomodoro, Notion), Rule-based, AI Workflow và Agent.
- **Lý do không chọn các đề tài khác:**
  - _Onboarding Vinhomes:_ Rất tiềm năng nhưng dữ liệu về bảng giá, dịch vụ biến động nhanh và mang tính địa phương caoy.
  - _Onboarding Doanh nghiệp:_ Phụ thuộc vào tài liệu nội bộ chuẩn và mô hình phân quyền RAG phức tạp hơn phạm vi bài lab.

---

## 3. Quick Validation (Kiểm chứng nhanh)

Nhóm đã tiến hành phỏng vấn nhanh các thành viên trong nhóm:

| Nguồn               | Số lượng | Tín hiệu xác nhận                                                                                                    | Tín hiệu phản bác                                          | Nhóm chỉnh sửa Problem                                                                                      |
| ------------------- | -------: | -------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Quick Interview** |  3 người | 3/3 thành viên xác nhận mất 40–60h/tuần tự học nhưng học dàn trải, thiếu bài test nhận biết gap kiến thức trước thi. | 1 người quen học nhóm tự do, không thích gò bó theo app.   | Thu hẹp problem: Không thay đổi thói quen tự học, chỉ tập trung tự động hóa bước "Check Gap & Lập Lịch Ôn". |
| **Mini Poll**       |  8 người | 6/8 bị dồn bài (cramming) sát ngày thi do không phân bổ được lịch học theo từng concept.                             | 2 người có study plan tĩnh trên Google Calendar từ đầu kỳ. | Bổ sung phương án Non-AI thay thế: Template Google Calendar / Phương pháp Pomodoro.                         |

> **Key Insight sau Validation:** Pain point thực sự không nằm ở việc "thiếu tài liệu", mà nằm ở khâu **không biết mình đang yếu concept nào (Gap kiến thức)** và **tốn quá nhiều công sức để tự phân bổ lịch ôn tập cho đúng tiến độ**.

---

## 4. Research Giải pháp hiện có

| Nguồn / Tool   | Link                      | Giải quyết phần nào?                  | Điểm mạnh                         | Khoảng trống / Rủi ro                                             | Bài học cho nhóm                                                                         |
| -------------- | ------------------------- | ------------------------------------- | --------------------------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| **Anki**       | https://apps.ankiweb.net/ | Ôn tập ngắt quãng (Spaced Repetition) | Thuật toán ôn tập tối ưu tốt      | Phải tự gõ tạo flashcard thủ công rất tốn thời gian               | Tận dụng thuật toán Spaced Repetition nhưng dùng AI để auto-generate flashcard từ slide. |
| **Quizlet**    | https://quizlet.com/      | Tạo quiz & flashcard                  | Kho đề cộng đồng lớn, dễ dùng     | Đề chung chung, không bám sát trọng tâm slide/giảng viên trên lớp | AI phải đọc trực tiếp Slide/Docs môn học của sinh viên.                                  |
| **NotebookLM** | https://notebooklm.google | Tóm tắt & Hỏi đáp trên tài liệu       | Phản hồi bám sát context tài liệu | Thiếu hệ thống quản lý lịch trình và đo lường lộ trình ôn tập     | Dùng AI làm khâu trích xuất gap/tạo câu hỏi, không dùng như chatbot thả nổi.             |

> **Research Takeaway:** Giải pháp tối ưu không phải là một Chatbot tư vấn tự do, mà là một **AI Workflow**: _Phân tích Slide/Bài giảng $\rightarrow$ Phát hiện Gap kiến thức $\rightarrow$ AI Draft Lịch trình & Flashcards $\rightarrow$ Sinh viên review & làm chủ lộ trình học_.

---

## 5. Detailed Workflow Before & After

### Current Workflow (Trước khi có AI) — **Tổng thời gian: ~180 phút/tuần cho khâu chuẩn bị**

```text
[1. Gom Slide, Note, Video bài giảng: 30']
  └─► [2. Đọc lướt tổng hợp kiến thức: 60']
        └─► [3. Tự soạn Flashcard / Câu hỏi kiểm tra thủ công: 60']  <-- BOTTLENECK
              └─► [4. Lên lịch ôn tập thủ công trên Calendar: 20']
                    └─► [5. Ôn tập & Phát hiện học lệch khi làm đề thi thử: 10']
```

### Future Workflow (Sau khi tối ưu bằng AI) — **Tổng thời gian: ~18 phút/tuần**

```text
[1. Upload Slide/Docs vào hệ thống: 2']
  └─► [2. AI trích xuất Key Concept & Tạo Diagnostic Quiz: 3']
        └─► [3. Sinh viên làm Quiz 5 phút để AI phát hiện Gap: 5']
              └─► [4. AI Draft "Lịch ôn & Bộ Flashcard cá nhân hóa": 3']
                    └─► [5. Sinh viên Review, Edit & Chốt kế hoạch: 5']  <-- HUMAN BOUNDARY
```

- **Fallback Strategy:** Nếu AI trích xuất sai trọng tâm slide hoặc tạo câu hỏi thiếu chính xác, sinh viên bấm "Regenerate theo chương X" hoặc tự chỉnh sửa trực tiếp câu hỏi trên giao diện.

### Impact So Sánh (Before vs After)

| Metric                         | Trước (Current)                  | Sau (Future Target)                          | Ghi chú                                       |
| ------------------------------ | -------------------------------- | -------------------------------------------- | --------------------------------------------- |
| **Thời gian chuẩn bị ôn tập**  | 180 phút/tuần                    | ~18 phút/tuần                                | Giảm 90% thời gian tạo công cụ học            |
| **Số bước thủ công**           | 5/5 bước                         | 2/5 bước (Làm Diagnostic Quiz + Review plan) | AI tự động hóa khâu đọc & trích xuất          |
| **Độ phủ kiến thức yếu (Gap)** | Bị động, chỉ biết khi làm đề thi | Chủ động phát hiện ngay ở tuần học           | Tránh tình trạng cramming dồn bài sát giờ thi |

---

## 6. Problem Statement v0 & v1

### Problem Statement v0 (Bản phác thảo ban đầu)

- **Actor:** Sinh viên đại học / Học viên khóa học ngắn hạn.
- **Workflow:** Đọc slide $\rightarrow$ Tóm tắt $\rightarrow$ Tự soạn câu hỏi $\rightarrow$ Lên lịch ôn tập $\rightarrow$ Ôn thi.
- **Bottleneck:** Tốn quá nhiều thời gian tự tạo Flashcard và không biết mình đang hổng kiến thức ở phần nào.
- **Impact:** Mất 3–4 tiếng/tuần chuẩn bị; học nhiều nhưng kết quả GPA không cao do bị dồn bài cuối kỳ.
- **Success Metric:** Giảm thời gian chuẩn bị công cụ ôn tập xuống dưới 30 phút/tuần.
- **Boundary:** Không làm bài thay sinh viên, không tự ý thay đổi lịch học mà chưa qua xác nhận.

### Problem Statement v1 (Bản chuẩn hóa chi tiết)

| Field                       | Nội dung chi tiết                                                                                                                                                                            |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actor**                   | Sinh viên / Học viên cần tối ưu hiệu suất học tập và phân bổ thời gian ôn thi hợp lý.                                                                                                        |
| **Workflow**                | Upload tài liệu môn học $\rightarrow$ AI phân tích concept $\rightarrow$ Làm Diagnostic Quiz kiểm tra gap $\rightarrow$ AI tạo Study Plan & Flashcards $\rightarrow$ Sinh viên Review & Học. |
| **Bottleneck**              | Khâu đọc trích xuất lý thuyết và gõ thủ công bộ câu hỏi ôn tập (mất 120 phút/tuần) làm gián đoạn thời gian tư duy thực tế.                                                                   |
| **Impact**                  | Tốn 15–20 giờ/tháng cho việc chuẩn bị học; học lệch trọng tâm dẫn đến tâm lý hoảng loạn/cramming trước ngày thi.                                                                             |
| **Success Metric**          | - Giảm thời gian tạo công cụ ôn tập từ 180 phút xuống < 20 phút/tuần.<br>- Phủ 100% các khái niệm trọng tâm trong slide môn học.                                                             |
| **Boundary**                | - AI KHÔNG làm bài tập/đồ án thay sinh viên.<br>- AI KHÔNG tự động chốt lịch ôn nếu sinh viên chưa bấm Approve.<br>- AI phải dẫn nguồn (trích dẫn slide/trang) cho mọi câu hỏi ôn tập.       |
| **AI Intervention Point**   | Giai đoạn trích xuất Key Concepts từ Slide và giai đoạn tự động hóa việc biến Key Concepts thành Diagnostic Quiz & Flashcards.                                                               |
| **Mức chọn**                | AI Workflow (Rule-based cho thuật toán Spaced Repetition + AI cho xử lý ngôn ngữ/trích xuất tài liệu).                                                                                       |
| **Rủi ro & Người kiểm tra** | **Rủi ro:** AI sinh câu hỏi sai lệch hoặc ảo giác (hallucination) nội dung slide.<br>**Người kiểm tra:** Sinh viên trực tiếp review, chỉnh sửa câu hỏi/lịch trình trước khi bấm Chốt.        |

---

## 7. Đánh giá Ma trận Độ phù hợp AI & Lựa chọn (Rule / Workflow / Agent)

### So sánh các Phương án

| Mức          | Phương án thực hiện                                                                                                                                                    | Khi nào đủ?                                                                                    | Rủi ro                                                                   | Lựa chọn?                                                                  |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------------- |
| **Rule**     | Dùng Google Calendar + Template Notion/Excel cố định.                                                                                                                  | Đủ nếu sinh viên tự giác và có sẵn kho đề chuẩn.                                               | Mất thời gian nhập liệu thủ công 100%, không tự phát hiện gap kiến thức. | Không chọn làm toàn bộ (Chỉ dùng Rule cho thuật toán nhắc lịch).           |
| **Workflow** | Upload Slide $\rightarrow$ AI Extract Key Terms $\rightarrow$ AI Draft Quiz $\rightarrow$ User test gap $\rightarrow$ System Map Study Plan $\rightarrow$ User Review. | Hợp lý vì quy trình từng bước rõ ràng, AI hỗ trợ xử lý tài liệu, con người làm chủ quyết định. | AI có thể draft câu hỏi chưa sát; cần khâu review của sinh viên.         | **CHỌN** (Tối ưu nhất cho bài lab)                                         |
| **Agent**    | AI Agent tự truy cập LMS, tự làm bài tập, tự sắp xếp lại toàn bộ lịch sống của sinh viên.                                                                              | Chỉ cần khi hệ thống tự động hoàn toàn không cần con người can thiệp.                          | Rủi ro bảo mật dữ liệu, chi phí cao, dễ mất kiểm soát hành vi agent.     | Không chọn (Quá rộng và vi phạm nguyên tắc "AI hỗ trợ, người quyết định"). |

> **Lý do chọn Workflow:** Đáp ứng đúng nguyên tắc Problem First, quy trình tuyến tính rõ ràng, kiểm soát được rủi ro hallucination thông qua khâu Human Review.

---

## 8. Final Decision (Quyết định cuối cùng của Nhóm)

| Tiêu chí tự kiểm                                   | Trạng thái (Yes / Not Yet / No) | Ghi chú chi tiết                                              |
| -------------------------------------------------- | :-----------------------------: | ------------------------------------------------------------- |
| **Actor và Workflow đã rõ ràng chưa?**             |               Yes               | Actor là sinh viên/học viên; Workflow 5 bước chi tiết.        |
| **Baseline và Success Metric đo lường được chưa?** |               Yes               | Baseline: 180 phút $\rightarrow$ Target: < 20 phút/tuần.      |
| **Có đủ dữ liệu / Input sử dụng chưa?**            |               Yes               | Slide bài giảng, file PDF/Docs môn học.                       |
| **Hậu quả nếu AI sai có chấp nhận được không?**    |               Yes               | Sinh viên có thể chỉnh sửa/xóa câu hỏi sai trong bước Review. |
| **Có người thật (Human Owner) kiểm tra không?**    |               Yes               | Sinh viên là người trực tiếp review và Approve lộ trình.      |
| **Có phương án Non-AI đơn giản hơn không?**        |               Yes               | Đã so sánh với phương pháp Pomodoro + Notion Template.        |

- **Quyết định:** **GO** (Thực hiện dự án với scope nhỏ)

### Kế hoạch Pilot nhỏ nhất (MVP):

- **Thử nghiệm:** Trên 1 môn học cụ thể (ví dụ: Môn Kiến thức AI/Python).
- **Input:** 1 file Slide PDF bài giảng.
- **Output của AI:** Tạo ra 10 câu hỏi Diagnostic Quiz + 1 Lịch ôn tập 3 ngày.
- **Metric đánh giá:** Đo thời gian sinh viên review/sửa đổi và mức độ hài lòng về độ phủ kiến thức.
