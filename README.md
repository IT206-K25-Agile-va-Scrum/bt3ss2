# BÁO CÁO BÀI TẬP: THIẾT KẾ VẬN HÀNH SCRUM CHO TÍNH NĂNG ĐẶT XE GHÉP

> 👤 **Học viên:** Đỗ Hoàng Sơn | **Mã SV:** PTIT-HCM-055
> 🏫 **Môn học:** IT206-K25-Agile-va-Scrum

---

## Phần 1 - Phân tích

Trong một Sprint chuẩn của đội RikkeiGo, đầu vào bao gồm Product Backlog đã được Product Owner tinh chỉnh, Sprint Goal (mục tiêu của Sprint) và năng lực thực tế của đội (Velocity). Đầu ra là một Incremental (phần mềm có thể chạy được, đáp ứng định nghĩa hoàn thành - Definition of Done) và Product Backlog được cập nhật lại.

Tôi chọn độ dài mỗi Sprint là 2 tuần (14 ngày). Với thời hạn tổng cộng là 6 tuần để ra mắt tính năng đặt xe ghép, 6 tuần này sẽ được chia trọn vẹn thành 3 Sprint (Sprint 1, Sprint 2, Sprint 3).

Lựa chọn độ dài 2 tuần gắn liền chặt chẽ với trụ cột 'Sự minh bạch' (Transparency) và 'Sự thanh tra' (Inspection) trong Scrum. Cụ thể, sau mỗi 2 tuần, sản phẩm chạy được phải được mang ra thanh tra cùng các bên liên quan và khách hàng mẫu, giúp đội ngũ kiểm chứng xem tính năng ghép chuyến hay tính năng thanh toán đang vận hành ra sao, tránh việc 'đóng cửa gõ code' suốt 6 tuần mới đem ra sản phẩm không đúng ý thị trường.

- Đầu vào Sprint: Product Backlog ưu tiên, Sprint Goal, Năng lực đội ngũ (Velocity).
- Đầu ra Sprint: Phần mềm chạy được (Increment), Product Backlog tối ưu hóa.
- Độ dài Sprint: 2 tuần (3 Sprint cho tổng thời gian 6 tuần dự án).

## Phần 2 - Thiết kế

Dựa trên các nhu cầu thô do Đức (Product Owner) cung cấp, tôi sắp xếp lại thành Product Backlog theo thứ tự ưu tiên từ cao xuống thấp dựa trên giá trị cốt lõi mang lại cho khách hàng và tính khả thi kỹ thuật của mô hình xe ghép.

| Thứ tự | Hạng mục (Product Backlog Item) | Mô tả chi tiết | Lý do sắp xếp thứ tự |
| --- | --- | --- | --- |
| 1 | Ghép khách đi chung tuyến đường | Hệ thống tự động gom các khách hàng có chung lộ trình vào một chuyến xe ghép. | Đây là giá trị cốt lõi (Core Value) và là bản chất của dịch vụ RikkeiGo. Không có tính năng này thì không hình thành mô hình đặt xe ghép. |
| 2 | Tự động chia tiền cho từng khách | Sau chuyến đi, hệ thống tự động tính toán và chia đều hoặc chia theo thỏa thuận số tiền cước cho từng khách. | Giải quyết bài toán thanh toán phức tạp của xe ghép. Khách hàng cần biết rõ số tiền mình phải trả ngay sau khi kết thúc chuyến đi. |
| 3 | Thanh toán bằng thẻ ngân hàng | Tích hợp cổng thanh toán thẻ quốc tế và nội địa để khách thanh toán trực tuyến. | Đáp ứng nhu cầu giao dịch không tiền mặt, tuy nhiên xếp sau lõi nghiệp vụ ghép xe và chia tiền vì có thể dùng tiền mặt hoặc các hình thức tạm thời trong giai đoạn đầu. |
| 4 | Khách đánh giá bạn đi ghép | Cho phép hành khách chấm điểm và để lại đánh giá về tài xế hoặc bạn đi ghép sau chuyến đi. | Tính năng bổ trợ giúp tăng chất lượng dịch vụ dài hạn, nên được đưa vào Sprint cuối khi hệ thống cốt lõi đã chạy ổn định. |

## Phần 3 - Xử lý thay đổi

Giữa tuần thứ 2 của Sprint (khi đội đang làm dở công việc), khách hàng yêu cầu ưu tiên thanh toán qua ví điện tử trước thẻ ngân hàng. Theo tinh thần Agile 'Phản hồi với thay đổi hơn bám sát kế hoạch', cách xử lý của chúng tôi như sau:

1. Người quyết định: Product Owner (Đức) là người tiếp nhận yêu cầu từ thị trường, đánh giá lại giá trị kinh doanh và quyết định đưa yêu cầu này vào Product Backlog, đồng thời thương lượng với Development Team về việc điều chỉnh phạm vi Sprint hiện tại nếu cần hoặc đưa vào Sprint tiếp theo tùy thuộc vào mức độ khẩn cấp.

2. Nơi ghi nhận: Yêu cầu mới được cập nhật ngay lập tức vào Product Backlog trên công cụ quản lý (Jira/Trello), dịch chuyển độ ưu tiên của ví điện tử lên trên thẻ ngân hàng.

3. Thời điểm áp dụng: Do đội đang làm dở một Sprint, nguyên tắc Scrum là không phá vỡ mục tiêu Sprint hiện tại (Sprint Goal) trừ khi Sprint đó mất hẳn ý nghĩa. Do đó, đội ngũ giữ nguyên Sprint Goal hiện tại để hoàn thành dở dang, nhưng hạng mục thanh toán qua ví điện tử sẽ được đưa thẳng lên vị trí số 1 trong buổi Sprint Planning tiếp theo ngay khi kết thúc Sprint này để phát triển và ra mắt sớm nhất có thể.

- Người quyết định: Product Owner (Đức).
- Nơi ghi nhận: Product Backlog trên hệ thống quản lý công việc.
- Thời điểm áp dụng: Đưa vào đầu Sprint kế tiếp để đảm bảo không làm gián đoạn Sprint Goal hiện tại.

---

## 📁 Danh sách tệp tin nộp bài trong Repository
- 📝 `bt3.docx`: Báo cáo tài liệu phân tích nghiệp vụ hoàn chỉnh.
