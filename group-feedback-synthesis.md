# Group Feedback Synthesis — Day 19 · Chặng 6

## 1. Phạm vi tổng hợp

Bản tổng hợp kết hợp kết quả từ ba phiên kiểm thử độc lập:

| Người thực hiện | Người trải nghiệm | Phương án được người trải nghiệm ưu tiên |
|---|---|---|
| Đào Trọng Khang | Linh | **Option B — Chẩn đoán khó khăn và hỗ trợ chủ động** |
| Đỗ Trọng Bình | Duyên | **Option C — Giải thích nội dung do người học lựa chọn**, biến thể C2 |
| Nguyễn Tiến Phát | Khuê | **Option C — Giải thích nội dung do người học lựa chọn**, bản của Bình |

Cả ba người trải nghiệm đều thử ba phương án A, B và C trong bối cảnh cần làm rõ phần kiến thức chưa hiểu khi đang học bằng slide. Nội dung dưới đây đã được gộp theo chủ đề và loại bỏ các nhận xét trùng lặp giữa các bản ghi.

**Kết quả lựa chọn:** Duyên và Khuê chọn bản của Bình, Linh chọn bản của Khang. Như vậy, **2/3 tester ưu tiên Option C**, là cơ sở để nhóm chọn C2 làm hướng phát triển tiếp theo.

Trong ghi chép của Phát, **O1 = Phát = Option A**, **O2 = Bình = Option C**, **O3 = Khang = Option B**. Các phản hồi được diễn ý từ ghi chép, không phải trích dẫn nguyên văn của tester.

## 2. Tổng hợp quan sát theo phương án

### Option A — Gợi ý mở rộng theo nhu cầu

**Tín hiệu tích cực**

- Thao tác bấm vào nội dung tương đối trực quan và không đòi hỏi nhiều thời gian làm quen.
- Linh nhanh chóng hiểu cách sử dụng; Duyên cũng nhận biết phần chữ có tương tác khi di chuột và thực hiện được thao tác mà không có thắc mắc đáng kể.
- Khuê thích tính năng của A, nhận xét bản này tiện và dễ sử dụng.

**Hạn chế**

- Một số nội dung lý thuyết được Linh nhận xét là chưa chính xác và cần được rà soát.
- Phương án phụ thuộc vào việc người học chủ động nhận ra và bấm vào đúng nội dung có thể tương tác.
- Khuê muốn so sánh hai phần lý thuyết nhưng chưa thực hiện được trong bản này; đồng thời muốn tra lý thuyết hoặc yêu cầu ví dụ theo ý muốn.

### Option B — Chẩn đoán khó khăn và hỗ trợ chủ động

**Tín hiệu tích cực**

- Linh đánh giá các câu hỏi dễ nắm bắt, phần ghi chú kiến thức quan trọng rõ ràng và ví dụ minh họa trực quan.
- Linh tích cực thao tác và có biểu hiện đồng tình trong quá trình trải nghiệm.
- Cơ chế hỏi theo lựa chọn giúp người học nhận hỗ trợ mà không cần tự viết đầy đủ câu hỏi hoặc xác định chính xác phần mình chưa hiểu ngay từ đầu.
- Khuê nhận xét cơ chế này hữu ích khi gặp lý thuyết chưa hiểu, nếu bỏ qua vấn đề gây gián đoạn.

**Hạn chế**

- Linh nhận thấy thông báo xuất hiện khá sớm, có nguy cơ làm gián đoạn khi người học vẫn đang đọc bài.
- Duyên từng bấm vào slide trước khi thông báo xuất hiện nhưng không nhận được phản hồi. Điều này cho thấy một số người học có thể mong đợi khả năng chủ động gọi hỗ trợ thay vì chỉ chờ hệ thống can thiệp.
- Prototype chưa cung cấp đủ dữ liệu để xác nhận câu hỏi chủ động có thực sự giúp người học hiểu hoặc ghi nhớ kiến thức tốt hơn.
- Khuê thấy thông báo gây phiền khi đang đọc nội dung và một số phần trong bản demo còn khó hiểu.

### Option C — Giải thích nội dung do người học lựa chọn

**Tín hiệu tích cực**

