# Lab Day 25 - Workshop 2: Roadmap Now / Next / Later (NiBi AI)
**Học viên:** Đặng Trần Đạt - 2A202600662

## 1. Giới thiệu sản phẩm

**NiBi AI** — Trợ lý AI lập lịch trình du lịch Ninh Bình, giúp khách tạo itinerary cá nhân hóa và để lại nhu cầu tư vấn tour / homestay / thuê xe.

---

## 2. Roadmap 1 trang (Problem-based)

*Quy tắc: Không ghi ngày tháng. Tập trung vào vấn đề cần giải quyết thay vì tính năng cụ thể.*

| NOW (Hiện tại) | NEXT (Tiếp theo) | LATER (Tương lai) |
|---|---|---|
| **Vấn đề 1:** Khách du lịch mất nhiều thời gian để tự gom thông tin và biến nhu cầu mơ hồ thành một lịch trình Ninh Bình khả thi.<br><br>*Người dùng thường không biết nên đi đâu trước, đi trong bao lâu, chi phí khoảng bao nhiêu, tuyến đường có hợp lý không. Đây là core problem cần giải đầu tiên vì nếu không tạo được lịch trình hữu ích, mọi tính năng phía sau đều không có giá trị.* | **Vấn đề 1:** Dữ liệu tour, homestay, thuê xe và địa điểm còn rời rạc, khiến AI dễ trả lời chung chung hoặc thiếu căn cứ địa phương.<br><br>*Sau khi core flow chạy được, sản phẩm cần nguồn dữ liệu riêng để gợi ý đáng tin hơn, giảm phụ thuộc vào kiến thức chung của LLM và tạo lợi thế cạnh tranh dài hạn.* | **Vấn đề 1:** Người dùng muốn đặt dịch vụ du lịch liền mạch, nhưng booking / thanh toán thật có quá nhiều rủi ro vận hành ở giai đoạn MVP.<br><br>*Đây là tầm nhìn dài hạn, nhưng chưa nên làm ngay vì cần đối tác, tồn kho, chính sách hủy, thanh toán, hoàn tiền và chăm sóc khách hàng.* |
| **Vấn đề 2:** Sau khi nhận lịch trình, khách chưa có cách đơn giản để chuyển nhu cầu thành yêu cầu tư vấn thật.<br><br>*Đây là Quick Win từ RICE vì effort thấp nhưng tạo outcome kinh doanh rõ ràng: qualified lead cho sales hoặc đội tư vấn du lịch.* | **Vấn đề 2:** Team chưa biết lịch trình nào hữu ích, lịch trình nào sai, và người dùng muốn chỉnh gì sau khi nhận output từ AI.<br><br>*Cần vòng feedback để học từ hành vi thật: lưu lịch trình, chia sẻ, tải xuống, sửa yêu cầu, đánh giá hữu ích / chưa đúng.* | **Vấn đề 2:** Khách du lịch có thể muốn nhận lại lịch trình và chăm sóc sau tư vấn qua các kênh quen thuộc như Zalo OA hoặc mini app.<br><br>*Đây là hướng mở rộng retention và CRM, nhưng chỉ nên làm khi đã chứng minh người dùng thật sự dùng lịch trình và để lại lead.* |
| **Vấn đề 3:** Team cần chứng minh sản phẩm không chỉ là chatbot demo, mà tạo được value có thể đo bằng số.<br><br>*Cần theo dõi các chỉ số như tỷ lệ hoàn tất tạo lịch trình, thời gian đến lịch trình đầu tiên, tỷ lệ để lại lead, tỷ lệ user bấm chỉnh sửa / lưu / chia sẻ.* | **Vấn đề 3:** Admin / editor cần cách cập nhật dữ liệu dịch vụ mà không phải sửa code mỗi lần.<br><br>*Khi bắt đầu có dữ liệu thật, hệ thống cần quy trình quản trị nội dung để thêm / sửa tour, homestay, thuê xe, địa điểm và bài viết.* | |

---

## 3. Bản mapping từ RICE sang Roadmap

| Từ bảng RICE Workshop 1 | Đưa vào đâu? | Lý do |
|---|---|---|
| **AI tạo lịch trình du lịch cá nhân hóa** | **NOW** | Đây là core value. Nếu không giải được vấn đề lập lịch trình, sản phẩm không có lý do tồn tại. |
| **Lead form + sales handoff** | **NOW** | Quick Win có RICE score cao nhất, effort thấp, gắn trực tiếp với business outcome. |
| **Tracking / feedback / lưu / chia sẻ lịch trình** | **NOW → NEXT** | Một phần tracking cơ bản nên có ngay ở NOW; feedback nâng cao có thể làm ở NEXT. |
| **Dữ liệu tour / homestay / thuê xe / địa điểm có quản trị** | **NEXT** | Strategic Bet tạo moat dài hạn, nhưng cần effort và dữ liệu sạch nên không nên làm trước core flow. |
| **Booking và thanh toán thật** | **LATER** | Non-starter ở MVP vì quá nhiều dependency và rủi ro vận hành. |
