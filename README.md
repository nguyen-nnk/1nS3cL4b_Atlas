# 1nS4cL4b Atlas

*An independent, learner-driven atlas of cybersecurity research papers.*

> Đọc paper, cố hiểu xem người ta đang làm gì, rồi thử nối những mảnh kiến thức đó lại với nhau qua Atlas - infinity loop cho đến khi tôi publish được 100 paper...

## Tôi lập cái repo này làm gì?

Là sinh viên An toàn thông tin và cực kì hứng thu với chuyện research, tôi không muốn đọc tiêu đề rồi nhớ được vài thuật ngữ nghe có vẻ hay, mà là hiểu một paper đang giải quyết chuyện gì, tác giả làm thế nào, và kết quả của họ thật sự nói lên được điều gì.

Vấn đề là đọc paper không phải lúc nào cũng trôi chảy. Có đoạn đọc một lần là hiểu đại khái. Có đoạn phải mở thêm vài tab để tra. Rồi có những chỗ tưởng đã hiểu, đến khi tự giải thích lại mới phát hiện mình chỉ đang đoán.

Tôi muốn ghi lại quá trình ấy ở đây. Cả phần đã hiểu, phần đang hiểu dở, và những câu hỏi chưa có lời giải, maybe khi vào được Lab rồi tiện đi hỏi owner luôn cho nhanh..

Atlas hiện tại chỉ có một paper làm điểm gờ xuất phát. Mong sao sau này sẽ chằng chịt điểm G hơn...

## Vậy Atlas khác gì một folder chứa paper note?

Tôi thấy trung bình vài ngày là các Lab ở trường lại ra paper mới, ôi sao nhanh thế! Chắc hẳn các Lab đều có các linking các paper lại theo topic. Còn tôi có thể nhớ mỗi bài nói gì. Nhưng sau vài bài, câu hỏi thú vị hơn là: **chúng có liên quan gì đến nhau?**

Chẳng hạn, Paper 01 có nhắc đến Malware Analysis, LLM, RAG, Threat Intelligence và MITRE ATT&CK. Những cái tên này đều có thể thành một topic để tìm hiểu tiếp. Nhưng chỉ vì chúng cùng xuất hiện trong một paper không có nghĩa là tôi đã hiểu mối quan hệ giữa chúng.

Atlas lập ra với mong muốn dần dần tìm ra mối liên hệ ấy. Paper nào giải quyết một phần vấn đề? Paper nào dùng cách tiếp cận khác? Kết quả nào có bằng chứng tốt? Và điều gì vẫn chưa được giải quyết?

Vì thế, Atlas có ba loại nội dung chính:

- **Papers:** tôi đã đọc gì, hiểu được gì, còn mắc ở đâu.
- **Topics:** những khái niệm và câu hỏi xuất hiện qua nhiều paper.
- **Maps:** các mối liên hệ giữa paper, kỹ thuật, vấn đề và câu hỏi tiếp theo.

Nghe hơi tham vọng nhỉ. Nhưng không sao, 10 năm... 20 năm... 30 năm... (trích anhzai Khoai Lang thang)

## Một paper sẽ được tôi đọc như thế nào?

Tôi cố gắng lần theo mạch:

**Problem → Method → Evidence → Limitation → New Question**

- **Problem:** Tác giả đang muốn giải quyết chuyện gì? Vì sao chuyện đó đáng quan tâm?
- **Method:** Họ thực sự làm gì? Tôi có thể giải thích lại bằng lời của mình không?
- **Evidence:** Họ dùng dataset, baseline, metric hay experiment nào để hỗ trợ kết luận?
- **Limitation:** Kết quả còn giới hạn ở đâu? Tác giả đã nói gì, và tôi còn nghi ngờ điều gì?
- **New Question:** Sau khi đọc xong, điều gì khiến tôi muốn tìm hiểu tiếp?

Tôi cũng cố tách ba thứ ra khỏi nhau: điều được nguồn xác nhận, cách tôi đang hiểu, và điều tôi chưa biết. Nếu tôi mới đọc overview mà chưa kiểm tra full paper, tôi sẽ nói rõ. Không có lợi gì khi viết cho thật chắc chắn rồi sau đó không giải thích nổi vì sao mình kết luận như vậy.

## Đi một vòng trong repository

- [Papers/](Papers/) — Mỗi paper có một note riêng.
- [Topics/](Topics/) — Các câu hỏi và khái niệm đang được theo dõi.
- [Maps/](Maps/) — Những kết nối tôi đã nhận ra hoặc đang muốn kiểm tra.
- [Templates/](Templates/) — Một khung ghi chú để khỏi phải nghĩ lại cách trình bày từ đầu mỗi lần.

### Điểm bắt đầu: Paper 01

**Leveraging LLMs to Support Malware Analysis from Structured and Semantic Binary Data**

Tôi chọn bài này vì nó chạm đến nhiều thứ tôi đang tò mò: Malware Analysis, Static/Dynamic Analysis, LLM, RAG, Threat Intelligence và MITRE ATT&CK.

- [Đọc Paper 01](Papers/Paper-01_LLM-Malware-Analysis.md)
- [Xem danh mục paper](Papers/README.md)
- [Xem Topics ban đầu](Topics/README.md)
- [Xem Map ban đầu](Maps/README.md)
- [Lấy template ghi chú](Templates/Paper-Note-Template.md)

Một lưu ý quan trọng: Paper 01 hiện mới được khởi tạo từ thông tin thư mục và phần giới thiệu công khai của InSecLab. Các chi tiết về architecture, dataset, metrics, bảng kết quả và limitations vẫn cần được kiểm tra trong toàn văn. Đây là nhật ký đọc đang phát triển, chưa phải expert review.

## Vài nguyên tắc để khỏi tự làm khó mình

1. **Viết như người đang học thật.** Keep it riel
2. **Không bắt buộc paper nào cũng phải có câu trả lời cho mọi thứ.** Một câu hỏi tốt cũng có ích.
3. **Không thêm paper chỉ để làm repo trông đông vui.** Bài nào thích linking với nhau thì quăng vô, vì mục tiêu là để học.
4. **Dẫn nguồn để người khác kiểm tra lại được.** ... 

Cuối cùng, nói cho rõ: đây là project cá nhân độc lập. Atlas là một dự án đường dài có thể phát triển trong nhiều tháng, thậm chí nhiều năm.
