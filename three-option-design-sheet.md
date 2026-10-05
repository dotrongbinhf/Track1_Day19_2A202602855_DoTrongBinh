# Three Option Design Sheet — Day 19

**Nhóm:** ThreeWhites  
**Case:** Case A — AI Tutor: Diagnostic Refresher

## 1. Bối cảnh chung và Hypothesis Problem

Khi đang học slide và gặp phần chưa hiểu trong lúc bài giảng vẫn tiếp tục, người học phải rời luồng bài để tìm công cụ giải thích bên ngoài hoặc ghi lại để xem sau. Việc chụp màn hình, chuyển tab và mô tả lại ngữ cảnh làm mất thời gian, trì hoãn việc làm rõ và có thể khiến kiến thức chưa hiểu tích tụ.

**Mục tiêu thiết kế:** Giúp người học làm rõ nội dung ngay trong ngữ cảnh bài học, đồng thời có quyền quyết định sử dụng hỗ trợ và tiếp tục học.

**Nội dung dùng chung:** Slide “Evidence về problem không phải evidence về solution”, sơ đồ Double Diamond và bốn giai đoạn Discover, Define, Develop, Deliver. Ba prototype đều có luồng chuyển sang hai slide tiếp theo.

**Nhiệm vụ mẫu đề xuất cho lượt kiểm thử tiếp theo:** Bạn chưa hiểu vì sao evidence về problem không phải evidence về solution. Hãy dùng hỗ trợ trên giao diện để làm rõ, đọc lời giải thích và quyết định có tiếp tục bài học hay cần hỗ trợ thêm. Dùng cùng nhiệm vụ cho A/B/C; đây không phải bản ghi nguyên văn nhiệm vụ đã giao trong phiên với Duyên.

## 2. Thiết kế ba option

### Option A — Giải thích thuật ngữ tại chỗ

**Phụ trách:** Nguyễn Tiến Phát — 2A202602387  
**Prototype:** [Mở Option A](prototypes/prototype_phat/prototype/option-a.html)

- **Bối cảnh:** Người học đang đọc slide; thuật ngữ có thể bấm được làm nổi bật khi hover.
- **Tương tác then chốt:** Người học bấm một thuật ngữ để mở pop-up giải thích cạnh nội dung vừa chọn. Hệ thống chọn phần giải thích tương ứng với thuật ngữ.
- **Kết quả và quyết định:** Người học đọc, đóng pop-up bằng nút đóng, Escape hoặc bấm ra ngoài; chọn thuật ngữ khác hoặc tiếp tục học.
- **Giả thuyết giá trị:** Tra cứu nhanh, ít thao tác, giữ lời giải thích gần nội dung gốc.
- **Đánh đổi:** Chỉ hỗ trợ các thuật ngữ đã gắn tương tác; không nhập câu hỏi tự do hoặc khoanh vùng ảnh tùy ý trong luồng này.

### Option B — Hỏi kiểm tra mức độ hiểu chủ động (Guided Check)

**Phụ trách:** Đào Trọng Khang — 2A202602974  
**Prototype:** [Mở Option B3](prototypes/prototype_khang.html)

- **Bối cảnh:** Người học bấm **Bắt đầu** và đọc slide Double Diamond. Hệ thống dùng thời gian ở lại slide làm tín hiệu để đề nghị hỗ trợ.
- **Tương tác then chốt:** Hộp thoại tự xuất hiện, hỏi người học đã hiểu chưa. Người học xác nhận đã hiểu hoặc chọn khó khăn về hai viên kim cương, bốn giai đoạn, hay Divergence/Convergence.
- **Kết quả và quyết định:** Nếu chọn khó khăn, hệ thống hiển thị giải thích, ví dụ, ý chính và phản hồi theo lựa chọn. Người học chọn **Đã hiểu / Chưa hiểu**, chuyển slide hoặc về trang bắt đầu.
- **Giả thuyết giá trị:** Hỗ trợ người học chưa chủ động hỏi và giảm công sức mô tả khó khăn.
- **Đánh đổi:** Có thể ngắt luồng đọc; thời gian ở lại chưa chứng minh người học gặp khó khăn; các lựa chọn có sẵn giới hạn phạm vi hỏi.

**Giới hạn hiện tại:** Bộ đếm trong mã mở hộp thoại sau khoảng 8 giây nhưng thông báo nói hơn 15 giây. Giao diện nói có thể đóng thông báo, song mã hiện chưa có nút đóng riêng; chọn “Tôi đã hiểu, tiếp tục” đưa về slide và khởi động lại bộ đếm. Các điểm này cần đồng bộ trong vòng sửa prototype.

### Option C — Giải thích nội dung do người học khoanh chọn (C2)

