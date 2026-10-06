# [Vận dụng chuyên sâu] THIẾT KẾ VẬN HÀNH SCRUM CHO TÍNH NĂNG ĐẶT XE GHÉP

> 👤 **Học viên:** Đỗ Hoàng Sơn | **Mã SV:** PTIT-HCM-066
> 🏫 **Môn học:** IT206-K25-Agile-va-Scrum

---

## Phần 1 - Phân tích

Trong bối cảnh đội RikkeiGo cần ra mắt tính năng đặt xe ghép trong vòng 6 tuần với nhiều biến động từ yêu cầu người dùng, việc thiết kế nhịp làm việc chuẩn Scrum là cực kỳ quan trọng.

Đầu vào (Sprint Input) của một Sprint bao gồm: Product Backlog đã được Product Owner ưu tiên, năng lực của đội ngũ (Team Capacity) từ các Sprint trước, và định nghĩa hoàn thành (Definition of Done - DoD).

Đầu ra (Sprint Output) của một Sprint bao gồm: Bản chạy được (Increment) có thể sử dụng hoặc đem đi kiểm thử ngay với người dùng thực tế, và Sprint Backlog chưa hoàn thành (nếu có) được đánh giá lại trong buổi Review.

Độ dài Sprint được chọn là 2 tuần (2-week Sprint). Với tổng thời gian 6 tuần, đội sẽ trải qua chính xác 3 Sprint trọn vẹn (Sprint 1, Sprint 2, Sprint 3).

Lý do chọn Sprint kéo dài 2 tuần gắn liền với trụ cột 'Thanh tra và Thích ứng' (Inspection & Adaptation) của Scrum: Khoảng thời gian 2 tuần đủ dài để đội hoàn thành một lượng tính năng có giá trị sử dụng (Increment), nhưng lại đủ ngắn để không đi sai hướng quá lâu nếu phản hồi từ thị trường hoặc yêu cầu nghiệp vụ thay đổi.

- Độ dài Sprint: 2 tuần (3 Sprint trong 6 tuần).
- Trụ cột Scrum áp dụng: Thanh tra (Inspection) và Thích ứng (Adaptation).
- Sản phẩm bàn giao: Increment chạy được sau mỗi 2 tuần để người dùng thử nghiệm.

## Phần 2 - Thiết kế

Product Owner (Đức) đã tiếp nhận 4 nhu cầu thô từ khách hàng và tiến hành sắp xếp lại thành Product Backlog theo thứ tự ưu tiên dựa trên giá trị cốt lõi mang lại cho người dùng và bài toán kinh doanh của RikkeiGo.

| Thứ tự | Hạng mục Product Backlog | Mô tả chi tiết | Lý do sắp xếp ưu tiên |
| --- | --- | --- | --- |
| 1 | Ghép khách đi chung tuyến đường | Thuật toán gom các khách hàng có chung lộ trình vào cùng một chuyến xe ghép. | Đây là giá trị cốt lõi (Core Value) quyết định bản chất của dịch vụ xe ghép, không thể thiếu ở bản ra mắt đầu tiên. |
| 2 | Tự động chia tiền cho từng khách | Hệ thống tự động tính toán và chia đều hoặc chia theo quãng đường cho các khách trong cùng chuyến. | Đi kèm ngay sau tính năng ghép xe để giải quyết bài toán thanh toán minh bạch, nếu không có tính năng này thì việc đi ghép không khả thi. |
| 3 | Thanh toán bằng thẻ ngân hàng | Tích hợp cổng thanh toán thẻ để khách hàng thanh toán trực tuyến. | Đáp ứng nhu cầu thanh toán điện tử cơ bản, dù có thể thay đổi phương thức nhưng cần có sẵn một cổng thanh toán mẫu ở giai đoạn đầu. |
| 4 | Khách đánh giá bạn đi ghép | Cho phép khách hàng rate sao và để lại feedback về tài xế hoặc bạn đồng hành sau chuyến đi. | Tính năng bổ trợ giúp nâng cao chất lượng dịch vụ dài hạn, đưa vào Sprint cuối khi hệ thống cốt lõi đã chạy ổn định. |

## Phần 3 - Xử lý thay đổi

Vào giữa tuần thứ 2, khi đội đang làm dở Sprint 1 và có yêu cầu đổi ưu tiên từ 'Thanh toán thẻ ngân hàng' sang 'Thanh toán qua ví điện tử', Scrum Team xử lý theo đúng tinh thần linh hoạt của Agile:

1. Ai quyết định: Product Owner (Đức) là người duy nhất có quyền thay đổi và sắp xếp lại Product Backlog sau khi đã cân nhắc giá trị kinh doanh và áp lực từ phản hồi thị trường.

2. Đưa vào đâu: Yêu cầu 'Thanh toán qua ví điện tử' được đưa vào Product Backlog, thay thế vị trí ưu tiên của thẻ ngân hàng cho các Sprint tiếp theo.

3. Áp dụng từ khi nào: Do Sprint hiện tại (Sprint 1) đang chạy dở và đội đang tập trung hoàn thành mục tiêu Sprint Goal (Ghép khách và chia tiền), việc thay đổi sẽ không nhồi nhét vào giữa Sprint để tránh phá vỡ cam kết của đội. Thay vào đó, yêu cầu ví điện tử sẽ chính thức được đưa vào Sprint Planning của Sprint tiếp theo (Sprint 2) để đội lên kế hoạch kỹ thuật và triển khai.

- Người quyết định: Product Owner.
- Nơi ghi nhận: Product Backlog.
- Thời điểm áp dụng: Bắt đầu từ Sprint tiếp theo (Sprint 2), bảo vệ tiến độ của Sprint hiện tại.

---

## 📁 Danh sách tệp tin nộp bài trong Repository
- 📝 `bt3.docx`: Báo cáo tài liệu phân tích nghiệp vụ hoàn chỉnh.
