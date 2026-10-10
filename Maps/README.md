# Maps — Nối các mảnh ghép

Paper note giúp tôi ghi lại từng bài riêng lẻ. Maps là nơi tôi thử trả lời câu hỏi: *Những ý này có liên quan với nhau như thế nào, và mối liên hệ ấy có ý nghĩa gì?*

Tôi chưa muốn vẽ một sơ đồ lớn chỉ để trông có vẻ nghiên cứu. Mỗi connection cần có lý do, và phải phân biệt connection đã xác nhận với connection mới là hướng đọc tiềm năng.

## Map 00 — Điểm xuất phát từ Paper 01

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

**Nguồn:** sơ đồ khái quát được dựng lại từ phần giới thiệu chính thức của InSecLab. Đây không phải reconstruction của toàn bộ architecture trong paper.

## Các connection đang theo dõi

| Từ | Đến | Vì sao đáng nối? | Trạng thái |
|---|---|---|---|
| Malware Analysis | Static / Dynamic Analysis | Cần hiểu hai kiểu report đóng góp evidence gì và khác nhau ở đâu. | Câu hỏi nền tảng |
| LLM | RAG + Threat Intelligence | Cần xác định context được truy xuất bổ sung gì cho model. | Chưa kiểm tra Method |
| TTP mapping | MITRE ATT&CK | Cần hiểu mapping unit, ground truth và cách đo độ chính xác. | Chưa kiểm tra Evaluation |
| APT ranking | Empirical Evaluation | Cần hiểu ranking được đánh giá ra sao và mức độ nào có thể hỗ trợ attribution. | Chưa kiểm tra Evaluation |

## Quy tắc vẽ map

1. Không nối hai chủ đề chỉ vì chúng xuất hiện trong cùng một abstract.
2. Ghi rõ connection dựa trên câu chữ của paper, kết quả thực nghiệm hay suy luận của tôi.
3. Khi có paper khác, bổ sung connection kèm lý do cụ thể; đừng chỉ thêm một nút để sơ đồ trông lớn hơn.
4. Nếu một mối liên hệ không đứng vững sau khi đọc kỹ hơn, sửa hoặc xóa nó.

Mục tiêu không phải là làm ra một sơ đồ đẹp nhất ngay từ đầu. Mục tiêu là tạo ra một bản đồ ngày càng có ích cho những câu hỏi nghiên cứu tiếp theo.
