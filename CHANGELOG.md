# Nhật ký thay đổi

## 1.2.7 — 15/11/2026

- Thêm link các trang chính thống ngành thuế (đã mở thử ngày 15/11/2026): cổng Cục Thuế, phần mềm HTKK, thuế điện tử cho doanh nghiệp và cá nhân, dịch vụ công thuế, cổng hóa đơn điện tử, tra cứu hóa đơn, tra cứu người nộp thuế, Bộ Tài chính. Ghi chú cổng `etaxvn` chỉ dành cho nhà cung cấp nước ngoài.
- Quy tắc dùng nội dung trên trang Cục Thuế: văn bản quy phạm là nguồn nhóm 2; công văn hướng dẫn không phải văn bản quy phạm, nhãn tối đa ⚠️; mục hỏi đáp không dùng làm căn cứ; không ghi link dạng phiên làm việc.
- Nhóm 5: thêm mục 3.8 (nơi lấy mẫu, nơi nộp, nơi tra cứu) và 3 điểm dễ sai. Soạn văn bản: tờ khai thuế trỏ tới HTKK và cổng thuế điện tử.

## 1.2.6 — 15/11/2026

- Sửa lỗi: file mẫu `references/ho-so-doanh-nghiep-mau.md` bị `.gitignore` chặn nên thiếu trong kho và các bản zip trước. Đã thêm ngoại lệ để file được đưa vào kho.

## 1.2.5 — 15/11/2026

- README: mục **Skill làm được gì** viết chi tiết cho từng chức năng (dùng khi nào, cách gọi, skill làm gì, kết quả nhận được, giới hạn).

## 1.2.4 — 15/11/2026

- README: viết lại phần **Giới thiệu** theo mạch nỗi đau, vấn đề, giải pháp; thêm bảng **Skill làm được gì** (8 chức năng) và **Tra được gì** (8 nhóm, nội dung và câu hỏi ví dụ). Đưa phần Giới thiệu lên ngay sau khối miễn trừ trách nhiệm.

## 1.2.3 — 15/11/2026

- README: thêm mục **Nguồn tham khảo** (các trang đã dùng để tra cứu, xác minh, và cách dùng từng nhóm nguồn) và mục **Không chịu trách nhiệm**; thêm kênh yêu cầu chỉnh sửa hoặc gỡ bỏ qua GitHub Issues.

## 1.2.2 — 15/11/2026

- Thêm mục **Ghi công** trong README và LICENSE: skill được phát triển dựa trên skill "Tư vấn pháp luật" của tác giả Nguyễn Duy Tùng (duytung.vn). Nêu rõ phần kế thừa, phần làm lại, và giới hạn phạm vi của giấy phép MIT.

## 1.2.1 — 15/11/2026

- Thêm giấy phép MIT (`LICENSE`), ghi rõ cung cấp nguyên trạng, không bảo đảm.
- Thêm khối miễn trừ trách nhiệm ở đầu README: công cụ hỗ trợ tra cứu, không phải dịch vụ tư vấn pháp luật.

## 1.2.0 — 14/11/2026

- **Soạn văn bản theo chuẩn thể thức của Nghị định về công tác văn thư (Phụ lục I).** Đã đọc nguyên văn phạm vi áp dụng (bắt buộc với doanh nghiệp nhà nước, doanh nghiệp khác không bắt buộc), 9 thành phần thể thức, và các thông số trình bày: khổ A4, lề, phông Times New Roman, cỡ chữ từng thành phần, cách ghi nơi nhận, quyền hạn ký. Thông số được đưa vào kho trích dẫn (nhãn ⚠️ vì đọc từ bản đăng lại).
- Tính năng soạn văn bản mặc định trình bày theo Phụ lục I, có mẫu bố cục và danh sách cài đặt định dạng cho Word.
- Bộ kiểm thử: thêm câu 20.

## 1.1.1 — 14/11/2026

Xử lý các phần còn tồn của bản 1.1.0.

