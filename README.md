# BIT230239_KTPM
#Tuần 1:
<img width="1867" height="882" alt="image" src="https://github.com/user-attachments/assets/0e690974-a1dd-43a4-acfd-9584587217f3" />
#Tuần 3:
<img width="1886" height="829" alt="Screenshot 2026-01-29 000105" src="https://github.com/user-attachments/assets/ccd168a1-313b-4276-9b0a-2d6f21407a52" />
#Tuần 4:
# Kiểm thử hiệu năng với Apache JMeter
## Website được kiểm thử
https://example.com
## Công cụ sử dụng
Apache JMeter 5.6.3
---

## Thread Group 1 – Kịch bản cơ bản
- 20 users
- Loop: 10
- GET trang chủ (/)
Kết quả:
- Total Samples: 13,357
- Average Response Time: 41 ms
- Error Rate: 0%
- Throughput: 222.5 requests/sec

---

## Thread Group 2 – Tải nặng
- 50 users
- Ramp-up: 30s
- 2 HTTP Requests (Home, Home2)

Kết quả:
- Total Samples: 26,703
- Average Response Time: 41 ms
- Max Response Time: 874 ms
- Error Rate: 0%
- Throughput: 444.7 requests/sec

---

## Thread Group 3 – Kiểm thử đồng thời cao
- Nhiều người dùng đồng thời
- 2 HTTP Requests

Kết quả:
- Average Response Time: ~41 ms
- Error Rate: 0%
- Throughput: Ổn định và cao

---

## Kết luận
- Hệ thống không xảy ra lỗi (0% Error Rate).
- Thời gian phản hồi ổn định (~41 ms).
- Throughput cao, xử lý tốt nhiều request đồng thời.
- Website hoạt động ổn định dưới tải kiểm thử.
