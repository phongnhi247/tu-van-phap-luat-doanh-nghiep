# Lịch tuân thủ

Dùng khi người dùng hỏi "tháng hoặc quý này phải nộp gì", "hạn nộp ... là khi nào", hoặc "lịch nộp năm".

> **Không ghi hạn nộp cố định trong file này.** Hạn nộp đã thay đổi khi luật quản lý thuế mới có hiệu lực từ 01/07/2026, và có thể còn thay đổi tiếp. Mỗi lần trả lời phải tra nguyên văn điều khoản quy định hạn nộp.

## 1. Quy trình trả lời

1. **Đọc hồ sơ doanh nghiệp.** Cần các thông tin: phương pháp và kỳ kê khai thuế GTGT (tháng hay quý), có người lao động không và có khấu trừ TNCN không, năm tài chính, loại hình, số lao động, có lao động nước ngoài không, có giao dịch liên kết không, doanh nghiệp có thuộc diện phải kiểm toán báo cáo tài chính không. Thiếu thông tin nào thì hỏi người dùng.
2. **Xác định khoảng thời gian** người dùng hỏi: tháng, quý hay năm.
3. **Lọc bảng nghĩa vụ** ở mục 2, chỉ giữ những nghĩa vụ áp dụng cho doanh nghiệp này.
4. **Tra nguyên văn hạn nộp** của từng nghĩa vụ theo cột Căn cứ. Hạn nộp hồ sơ khai thuế theo tháng, quý, năm và quyết toán đã có nguyên văn trong `trich-dan-xac-minh.md` (mục ND-QLT Điều 10); hạn nộp tiền thuế trùng ngày cuối của hạn nộp hồ sơ khai (mục LQLT). Hạn nộp rơi vào ngày nghỉ: LQLT và ND-QLT không có quy định riêng, nên áp dụng quy tắc chung của BLDS về ngày cuối cùng của thời hạn là ngày nghỉ (xem `trich-dan-xac-minh.md`, mục ND-QLT Điều 10). Với hạn rơi vào tháng 1 hoặc tháng 2, kiểm tra thêm lịch nghỉ Tết của năm đó. Luôn khuyến nghị nộp trước ngày nghỉ. Tạm nộp TNDN quý 4 có ngưỡng tối thiểu tính trên số quyết toán năm (ND-QLT Điều 24, có trong kho trích dẫn).
5. **Trả lời bằng bảng** sắp theo ngày:

| Hạn | Việc | Ai làm | Căn cứ (trích dẫn) | Phạt nếu trễ (trích dẫn) | Nhãn |
|---|---|---|---|---|---|

6. Thêm phần **"Cần lưu ý thêm"**: nghĩa vụ phát sinh theo sự kiện, không định kỳ (mục 3), nếu doanh nghiệp có thể gặp trong khoảng thời gian đó.
7. Đề nghị người dùng lưu lịch vào file `lich-tuan-thu-<nam>.md` trong thư mục làm việc nếu họ muốn.

## 2. Nghĩa vụ định kỳ

