# Maps — Nối các mảnh ghép

Một paper note giúp tôi nhớ một bài viết đã nói gì. Nhưng tôi muốn Atlas đi xa hơn một chút: khi đọc nhiều bài, liệu có nhìn ra được kỹ thuật nào được dùng lại, vấn đề nào vẫn còn khó, hoặc câu trả lời nào lại dẫn đến câu hỏi khác không?

Đó là lý do có mục Maps.

Tôi không định vẽ một sơ đồ thật lớn chỉ để repo trông giống một công trình nghiên cứu đồ sộ. Mỗi đường nối nên có lý do. Nếu mới là phỏng đoán thì cứ ghi là phỏng đoán.

## Map 00 — Những gì tôi thấy trong Paper 01

Theo phần giới thiệu công khai của InSecLab, bài báo kết nối các thành phần sau:

```text
Paper 01: LLMs for Malware Analysis
       |
       +--> Static Analysis reports
       |
       +--> Dynamic Analysis reports
       |
       +--> LLM + RAG + Threat Intelligence
                    |
                    +--> MITRE ATT&CK / TTP mapping
                    |
                    +--> APT ranking / attribution support
```

Đây chỉ là sơ đồ khái quát để tôi dễ hình dung câu chuyện của paper. Nó không phải bản dựng lại toàn bộ architecture; tôi vẫn cần đọc phần Method để xác minh các bước, dữ liệu đi qua đâu và từng thành phần làm gì.

## Những đường nối đang theo dõi

| Từ | Đến | Vì sao tôi muốn nối? | Hiện trạng |
|---|---|---|---|
| Malware Analysis | Static / Dynamic Analysis | Tôi muốn hiểu mỗi kiểu report đóng góp loại evidence nào và chúng bổ sung nhau ra sao. | Câu hỏi nền tảng |
| LLM | RAG + Threat Intelligence | Tôi muốn biết context được truy xuất thêm vào giúp model ở bước nào. | Chưa kiểm tra Method |
| TTP mapping | MITRE ATT&CK | Tôi muốn hiểu đơn vị mapping, ground truth và cách đánh giá độ đúng. | Chưa kiểm tra Evaluation |
| APT ranking | Empirical Evaluation | Tôi muốn hiểu thứ hạng được đánh giá thế nào, và nó hỗ trợ attribution tới đâu. | Chưa kiểm tra Evaluation |

Tạm thời, các đường nối trên dựa trên phần overview và câu hỏi của tôi. Chúng chưa phải kết luận về mức độ hiệu quả của framework.

## Quy tắc tôi muốn giữ khi vẽ map

1. Hai chủ đề xuất hiện cùng abstract chưa chắc đã có mối quan hệ sâu sắc.
2. Mỗi connection cần ghi nó dựa trên câu chữ của paper, kết quả thực nghiệm hay suy luận của tôi.
3. Khi có paper mới, tôi sẽ thêm lý do cho mối nối đó, không chỉ thêm một cái tên vào sơ đồ.
4. Nếu đọc kỹ hơn và thấy kết nối ban đầu không đứng vững, sửa hoặc xóa nó. Map là thứ được phép thay đổi khi mình hiểu thêm.

Mục tiêu không phải là làm cho bản đồ đẹp ngay từ đầu. Mục tiêu là vài tháng sau nhìn lại, tôi có thể hiểu vì sao mình nối hai ý tưởng với nhau — và bằng chứng nào khiến mình tin vào mối nối ấy.
