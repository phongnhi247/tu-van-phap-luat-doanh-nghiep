# Nhật ký thay đổi

## 1.0.2 — 14/11/2026

Đã chạy lại câu 7 (hạn nộp tờ khai GTGT quý 4) và câu 12 (lịch tuân thủ tháng 1/2027) trên bản 1.0.1: cả hai đều đạt. **Đủ 15/15 câu kiểm thử đạt.**

- Kho trích dẫn: thêm điều về tạm nộp thuế TNDN theo quý (ND-QLT Điều 24). Ghi rõ Luật Quản lý thuế và nghị định hướng dẫn không có quy tắc riêng khi hạn nộp trùng ngày nghỉ, nên áp dụng quy tắc chung của Bộ luật Dân sự.
- Lịch tuân thủ: thêm việc kiểm tra lịch nghỉ Tết cho các hạn nộp rơi vào tháng 1, tháng 2; thêm ngưỡng tạm nộp TNDN quý 4.
- Danh mục: ghi các luật sửa Luật BHXH năm 2025 (chưa xác minh) và nguồn đọc được của Bộ luật Dân sự về cách tính thời hạn.
- Bộ kiểm thử: thống nhất cách chấm trường hợp hạn nộp trùng ngày nghỉ, và cách chấm khi lệ phí môn bài được nhắc ở mục "không áp dụng".

## 1.0.1 — 14/11/2026

Sửa sau khi chạy đủ 15 câu kiểm thử: 13 câu đạt ngay; 2 câu về hạn nộp thuế (7 và 12) chưa đạt vì không đọc được văn bản, và đã được khắc phục trong bản này.

- **Mới:** `references/trich-dan-xac-minh.md`, kho các đoạn trích nguyên văn đã đối chiếu với file gốc. Gồm: hạn nộp hồ sơ khai thuế (ND-QLT Điều 10), các điều của Luật Quản lý thuế về hạn nộp, khai bổ sung và tiền chậm nộp, xử lý hóa đơn sai sót (TT-HDDT Điều 10), mức phạt chậm đóng BHXH, lương tối thiểu 2027, chuyển nhượng vốn trong công ty TNHH, các điều Bộ luật Lao động về kỷ luật và thử việc. Skill dùng được kho này cả khi không tra được web.
- **Sửa sai:** nghị định xử phạt lao động, BHXH năm 2026 **thay thế** nghị định năm 2022, không phải chỉ sửa đổi. Mã ND-XPLD nay trỏ vào văn bản mới; văn bản cũ chuyển xuống mục hết hiệu lực, kèm quy tắc chuyển tiếp.
- **Danh mục:** nâng nhãn ✅ cho nhiều dòng (Luật Doanh nghiệp và luật sửa đổi 2025, nghị định đăng ký doanh nghiệp, nghị định hướng dẫn Luật Đầu tư, Nghị quyết 198, Luật Thuế GTGT, Luật BHXH, Luật Bảo vệ dữ liệu cá nhân, nghị định hướng dẫn Luật Quản lý thuế, nghị định và thông tư hóa đơn). Thêm: luật sửa đổi Luật Thuế GTGT có hiệu lực từ 01/01/2026, nghị định hướng dẫn Nghị quyết 198, nghị định thuế hộ kinh doanh, thông tư về người nộp thuế rủi ro cao, luật sửa đổi Luật Công đoàn. Ghi các mốc hiệu lực riêng và quy định chuyển tiếp của Luật Quản lý thuế. Cập nhật các luật sửa Bộ luật Lao động và văn bản hợp nhất năm 2026.
- **Hướng dẫn:**
  - File có chữ ký số được coi là nguồn gốc dù tải từ đâu.
  - Nhãn ⚠️ không được kèm con số.
  - Thêm cách đọc PDF dạng scan và thứ tự nguồn khi trang bị chặn.
  - Thêm điểm khai bổ sung khi đang bị thanh tra (nhóm 7).
  - Xác định doanh nghiệp nhỏ và vừa trước khi chọn chế độ kế toán (nhóm 5).
  - Thêm độ dài câu trả lời theo loại câu hỏi.
- **Gem:** bản đóng gói cho Gem có thêm kho trích dẫn (7 file).

## 1.0.0 — 14/11/2026

