# PRD Day 17 — NiBi AI

## 1. Product Overview

NiBi AI là trợ lý AI lập lịch trình du lịch Ninh Bình, giúp người dùng tạo itinerary cá nhân hóa theo thời gian, ngân sách, sở thích và nhu cầu dịch vụ.

## 2. Problem Statement

Khách du lịch mất nhiều thời gian để gom thông tin rời rạc, so sánh địa điểm, ước tính chi phí và biến nhu cầu mơ hồ thành lịch trình có thể hành động.

## 3. Target Users

- Khách du lịch trẻ, nhóm bạn, cặp đôi, gia đình nhỏ.
- Người có ý định đi Ninh Bình 1–2 ngày.
- Người chưa chốt lịch trình, tour, homestay hoặc xe.

## 4. Jobs To Be Done

Khi tôi muốn đi Ninh Bình nhưng chưa biết nên sắp xếp lịch trình thế nào, tôi muốn có một kế hoạch phù hợp với thời gian, ngân sách và sở thích để có thể ra quyết định nhanh hơn.

## 5. Solution

NiBi AI hỏi nhu cầu người dùng, tạo lịch trình cá nhân hóa, hiển thị timeline, chi phí ước tính, lý do gợi ý và CTA để lại nhu cầu tư vấn.

## 6. MVP Scope

### In Scope

- Form nhập nhu cầu.
- AI tạo lịch trình.
- Màn hình kết quả lịch trình.
- Lead form.
- Feedback cơ bản.
- Tracking core events.

### Out of Scope

- Booking thật.
- Thanh toán thật.
- Mobile app.
- Voice AI realtime.
- Mở rộng toàn Việt Nam.

## 7. Core User Flow

```
User nhập nhu cầu → AI tạo lịch trình → User xem/chỉnh/lưu → User để lại thông tin tư vấn → Team nhận lead
```

## 8. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR1 | Người dùng nhập ngày đi, số người, ngân sách, sở thích | Must |
| FR2 | Hệ thống tạo lịch trình Ninh Bình cá nhân hóa | Must |
| FR3 | Người dùng xem timeline, chi phí, lý do gợi ý | Must |
| FR4 | Người dùng để lại thông tin tư vấn | Must |
| FR5 | Team lưu lead vào Google Sheet/Supabase | Should |
| FR6 | Người dùng đánh giá lịch trình hữu ích/chưa đúng | Should |

## 9. Non-functional Requirements

- Thời gian tạo lịch trình đủ nhanh cho demo/pilot.
- Không thu thập dữ liệu cá nhân không cần thiết.
- Có fallback nếu AI/API lỗi.
- Có disclaimer rằng giá và tình trạng dịch vụ cần xác nhận lại.

## 10. Success Metrics

- Itinerary completion rate.
- Lead conversion rate.
- Qualified leads.
- Satisfaction score.
- Save/share/edit rate.