**Phụ trách:** Đỗ Trọng Bình — 2A202602855  
**Prototype dùng kiểm thử:** [Mở Option C2](prototypes/prototype_binh/prototype-c2-region.html)

- **Bối cảnh:** Slide và panel trợ lý hiển thị sẵn. Người học tự xác định phần chưa hiểu.
- **Tương tác then chốt:** Kéo chuột khoanh vùng sơ đồ hoặc dùng nút chọn vùng nhanh, kiểm tra ảnh preview rồi yêu cầu giải thích. Có thể nhập thêm câu hỏi để hỏi ví dụ hoặc làm rõ một trọng tâm.
- **Kết quả và quyết định:** Đọc giải thích, ví dụ và ý chính; dùng **Giải thích lại**, **Sửa yêu cầu**, **Đổi phần chọn**, **Hủy kết quả** hoặc **Đối chiếu sơ đồ và Chosen opportunity**. Người học quyết định tiếp tục bài học khi đã hiểu.
- **Giả thuyết giá trị:** Chủ động kiểm soát phạm vi nội dung và trọng tâm câu hỏi, hướng tới hỗ trợ cả nội dung trực quan.
- **Đánh đổi:** Cần khoanh đúng vùng và đọc nhiều lựa chọn hơn. Tester Duyên đã phát hiện hạn chế không chọn được hết phần ảnh mong muốn; cần sửa và thử lại.

**Giới hạn hiện tại:** C2 cắt vùng từ SVG của sơ đồ để mô phỏng chọn ảnh; chưa chụp toàn bộ slide, chưa OCR hoặc phân tích ảnh thật. C1 và C3 là biến thể khác của Option C, không thay thế A/B của nhóm.

## 3. Human–AI Decision Table

Bảng dưới tổng hợp cơ chế đang có trong ba prototype. “AI” chỉ vai trò hỗ trợ được mô phỏng; cả ba dùng nội dung dựng sẵn.

| Điểm quyết định | Option A — Phát | Option B — Khang | Option C2 — Bình |
|---|---|---|---|
| **Ai khởi phát hỗ trợ?** | Người học bấm thuật ngữ | Hệ thống mở câu hỏi theo bộ đếm thời gian | Người học chọn vùng và gửi yêu cầu |
| **Người học quyết định gì?** | Khi nào hỏi và thuật ngữ cần giải thích | Xác nhận mức độ hiểu và chọn khó khăn | Phạm vi nội dung, câu hỏi và lúc gửi |
| **AI/hệ thống đảm nhiệm gì?** | Chọn và hiển thị giải thích theo thuật ngữ | Đề nghị hỗ trợ, hiển thị giải thích theo lựa chọn | Hiển thị preview và phản hồi dựng sẵn theo trọng tâm yêu cầu |
| **Cơ sở/ngữ cảnh hỗ trợ** | Thuật ngữ và nội dung slide mẫu | Thời gian ở lại slide và lựa chọn người học | Vùng sơ đồ được chọn, câu hỏi tùy chọn và slide mẫu |
| **Nếu hỗ trợ chưa phù hợp?** | Đóng pop-up hoặc bấm thuật ngữ khác | Chọn Chưa hiểu để mở lại câu hỏi; không sửa câu hỏi tự do | Sửa yêu cầu, đổi phần chọn, giải thích lại hoặc hủy kết quả |
| **Ai quyết định tiếp tục?** | Người học chuyển slide | Người học chuyển slide | Người học chọn tiếp tục bài học |
| **Đánh đổi chính** | Nhanh nhưng giới hạn nội dung hỏi | Chủ động nhưng có thể gián đoạn | Kiểm soát chi tiết nhưng thêm thao tác |

Theo cách làm nhóm đã thống nhất, mỗi thành viên tự điền phần option phụ trách, sau đó cả nhóm góp ý và chỉnh sửa cho nhau. Bảng tổng hợp này cần được đọc cùng phạm vi thực tế của prototype, không xem khả năng mô phỏng là năng lực AI đã triển khai.

## 4. Những điểm cần quan sát khi so sánh

- Người học có tự nhận ra cách yêu cầu hỗ trợ ở từng option không?
- Lời giải thích có khớp phần người học muốn hỏi không, và họ có đối chiếu với slide không?
- Khi chưa hiểu hoặc hỗ trợ chưa phù hợp, người học có tìm được cách điều chỉnh không?
- Người học ưu tiên tra cứu nhanh (A), được hệ thống gợi hỏi (B), hay tự kiểm soát phạm vi câu hỏi (C2)? Họ chấp nhận đánh đổi gì?

Các câu hỏi trên là tiêu điểm cho kiểm thử, chưa phải kết luận về hiệu quả. Dữ liệu phiên do Bình điều phối được ghi riêng trong [Prototype Feedback Note](prototype-feedback-note.md).
