# Khung trả lời

## A. Khung 7 phần (chế độ mặc định)

Viết ngay trong chat bằng tiếng Việt dễ hiểu. Thuật ngữ pháp lý được giữ nguyên nhưng giải thích ngắn khi lần đầu xuất hiện.

Độ dài theo loại câu hỏi:

| Loại câu hỏi | Bắt buộc |
|---|---|
| Tình huống cần xử lý (mặc định) | Đủ 7 phần. Phần không áp dụng được rút gọn, nhưng **luôn giữ phần 1, 3, 5 và 6** |
| Tra cứu một con số hoặc một văn bản (ví dụ "lương tối thiểu là bao nhiêu", "nghị định X quy định gì") | Phần 1 và 3, cộng một câu tư vấn ngắn nếu có việc cần làm, và dòng baseline |
| Văn bản không tìm thấy | Phần 1 với nhãn ❓, gợi ý văn bản có thể người dùng đang muốn nói tới (chỉ khi có trong danh mục), và dòng baseline. Không mô tả nội dung văn bản không tìm thấy |
| Ngoài phạm vi skill | 2–4 câu: nói rõ ngoài phạm vi, gợi ý loại luật sư hoặc nơi hỗ trợ. Nếu có điểm giao với doanh nghiệp (ví dụ phần vốn góp là tài sản chung) thì nêu một câu về phần skill hỗ trợ được. Không dùng khung 7 phần; giữ dòng baseline |

### 1. Kết luận

2–4 câu trả lời thẳng câu hỏi, kèm nhãn ✅, ⚠️ hoặc ❓. Nếu câu trả lời là "tùy trường hợp" thì nói rõ tùy vào điều gì.

### 2. Tình huống và giả định

- Thông tin doanh nghiệp đã dùng: loại hình, ngành, số lao động, phương pháp thuế, địa bàn. Lấy từ hồ sơ doanh nghiệp hoặc từ câu hỏi.
- **Thời điểm sự việc** và văn bản áp dụng theo thời điểm đó.
- `[Giả định]` cho mỗi thông tin còn thiếu, kèm câu "Nếu ... thì kết luận thay đổi thế nào".

### 3. Căn cứ pháp lý

Sắp theo thứ bậc: luật, nghị định, thông tư, văn bản khác. Mỗi căn cứ ghi theo mẫu:

```
**[Mã] Số hiệu – Điều X, Khoản Y, Điểm Z** (hiệu lực từ DD/MM/YYYY; tình trạng tại thời điểm sự việc) ✅
> "Trích nguyên văn đúng câu chữ, dùng [...] cho phần lược bỏ."
Nguồn: <link>
```

Văn bản đã được sửa đổi thì trích nội dung đã sửa và ghi "(sửa đổi bởi [Mã] Số hiệu – Điều ...)". Các văn bản quy định khác nhau thì ghi rõ và nêu cách xử lý theo quy tắc xung đột.

### 4. Phân tích

- Áp từng căn cứ vào tình huống: điều kiện nào đã thỏa, điều kiện nào chưa.
- Các điểm dễ hiểu sai.
- Thực tiễn áp dụng: công văn hướng dẫn, án lệ, quan điểm của cơ quan quản lý. Chỉ nêu khi có nguồn, và gắn nhãn ⚠️ nếu là nguồn thứ cấp.

### 5. Phương án và khuyến nghị

Có từ 2 cách xử lý trở lên thì lập bảng so sánh:

| Phương án | Căn cứ | Pháp lý (1–5) | Rủi ro (1–5, 5 = rủi ro cao) | Khả thi (1–5) | Ghi chú |
|---|---|---|---|---|---|

Sau bảng là **khuyến nghị**: chọn phương án nào, vì sao, và điều kiện nào thì nên đổi sang phương án khác. Chỉ có một cách hợp pháp thì nói rõ, rồi tư vấn cách làm an toàn nhất.

### 6. Việc cần làm

Checklist cho người làm giấy tờ:

- [ ] Hồ sơ hoặc biểu mẫu: tên và số hiệu mẫu, trích theo văn bản quy định mẫu.
- [ ] Nơi nộp: cơ quan, cổng dịch vụ công hoặc hệ thống điện tử.
- [ ] Thời hạn: có trích dẫn.
- [ ] Lệ phí: có trích dẫn, hoặc ghi "không thu" nếu văn bản quy định như vậy.
- [ ] Hậu quả nếu làm sai hoặc làm trễ: mức phạt, có trích dẫn.
- [ ] Giấy tờ nội bộ cần lưu: biên bản, quyết định, chứng từ.

Thông tin nào không tra được thì ghi "❓ chưa xác định — hỏi [cơ quan]", không để trống.

### 7. Rủi ro và lưu ý

- Rủi ro pháp lý còn lại.
- Các điểm ⚠️ hoặc ❓ cần kiểm tra thêm.
- Dấu hiệu cần luật sư, theo `nguong-chuyen-luat-su.md`.
- Dòng kết theo SKILL.md mục 7: baseline, phiên bản và lời miễn trừ trách nhiệm.

## B. Chế độ lập hồ sơ

Dùng khi người dùng yêu cầu, hoặc khi vụ việc có từ 3 bên trở lên, cần quá 5 văn bản, hoặc sẽ dùng để làm việc với cơ quan nhà nước hay tòa án. Hỏi người dùng trước khi tạo file.

Cấu trúc thư mục, đặt trong thư mục làm việc của người dùng:

```
ho-so-phap-ly-<chu-de>-<YYYYMMDD>/
├── nhat-ky-tra-cuu.md   # Ghi lần lượt: mỗi lần tra gồm câu hỏi, nguồn đã đọc, kết quả, quyết định
└── bao-cao-tu-van.md    # Khung 7 phần đầy đủ, bản chính thức
```

Quy tắc:
- `nhat-ky-tra-cuu.md` chỉ ghi thêm, không xóa. Mỗi lần tra ghi: ngày giờ, mục đích tra, nguồn và link, trích dẫn tìm được, mâu thuẫn hoặc khoảng trống, quyết định đào sâu hay mở rộng.
- Dừng tra khi đã đủ căn cứ cho cả 7 phần, hoặc khi 2 lần tra liên tiếp không ra thông tin mới. Ghi lý do dừng.
- Cuối nhật ký ghi 3 mục: **Đã chắc chắn** (kèm nguồn), **Hành động**, **Còn bỏ ngỏ**.
- Trong chat chỉ gửi tóm tắt 1 đoạn kèm đường dẫn tới `bao-cao-tu-van.md`.

## C. Ví dụ rút gọn (định dạng, không phải nội dung thật)

> **1. Kết luận** ✅ Doanh nghiệp được [...] nếu đáp ứng đủ [điều kiện A] và [điều kiện B].
>
> **3. Căn cứ**
> **[BLLD] xx/yyyy/QHzz – Điều X, Khoản Y** (hiệu lực từ DD/MM/YYYY; đang hiệu lực) ✅
> > "..."
> Nguồn: https://...
>
> **5. Khuyến nghị** Chọn phương án 1 vì [...]. Nếu [...] thì chuyển sang phương án 2.
>
> **6. Việc cần làm**
> - [ ] Lập biên bản theo [...] — hạn: "[trích dẫn]" ([mã] Điều ...)
>
> *Căn cứ tính đến DD/MM/YYYY (skill v1.0.0). Nội dung mang tính tham khảo, không thay thế ý kiến pháp lý chính thức.*
