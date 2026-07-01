# Lab Day 25 - Track 1: Roadmap & Execution (NiBi AI)
**Học viên:** Đặng Trần Đạt - 2A202600662

## 1. RICE Prioritization cho NiBi AI

**Giả định chung:**
- Dự án đang ở giai đoạn MVP/pilot.
- **Reach**: Tính theo số user hoặc lượt user bị ảnh hưởng trong 1 quý.
- **Confidence**: Chỉ để 50% hoặc 80% vì chưa có dữ liệu thị trường thật lớn.
- **Effort**: Tính theo person-month, tức 1 người làm trong 1 tháng.

### Bảng chấm điểm RICE (5 tính năng cốt lõi)

| # | Tính năng cốt lõi | Reach / quý | Impact | Confidence | Effort (PM) | RICE Score | Nhận định |
|---|---|---|---|---|---|---|---|
| 1 | AI tạo lịch trình du lịch Ninh Bình cá nhân hóa theo thời gian, ngân sách, sở thích | 500 | 3 | 80% | 1.5 | **800** | Core value của sản phẩm. Phải có trong MVP |
| 2 | Form để lại nhu cầu tư vấn sau khi xem lịch trình, tự chuyển thành lead cho sales | 350 | 2 | 80% | 0.5 | **1120** | Quick Win mạnh nhất vì effort thấp, gắn trực tiếp business |
| 3 | Bộ dữ liệu tour / homestay / thuê xe / địa điểm được quản trị bởi admin-editor để AI gợi ý có căn cứ | 400 | 2 | 50% | 2.0 | **200** | Strategic Bet, tạo moat dài hạn nhưng cần dữ liệu sạch |
| 4 | Lưu / xuất / chia sẻ lịch trình, kèm nút feedback “hữu ích / chưa đúng / muốn chỉnh” | 250 | 1 | 80% | 0.75 | **267** | Tốt cho engagement và học từ user, nhưng không phải ưu tiên số 1 |
| 5 | Booking và thanh toán thật cho tour / homestay / xe ngay trong app | 80 | 2 | 50% | 4.0 | **20** | Non-starter ở MVP vì effort cao, nhiều dependency, rủi ro vận hành lớn |

*(Cách tính ví dụ dòng 2: Score = 350 × 2 × 0.8 / 0.5 = 1120)*

### Xếp hạng ưu tiên theo RICE

1. **Lead form + sales handoff** — 1120
2. **AI tạo lịch trình cá nhân hóa** — 800
3. **Lưu/chia sẻ lịch trình + feedback** — 267
4. **Dữ liệu tour/homestay/xe có quản trị** — 200
5. **Booking/thanh toán thật** — 20

> **Nhận xét:** Nhìn qua có thể thấy tính năng Lead form có điểm cao nhất vì effort rất thấp nhưng tác động trực tiếp đến business. Tuy nhiên, nó chỉ có giá trị nếu tính năng AI tạo lịch trình đã chạy ổn. Vì vậy, trong execution thực tế, hai tính năng này nên đi cùng nhau trong giai đoạn NOW.

---

## 2. 2x2 Value-Effort Matrix

**Quy ước:**
- **Value cao:** Impact ≥ 2 hoặc ảnh hưởng trực tiếp đến core value / revenue.
- **Effort thấp:** Effort ≤ 1 person-month.
- **Effort cao:** Effort ≥ 2 person-month.

| | Effort thấp | Effort cao |
|---|---|---|
| **Value cao** | **Quick Win:** Lead form + sales handoff.<br>*Tạo business value nhanh, dễ demo với mentor/investor.* | **Strategic Bet:** Bộ dữ liệu tour/homestay/xe có quản trị.<br>*Đây là moat dài hạn vì giúp AI trả lời dựa trên dữ liệu riêng, không chỉ là chatbot chung chung.* |
| **Value thấp/trung bình** | **Fill-in:** Lưu / xuất / chia sẻ lịch trình + feedback.<br>*Nên làm sau khi core flow chạy được.* | **Non-starter:** Booking và thanh toán thật trong app.<br>*Không nên làm ở MVP vì phức tạp về đối tác, vận hành, chính sách hoàn/hủy và thanh toán.* |

---

## 3. Kết luận đưa vào Report

### Quick Win nên làm trước
**Lead form + sales handoff sau khi user xem lịch trình.**
- *Lý do:* Effort thấp, dễ triển khai, tạo outcome kinh doanh rõ ràng là qualified lead. Đây là tính năng giúp chứng minh sản phẩm không chỉ “AI trả lời hay” mà có thể tạo cơ hội bán tour/homestay/xe.

### Strategic Bet / Moat dài hạn
**Bộ dữ liệu tour, homestay, thuê xe, địa điểm được quản trị bởi admin/editor và dùng làm nguồn cho AI.**
- *Lý do:* Nếu chỉ dùng LLM chung, NiBi AI rất dễ bị copy. Nhưng nếu có dữ liệu địa phương, giá, lịch trình mẫu, đối tác, kinh nghiệm tuyến điểm, sản phẩm sẽ có lợi thế riêng.

### Non-starter nên bỏ ở MVP
**Booking và thanh toán thật trong app.**
- *Lý do:* Nghe có vẻ tạo doanh thu nhanh, nhưng quá nhiều dependency: đối tác, tồn kho phòng/tour, chính sách hủy, thanh toán, hoàn tiền, pháp lý, chăm sóc khách hàng. Ở MVP, chỉ nên dừng ở lead capture / booking request, chưa cần giao dịch thật.

---

## 4. Tổng kết đánh giá ưu tiên (Executive Summary)

Trong giai đoạn MVP, nhóm ưu tiên các tính năng theo outcome thay vì số lượng feature. Kết quả chấm RICE cho thấy tính năng có điểm cao nhất là **Lead form + sales handoff** với 1120 điểm, vì effort thấp nhưng tác động trực tiếp đến mục tiêu kinh doanh. Tính năng **AI tạo lịch trình cá nhân hóa** đạt 800 điểm và là core value bắt buộc của sản phẩm. Tính năng **dữ liệu tour/homestay/xe có quản trị** có điểm RICE thấp hơn do effort cao và confidence thấp hơn, nhưng được xếp vào Strategic Bet vì tạo lợi thế dài hạn cho sản phẩm. Ngược lại, **booking và thanh toán thật** được xác định là Non-starter ở giai đoạn MVP vì effort cao, dependency lớn và chưa cần thiết để kiểm chứng giá trị cốt lõi.


