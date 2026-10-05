# Chặng 4: Build

# 1. Thông tin cá nhân & Đội ngũ

| Thông tin | Nội dung |
|---|---|
| Mã học viên | 2A202602855 |
| Họ và tên | Đỗ Trọng Bình |
| Tên nhóm | ThreeWhites |
| Số thành viên | 3 |
| Thành viên 1 | Đào Trọng Khang — MHV: 2A202602974 |
| Thành viên 2 | Nguyễn Tiến Phát — MHV: 2A202602387 |
| Thành viên 3 | Đỗ Trọng Bình — MHV: 2A202602855 |
| Case đã chọn | Case A — AI Tutor: Diagnostic Refresher |

# 2. Hypothesis Problem

Khi đang học (trên lớp hoặc trực tuyến) và gặp phần chưa hiểu trong lúc bài giảng vẫn tiếp tục, học viên gặp khó khăn trong việc làm rõ phần đó ngay trong ngữ cảnh bài học vì phải rời luồng bài sang công cụ bên ngoài (chụp màn hình, chuyển tab, tự mô tả lại ngữ cảnh) hoặc ghi lại để xem sau. Quá trình này làm mất thêm thời gian và trì hoãn việc làm rõ, khiến những kiến thức chưa hiểu dần tích tụ, tạo thành các lỗ hổng kiến thức và lâu dài làm chậm tiến độ học các bài tiếp theo.

# 3. Three Solution Options

Ba phương án cùng giải quyết tình huống người học chưa hiểu nội dung slide và cần được làm rõ ngay trong luồng học. Nhóm sử dụng slide Double Diamond “Evidence về problem không phải evidence về solution” làm bối cảnh chung. Các phương án khác nhau ở thời điểm hỗ trợ, cách xác định phần chưa hiểu và quyền quyết định của người học.

## Option A — Giải thích thuật ngữ ngay trên slide

**Người phụ trách:** Nguyễn Tiến Phát — MHV: 2A202602387  
**Prototype:** [prototype_phat — Option A](prototypes/prototype_phat/prototype/option-a.html)

- **Cơ chế và luồng tương tác:** Người học hover vào thuật ngữ trên slide để thấy dấu hiệu tương tác, sau đó bấm vào thuật ngữ. Một pop-up xuất hiện cạnh phần vừa chọn, hiển thị nội dung giải thích tương ứng. Người học đọc, đóng pop-up hoặc bấm thuật ngữ khác rồi tiếp tục học.
- **Vai trò Người–AI:** Người học chủ động quyết định khi nào cần hỗ trợ và thuật ngữ nào cần làm rõ. Vai trò AI được mô phỏng bằng việc cung cấp lời giải thích theo thuật ngữ đã bấm; hệ thống không tự chen vào luồng học.
- **Quyền kiểm soát:** Có thể đóng pop-up bằng nút đóng, phím Escape hoặc bấm ra ngoài; chọn thuật ngữ khác để đổi nội dung giải thích. Bản hiện tại không có luồng nhập câu hỏi tự do hay chỉnh sửa yêu cầu trong pop-up.
- **Lợi ích kỳ vọng và đánh đổi:** Ít thao tác, giải thích gần nội dung gốc, phù hợp với nhu cầu tra cứu nhanh. Đổi lại, người học chỉ hỏi được qua các thuật ngữ đã gắn tương tác, chưa chọn tùy ý một vùng ảnh, bảng hoặc đặt câu hỏi chuyên sâu.

## Option B — Kiểm tra mức độ hiểu và hỗ trợ chủ động (Guided Check)

**Người phụ trách:** Đào Trọng Khang — MHV: 2A202602974  
**Prototype:** [prototype_khang — Option B3](prototypes/prototype_khang.html)

- **Cơ chế và luồng tương tác:** Sau khi người học bắt đầu và ở lại slide Double Diamond đủ thời gian, hệ thống tự mở hộp thoại hỏi đã hiểu slide chưa. Người học chọn “Tôi đã hiểu, tiếp tục” hoặc chọn một trong ba khó khăn: hai viên kim cương, mối liên hệ giữa bốn giai đoạn, hay Divergence/Convergence. Với lựa chọn chưa hiểu, hệ thống hiển thị giải thích chung, ví dụ, ý chính và phần trả lời theo khó khăn đã chọn.
- **Vai trò Người–AI:** Hệ thống chủ động xác định thời điểm hỏi từ tín hiệu thời gian ở lại slide. Người học xác nhận mức độ hiểu và chọn vấn đề cần làm rõ; thời gian ở lại không được coi là kết luận chắc chắn rằng họ chưa hiểu.
- **Quyền kiểm soát:** Người học có thể xác nhận đã hiểu, chọn khó khăn, tiếp tục sang slide sau hoặc quay lại trang bắt đầu. Sau lời giải thích, nút **Đã hiểu / Chưa hiểu** cho phép quay về slide hoặc mở lại câu hỏi kiểm tra. Bản hiện tại chưa có ô nhập câu hỏi tự do.
- **Lợi ích kỳ vọng và đánh đổi:** Có thể hỗ trợ người học chưa chủ động hỏi và giảm công sức mô tả khó khăn. Đổi lại, câu hỏi tự xuất hiện có thể ngắt luồng đọc; tín hiệu thời gian có thể không phản ánh đúng nhu cầu và các lựa chọn có sẵn chưa bao quát mọi thắc mắc.

