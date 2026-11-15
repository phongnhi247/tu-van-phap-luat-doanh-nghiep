# Tư vấn pháp luật doanh nghiệp

> **MIỄN TRỪ TRÁCH NHIỆM — ĐỌC TRƯỚC KHI DÙNG**
>
> - Đây là **công cụ hỗ trợ tra cứu và nghiên cứu pháp luật** chạy trên trợ lý AI. Đây **không phải dịch vụ tư vấn pháp luật**, không do luật sư hay tổ chức hành nghề luật sư cung cấp, và không thiết lập quan hệ luật sư – khách hàng.
> - Câu trả lời do AI tạo ra **có thể sai, thiếu, hoặc đã lỗi thời** so với văn bản mới ban hành sau ngày căn cứ (baseline). Người dùng phải tự kiểm tra văn bản gốc trước khi áp dụng, và **tự chịu trách nhiệm** về quyết định của mình.
> - Với vụ việc có giá trị lớn, có dấu hiệu hình sự, đang bị thanh tra, kiểm tra, hoặc đang tranh chấp, hãy hỏi luật sư hoặc cơ quan có thẩm quyền.
> - Skill được phát hành theo giấy phép MIT (xem `LICENSE`), **cung cấp nguyên trạng, không kèm bất kỳ bảo đảm nào**.

## Ghi công

Skill này được phát triển dựa trên skill **"Tư vấn pháp luật" của tác giả Nguyễn Duy Tùng**, tải miễn phí tại https://duytung.vn/tai-nguyen/tu-van-phap-luat (© 2026 Nguyễn Duy Tùng).

- **Kế thừa từ bản gốc:** ý tưởng và phương pháp tra cứu, gồm tra chéo văn bản theo 3 chiều, xây bảng căn cứ trích dẫn nguyên văn có tọa độ (Source of Truth), quy tắc xử lý xung đột văn bản, và cách lưu vết quá trình tra cứu.
- **Phần làm lại:** chuyển sang phạm vi doanh nghiệp; viết lại toàn bộ hướng dẫn; danh mục căn cứ duy nhất cập nhật đến năm 2026; nguyên tắc "chỉ nói khi có căn cứ" với nhãn tin cậy; kho trích dẫn đã xác minh; 8 nhóm nghiệp vụ; các tính năng lịch tuân thủ, rà soát văn bản, soạn văn bản theo mẫu, cập nhật căn cứ; bộ câu hỏi kiểm thử.
- Trang gốc không công bố giấy phép cho việc sửa đổi hay phát hành lại. **Trước khi chia sẻ công khai bản phái sinh này, cần có sự đồng ý của tác giả gốc.** Giấy phép MIT trong file `LICENSE` chỉ áp dụng cho phần do người phát hành skill này viết.

## Giới thiệu

Skill AI hỗ trợ tra cứu pháp lý chuyên sâu cho doanh nghiệp Việt Nam. Dành cho chủ doanh nghiệp, kế toán và nhân viên làm giấy tờ.

- **Làm được:** thành lập và đầu tư, quản trị và vốn, hợp đồng và thương mại (gồm khuyến mại, hợp đồng điện tử), lao động, BHXH, BHYT và an toàn lao động, thuế, hóa đơn và kế toán, dữ liệu cá nhân, nhãn hiệu, môi trường, PCCC, tranh chấp, thanh tra, giải thể, phá sản, hải quan và xuất nhập khẩu. Có lịch tuân thủ, rà soát hợp đồng và văn bản nội bộ, soạn văn bản theo mẫu, hồ sơ doanh nghiệp lưu lại, và lệnh tự cập nhật căn cứ.
- **Cách trả lời:** chuyên sâu theo 7 phần: kết luận, giả định, căn cứ trích nguyên văn, phân tích, phương án và khuyến nghị, checklist hồ sơ, rủi ro.
- **Nguyên tắc:** chỉ nói khi có căn cứ. Mỗi kết luận có nhãn ✅ (đã đối chiếu nguyên văn), ⚠️ (chưa chắc chắn) hoặc ❓ (không tìm thấy). Không tìm thấy thì nói "không biết", không bịa.
- **Không làm:** hôn nhân, thừa kế, đất đai hộ gia đình, hình sự cá nhân.