- **Đã đọc nguyên văn Thông tư hướng dẫn Luật Quản lý thuế (TT-QLT)** từ file ký số: tổ chức trả lương **khai thuế TNCN đã khấu trừ theo quý** từ 01/07/2026; danh sách 10 thông tư bị bãi bỏ (thông tư đăng ký thuế năm 2024 **vẫn còn hiệu lực**); mẫu tờ khai GTGT 01/GTGT; quy định chuyển tiếp. Đã đưa vào kho trích dẫn và lịch tuân thủ.
- **Hải quan:** thêm nghị định xử phạt hải quan mới (từ 01/07/2026), Luật Quản lý ngoại thương và nghị định hướng dẫn mới (từ tháng 9/2026), nghị định về khu công nghiệp, khu chế xuất.
- **Thuế GTGT:** nâng nhãn ✅ cho nghị định hướng dẫn; thêm thông tư hướng dẫn. **BHXH:** ghi văn bản bị thay thế của nghị định BHXH bắt buộc.
- **Đa nền tảng:** chạy thử thành công trên Antigravity CLI. Ghi chú Gemini CLI không còn hỗ trợ tài khoản cá nhân miễn phí.

## 1.1.0 — 14/11/2026

Mở rộng lĩnh vực và thêm tính năng soạn văn bản.

- **Module mới nhóm 8: Hải quan và xuất nhập khẩu.** Gồm Luật Hải quan (có luật sửa đổi năm 2026, hiệu lực 01/03/2027), Luật Thuế xuất khẩu, thuế nhập khẩu, luật sửa đổi năm 2025 về xuất nhập khẩu tại chỗ, nghị định và thông tư về thủ tục hải quan.
- **Tính năng mới: soạn văn bản theo mẫu** (`soan-van-ban.md`). Văn bản có mẫu bắt buộc thì chỉ hướng dẫn lấy mẫu chính thức và điền, không tự dựng mẫu. Văn bản nội bộ thì soạn có căn cứ, để `[...]` cho thông tin chưa biết.
- **Bổ sung căn cứ:**
  - Luật An toàn, vệ sinh lao động và nghị định về huấn luyện (nhóm 4).
  - Luật Hỗ trợ doanh nghiệp nhỏ và vừa và nghị định tiêu chí (nhóm 5, dùng để chọn chế độ kế toán).
  - Bộ luật Hình sự và luật sửa đổi năm 2025 (ngưỡng chuyển sang luật sư).
  - Luật Giao dịch điện tử, nghị định chữ ký điện tử (nhóm 3).
  - Nghị định khuyến mại và các lần sửa đổi năm 2024, 2026 (nhóm 3).
  - Luật Tố tụng hành chính, nghị quyết về thẩm quyền Tòa án, Luật Thi hành án dân sự mới (từ 01/07/2026), nghị quyết án phí (nhóm 7).
- Bộ kiểm thử: thêm 4 câu (hải quan, soạn văn bản, soạn văn bản có mẫu, an toàn lao động).
- Danh mục: 114 văn bản.

## 1.0.3 — 14/11/2026

Rà soát lại nhóm thuế và BHXH.

- **Thuế:**
  - Thêm thông tư hướng dẫn Luật Quản lý thuế 2025 (mã TT-QLT, hiệu lực 01/07/2026). Thông tư này có biểu mẫu tờ khai mới và bãi bỏ 10 thông tư cũ, trong đó có thông tư hướng dẫn quản lý thuế năm 2021. Đây là khoảng trống lớn nhất của các bản trước.
  - Xác định ngày hiệu lực của nghị định sửa đổi thuế TNDN năm 2026 (01/01/2026, hồi tố), nghị định sửa đổi thuế GTGT năm 2026 (20/06/2026) và nghị định sửa đổi xử phạt thuế (21/07/2026).
  - Ghi chú: kỳ khai TNCN đối với tiền lương có thể đã thay đổi từ 01/07/2026; thông tư đăng ký thuế cần kiểm tra lại.
- **BHXH:**
  - Thêm Luật Bảo hiểm y tế, luật sửa đổi năm 2024 và nghị định hướng dẫn; thông tư hướng dẫn BHXH bắt buộc; thông tư về sổ BHXH điện tử.
  - Nâng nhãn ✅ cho nghị định về bảo hiểm thất nghiệp.
  - Ghi chú danh sách luật sửa Luật BHXH chưa xác minh, và dự thảo sửa Luật BHXH đang lấy ý kiến.
- **Module:** nhóm 4, nhóm 5 và lịch tuân thủ trỏ tới các mã mới.

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
