# Prototype Feedback Note — Day 19 · Chặng 6

**Họ tên người phỏng vấn:** Đỗ Trọng Bình · **Mã học viên:** 2A202602855  
**Tester:** Duyên · Người dùng bên ngoài nhóm  
**Bối cảnh kiểm thử:** Học slide bài giảng nhưng chưa hiểu một số nội dung trong bài, thao tác hệ thống để xem các cách giải quyết giúp người học hiểu ngay được nội dung đó để tiếp tục theo dõi bài giảng.

Đây là bản ghi cá nhân cho phiên kiểm thử do Đỗ Trọng Bình điều phối, trong đó Duyên trải nghiệm đủ ba phương án A/B/C. Nội dung được tổng hợp từ ghi nhớ của người phỏng vấn; các phản hồi của tester dưới đây là diễn ý, không phải trích dẫn nguyên văn.

## 1. Bối cảnh và phạm vi phiên kiểm thử

**Câu hỏi xác thực bối cảnh đã đặt:** “Trong vòng 7 ngày gần đây bạn có từng gặp khó khăn học slide bài giảng mà không hiểu được ngay không?”

Chưa ghi nhận câu trả lời cụ thể của Duyên cho câu hỏi này, cũng như nghề nghiệp hoặc tình huống học tập gần đây của tester. Nhiệm vụ mẫu được giao, thứ tự trải nghiệm và thời lượng thực tế của từng phương án chưa được ghi lại trong thông tin tổng hợp.

| Phương án | Prototype được thử | Cơ chế hỗ trợ |
|---|---|---|
| **Option A — Phát** | [prototype_phat](prototypes/prototype_phat/prototype/option-a.html) | Người học bấm vào phần chữ có tương tác trên slide để mở nội dung hỗ trợ. |
| **Option B — Khang** | [prototype_khang](prototypes/prototype_khang.html) | Hệ thống chủ động hiển thị câu hỏi; người học tương tác sau khi câu hỏi xuất hiện. |
| **Option C — Bình, biến thể C2** | [prototype-c2-region.html](prototypes/prototype_binh/prototype-c2-region.html) | Người học kéo chuột khoanh vùng nội dung chưa hiểu, có thể nhập thêm câu hỏi rồi yêu cầu AI giải thích. |

**Lưu ý phạm vi:** C2 là biến thể của Option C được sử dụng trong phiên này. Ba phương án so sánh là bản của Phát, Khang và Bình; không phải ba biến thể C1/C2/C3.

## 2. Ghi nhận phản hồi cá nhân

| Tiêu điểm quan sát hành vi | Ghi chép chi tiết hành vi thực tế (Fact-First) |
|---|---|
| **First Action — Hành động đầu tiên** | Ở cả ba bản, Duyên đều đưa chuột vào slide trước. **A:** Khi hover vào phần chữ và thấy nội dung tương tác hiển thị, tester bấm vào phần chữ đó. **C2:** Tester thấy con trỏ chuyển thành dấu “+” và nhận biết thao tác kéo để chọn vùng chụp. **B:** Tester bấm vào slide nhưng không thấy phản ứng, sau đó chờ hệ thống hiển thị câu hỏi. |
| **Hesitation — Điểm do dự hoặc hiểu sai** | **A:** Người phỏng vấn không ghi nhận thắc mắc đáng kể; tester sử dụng thao tác bấm vào chữ để mở nội dung. **C2:** Sau khi yêu cầu AI giải thích, tester dừng lại đọc các lựa chọn; không ghi nhận bấm nhầm hoặc hỏi lại. **B:** Lần bấm ban đầu vào slide không tạo phản ứng; tester chỉ tiếp tục bấm sau khi câu hỏi hiển thị. |
| **Evidence Checking — Minh chứng được đọc hay bỏ qua** | **Chưa ghi nhận** tester có đối chiếu lời giải thích với slide, đọc cảnh báo hay kiểm tra nguồn hay không. C2 có nút **Đối chiếu sơ đồ và Chosen opportunity** và thông báo dùng câu trả lời dựng sẵn, nhưng sự hiện diện của các thành phần này không chứng minh tester đã đọc hoặc sử dụng. |
| **Control & Recovery — Sửa sai hoặc lấy lại quyền kiểm soát** | Theo ghi nhận của người phỏng vấn, C2 có khả năng sửa yêu cầu hoặc đặt câu hỏi khác, còn hai bản kia không có khả năng tương ứng trong lượt thử. |
| **Selected Option — Phương án được lựa chọn** | **Option C — bản C2 của Bình.** |
| **Trade-offs — Lý do chọn và đánh đổi chấp nhận** | Theo phản hồi được người phỏng vấn thuật lại, Duyên chọn C2 vì muốn khoanh đúng phần cần hỏi, bao gồm nội dung dạng ảnh hoặc bảng; có thể hỏi sâu hoặc chỉ yêu cầu ví dụ. Tester chấp nhận phải tự thao tác chụp đúng vùng vì đó cũng là phần mình muốn tập trung làm rõ. Tester muốn tự chọn vùng và nhập câu hỏi chi tiết khi cần, giao AI việc tìm ngữ cảnh và giải thích cụ thể. |
| **Counter-evidence — Dữ kiện đi ngược kỳ vọng** | Việc Duyên chọn C2 phù hợp với kỳ vọng ban đầu của Bình. Tuy nhiên, tester phát hiện hạn chế khi không thể chụp hết phần ảnh trên slide; điều này đi ngược kỳ vọng rằng thao tác chọn vùng đã thuận tiện và hoàn chỉnh. Việc tester dừng đọc các lựa chọn cũng cho thấy vẫn cần xem xét độ rõ ràng của giao diện, dù không ghi nhận bấm nhầm hay hỏi lại. |