- Duyên ưu tiên C2 vì có thể tự khoanh đúng phần muốn hỏi, đặc biệt với hình ảnh hoặc bảng, đồng thời có thể nhập thêm yêu cầu để hỏi sâu hoặc xin ví dụ.
- Con trỏ dấu “+” giúp Duyên nhận biết thao tác kéo chọn vùng.
- Khuê chọn bản của Bình vì cho rằng cơ chế này khắc phục hạn chế của A về việc hỏi theo nhu cầu; Khuê đánh giá bản này khá trực quan và dễ dùng.
- Sau khi làm quen, Linh cũng đánh giá thao tác khoanh vùng ở mức có thể sử dụng được.

**Hạn chế**

- Linh gặp khó khăn ban đầu với thao tác kéo, thả và cho rằng việc phải tự nhập kiến thức muốn hỏi làm tăng công sức tương tác.
- Nội dung giải thích có xu hướng hiển thị toàn bộ thay vì chia nhỏ theo nhu cầu; tương tác chủ yếu dựa trên nút bấm.
- Duyên phát hiện vùng chọn không bao phủ được toàn bộ phần ảnh mong muốn, cho thấy giới hạn kỹ thuật của prototype C2.
- Khuê góp ý hoàn thiện phần LLM để bản demo trở thành công cụ hữu ích hơn. Đây là mong muốn cho phiên bản tiếp theo; phản hồi không chứng minh C2 hiện đã xử lý được mọi câu hỏi hoặc so sánh hai phần lý thuyết.

## 3. Những nhu cầu chung được rút ra

Sau khi loại bỏ các ý trùng lặp, ba phiên thử cho thấy năm nhu cầu chính:

1. **Hỗ trợ phải dễ tiếp cận:** Người học cần nhanh chóng hiểu cách bắt đầu mà không phải học nhiều thao tác mới.
2. **Người học cần quyền kiểm soát:** Hệ thống chủ động là hữu ích, nhưng người học cần được hoãn, đóng hoặc tự gọi hỗ trợ khi muốn.
3. **Nội dung phải đúng trọng tâm:** Câu hỏi ngắn, ghi chú quan trọng và ví dụ trực quan giúp người học dễ theo dõi; nội dung lý thuyết vẫn cần được kiểm tra độ chính xác.
4. **Can thiệp phải đúng thời điểm:** Thông báo quá sớm có thể gây gián đoạn, trong khi chờ hoàn toàn thụ động có thể không đáp ứng kỳ vọng của người muốn hỏi ngay.
5. **Câu hỏi cần linh hoạt:** Phản hồi của Khuê cho thấy nhu cầu so sánh các phần lý thuyết và yêu cầu ví dụ theo ý muốn, vượt ra ngoài các nội dung hoặc lựa chọn đã gắn sẵn.

## 4. Lựa chọn của nhóm

Nhóm lựa chọn **Option C — Giải thích nội dung do người học lựa chọn**, với **bản C2 của Đỗ Trọng Bình**, làm hướng phát triển tiếp theo.

Quyết định dựa trên ba cơ sở:

1. **Hai trong ba tester ưu tiên C:** Duyên và Khuê đều chọn bản của Bình. Duyên coi trọng việc tự chọn đúng phần muốn hỏi; Khuê coi trọng khả năng hỏi linh hoạt hơn bản A.
2. **Có tín hiệu tích cực về cách tương tác:** Duyên nhận biết cách kéo chọn qua con trỏ dấu “+”, còn Khuê đánh giá giao diện khá trực quan và dễ dùng. Cơ chế người học tự khởi phát hỗ trợ cũng phù hợp với nhu cầu tránh bị ngắt luồng đọc được ghi nhận ở B.
3. **Có hướng cải thiện cụ thể:** Sửa giới hạn vùng chọn, giảm công sức nhập câu hỏi, chia nhỏ lời giải thích và tích hợp LLM là các hướng phát triển có thể kiểm thử tiếp. Các hạn chế này cần được giải quyết trước khi đánh giá hiệu quả thực tế.

Linh vẫn ưu tiên B và gặp khó khăn ban đầu với thao tác kéo thả ở C. Nhóm giữ phản hồi này làm dữ kiện đối trọng để cải thiện khả năng làm quen và giảm thao tác của C2. Kết quả 2/3 là tín hiệu lựa chọn trong phạm vi ba phiên thử, chưa chứng minh C hiệu quả hơn A hoặc B với mọi người học.

## 5. DECIDED — Thay đổi tiếp theo cho Option C2

**Mục tiêu của vòng tiếp theo:** giữ quyền chủ động chọn nội dung của người học, làm thao tác khoanh vùng thuận tiện hơn và cung cấp lời giải thích đúng trọng tâm câu hỏi.