| Nghĩa vụ | Đối tượng | Căn cứ để tra hạn nộp và mẫu biểu |
|---|---|---|
| Tờ khai thuế GTGT theo tháng hoặc quý | Doanh nghiệp kê khai GTGT | LQLT, ND-QLT, LGTGT |
| Tờ khai khấu trừ TNCN đối với tiền lương, tiền công: **khai theo quý** từ 01/07/2026 (TT-QLT Điều 22 khoản 1, có trong kho trích dẫn). Kỳ trước 01/07/2026 theo quy định cũ | Tổ chức trả thu nhập | LQLT, ND-QLT, TT-QLT, LTNCN, ND-TNCN |
| Nộp thuế: hạn nộp tiền thuế theo từng kỳ | Người nộp thuế | LQLT, ND-QLT |
| Tạm nộp thuế TNDN theo quý; tổng tạm nộp các quý đạt tỷ lệ tối thiểu theo quy định | Doanh nghiệp nộp TNDN | LTNDN, ND-TNDN, ND-TNDN-SD, LQLT |
| Quyết toán thuế TNDN năm | Doanh nghiệp | LQLT, ND-QLT, LTNDN |
| Quyết toán thuế TNCN năm, gồm cả quyết toán thay người lao động | Tổ chức trả thu nhập | LQLT, ND-QLT, LTNCN, ND-TNCN |
| Phụ lục giao dịch liên kết (nộp cùng quyết toán TNDN) | Doanh nghiệp có giao dịch liên kết | ND-GDLK |
| Báo cáo tài chính năm: nộp cho cơ quan thuế và các cơ quan khác theo quy định | Doanh nghiệp | LKT, TT-KTDN, TT-KTDNNV hoặc TT-KTSN, LQLT |
| Đóng BHXH, BHYT, BHTN hằng tháng (hoặc theo phương thức đã đăng ký) | Người sử dụng lao động | LBHXH, ND-BHXH, TT-BHXH, LBHYT, LBHYT-SD, LVL, ND-BHTN |
| Kinh phí công đoàn: 2% quỹ tiền lương làm căn cứ đóng BHXH bắt buộc | Người sử dụng lao động | LCDOAN Điều 29 khoản 1 điểm b (✅, xem `trich-dan-xac-minh.md`). Phương thức, thời hạn đóng do Chính phủ quy định, văn bản này chưa có trong danh mục |
| Báo cáo tình hình sử dụng lao động (định kỳ) | Người sử dụng lao động | BLLD, ND-QHLD. Phải kiểm tra vì có dự thảo sửa đổi năm 2026 đơn giản hóa chế độ báo cáo |
| Báo cáo sử dụng người lao động nước ngoài: định kỳ trước ngày 05/6 và 05/12 hằng năm (từ 05/12/2026), trừ khi thông tin đã có trong cơ sở dữ liệu người lao động nước ngoài | Doanh nghiệp có lao động nước ngoài | ND-LDNN-26 Điều 37 khoản 6 điểm đ (✅, xem `trich-dan-xac-minh.md`); trước 05/12/2026 là ND-LDNN |
| Báo cáo công tác bảo vệ môi trường | Cơ sở thuộc diện | ND-BVMT |
| Lệ phí môn bài | **Không còn từ năm 2026** | NQ-KTTN |

Bảng này là danh sách để kiểm tra, không phải danh sách đầy đủ cho mọi ngành. Doanh nghiệp ngành đặc thù (tài chính, xây dựng, xuất nhập khẩu...) có thêm báo cáo chuyên ngành. Với các ngành này, skill phải nói rõ là chưa bao gồm.

## 3. Nghĩa vụ phát sinh theo sự kiện

| Sự kiện | Việc cần làm | Căn cứ |
|---|---|---|
| Thay đổi thông tin đăng ký doanh nghiệp | Đăng ký hoặc thông báo thay đổi trong thời hạn | ND-DKDN, ND-DKDN-SD |
| Thay đổi chủ sở hữu hưởng lợi | Cập nhật thông tin | LDN-SD25, ND-DKDN-SD |
| Tuyển hoặc chấm dứt hợp đồng với người lao động | Báo tăng hoặc giảm lao động tham gia BHXH | LBHXH, ND-BHXH |
| Phát hiện hóa đơn sai | Xử lý theo quy định về hóa đơn sai sót | ND-HDDT |
| Tạm ngừng kinh doanh | Thông báo trước thời hạn luật định | ND-DKDN, ND-DKDN-SD, LQLT |
| Chuyển nhượng vốn của cá nhân | Khai thuế TNCN | LTNCN, ND-TNCN, LQLT |
| Rò rỉ dữ liệu cá nhân | Thông báo trong thời hạn | LBVDLCN, ND-BVDLCN |

## 4. Lịch quý 1/2027 (dựng sẵn)

Mục này là ngoại lệ của nguyên tắc "không ghi hạn cố định": dựng sẵn vì quý 1/2027 có nhiều mốc dồn lại. Ngày được tính từ các điều khoản đã đọc nguyên văn. Trước khi dùng vẫn phải: (1) chạy "cập nhật căn cứ" để chắc không có văn bản mới thay đổi hạn; (2) lọc theo hồ sơ doanh nghiệp; (3) kiểm tra lịch nghỉ Tết Nguyên đán 2027 (mùng 1 Tết là thứ Bảy 06/02/2027; lịch nghỉ chính thức chưa có trong danh mục).

