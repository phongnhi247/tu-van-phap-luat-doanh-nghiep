# Tra cứu, trích dẫn và xử lý xung đột văn bản

## 1. Tra chéo 3 chiều

Mỗi căn cứ quan trọng phải được kiểm tra theo cả 3 chiều trước khi đưa vào câu trả lời.

### Chiều xuống: từ luật tới văn bản hướng dẫn

Luật thường chỉ quy định khung. Thủ tục, mẫu biểu, mức phạt và thời hạn chi tiết nằm trong nghị định và thông tư.

1. Đọc điều luật và tìm các cụm "Chính phủ quy định chi tiết", "Bộ trưởng Bộ ... hướng dẫn".
2. Tìm nghị định hướng dẫn. Kiểm tra cột Quan hệ trong `danh-muc-can-cu.md` trước, sau đó mới tìm web:
   - `"quy định chi tiết" "<tên luật>" nghị định`
3. Trong nghị định, tìm thông tư hướng dẫn tiếp theo cùng cách.
4. Phần mở đầu của nghị định luôn có dòng "Căn cứ Luật ...". Dùng dòng này để xác nhận nghị định hướng dẫn đúng luật đang hiệu lực, không phải luật cũ.

### Chiều ngang: sửa đổi, thay thế, bãi bỏ

1. Xem cột Quan hệ trong danh mục.
2. Tìm thêm trên web:
   - `"sửa đổi" "<số hiệu>"`
   - `"thay thế" "<số hiệu>"`
   - `"bãi bỏ" "<số hiệu>"`
3. Trên thuvienphapluat.vn, xem banner tình trạng hiệu lực, tab "Lược đồ" hoặc "Văn bản liên quan", và mục "Văn bản sửa đổi" hoặc "Văn bản thay thế".
4. Có văn bản hợp nhất (VBHN) thì đọc để biết nội dung hiện hành. Khi trích dẫn, vẫn ghi theo văn bản gốc và văn bản sửa đổi.

### Chiều thời gian: phiên bản tại thời điểm sự việc

1. Xác định ngày xảy ra sự việc.
2. So với ngày hiệu lực của từng phiên bản.
3. Sự việc kéo dài qua ngày văn bản mới có hiệu lực (ví dụ hợp đồng ký trước, vi phạm kéo dài) thì đọc điều khoản chuyển tiếp của văn bản mới.

## 2. Cú pháp tìm kiếm gợi ý

```
site:vbpl.vn "<số hiệu>"
site:thuvienphapluat.vn "<số hiệu>"
site:thuvienphapluat.vn "<tên luật>" "điều <X>"
"<từ khóa nghiệp vụ>" "nghị định" "<năm>"
"<từ khóa nghiệp vụ>" "có hiệu lực" "<năm>"
```

Sau khi tìm được URL thì đọc trang để lấy nguyên văn.

### Khi trang chặn hoặc không hiển thị nội dung

Một số trang chặn đọc tự động (ví dụ trả lỗi 403), hoặc chỉ hiện nội dung sau khi chạy JavaScript (ví dụ trang tra cứu của vbpl.vn). Khi đó, ưu tiên tìm **file gốc** dạng PDF hoặc DOC:

- `datafiles.chinhphu.vn/cpp/files/vbpq/...` (văn bản có chữ ký số của Chính phủ)
- `congbaocdn.chinhphu.vn/...` (Công báo)
- `vbpl.vn/TW/Lists/vbpq/Attachments/...` (file đính kèm trên cơ sở dữ liệu quốc gia)
- `static.luatvietnam.vn/...pdf` (file gốc, kể cả văn bản hợp nhất)

Truy vấn gợi ý: `"<số hiệu>" filetype:pdf` hoặc `"<số hiệu>" signed`.

Công cụ đọc web trả về PDF dạng nhị phân và nền tảng cho chạy lệnh: trích văn bản cục bộ bằng thư viện đọc PDF (ví dụ pymupdf). Lưu file tạm ngoài thư mục skill. Một số công cụ dòng lệnh đọc sai dấu tiếng Việt, nên kiểm tra lại câu chữ trước khi trích.

**PDF dạng scan** (trích chữ ra gần như rỗng): chuyển từng trang thành ảnh (ví dụ pymupdf `get_pixmap`) và đọc bằng khả năng nhìn ảnh của mô hình. Để không phải đọc cả trăm trang, hãy tìm số điều cần đọc trước (qua bài tóm tắt hoặc mục lục), rồi đoán trang theo tiến độ (thường mỗi trang khoảng 1–2 điều ở phần đầu văn bản) và mở thử vài trang quanh đó.

Ưu tiên tìm file trên `datafiles.chinhphu.vn`, `xdcs.cdnchinhphu.vn` (trang "Toàn văn" của xaydungchinhsach.chinhphu.vn có link file ký số) và Công báo **trước** khi thử thuvienphapluat.vn, vì trang này thường chặn cả công cụ đọc web lẫn lệnh tải.

