# Báo Cáo Thực Hành Lab 03 - Nhập Môn Điện Toán

Báo cáo thực hành môn **Nhập môn Điện toán** (Trường Đại học Bách Khoa - ĐHQG TP.HCM).  
Chủ đề: **Lập trình C cơ bản và điều khiển LED – RGB – Nút nhấn** trên nền tảng **OhStem Virtual Device / Yolo UNO**.

---

## 📌 Thông Tin Chung

- **Môn học:** Nhập môn Điện toán (CO1007)
- **Lớp:** L01
- **Giảng viên hướng dẫn:** ThS. Lê Trường Thống
- **Sinh viên thực hiện:** Nguyễn Thảo Vi
- **MSSV:** 2610353
- **Niên khóa:** 2026 - 2027

---

## 📂 Cấu Trúc Thư Mục Dự Án

```text
Nhapmondientoan/
├── main.tex               # File TeX chính kết nối toàn bộ báo cáo
├── cover-page.tex         # Trang bìa chuẩn mẫu Bách Khoa (TikZ border, logo)
├── hcmut.png              # Logo Trường Đại học Bách Khoa
├── bia3.png               # Hình minh họa trang bìa
├── README.md              # Tài liệu hướng dẫn sử dụng dự án
└── sections/              # Thư mục chứa nội dung chi tiết 30 bài tập
    ├── phanA.tex          # Phần A: Console và LED đầu tiên (BT01 - BT04)
    ├── phanB.tex          # Phần B: LED đơn, thời gian, vòng lặp (BT05 - BT08)
    ├── phanC.tex          # Phần C: LED RGB và mô phỏng trạng thái (BT09 - BT12)
    ├── phanD.tex          # Phần D: Ứng dụng rẽ nhánh và vòng lặp (BT13 - BT16)
    ├── phanE.tex          # Phần E: Nút bấm, trạng thái và sự kiện (BT17 - BT20)
    └── phanF.tex          # Phần F: Bài tập tổng hợp và nâng cao (BT21 - BT30)
```

---

## 📝 Danh Sách 30 Bài Tập Thực Hành