Bản đầu tiên. Xây lại từ skill tư vấn pháp luật tổng quát `tu-van-phap-luat` (baseline 20/07/2026), chuyển sang chuyên cho doanh nghiệp.

### Thay đổi so với skill cũ

- **Phạm vi:** bỏ dân sự cá nhân, hôn nhân, hình sự cá nhân, đất đai hộ gia đình. Tổ chức lại thành 7 nhóm theo vòng đời doanh nghiệp.
- **Một danh mục căn cứ duy nhất** (`references/danh-muc-can-cu.md`). Các file khác chỉ dùng mã văn bản. Khi luật thay đổi, chỉ cần sửa một dòng.
- **Nguyên tắc "chỉ nói khi có căn cứ"** với 3 nhãn ✅ ⚠️ ❓. Mọi con số phải có trích dẫn nguyên văn.
- **Mặc định trả lời chuyên sâu** ngay trong chat theo khung 7 phần. Chế độ lập hồ sơ (ghi file) chỉ dùng khi cần, thay cho việc mọi câu hỏi đều phải tạo thư mục và nhật ký như trước.
- **Tính năng mới:** lịch tuân thủ, rà soát văn bản (5 checklist), hồ sơ doanh nghiệp lưu ngoài thư mục skill, ngưỡng chuyển sang luật sư, lệnh "cập nhật căn cứ", bộ 15 câu hỏi kiểm thử.
- **Chạy được trên nhiều nền tảng:** hướng dẫn công cụ viết theo chức năng, có bảng tương ứng cho Claude, Gemini và Antigravity; có hướng dẫn tạo Gem.

### Căn cứ cập nhật so với skill cũ

- Đầu tư: nghị định hướng dẫn mới (mã ND-DT) thay nghị định năm 2021.
- Đăng ký doanh nghiệp: thêm nghị định sửa đổi năm 2026 (mã ND-DKDN-SD).
- Lệ phí môn bài: chấm dứt thu từ 01/01/2026 (mã NQ-KTTN).
- Quản lý thuế: luật mới và nghị định hướng dẫn có hiệu lực từ 01/07/2026 (mã LQLT, ND-QLT).
- Hóa đơn: nghị định và thông tư mới từ 01/07/2026 (mã ND-HDDT, TT-HDDT), thay nghị định hóa đơn năm 2020.
- Đăng ký thuế: thông tư năm 2024 (mã TT-DKT) thay thông tư năm 2020.
- Thuế TNCN và TNDN: thêm nghị định, thông tư hướng dẫn năm 2025–2026.
- Xử phạt thuế và hóa đơn: thêm các nghị định sửa đổi năm 2025–2026.
- Giao dịch liên kết: nghị định mới từ 01/07/2026 (mã ND-GDLK).
- Kế toán: thông tư chế độ kế toán doanh nghiệp mới từ 01/01/2026 (mã TT-KTDN).
- Lao động: lương tối thiểu từ 01/01/2027 (mã ND-LTT-2027); nghị định sửa đổi về xử phạt lao động và BHXH từ 10/09/2026 (mã ND-XPLD-SD); hợp đồng lao động điện tử; lao động nước ngoài; Luật Việc làm và nghị định về bảo hiểm thất nghiệp.
- Dữ liệu cá nhân: luật và nghị định mới từ 01/01/2026, thay nghị định năm 2023.
- Thương mại điện tử, quảng cáo, sở hữu trí tuệ, môi trường, PCCC, thanh tra, khiếu nại, phá sản: cập nhật theo văn bản năm 2025–2026.
- Tố tụng: Tòa án nhân dân khu vực thay cho Tòa án cấp huyện từ 01/07/2025. Thứ bậc văn bản bỏ cấp huyện.

### Đã biết

- Nhiều dòng trong danh mục còn nhãn ⚠️. Ưu tiên nâng nhãn ở bản 1.0.x.
- Đang theo dõi: dự án sửa Luật Thương mại, Luật Cạnh tranh, Luật Bảo vệ quyền lợi người tiêu dùng (năm 2026); dự thảo sửa nghị định hướng dẫn Bộ luật Lao động; dự thảo thông tư thay chế độ kế toán doanh nghiệp nhỏ và vừa.