Không lấy được toàn văn từ bất kỳ nguồn nào: gắn nhãn ⚠️ và không nêu con số.

## 3. Đọc số hiệu văn bản

| Dạng | Loại văn bản |
|---|---|
| `xx/yyyy/QHzz` | Luật hoặc Bộ luật do Quốc hội khóa zz ban hành |
| `xx/yyyy/NQ-QHzz`, `xx/yyyy/NQ-UBTVQHzz` | Nghị quyết của Quốc hội hoặc Ủy ban Thường vụ Quốc hội |
| `xx/yyyy/NĐ-CP` | Nghị định của Chính phủ |
| `xx/yyyy/NQ-CP` | Nghị quyết của Chính phủ |
| `xx/yyyy/QĐ-TTg` | Quyết định của Thủ tướng |
| `xx/yyyy/TT-<Bộ>` | Thông tư, ví dụ TT-BTC (Bộ Tài chính), TT-BNV (Bộ Nội vụ) |
| `xx/VBHN-<cơ quan>` | Văn bản hợp nhất. Không phải văn bản mới, chỉ gộp nội dung đã sửa đổi |
| `xx/<cơ quan>-<đơn vị>` không có năm ở giữa | Công văn: không phải văn bản quy phạm pháp luật, chỉ có giá trị tham khảo |

## 4. Thứ bậc văn bản

Văn bản cấp trên có giá trị pháp lý cao hơn văn bản cấp dưới. Danh sách đầy đủ các loại văn bản nằm trong luật ban hành văn bản quy phạm pháp luật hiện hành ([LBHVB] cùng văn bản sửa đổi [LBHVB-SD] trong danh mục). Khi cần trích dẫn chính xác thứ bậc, mở Điều 4 của luật này để đọc.

Thứ bậc rút gọn hay dùng trong tư vấn doanh nghiệp:

1. Hiến pháp
2. Bộ luật, Luật, Nghị quyết của Quốc hội
3. Pháp lệnh, Nghị quyết của Ủy ban Thường vụ Quốc hội
4. Nghị định, Nghị quyết của Chính phủ
5. Quyết định của Thủ tướng Chính phủ
6. Nghị quyết của Hội đồng Thẩm phán Tòa án nhân dân tối cao
7. Thông tư của Bộ trưởng
8. Văn bản của chính quyền địa phương cấp tỉnh, rồi cấp xã. Cấp huyện không còn từ 01/07/2025.

**Không phải văn bản quy phạm pháp luật:** công văn, văn bản hợp nhất, quyết định cá biệt (ví dụ quyết định xử phạt một doanh nghiệp cụ thể), bài hỏi đáp. Những văn bản này chỉ có giá trị tham khảo hoặc chỉ áp dụng cho trường hợp cụ thể đó.

## 5. Xử lý xung đột

Khi hai văn bản trở lên quy định khác nhau về cùng một vấn đề:

1. **Văn bản cấp cao hơn được áp dụng trước** (lex superior). Ví dụ luật được áp dụng trước nghị định.
2. **Cùng cấp thì văn bản ban hành sau được áp dụng trước** (lex posterior).
3. **Cùng cấp thì văn bản chuyên ngành được áp dụng trước văn bản chung** (lex specialis). Ví dụ luật thuế được áp dụng trước Bộ luật Dân sự về nghĩa vụ thuế.
4. Luật chuyên ngành có điều khoản ưu tiên áp dụng riêng thì đọc và trích điều khoản đó.

Ba quy tắc trên không phân định được thì trình bày Tuyến A và Tuyến B với các điều, khoản mâu thuẫn, chấm điểm theo bảng phương án, và khuyến nghị gửi văn bản hỏi cơ quan có thẩm quyền.

## 6. Chuẩn trích dẫn

Mỗi trích dẫn có đủ 4 phần:

1. **Tọa độ:** `[Mã] <Cấp văn bản> <số hiệu> – Điều X, Khoản Y, Điểm Z`
   - Viết tắt cấp văn bản: BL (Bộ luật), Luật, NQ, NĐ, QĐ, TT.
2. **Nguyên văn:** chép đúng câu chữ, dấu câu và cách đánh số của văn bản. Phần lược bỏ ghi `[...]`. Không diễn giải bên trong dấu ngoặc kép.
3. **Trạng thái tại thời điểm sự việc:** `đang hiệu lực`, `đã sửa đổi bởi <mã/số hiệu>`, `hết hiệu lực`, hoặc `áp dụng theo chuyển tiếp`.
4. **Ngày hiệu lực** theo định dạng DD/MM/YYYY (ngày bắt đầu có hiệu lực, không phải ngày ban hành), kèm **link nguồn**.

Ngày tháng luôn viết theo định dạng DD/MM/YYYY.
