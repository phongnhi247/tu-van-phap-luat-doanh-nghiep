# Lịch tuân thủ

Dùng khi người dùng hỏi "tháng hoặc quý này phải nộp gì", "hạn nộp ... là khi nào", hoặc "lịch nộp năm".

> **Không ghi hạn nộp cố định trong file này.** Hạn nộp đã thay đổi khi luật quản lý thuế mới có hiệu lực từ 01/07/2026, và có thể còn thay đổi tiếp. Mỗi lần trả lời phải tra nguyên văn điều khoản quy định hạn nộp.

## 1. Quy trình trả lời

1. **Đọc hồ sơ doanh nghiệp.** Cần các thông tin: phương pháp và kỳ kê khai thuế GTGT (tháng hay quý), có người lao động không và có khấu trừ TNCN không, năm tài chính, loại hình, số lao động, có lao động nước ngoài không, có giao dịch liên kết không, doanh nghiệp có thuộc diện phải kiểm toán báo cáo tài chính không. Thiếu thông tin nào thì hỏi người dùng.
2. **Xác định khoảng thời gian** người dùng hỏi: tháng, quý hay năm.
3. **Lọc bảng nghĩa vụ** ở mục 2, chỉ giữ những nghĩa vụ áp dụng cho doanh nghiệp này.
4. **Tra nguyên văn hạn nộp** của từng nghĩa vụ theo cột Căn cứ. Hạn nộp hồ sơ khai thuế theo tháng, quý, năm và quyết toán đã có nguyên văn trong `trich-dan-xac-minh.md` (mục ND-QLT Điều 10); hạn nộp tiền thuế trùng ngày cuối của hạn nộp hồ sơ khai (mục LQLT). Hạn nộp rơi vào ngày nghỉ thì tra quy định về cách tính thời hạn (LQLT, ND-QLT, BLDS) để xác định ngày làm việc tiếp theo.
5. **Trả lời bằng bảng** sắp theo ngày:

| Hạn | Việc | Ai làm | Căn cứ (trích dẫn) | Phạt nếu trễ (trích dẫn) | Nhãn |
|---|---|---|---|---|---|

6. Thêm phần **"Cần lưu ý thêm"**: nghĩa vụ phát sinh theo sự kiện, không định kỳ (mục 3), nếu doanh nghiệp có thể gặp trong khoảng thời gian đó.
7. Đề nghị người dùng lưu lịch vào file `lich-tuan-thu-<nam>.md` trong thư mục làm việc nếu họ muốn.

## 2. Nghĩa vụ định kỳ

| Nghĩa vụ | Đối tượng | Căn cứ để tra hạn nộp và mẫu biểu |
|---|---|---|
| Tờ khai thuế GTGT theo tháng hoặc quý | Doanh nghiệp kê khai GTGT | LQLT, ND-QLT, LGTGT |
| Tờ khai khấu trừ TNCN theo tháng hoặc quý (nếu phát sinh khấu trừ) | Tổ chức trả thu nhập | LQLT, ND-QLT, LTNCN, ND-TNCN |
| Nộp thuế: hạn nộp tiền thuế theo từng kỳ | Người nộp thuế | LQLT, ND-QLT |
| Tạm nộp thuế TNDN theo quý; tổng tạm nộp các quý đạt tỷ lệ tối thiểu theo quy định | Doanh nghiệp nộp TNDN | LTNDN, ND-TNDN, ND-TNDN-SD, LQLT |
| Quyết toán thuế TNDN năm | Doanh nghiệp | LQLT, ND-QLT, LTNDN |
| Quyết toán thuế TNCN năm, gồm cả quyết toán thay người lao động | Tổ chức trả thu nhập | LQLT, ND-QLT, LTNCN, ND-TNCN |
| Phụ lục giao dịch liên kết (nộp cùng quyết toán TNDN) | Doanh nghiệp có giao dịch liên kết | ND-GDLK |
| Báo cáo tài chính năm: nộp cho cơ quan thuế và các cơ quan khác theo quy định | Doanh nghiệp | LKT, TT-KTDN, TT-KTDNNV hoặc TT-KTSN, LQLT |
| Đóng BHXH, BHYT, BHTN hằng tháng (hoặc theo phương thức đã đăng ký) | Người sử dụng lao động | LBHXH, ND-BHXH, LVL, ND-BHTN |
| Kinh phí công đoàn | Người sử dụng lao động | LCDOAN (⚠️ chưa kiểm tra trong đợt lập danh mục) |
| Báo cáo tình hình sử dụng lao động (định kỳ) | Người sử dụng lao động | BLLD, ND-QHLD. Phải kiểm tra vì có dự thảo sửa đổi năm 2026 đơn giản hóa chế độ báo cáo |
| Báo cáo sử dụng người lao động nước ngoài | Doanh nghiệp có lao động nước ngoài | ND-LDNN |
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

## 4. Mẫu trả lời

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