### Thay đổi ưu tiên

1. **Sửa phạm vi khoanh vùng và ảnh preview**
   - Tái hiện lỗi Duyên phát hiện: không chọn được hết phần ảnh mong muốn.
   - Kiểm tra giới hạn kéo chọn, tọa độ và preview để người học lấy đúng phần cần hỏi, kể cả vùng sát mép.
   - Kiểm thử lại với các kích thước cửa sổ và vùng chọn khác nhau trước khi coi lỗi đã được xử lý.

2. **Giảm công sức thao tác và nhập câu hỏi**
   - Làm rõ hướng dẫn kéo chọn; giữ các nút chọn vùng nhanh và thao tác Chọn lại.
   - Giữ câu hỏi là tùy chọn: chọn nội dung rồi gửi vẫn nhận được giải thích chung.
   - Thử thêm gợi ý ngắn như **Cho ví dụ**, **Giải thích đơn giản hơn** để người học không phải tự gõ mọi yêu cầu; vẫn giữ ô nhập tự do và Sửa yêu cầu.

3. **Chia nhỏ lời giải thích theo nhu cầu**
   - Hiển thị phần trả lời trực tiếp và ý chính trước; cho phép mở thêm ví dụ hoặc giải thích sâu.
   - Giữ cách diễn đạt dễ hiểu và ví dụ trực quan, tiếp thu điểm tích cực được ghi nhận ở B.
   - Giữ quyền đổi vùng chọn, sửa yêu cầu, đối chiếu slide và tiếp tục học theo quyết định của người dùng.

4. **Hoàn thiện phần LLM và thử nhu cầu so sánh lý thuyết**
   - Phát triển khả năng trả lời dựa trên nội dung được chọn và ngữ cảnh slide, thay cho phản hồi dựng sẵn.
   - Thử luồng chọn hoặc bổ sung phần nội dung thứ hai để hỏi so sánh, xuất phát từ nhu cầu Khuê nêu khi trải nghiệm A.
   - Kiểm tra độ đúng của lời giải thích, ví dụ và so sánh; khi thiếu ngữ cảnh, yêu cầu người học bổ sung thay vì trả lời chắc chắn.

Các mục trên là quyết định cho vòng tiếp theo, chưa phải các thay đổi đã triển khai hoặc kiểm chứng thành công.

## 6. Kế hoạch kiểm thử vòng tiếp theo

Phiên bản Option C2 sau khi chỉnh sửa sẽ được đánh giá bằng các tiêu chí sau:

- Người học có tự khoanh đúng vùng và nhận được preview khớp nội dung mong muốn không; ghi lại số lần phải chọn lại.
- Thời gian từ khi muốn hỏi đến khi gửi được yêu cầu, cùng những điểm dừng hoặc cần hướng dẫn.
- Người học có biết để trống câu hỏi, dùng gợi ý nhanh hoặc nhập yêu cầu riêng không.
- Người học có sửa yêu cầu, đổi vùng chọn và đối chiếu với slide khi kết quả chưa phù hợp không.
- Với luồng so sánh lý thuyết, người học có chọn đủ ngữ cảnh và nhận được câu trả lời đúng trọng tâm không.
- Nếu tích hợp LLM, kiểm tra độ chính xác của phản hồi trên nội dung chữ, sơ đồ và bảng trước khi kết luận về khả năng xử lý.
- Người học có trả lời đúng một câu hỏi kiến thức ngắn sau phần giải thích hay không.

## 7. Những điều vẫn chưa được chứng minh

- Ba phiên thử chưa đủ để khái quát lựa chọn cho toàn bộ người học.
- Chưa có số liệu chứng minh Option C2 cải thiện khả năng hiểu bài, ghi nhớ hoặc tiết kiệm thời gian hơn A và B.
- Chưa biết việc bổ sung hướng dẫn và gợi ý nhanh có giải quyết được khó khăn kéo thả, nhập câu hỏi mà Linh gặp hay không.
- Chưa xác minh lỗi chọn ảnh đã được sửa; chưa biết thao tác có ổn định trên các kích thước màn hình và loại nội dung khác nhau không.
- Nhu cầu so sánh lý thuyết của Khuê đã được ghi nhận, nhưng cơ chế đáp ứng nhu cầu này vẫn cần dựng và kiểm thử.
- Độ chính xác của nội dung do AI giải thích và khả năng xử lý tình huống thực tế vẫn cần được kiểm tra riêng.