| Phần | Mã bài | Tên bài tập | Kiến thức trọng tâm |
| :--- | :---: | :--- | :--- |
| **Phần A** | BT01 | In hồ sơ sinh viên | `main()`, `printf()`, ký tự xuống dòng `\n` |
| | BT02 | Hai số và phép toán | `scanf()`, ép kiểu `float`, xử lý chia cho 0 |
| | BT03 | Bật cảnh báo từ giá trị đo giả lập | Cấu trúc rẽ nhánh `if / else if / else` |
| | BT04 | Đèn LED nhấp nháy đầu tiên | Khung `setup() / loop()`, `digitalWrite()`, `delay()` |
| **Phần B** | BT05 | LED sáng liên tục | Khởi tạo trạng thái phần cứng trong `setup()` |
| | BT06 | Hai nhịp nháy với cùng chu kỳ | Chu kỳ $T$ và tỷ lệ thời gian sáng (Duty Cycle) |
| | BT07 | Chớp kép rồi nghỉ | Vòng lặp `for`, điều khiển cụm xung tín hiệu |
| | BT08 | Đếm ngược bằng LED và console | Kết hợp vòng lặp giảm, đồng bộ console và LED |
| **Phần C** | BT09 | Ba kênh R – G – B | Điều khiển LED 3 kênh độc lập qua `rgb_set()` |
| | BT10 | Pha bốn màu | Hòa sắc cộng ánh sáng (Yellow, Cyan, Magenta, White) |
| | BT11 | Đèn giao thông 3 pha | Chu trình tuần tự 3 pha (Đỏ $\to$ Xanh $\to$ Vàng) |
| | BT12 | Đèn cảnh báo hai màu | Đèn ưu tiên cấp cứu chớp xen kẽ có khoảng nghỉ |
| **Phần D** | BT13 | Đèn báo nhiệt độ giả lập | Phân ngưỡng nhiệt độ thực tế bằng `if / else` |
| | BT14 | Bộ chọn 4 chế độ dùng switch | Cấu trúc rẽ nhiều nhánh `switch / case / default` |
| | BT15 | Tăng giảm cường độ sáng RGB | Hiệu ứng nhịp thở (Breathing LED) qua bước nhảy `for` |
| | BT16 | Tín hiệu SOS bằng LED | Mã hóa điện tín Morse quốc tế bằng 2 chu kỳ nháy |
| **Phần E** | BT17 | Giữ nút để bật LED | Đọc tín hiệu số nút bấm qua `button_pressed()` |
| | BT18 | Bấm một lần để đổi bật/tắt | Thuật toán phát hiện cạnh nhấn (Edge Detection) |
| | BT19 | Bộ đếm số lần nhấn | Đếm sự kiện xung nút bấm, cập nhật trạng thái |
| | BT20 | Nút bấm chuyển 3 màu vòng tròn | Máy trạng thái tuần hoàn (Finite State Machine) |
| **Phần F** | BT21 | Bài học lỗi thường gặp | Kỹ năng debug và khắc phục lỗi cú pháp C |
| | BT22 | Máy tính 4 phép | Menu lựa chọn phép toán và bảo vệ chia cho 0 |
| | BT23 | Bảng nhân LED | Vòng lặp in bảng cửu chương và nháy LED tương ứng |
| | BT24 | Mã Morse ký tự S và O | Tách module chương trình với hàm con tự tạo |
| | BT25 | Đèn giao thông có chế độ ban đêm | Điều khiển đa chu trình thông qua cờ trạng thái |
| | BT26 | Đèn RGB màu tự chọn | Pha màu 24-bit với giá trị trung gian $[0, 255]$ |
| | BT27 | LED điều chỉnh chu kỳ | Biến thiên tần số phát xung theo `period` |
| | BT28 | Chọn mode bằng nút nhấn | Chuyển đổi 3 cấp báo động (Normal - Warning - Danger) |
| | BT29 | Thống kê số nhấn lẻ/chẵn | Toán tử modulo `%` phân loại tính chẵn/lẻ |
| | BT30 | Trình diễn ánh sáng 20 giây | Tự thiết kế kịch bản ánh sáng kết hợp hàm và `for` |

---

## 🛠️ Quy Chuẩn Của Mỗi Bài Tập Trong Báo Cáo

Mỗi bài tập đều được trình bày đồng bộ theo 4 phần:
1. **Mã nguồn**: Code C hoàn chỉnh, chuẩn cú pháp OhStem (`#include "ohstem.h"`), định dạng đẹp qua gói `listings`.
2. **Giải thích các câu lệnh quan trọng**: Phân tích chi tiết chức năng của các hàm, biến và thuật toán xử lý.
3. **Kiểm thử (ảnh)**: Đã tạo sẵn khung hình `figure` có chú thích chuẩn. Để chèn ảnh, chỉ cần bỏ dấu `%` trước dòng `\includegraphics{...}` và thêm đường dẫn ảnh vào.
4. **Nhận xét, kết luận**: Đánh giá kết quả mô phỏng, độ chính xác so với yêu cầu đề bài.

---

## 🚀 Hướng Dẫn Biên Dịch Sang PDF

### 1. Yêu cầu môi trường
- Bộ cài TeX: **MiKTeX** hoặc **TeX Live**.
- Trình biên dịch khuyên dùng: **`pdflatex`** (đã cấu hình bảng mã UTF-8 với font Times Roman qua `[utf8]{vietnam}` và `mathptmx`).

### 2. Lệnh biên dịch bằng Terminal (PowerShell / Command Prompt)

Tại thư mục chứa dự án, chạy lệnh `pdflatex` **2 lần** để cập nhật mục lục và số trang chính xác:

```powershell
pdflatex -interaction=nonstopmode main.tex
pdflatex -interaction=nonstopmode main.tex
```

File kết quả **`main.pdf`** sẽ xuất hiện trực tiếp trong thư mục dự án.
