# InSecLab Atlas

*An independent, learner-driven atlas of cybersecurity research papers.*

> Đọc từng paper, hiểu từng ý, rồi nối những gì mình học được thành một bản đồ tri thức.

## Vì sao tôi bắt đầu Atlas?

Tôi đang học An toàn thông tin và muốn hiểu cách người ta làm nghiên cứu bảo mật, chứ không chỉ dừng lại ở việc đọc một tiêu đề hay ghi nhớ vài thuật ngữ mới.

Khi đọc paper, có những đoạn tôi hiểu ngay, có chỗ phải dừng lại tra kiến thức nền, và cũng có những kết quả tôi chưa đủ cơ sở để tự kết luận. Tôi muốn ghi lại cả quá trình đó một cách trung thực.

Vì vậy, **InSecLab Atlas** không được tạo ra để thi xem ai đọc được nhiều paper hơn. Tôi muốn xây một bản đồ giúp mình trả lời dần những câu hỏi:

- Paper đang cố giải quyết vấn đề gì?
- Tác giả đã làm gì để giải quyết nó?
- Bằng chứng nào hỗ trợ cho kết luận?
- Kết quả còn giới hạn ở đâu?
- Từ đó, mình có thể đặt câu hỏi hoặc tìm hướng đọc tiếp nào?

## Atlas không chỉ là một folder chứa paper note

Một ghi chú riêng lẻ giúp tôi nhớ nội dung của một paper. Nhưng khi có nhiều paper, điều thú vị hơn là nhận ra chúng có liên quan gì đến nhau.

Ví dụ, một paper có thể dùng **LLM**, **RAG** và **Threat Intelligence** để hỗ trợ **Malware Analysis**. Một paper khác sau này có thể tập trung vào cách trích xuất hành vi từ binary, hoặc đánh giá độ tin cậy của LLM trong security tasks. Khi có đủ căn cứ, tôi muốn nối các ý tưởng đó lại để thấy kỹ thuật nào đang được dùng, câu hỏi nào vẫn còn mở và paper nào đáng đọc tiếp.

Bản đồ này sẽ được xây dần. Hiện tại Atlas mới bắt đầu từ một paper; tôi không xem đó là thư viện nghiên cứu đã hoàn chỉnh.

## Cách tôi đọc và ghi lại một paper

Tôi cố gắng lần theo mạch:

**Problem → Method → Evidence → Limitation → New Question**

1. **Problem:** Tác giả muốn giải quyết vấn đề gì, và tại sao nó đáng quan tâm?
2. **Method:** Họ thực sự làm gì? Tôi giải thích lại bằng lời của mình, thay vì chép thuật ngữ.
3. **Evidence:** Họ dùng dataset, baseline, metric hay thí nghiệm nào để hỗ trợ claim?
4. **Limitation:** Kết quả chưa nói được điều gì? Giới hạn nào do tác giả nêu, giới hạn nào tôi còn nghi ngờ?
5. **New Question:** Sau khi hiểu paper hơn, tôi muốn tìm hiểu điều gì tiếp theo?

Tôi cũng phân biệt rõ ba thứ: **điều nguồn xác nhận**, **cách tôi đang hiểu**, và **điều tôi chưa biết**. Nếu một nhận xét mới dựa trên abstract hoặc phần giới thiệu của nhóm nghiên cứu, tôi sẽ ghi rõ như vậy, không giả vờ đã kiểm tra toàn bộ paper.

## Cấu trúc repository

- [`Papers/`](Papers/) — Mỗi paper có một note riêng.
- [`Topics/`](Topics/) — Các trang tổng hợp kiến thức theo chủ đề; chỉ mở rộng khi có nội dung đủ cơ sở.
- [`Maps/`](Maps/) — Ghi lại những mối liên hệ giữa paper, kỹ thuật, vấn đề và câu hỏi nghiên cứu.
- [`Templates/`](Templates/) — Khung ghi chú để giữ cách làm nhất quán, nhưng không ép mọi paper vào cùng một khuôn cứng nhắc.

## Điểm bắt đầu

### Paper 01 — Leveraging LLMs to Support Malware Analysis from Structured and Semantic Binary Data

Tôi chọn paper này làm điểm xuất phát vì nó chạm đến nhiều chủ đề tôi muốn tìm hiểu: malware analysis, static/dynamic analysis, LLM, RAG, Threat Intelligence và MITRE ATT&CK.

- [Đọc Paper 01 note](Papers/Paper-01_LLM-Malware-Analysis.md)
- [Bản đồ chủ đề ban đầu](Maps/README.md)
- [Danh mục Topics](Topics/README.md)

**Trạng thái hiện tại:** note đầu tiên được khởi tạo từ phần giới thiệu chính thức và thông tin thư mục của bài báo. Các chi tiết về Method, dataset, metric, kết quả và limitations vẫn cần được đối chiếu với toàn văn. Đây là điểm bắt đầu, không phải một expert review.

## Nguyên tắc của project

- Viết từ góc nhìn người đang học; không giả vờ là chuyên gia.
- Ưu tiên hiểu đúng hơn là dùng nhiều thuật ngữ.
- Không biến một kết quả trong một setup cụ thể thành kết luận đúng cho mọi trường hợp.
- Khi chưa xác minh, nói rõ là chưa xác minh.
- Không đặt quota paper cho đẹp profile. Paper tiếp theo nên xuất hiện từ một câu hỏi hoặc kết nối có ý nghĩa.
- Dẫn về nguồn chính thức; không tự ý đưa bản PDF có bản quyền vào repository.
- Đây là project cá nhân độc lập, không phải repository chính thức, không đại diện hay hàm ý được InSecLab hoặc UIT bảo trợ.

Atlas có thể phát triển trong nhiều tháng hoặc nhiều năm. Trước mắt, tôi chỉ cần làm tốt paper đầu tiên và học cách nối những điều mình đọc được thành một câu chuyện có căn cứ.
