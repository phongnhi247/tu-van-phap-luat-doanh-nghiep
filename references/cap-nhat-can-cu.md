# Cập nhật căn cứ

Dùng khi người dùng nói "cập nhật căn cứ", "kiểm tra văn bản mới", "có luật gì mới không", hoặc khi baseline đã quá 3 tháng và người dùng đồng ý cập nhật.

## 1. Phân vai

- **Người quản lý skill** (người phát hành bản chính thức) chạy quy trình này, duyệt thay đổi, chạy bộ câu hỏi kiểm thử, rồi phát hành bản mới (xem README, mục "Phát hành").
- **Người dùng thông thường** vẫn chạy được, nhưng trước khi bắt đầu phải nhận được cảnh báo:
  > Thay đổi bạn tự cập nhật sẽ bị **ghi đè** khi bạn cài bản chính thức tiếp theo. Nếu phát hiện văn bản mới, hãy gửi bảng đề xuất cho người quản lý skill để đưa vào bản chính thức.
- **Gemini Gem** hoặc nền tảng không ghi được file: chỉ làm đến bước 5 (xuất bảng đề xuất). Người dùng tự sửa file và tải lên lại.

## 2. Quy trình

1. **Chọn phạm vi:** hỏi người dùng muốn cập nhật toàn bộ danh mục, một nhóm (0–7), hay chỉ các dòng ⚠️. Mặc định đề xuất: **các dòng ⚠️ trước, sau đó đến nhóm 5 (thuế) và nhóm 4 (lao động)** vì hai nhóm này thay đổi nhiều nhất.
2. **Tra lại từng dòng trong phạm vi:**
   - Văn bản còn hiệu lực không? Đã bị sửa đổi hoặc thay thế chưa? Tìm theo cú pháp ở `tra-cuu-va-trich-dan.md`, mục 1 "Chiều ngang".
   - Các ô "chưa xác nhận" đã xác nhận được chưa?
   - Có link văn bản gốc trên nguồn nhóm 1–3 chưa? Có thì nâng nhãn lên ✅.
3. **Tìm văn bản mới ban hành sau ngày baseline** cho từng nhóm. Ví dụ truy vấn:
   - `"nghị định" "<lĩnh vực>" "có hiệu lực" "<tháng/năm sau baseline>"`
   - `"luật" "được Quốc hội thông qua" "<năm>"`
   - Trang tổng hợp "chính sách mới có hiệu lực từ tháng ..." của chinhphu.vn hoặc thuvienphapluat.vn
4. **Kiểm tra các dự án đang theo dõi.** Danh mục có ghi các dự án luật, dự thảo nghị định hoặc thông tư (ví dụ dự án sửa Luật Thương mại và luật liên quan, dự thảo sửa nghị định hướng dẫn BLLĐ, dự thảo thay thông tư kế toán doanh nghiệp nhỏ và vừa). Kiểm tra xem đã ban hành chưa.
5. **Lập bảng đề xuất**, chưa sửa file:

| # | Loại | Mã | Dòng cũ (tóm tắt) | Đề xuất mới | Nguồn | Nhãn mới |
|---|---|---|---|---|---|---|
| 1 | Thay thế | ND-XXX | NĐ cũ, đang hiệu lực | NĐ mới, hiệu lực từ ..., thay thế NĐ cũ | link | ✅ |
| 2 | Thêm mới | (mã mới) | — | ... | link | ⚠️ |
| 3 | Nâng nhãn | ... | ⚠️ | ✅, link gốc ... | link | ✅ |

   Loại thay đổi: `Thay thế`, `Sửa đổi` (thêm dòng văn bản sửa đổi), `Thêm mới`, `Nâng nhãn`, `Sửa thông tin` (ngày, tên), `Chuyển sang hết hiệu lực`.
6. **Chờ người dùng duyệt** từng dòng hoặc cả bảng.
7. **Ghi vào `danh-muc-can-cu.md`:**
   - **Thay thế:** giữ nguyên mã, sửa số hiệu, ngày hiệu lực và nguồn; chuyển văn bản cũ xuống mục 8 "Văn bản đã hết hiệu lực".
   - **Thêm mới:** đặt mã theo chức năng (ví dụ `ND-<viết tắt>`), không theo số hiệu. Mã không được trùng mã đã có.
   - Cập nhật cột Kiểm tra thành ngày hôm nay.
   - Sửa dòng `Baseline:` ở đầu file thành ngày hôm nay.
8. **Kiểm tra ảnh hưởng tới module:** mã mới cần xuất hiện ở module nào? Có điểm dễ sai nào cần thêm vào module không? Đề xuất sửa module nếu cần, nhưng **không ghi số hiệu vào module**.
9. **Gợi ý phát hành** (với người quản lý skill):
   - Nâng số phiên bản trong `VERSION`: sửa danh mục là bản vá (1.0.0 thành 1.0.1); thêm module hoặc tính năng là bản nhỏ (1.0.0 thành 1.1.0).
   - Ghi `CHANGELOG.md`.
   - Chạy `tests/bo-cau-hoi-kiem-thu.md`.
   - Đóng gói và phát hành theo README.

## 3. Quy tắc

- Không đưa vào danh mục văn bản chưa có số hiệu chính thức (dự thảo, "Luật số …/2026/QH16"). Ghi chúng vào cột Quan hệ của văn bản liên quan dưới dạng "đang có dự án/dự thảo".
- Chỉ có một nguồn thứ cấp thì nhãn tối đa là ⚠️.
- Không xóa dòng nào khỏi danh mục. Văn bản hết hiệu lực được chuyển xuống mục 8 để skill còn nhận diện được khi người dùng nhắc tới văn bản cũ.