## 3. Bóc tách 4 tầng tư duy

### 1. OBSERVED — Quan sát khách quan

- Duyên đưa chuột vào slide ở cả ba bản. Với A, tester bấm vào phần chữ sau khi thấy tương tác khi hover. Với B, tester bấm slide nhưng không thấy phản ứng, rồi tương tác sau khi câu hỏi xuất hiện.
- Với C2, tester nhận biết thao tác chọn vùng qua con trỏ dấu “+”; sau khi yêu cầu giải thích, tester dừng đọc các lựa chọn. Không ghi nhận bấm nhầm hoặc hỏi lại ở C2.
- Duyên chọn C2. Theo lời kể của người phỏng vấn, tester muốn tự chọn phần cần hỏi, nhập câu hỏi khi cần và giao AI tìm ngữ cảnh, giải thích.
- Tester phát hiện vấn đề không thể chụp hết phần ảnh trên slide. Chưa ghi lại vùng ảnh cụ thể, kích thước cửa sổ hoặc các bước tái hiện lỗi.
- Chưa có ghi nhận về thao tác đối chiếu minh chứng hoặc nút sửa yêu cầu mà tester thực tế sử dụng. Không có câu nói nguyên văn của tester được lưu trong bản tổng hợp này.

### 2. INTERPRETED — Diễn giải của người làm sản phẩm

- Lựa chọn C2 gợi ý rằng Duyên coi trọng khả năng chủ động xác định phạm vi câu hỏi. Với tester này, thao tác chọn vùng có thể mang lại cảm giác kiểm soát và tập trung, nên họ chấp nhận thêm thao tác.
- Con trỏ dấu “+” có thể giúp gợi đúng hành động kéo chọn vùng. Việc dừng đọc các lựa chọn có thể là bước cân nhắc bình thường hoặc cho thấy giao diện cần nhiều thời gian đọc hơn; chưa đủ dữ liệu để khẳng định tester bị quá tải.
- Lần bấm slide không có phản ứng ở B có thể phản ánh kỳ vọng được chủ động yêu cầu hỗ trợ, trong khi bản này chờ hệ thống đưa ra câu hỏi.
- Bình nhận định hạn chế chọn ảnh xuất phát từ mã prototype chưa hoàn thiện. Đây là nhận định sau phiên thử; nguyên nhân kỹ thuật cụ thể cần được tái hiện và kiểm tra.
- Kết quả ủng hộ kỳ vọng về sự hấp dẫn của C2 đối với Duyên, nhưng lựa chọn ưu tiên chưa chứng minh hiệu quả học tập cao khi triển khai thực tế.

### 3. DECIDED — NEXT CHANGE

**Ưu tiên vòng tiếp theo: sửa và kiểm thử phạm vi chọn ảnh của C2, bổ sung bôi đen text từ C1.** Đây là quyết định của người làm sản phẩm dựa trên lỗi tester phát hiện.

1. Tái hiện tình huống không thể chụp hết ảnh; kiểm tra giới hạn vùng kéo, tọa độ vùng chọn và ảnh preview. Điều chỉnh để người học chọn được toàn bộ phần ảnh mong muốn trên slide, thay vì bị giới hạn ngoài ý muốn.
2. Kiểm tra lại các trường hợp kéo ở mép ảnh, chọn toàn ảnh và đổi kích thước cửa sổ. Xác nhận ảnh preview khớp phần đã khoanh trước khi yêu cầu giải thích.
3. Giữ cơ chế người học tự chọn vùng và tùy chọn nhập câu hỏi. Giữ khả năng hỏi ví dụ, hỏi sâu, **Sửa yêu cầu** và **Đổi phần chọn** vì phù hợp với mong muốn kiểm soát mà tester nêu.
4. Ở lượt thử tiếp theo, quan sát cụ thể tester có dùng **Sửa yêu cầu**, **Đổi phần chọn** và **Đối chiếu sơ đồ và Chosen opportunity** không; ghi lại thao tác thực tế để bổ sung dữ liệu còn thiếu. Chưa có cơ sở loại bỏ A hoặc B chỉ từ phiên thử này.

### 4. STILL UNPROVEN — Điều vẫn chưa thể chứng minh

Các điểm sau vẫn chưa được kiểm chứng:

- C2 có được những người học khác ưu tiên hay không; chưa thể khái quát lựa chọn của Duyên cho toàn bộ người dùng.
- C2 có giúp hiểu bài tốt hơn, giảm gián đoạn hoặc tiết kiệm thời gian trong quá trình học thực tế hay không; chưa có đo lường hoặc theo dõi dài hạn.
- AI thật có tìm đúng ngữ cảnh và giải thích chính xác nội dung ảnh, bảng hay câu hỏi tự do hay không. Prototype hiện dùng phản hồi dựng sẵn, chưa phân tích ảnh thật.
- Tester có kiểm tra minh chứng và tự sửa yêu cầu thành công khi lời giải thích chưa phù hợp hay không; các hành vi này chưa được ghi nhận.
- Thay đổi mã nguồn có giải quyết được hạn chế chọn ảnh hay không; cần xác minh sau khi sửa và thử lại.