**Hạn trùng ngày nghỉ:** LQLT và ND-QLT không có quy định riêng. Áp dụng quy tắc chung của BLDS về ngày cuối cùng của thời hạn là ngày nghỉ (⚠️, chưa đọc nguyên văn điều của BLDS). Luôn khuyến nghị nộp trước ngày nghỉ.

| Hạn | Thứ | Việc | Ai làm | Căn cứ | Nhãn |
|---|---|---|---|---|---|
| 01/01/2027 | Thứ Sáu | Áp dụng lương tối thiểu vùng mới; hết mức giảm thuế GTGT 8% (nếu không gia hạn); hợp đồng lao động điện tử giao kết theo điều kiện mới | Người sử dụng lao động; người bán hàng | ND-LTT-2027 Điều 5; NQ-GTGT-GIAM Điều 2; NQ-HDLDDT Điều 1 | ✅ |
| 20/01/2027 | Thứ Tư | Tờ khai GTGT tháng 12/2026 (doanh nghiệp khai theo tháng) | Doanh nghiệp khai GTGT theo tháng | ND-QLT Điều 10 khoản 2 | ✅ |
| 31/01/2027 | Chủ nhật | Tờ khai GTGT quý 4/2026 (khai theo quý); tờ khai khấu trừ TNCN quý 4/2026; hạn tạm nộp TNDN quý 4/2026 (kiểm tra mức 80%) | Doanh nghiệp tương ứng | ND-QLT Điều 10 khoản 3, Điều 24 khoản 2, 3; TT-QLT Điều 22 | ✅ ngày theo điều khoản; ⚠️ cách lùi khi trùng ngày nghỉ |
| 20/02/2027 | Thứ Bảy | Tờ khai GTGT tháng 01/2027 | Doanh nghiệp khai theo tháng | ND-QLT Điều 10 khoản 2 | ✅ ngày; ⚠️ trùng ngày nghỉ, kiểm tra lịch nghỉ Tết |
| 20/03/2027 | Thứ Bảy | Tờ khai GTGT tháng 02/2027 | Doanh nghiệp khai theo tháng | ND-QLT Điều 10 khoản 2 | ✅ ngày; ⚠️ trùng ngày nghỉ |
| 31/03/2027 | Thứ Tư | Quyết toán thuế TNDN năm 2026 và nộp số thuế còn thiếu; quyết toán thuế TNCN năm 2026 của tổ chức trả thu nhập (gồm quyết toán thay); phụ lục giao dịch liên kết | Doanh nghiệp; tổ chức trả thu nhập | ND-QLT Điều 10 khoản 5 điểm a; LQLT Điều 14; ND-GDLK | ✅ (LQLT ⚠️) |
| 30/04/2027 | Thứ Sáu, ngày lễ | Cá nhân tự quyết toán thuế TNCN năm 2026 | Cá nhân | ND-QLT Điều 10 khoản 5 điểm c | ✅ ngày; ⚠️ trùng ngày nghỉ lễ |

Không ghi vào bảng các nghĩa vụ chưa đọc được hạn nguyên văn: đóng BHXH hằng tháng, kinh phí công đoàn, báo cáo tài chính năm, báo cáo tình hình sử dụng lao động. Với các nghĩa vụ này, tra căn cứ ở mục 2 trước khi nêu ngày. Xem thêm `quyet-toan-va-chuyen-nam.md`.

## 5. Mẫu trả lời

> **Lịch tuân thủ tháng MM/YYYY — <Tên doanh nghiệp>** (theo hồ sơ: kê khai GTGT theo quý, có khấu trừ TNCN theo tháng, N lao động)
>
> | Hạn | Việc | Căn cứ | Nhãn |
> |---|---|---|---|
> | DD/MM | Nộp tờ khai khấu trừ TNCN tháng trước | [ND-QLT] Điều ..., "[trích]" | ✅ |
> | ... | ... | ... | ... |
>
> **Không áp dụng tháng này:** tờ khai GTGT, vì doanh nghiệp kê khai theo quý.
> **Cần lưu ý thêm:** ...
>
> *Căn cứ tính đến <baseline> (skill v<VERSION>). Nội dung mang tính tham khảo, không thay thế ý kiến pháp lý chính thức.*
