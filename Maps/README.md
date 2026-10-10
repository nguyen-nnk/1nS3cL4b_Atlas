# Maps — Linking các mảnh ghép

Ghi chú riêng lẻ giúp tôi nhớ mỗi paper nói gì. Nhưng về lâu dài, tôi muốn xem thử các paper có nối với nhau thế nào: kỹ thuật nào được dùng lại, vấn đề nào vẫn còn khó, hoặc câu trả lời nào lại dẫn đến một câu hỏi mới.

Đó là lý do có mục Maps.

Tôi không định vẽ một sơ đồ thật chằng chịt cho có vẻ research. Một đường nối phải có lý do. Nếu mới là suy đoán thì ghi là suy đoán — sau này đọc kỹ hơn còn sửa được.

## Map 00 — Sơ đồ xuất phát từ Paper 01

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

Đây là sơ đồ tôi vẽ lại để dễ hình dung câu chuyện của paper. Chưa phải bản dựng lại toàn bộ architecture; muốn chắc hơn thì phải đọc Method để biết các bước cụ thể, data đi qua đâu và từng thành phần làm gì.

## Các đường link tôi đang theo dõi

| Từ | Đến | Sao tôi muốn nối hai thứ này? | Trạng thái |
|---|---|---|---|
| Malware Analysis | Static / Dynamic Analysis | Muốn hiểu mỗi kiểu report đóng góp evidence gì và chúng bổ sung nhau ra sao. | Câu hỏi nền tảng |
| LLM | RAG + Threat Intelligence | Muốn biết context được truy xuất thêm vào giúp model ở bước nào. | Chưa kiểm tra Method |
| TTP mapping | MITRE ATT&CK | Muốn hiểu mapping unit, ground truth và cách đánh giá độ đúng. | Chưa kiểm tra Evaluation |
| APT ranking | Empirical Evaluation | Muốn hiểu thứ hạng được đánh giá thế nào, và nó hỗ trợ attribution tới đâu. | Chưa kiểm tra Evaluation |

Các đường nối trên hiện dựa vào overview và câu hỏi của tôi. Chúng chưa phải kết luận rằng framework hiệu quả đến mức nào.

## Mấy quy tắc để khỏi nối dây điện bừa

1. Hai chủ đề xuất hiện cùng abstract chưa chắc đã có mối quan hệ sâu sắc.
2. Mỗi connection cần ghi rõ nó dựa trên câu chữ của paper, kết quả thực nghiệm hay suy luận của tôi.
3. Khi có paper mới, thêm lý do cho mối nối đó, đừng chỉ thêm tên vào sơ đồ.
4. Nếu đọc kỹ hơn và thấy kết nối ban đầu không đứng vững, cứ sửa hoặc xóa. Map mà không được cập nhật khi mình hiểu thêm thì chẳng khác gì treo bản đồ cũ lên tường.

Mục tiêu không phải làm map đẹp ngay từ đầu. Mục tiêu là vài tháng sau nhìn lại, tôi vẫn nhớ vì sao mình nối hai ý tưởng với nhau — và evidence nào khiến mình tin vào mối nối ấy.