> Nội dung mang tính tham khảo, **không thay thế ý kiến pháp lý chính thức** của luật sư hoặc cơ quan có thẩm quyền.

Phiên bản: xem file `VERSION`. Ngày căn cứ (baseline): xem đầu file `references/danh-muc-can-cu.md`.

---

## 1. Cài đặt

Skill là một thư mục tên `tu-van-phap-luat-doanh-nghiep`, bên trong có `SKILL.md`. Không cần cài thêm phần mềm nào. Nên bật quyền **tìm kiếm web** để skill tra được văn bản gốc.

### Claude Code

1. Giải nén file zip.
2. Chép thư mục `tu-van-phap-luat-doanh-nghiep` vào:
   - Windows: `C:\Users\<tên bạn>\.claude\skills\`
   - macOS/Linux: `~/.claude/skills/`
3. Mở phiên Claude Code mới. Skill tự kích hoạt khi bạn hỏi về doanh nghiệp, hoặc gọi trực tiếp bằng `/tu-van-phap-luat-doanh-nghiep`.

### Claude.ai (web, ứng dụng)

1. Vào **Settings → Capabilities → Skills**, chọn tải lên.
2. Chọn **file zip** (không giải nén).
3. Bật skill và bật tìm kiếm web.

### Gemini CLI

1. Chép thư mục skill vào `~/.gemini/skills/`. Nếu lấy từ kho git, có thể dùng `gemini skills install <link kho>`.
2. Trong phiên Gemini CLI, gõ `/skills reload`, rồi gõ `/skills list` để kiểm tra skill đã có trong danh sách.

### Antigravity

1. Chép thư mục skill vào một trong hai nơi:
   - Dùng cho mọi dự án: `~/.gemini/config/skills/`. Bản cũ dùng `~/.gemini/antigravity/skills/` vẫn được hỗ trợ.
   - Chỉ dùng cho một dự án: `<thư mục dự án>/.agents/skills/`.
2. Mở lại Antigravity. Skill tự kích hoạt theo mô tả trong `SKILL.md`.

### Gemini app (web, điện thoại) — dùng Gem

Ứng dụng Gemini không chạy được skill trực tiếp. Bạn có thể tạo một **Gem** thay thế:

1. Tạo Gem mới.
2. Mở file `SKILL.md`, chép toàn bộ nội dung **sau phần `---` đầu tiên** và dán vào ô **Hướng dẫn (Instructions)**.
3. Tải lên **Kiến thức (Knowledge)** các file trong bản đóng gói cho Gem (`...-gem-v<phiên bản>.zip`, xem mục 5). Gem giới hạn khoảng 10 file, nên bản cho Gem đã gộp sẵn thành 7 file.
4. Giới hạn của Gem:
   - Gem không tự ghi file, nên hồ sơ doanh nghiệp và lệnh cập nhật căn cứ chỉ xuất nội dung để bạn tự lưu.
   - Nếu Gem không tra được web, câu trả lời sẽ có nhãn ⚠️ và không nêu con số.

### Tự kiểm tra sau khi cài (30 giây)

Hỏi: **"Nghị định 999 năm 2026 về thuế điện tử quy định gì?"**

Skill đúng phải trả lời là **không tìm thấy văn bản này**. Nếu AI mô tả nội dung một nghị định như vậy, nghĩa là skill chưa được kích hoạt. Kiểm tra lại bước cài đặt.

---

## 2. Cách dùng

Cứ hỏi tự nhiên. Ví dụ:

- "Công ty TNHH 2 thành viên, một thành viên muốn bán vốn cho người ngoài thì làm thế nào?"
- "Xuất hóa đơn sai đơn giá tháng trước, khách đã kê khai rồi, xử lý sao?"
- "Tháng 1/2027 công ty tôi phải nộp những gì?" (lịch tuân thủ)
- "Rà soát giúp hợp đồng lao động này: [dán nội dung]" (rà soát văn bản)
- "Lập hồ sơ vụ tranh chấp công nợ với công ty X" (chế độ lập hồ sơ, lưu file)
- "Soạn giúp quyết định kỷ luật nhân viên A" (soạn văn bản theo mẫu)
- "Doanh nghiệp chế xuất bán hàng vào nội địa làm thủ tục gì?" (hải quan, xuất nhập khẩu)
- "Cập nhật căn cứ" (cập nhật danh mục văn bản)

**Hồ sơ doanh nghiệp:** lần đầu, skill hỏi một vài thông tin như loại hình, số lao động, cách kê khai thuế, rồi đề nghị lưu thành file `ho-so-doanh-nghiep.md` **trong thư mục làm việc của bạn**, không lưu trong thư mục skill. Lần sau bạn không phải khai lại. Làm cho nhiều doanh nghiệp thì mỗi doanh nghiệp một file `ho-so-<tên>.md`.

---

## 3. Cập nhật lên bản mới

Mỗi câu trả lời kết thúc bằng dòng "Căn cứ tính đến ... (skill v...)". Khi ngày căn cứ đã quá 3 tháng, skill sẽ nhắc bạn cập nhật.

| Nền tảng | Cách cập nhật |
|---|---|
| Claude Code, Antigravity, Gemini CLI | Xóa thư mục skill cũ, chép thư mục mới vào cùng chỗ. Nếu cài từ git thì chạy `git pull` trong thư mục skill. Hồ sơ doanh nghiệp không bị mất vì nằm ở thư mục làm việc của bạn |
| Claude.ai | Tải file zip mới lên thay bản cũ |
| Gem | Thay các file Kiến thức bằng bản cho Gem mới, và dán lại phần Hướng dẫn nếu `SKILL.md` có thay đổi |

Xem `CHANGELOG.md` để biết bản mới thay đổi gì.

Bạn cũng có thể tự gõ "cập nhật căn cứ" để skill tra văn bản mới. Tuy nhiên, thay đổi tự làm trên máy bạn sẽ **bị ghi đè** khi cài bản chính thức tiếp theo. Nếu phát hiện văn bản mới, hãy gửi bảng đề xuất cho người quản lý skill.

---

## 4. Cấu trúc thư mục

```
tu-van-phap-luat-doanh-nghiep/
├── SKILL.md                    Bộ định tuyến: nguyên tắc, chế độ, chọn file
├── VERSION, CHANGELOG.md, README.md
├── references/
│   ├── danh-muc-can-cu.md      NƠI DUY NHẤT chứa số hiệu văn bản
│   ├── trich-dan-xac-minh.md   Các đoạn trích nguyên văn đã đối chiếu với file gốc
│   ├── nguyen-tac-can-cu.md    Quy tắc chống bịa, nhãn tin cậy
│   ├── khung-tra-loi.md        Khung 7 phần, chế độ lập hồ sơ
│   ├── tra-cuu-va-trich-dan.md Tra chéo 3 chiều, trích dẫn, xung đột văn bản
│   ├── nhom-01 ... nhom-08     8 nhóm nghiệp vụ (chỉ ghi mã căn cứ)
│   ├── lich-tuan-thu.md, ra-soat-van-ban.md, ho-so-doanh-nghiep-mau.md
│   ├── nguong-chuyen-luat-su.md, cap-nhat-can-cu.md, soan-van-ban.md
└── tests/bo-cau-hoi-kiem-thu.md
```

---

## 5. Phát hành (dành cho người quản lý skill)

Chu kỳ gợi ý: **mỗi quý**, hoặc ngay khi có luật hoặc nghị định lớn về thuế, lao động, doanh nghiệp.

1. Gõ **"cập nhật căn cứ"**. Duyệt bảng đề xuất. Ưu tiên nâng các dòng ⚠️ lên ✅.
2. Chạy **kiểm tra tĩnh** trong thư mục skill. Cả hai lệnh phải trả về rỗng:
   ```bash
   grep -rnE "[0-9]+/[0-9]{4}/(QH[0-9]*|NĐ-CP|ND-CP|TT-[A-ZĐ]+|NQ-[A-Z]+|QĐ-[A-Z]+)" --include=*.md . | grep -v "references/danh-muc-can-cu.md"
   ```
   **Kiểm tra mã:** mọi mã dạng `ND-...`, `L...`, `TT-...` dùng trong module phải có trong cột Mã của danh mục.
3. Chạy **bộ câu hỏi** trong `tests/bo-cau-hoi-kiem-thu.md`, ít nhất các câu 1, 5, 8, 9, 13. Chỉ phát hành khi các câu bẫy (8, 9) đạt.
4. Nâng `VERSION`: sửa danh mục thì nâng bản vá (`1.0.1`); thêm tính năng thì nâng bản nhỏ (`1.1.0`). Ghi `CHANGELOG.md`. Đảm bảo phiên bản trong `VERSION` khớp với dòng `Phiên bản:` trong danh mục.
5. **Đóng gói.** Nếu thư mục skill là kho git, dùng lệnh sau để file zip không lẫn thư mục `.git`:
   ```bash
   git archive --format=zip --prefix=tu-van-phap-luat-doanh-nghiep/ -o ../tu-van-phap-luat-doanh-nghiep-v<phiên bản>.zip v<phiên bản>
   ```
   Nếu không dùng git, chạy trong PowerShell, từ thư mục **chứa** thư mục skill:
   ```powershell
   $v = (Get-Content tu-van-phap-luat-doanh-nghiep\VERSION).Trim()
   Compress-Archive -Path tu-van-phap-luat-doanh-nghiep -DestinationPath "tu-van-phap-luat-doanh-nghiep-v$v.zip" -Force
   ```
   Bản cho Gem gộp các module và tính năng để không vượt giới hạn file:
   ```powershell
   $s = "tu-van-phap-luat-doanh-nghiep\references"; $g = "gem-v$v"; New-Item -ItemType Directory -Force $g | Out-Null
   Copy-Item "$s\danh-muc-can-cu.md","$s\trich-dan-xac-minh.md","$s\nguyen-tac-can-cu.md","$s\khung-tra-loi.md","$s\tra-cuu-va-trich-dan.md" $g
   Get-Content -Encoding utf8 "$s\nhom-0*.md" | Set-Content -Encoding utf8 "$g\cac-nhom-nghiep-vu.md"
   Get-Content -Encoding utf8 "$s\lich-tuan-thu.md","$s\ra-soat-van-ban.md","$s\soan-van-ban.md","$s\ho-so-doanh-nghiep-mau.md","$s\nguong-chuyen-luat-su.md","$s\cap-nhat-can-cu.md" | Set-Content -Encoding utf8 "$g\cac-tinh-nang.md"
   Compress-Archive -Path "$g\*" -DestinationPath "tu-van-phap-luat-doanh-nghiep-gem-v$v.zip" -Force
   ```
6. **Phân phối.** Nếu dùng git: commit, gắn tag `v<phiên bản>`, đẩy lên kho và đính kèm 2 file zip vào mục Releases. Nếu không dùng git: gửi 2 file zip kèm nội dung CHANGELOG. Cập nhật Gem chia sẻ nếu có.

---

## 6. Giới hạn đã biết

- Căn cứ chỉ đúng đến ngày baseline. Văn bản ban hành sau ngày đó cần được tra bằng web hoặc bổ sung bằng lệnh cập nhật.
- Nhiều dòng trong danh mục bản 1.0.0 có nhãn ⚠️ vì chưa mở được văn bản gốc trong đợt lập danh mục. Skill vẫn bắt buộc tra nguyên văn khi trả lời.
- Chưa có sẵn căn cứ cho các ngành nghề kinh doanh có điều kiện riêng (thực phẩm, dược, xây dựng, vận tải, tài chính...), nghị định hướng dẫn thuế xuất nhập khẩu (chưa xác minh). Gặp các phần này, skill tra trực tiếp và gắn nhãn tương ứng.
- Đã chạy thử trên **Claude Code** (19 câu) và **Antigravity CLI** (câu bẫy và câu hạn nộp TNCN, đều đạt, cài skill ở `<thư mục dự án>/.agents/skills/`). Chưa chạy thử trên Gemini Gem.
- **Gemini CLI:** tài khoản cá nhân miễn phí (Gemini Code Assist for individuals) đã bị Google ngừng hỗ trợ trong Gemini CLI và chuyển sang Antigravity. Người dùng loại tài khoản này nên dùng Antigravity.