**Chi tiết cần đồng bộ trong prototype:** Mã hiện kích hoạt hộp thoại sau khoảng **8 giây**, trong khi thông báo trên giao diện nói **hơn 15 giây**. Đây là cơ chế mô phỏng bằng bộ đếm thời gian, chưa phải AI chẩn đoán khó khăn thực tế.

## Option C — Giải thích phần nội dung do người học khoanh chọn (C2)

**Người phụ trách:** Đỗ Trọng Bình — MHV: 2A202602855  
**Prototype dùng kiểm thử:** [prototype_binh — C2](prototypes/prototype_binh/prototype-c2-region.html)

- **Cơ chế và luồng tương tác:** Người học kéo chuột khoanh vùng sơ đồ cần làm rõ hoặc dùng nút chọn vùng nhanh. Panel trợ lý hiển thị ảnh preview để kiểm tra phần đã chọn. Người học có thể để trống câu hỏi để nhận giải thích chung, hoặc nhập thêm yêu cầu như hỏi ví dụ, hỏi sâu về một giai đoạn rồi gửi yêu cầu giải thích.
- **Vai trò Người–AI:** Người học quyết định thời điểm hỏi, phạm vi nội dung và trọng tâm câu hỏi. Vai trò AI là giải thích theo phần được chọn và ngữ cảnh bài học; trong prototype, phản hồi này được mô phỏng bằng nội dung dựng sẵn.
- **Quyền kiểm soát:** Có các thao tác **Chọn lại**, **Giải thích lại**, **Sửa yêu cầu**, **Đổi phần chọn**, **Hủy kết quả** và **Đối chiếu sơ đồ và Chosen opportunity**. Người học quyết định tiếp tục bài học khi đã hiểu.
- **Lợi ích kỳ vọng và đánh đổi:** Hướng tới việc hỏi đúng phần đang vướng, kể cả nội dung trực quan, đồng thời cho phép điều chỉnh câu hỏi. Đổi lại, người học phải tự khoanh đúng vùng và đọc nhiều lựa chọn hơn. Phiên thử với Duyên phát hiện hạn chế không chọn được hết phần ảnh mong muốn, cần sửa và kiểm thử lại.

**Phạm vi C2 hiện tại:** Chọn ảnh được mô phỏng bằng cách cắt vùng từ SVG của sơ đồ; chưa chụp toàn bộ slide, chưa OCR hay phân tích ảnh thật. C1 (chọn văn bản) và C3 (chọn khối) là các biến thể khác của Option C, không phải Option A và B của nhóm.

# 4. Đóng góp cụ thể của tôi trong sản phẩm nhóm:

- **Dựng Option C:** Tôi chịu trách nhiệm chính xây dựng prototype Option C — giải thích nội dung do người học lựa chọn. Bản C2 được sử dụng trong phiên kiểm thử, cho phép người học khoanh vùng nội dung trên slide, nhập thêm câu hỏi khi cần và yêu cầu AI giải thích.
- **Xây dựng bối cảnh chung:** Tôi cùng các thành viên thảo luận để thống nhất bối cảnh người học gặp phần chưa hiểu khi học slide, xây dựng Hypothesis Problem và đề xuất ba phương án A/B/C để giải quyết vấn đề.
- **Tham gia Human–AI Decision Table:** Ban đầu, mỗi thành viên tự điền phần tương ứng với option mình phụ trách; tôi điền phần Option C. Sau đó, cả nhóm trao đổi, góp ý và chỉnh sửa phần của nhau để hoàn thiện bảng chung.
- **Hỗ trợ đồng đội:** Tôi tham gia trao đổi ý tưởng, góp ý cho phần Human–AI Decision Table của Phát và Khang, đồng thời tiếp nhận góp ý của hai bạn để chỉnh sửa phần Option C của mình.

# 5. Dữ liệu kiểm thử & Bài học:

# 6. AI Support Log

- **Công cụ AI sử dụng:** ChatGPT/Codex để hỗ trợ sinh code giao diện prototype, gợi ý một số option và ý tưởng, đồng thời trau chuốt câu văn trong tài liệu.
- **Khâu AI hỗ trợ hiệu quả:** Tạo bản prototype nhanh hơn, bổ sung ý tưởng để thảo luận và giúp diễn đạt nội dung rõ ràng hơn.
- **Phần tôi tự chỉnh sửa:** Tôi rà soát các gợi ý, sửa những câu diễn đạt chưa đúng ý và điều chỉnh nội dung theo bối cảnh, phương án mà tôi và nhóm đã chọn. Các đầu ra của AI được xem là bản nháp để tôi kiểm tra và chỉnh sửa trước khi sử dụng.
