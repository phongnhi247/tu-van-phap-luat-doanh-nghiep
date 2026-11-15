# Tư vấn pháp luật doanh nghiệp

> **MIỄN TRỪ TRÁCH NHIỆM — ĐỌC TRƯỚC KHI DÙNG**
>
> - Đây là **công cụ hỗ trợ tra cứu và nghiên cứu pháp luật** chạy trên trợ lý AI. Đây **không phải dịch vụ tư vấn pháp luật**, không do luật sư hay tổ chức hành nghề luật sư cung cấp, và không thiết lập quan hệ luật sư – khách hàng.
> - Câu trả lời do AI tạo ra **có thể sai, thiếu, hoặc đã lỗi thời** so với văn bản mới ban hành sau ngày căn cứ (baseline). Người dùng phải tự kiểm tra văn bản gốc trước khi áp dụng, và **tự chịu trách nhiệm** về quyết định của mình.
> - Với vụ việc có giá trị lớn, có dấu hiệu hình sự, đang bị thanh tra, kiểm tra, hoặc đang tranh chấp, hãy hỏi luật sư hoặc cơ quan có thẩm quyền.
> - Skill được phát hành theo giấy phép MIT (xem `LICENSE`), **cung cấp nguyên trạng, không kèm bất kỳ bảo đảm nào**.

## Giới thiệu

### Vì sao có skill này

**Nỗi đau của người làm giấy tờ trong doanh nghiệp**

- Chỉ riêng năm 2025–2026, Luật Quản lý thuế, thuế GTGT, TNDN, TNCN, hóa đơn điện tử, lương tối thiểu, xử phạt BHXH, Luật Đầu tư, Luật Doanh nghiệp... đều có văn bản mới thay thế. Mẫu tờ khai, kỳ khai và hạn nộp cũng đổi theo.
- Kế toán, nhân sự, chủ doanh nghiệp nhỏ không có luật sư bên cạnh. Mỗi lần cần câu trả lời phải lục nhiều trang, đọc bài phân tích, rồi vẫn không chắc văn bản đó còn hiệu lực hay không.
- Hỏi AI thì nhanh, nhưng AI hay **trả lời tự tin bằng trí nhớ cũ**: trích nghị định đã bị thay, nêu mức phạt không có nguồn, thậm chí mô tả cả một văn bản không tồn tại.

**Vấn đề cốt lõi:** câu trả lời pháp lý chỉ có giá trị khi **đúng văn bản đang có hiệu lực tại thời điểm sự việc**, và người đọc **kiểm tra lại được**. Một câu trả lời nghe hợp lý nhưng không có nguồn còn nguy hiểm hơn không có câu trả lời.

**Giải pháp**

Skill biến trợ lý AI thành một trợ lý tra cứu có kỷ luật:

- **Chỉ nói khi có căn cứ.** Mọi con số (mức phạt, thời hạn, tỷ lệ) phải kèm câu trích nguyên văn. Mỗi kết luận có nhãn: ✅ đã đối chiếu, ⚠️ chưa chắc chắn, ❓ không tìm thấy. Không tìm thấy thì nói "không biết", không bịa.
- **Một danh mục căn cứ duy nhất** gồm 120 văn bản, cập nhật đến 14/11/2026, ghi rõ văn bản nào thay văn bản nào. Hỏi theo văn bản cũ, skill sẽ báo văn bản đó đã hết hiệu lực và chỉ ra văn bản thay thế.
- **Kho trích dẫn đã xác minh** từ file gốc (nhiều file có chữ ký số): hạn nộp tờ khai thuế, khai TNCN theo quý, xử lý hóa đơn sai sót, mức phạt chậm đóng BHXH, trình tự kỷ luật lao động, chuẩn trình bày văn bản...
- **Trả lời để làm được ngay:** kết luận, căn cứ, phân tích, phương án kèm khuyến nghị, và **checklist hồ sơ** (biểu mẫu, nơi nộp, thời hạn, rủi ro nếu làm trễ).
- **Dễ cập nhật:** gõ "cập nhật căn cứ", skill tự tra văn bản mới và đề xuất sửa danh mục để bạn duyệt.

Skill đã đạt 20 câu kiểm thử, kể cả các câu bẫy hỏi về văn bản không có thật hoặc đã hết hiệu lực.

**Dành cho:** chủ doanh nghiệp, kế toán, nhân sự, nhân viên làm hồ sơ, và người tư vấn cần một bản nháp có căn cứ để kiểm tra lại.

**Không làm:** hôn nhân, thừa kế, đất đai hộ gia đình, hình sự cá nhân.

### Skill làm được gì

Skill có 8 chức năng. Bạn không cần nhớ lệnh: cứ nói tự nhiên, skill tự chọn chức năng phù hợp. Muốn gọi chắc chắn thì dùng các câu mẫu ở mỗi mục.

#### 1. Tư vấn chuyên sâu (mặc định)

- **Dùng khi:** bạn có một tình huống cụ thể cần biết luật nói gì và nên làm gì.
- **Cách gọi:** hỏi tự nhiên. Ví dụ: "Nhân viên nghỉ không phép 6 ngày, công ty muốn sa thải thì làm thế nào?"
- **Skill làm gì:**
  - Xác định thời điểm sự việc, để chọn đúng văn bản có hiệu lực lúc đó (không phải lúc hỏi).
  - Tra danh mục căn cứ, đọc nguyên văn điều khoản trên nguồn chính thống hoặc trong kho trích dẫn đã xác minh.
  - Kiểm tra theo 3 chiều: văn bản hướng dẫn, văn bản sửa đổi hoặc thay thế, điều khoản chuyển tiếp.
- **Bạn nhận được** câu trả lời 7 phần:
  1. **Kết luận** ngắn, có nhãn ✅ ⚠️ ❓.
  2. **Tình huống và giả định:** thông tin đã dùng, chỗ nào còn `[Giả định]` và nếu khác đi thì kết luận đổi thế nào.
  3. **Căn cứ pháp lý:** số hiệu, điều, khoản, câu trích nguyên văn, ngày hiệu lực, link nguồn.
  4. **Phân tích:** áp từng điều luật vào tình huống, các điểm dễ hiểu sai.
  5. **Phương án và khuyến nghị:** từ 2 phương án trở lên nếu có, chấm điểm pháp lý, rủi ro, khả thi, và khuyến nghị nên chọn phương án nào.
  6. **Việc cần làm:** checklist hồ sơ, biểu mẫu, nơi nộp, thời hạn, lệ phí, hậu quả nếu làm trễ.
  7. **Rủi ro và lưu ý**, kèm dòng ngày căn cứ.
- **Giới hạn:** câu hỏi chỉ tra một con số thì trả lời gọn hơn (kết luận và căn cứ). Câu hỏi ngoài phạm vi doanh nghiệp thì từ chối và gợi ý nơi hỏi.

#### 2. Lịch tuân thủ

- **Dùng khi:** bạn cần biết tháng, quý hoặc năm này doanh nghiệp phải nộp những gì.
- **Cách gọi:** "Tháng 1/2027 công ty phải nộp gì?", "Lịch nộp quý 4", "Hạn nộp tờ khai GTGT quý 4/2026 là ngày nào?"
- **Skill làm gì:**
  - Lấy thông tin từ hồ sơ doanh nghiệp: kê khai thuế theo tháng hay quý, số lao động, có lao động nước ngoài, có giao dịch liên kết hay không...
  - Lọc ra các nghĩa vụ áp dụng: tờ khai GTGT, khấu trừ TNCN, tạm nộp TNDN, quyết toán năm, báo cáo tài chính, đóng BHXH, BHYT, BHTN, kinh phí công đoàn, báo cáo lao động...
  - Tra nguyên văn hạn nộp của từng nghĩa vụ. Kiểm tra hạn nộp có trùng ngày nghỉ, Tết hay không.
- **Bạn nhận được:** bảng sắp theo ngày, gồm hạn, việc cần làm, ai làm, căn cứ trích dẫn, mức phạt nếu trễ (khi có trích dẫn). Kèm danh sách việc **không** áp dụng cho bạn, và các việc sắp đến hạn. Có thể lưu lịch thành file để dùng cả năm.
- **Giới hạn:** chưa bao gồm báo cáo riêng của ngành đặc thù (tài chính, xây dựng...). Skill sẽ nói rõ khi gặp trường hợp đó.

#### 3. Rà soát văn bản

- **Dùng khi:** bạn có hợp đồng, nội quy, quyết định, điều lệ và muốn biết có trái luật hay rủi ro gì không.
- **Cách gọi:** dán nội dung hoặc gửi file, kèm câu "Rà soát giúp văn bản này".
- **Skill làm gì:**
  - Xác định loại văn bản, ngày ký và vai trò của bạn (bên soạn hay bên nhận).
  - Áp checklist nội dung bắt buộc cho 5 loại văn bản hay gặp: **hợp đồng lao động, nội quy lao động, quyết định kỷ luật hoặc sa thải, hợp đồng mua bán hàng hóa hoặc dịch vụ, điều lệ công ty**. Loại văn bản khác thì tra trực tiếp căn cứ.
  - Đọc toàn văn để tìm điều khoản mâu thuẫn nhau, điều khoản bất lợi bất thường, chỗ mơ hồ, chỗ thiếu thời hạn hay chế tài.
  - Với hợp đồng ký với người tiêu dùng: đối chiếu các điều khoản bị cấm trong hợp đồng mẫu.
  - Có thể góp ý cả phần trình bày (lề, phông, đánh số, chính tả, khung chữ ký).
- **Bạn nhận được:** bảng lỗi gồm vị trí, vấn đề, căn cứ trích dẫn, mức rủi ro (Cao, Trung bình, Thấp), đề xuất sửa. Kèm danh sách nội dung bắt buộc còn thiếu. Skill không chép lại thông tin cá nhân (số CCCD, lương...) trong câu trả lời.
- **Giới hạn:** skill chỉ ra lỗi và cách sửa. Bạn yêu cầu thì skill mới viết lại điều khoản hoặc cả văn bản.

#### 4. Soạn văn bản theo chuẩn Nghị định 30/2020

- **Dùng khi:** bạn cần bản nháp quyết định, biên bản, thông báo, công văn, hợp đồng, nghị quyết họp...
- **Cách gọi:** "Soạn giúp quyết định kỷ luật nhân viên A", "Soạn công văn giải trình gửi cơ quan thuế".
- **Skill làm gì:**
  - **Văn bản có mẫu bắt buộc** (tờ khai thuế, đề nghị gia hạn nộp hồ sơ khai thuế, hồ sơ đăng ký doanh nghiệp, thông báo khuyến mại...): skill **không tự dựng mẫu**. Skill chỉ ra số hiệu mẫu, văn bản ban hành mẫu, nơi lấy mẫu chính thức, và hướng dẫn điền từng mục.
  - **Văn bản nội bộ không có mẫu bắt buộc:** skill soạn bản nháp có đủ nội dung luật yêu cầu, phần căn cứ ghi đúng văn bản đang có hiệu lực, và để `[...]` cho mọi thông tin chưa biết (không tự điền tên, ngày, số tiền).
  - Trình bày theo **Phụ lục I Nghị định 30/2020**: bố cục 9 thành phần (Quốc hiệu và Tiêu ngữ, tên cơ quan, số và ký hiệu, địa danh và ngày tháng, tên loại và trích yếu, nội dung, chữ ký, dấu, nơi nhận); cách ghi quyền hạn ký (TM., KT., TL., TUQ.).
- **Bạn nhận được:** bản nháp, danh sách các chỗ cần điền, các bước tiếp theo (ký, đóng dấu, gửi, lưu), và **cài đặt định dạng cho Word**: khổ A4, lề, phông Times New Roman, cỡ chữ từng phần, giãn dòng, thụt đầu dòng.
- **Lưu ý:** Nghị định 30/2020 **bắt buộc** với doanh nghiệp nhà nước. Doanh nghiệp khác dùng làm chuẩn khuyến nghị. Doanh nghiệp có quy chế văn thư riêng thì theo quy chế đó.

#### 5. Hồ sơ doanh nghiệp

- **Dùng khi:** bạn hỏi nhiều lần cho cùng một doanh nghiệp và không muốn khai lại thông tin.
- **Cách hoạt động:** lần đầu, skill hỏi các thông tin ảnh hưởng tới câu trả lời: loại hình, ngành nghề, vốn nước ngoài, số lao động, công đoàn, phương pháp và kỳ kê khai thuế, chế độ kế toán, có giao dịch liên kết hay không... Skill chỉ hỏi những gì cần cho câu hỏi hiện tại, tối đa 4 câu một lượt.
- **Bạn nhận được:** file `ho-so-doanh-nghiep.md` lưu **trong thư mục làm việc của bạn**, không lưu trong thư mục skill, nên cập nhật skill không làm mất hồ sơ. Làm cho nhiều doanh nghiệp (ví dụ kế toán dịch vụ) thì mỗi doanh nghiệp một file `ho-so-<tên>.md`. Hồ sơ cũ hơn 6 tháng thì skill hỏi lại xem thông tin còn đúng không.
- **Bảo mật:** nội dung hồ sơ không được đưa vào truy vấn tìm kiếm web.

#### 6. Cảnh báo cần luật sư

- **Dùng khi:** skill tự kích hoạt khi tình huống có dấu hiệu nguy hiểm.
- **Các dấu hiệu skill theo dõi:**
  - dấu hiệu hình sự: mua bán hóa đơn, trốn thuế, trốn đóng BHXH kéo dài;
  - đang bị thanh tra, kiểm tra, bị ấn định thuế hoặc truy thu số lớn; nhận giấy triệu tập;
  - đã có đơn khởi kiện, yêu cầu trọng tài; tranh chấp giá trị lớn hoặc có yếu tố nước ngoài;
  - sắp hết thời hiệu khởi kiện, khiếu nại, thời hạn giải trình;
  - mua bán, sáp nhập doanh nghiệp; đình công, cắt giảm lao động hàng loạt, tai nạn lao động nghiêm trọng;
  - mất khả năng thanh toán; rò rỉ dữ liệu cá nhân trên diện rộng.
- **Bạn nhận được:** cảnh báo đặt ở **đầu** câu trả lời, nêu rõ dấu hiệu, việc nên làm trước khi ký hoặc nộp gì, và tài liệu cần mang theo khi gặp luật sư. Skill vẫn giải thích khung pháp lý, nhưng **từ chối** tư vấn cách che giấu, hợp thức hóa chứng từ hay đối phó trái luật.

#### 7. Lập hồ sơ vụ việc

- **Dùng khi:** vụ việc phức tạp, nhiều bên, nhiều văn bản, hoặc bạn cần tài liệu để làm việc với cơ quan nhà nước, tòa án.
- **Cách gọi:** "Lập hồ sơ vụ tranh chấp công nợ với công ty X".
- **Bạn nhận được:** một thư mục trong thư mục làm việc của bạn, gồm:
  - `nhat-ky-tra-cuu.md`: ghi lần lượt từng lần tra, gồm mục đích, nguồn, câu trích, mâu thuẫn tìm thấy, quyết định đào sâu hay mở rộng. Chỉ ghi thêm, không xóa.
  - `bao-cao-tu-van.md`: báo cáo đầy đủ theo khung 7 phần.
  - Cuối nhật ký có 3 mục: **đã chắc chắn** (kèm nguồn), **hành động**, **còn bỏ ngỏ**.
- **Lưu ý:** skill hỏi bạn trước khi tạo file.

#### 8. Cập nhật căn cứ

- **Dùng khi:** ngày căn cứ đã cũ (skill tự nhắc khi quá 3 tháng), hoặc bạn nghe tin có luật, nghị định mới.
- **Cách gọi:** "Cập nhật căn cứ", "Kiểm tra văn bản mới về thuế".
- **Skill làm gì:**
  - Hỏi phạm vi: toàn bộ, một nhóm, hay chỉ các dòng còn nhãn ⚠️ (mặc định ưu tiên nhóm thuế và lao động).
  - Tra lại từng văn bản: còn hiệu lực không, đã bị sửa hay thay thế chưa. Tìm văn bản mới ban hành sau ngày căn cứ. Kiểm tra các dự thảo đang theo dõi đã được ban hành chưa.
  - Lập **bảng đề xuất thay đổi** gồm dòng cũ, dòng mới, nguồn, nhãn mới, rồi **chờ bạn duyệt** trước khi ghi.
- **Bạn nhận được:** danh mục mới, ngày căn cứ mới, và gợi ý nâng số phiên bản, ghi nhật ký thay đổi, chạy lại bộ câu hỏi kiểm thử.
- **Lưu ý:** thay đổi bạn tự làm trên máy sẽ bị ghi đè khi cài bản chính thức tiếp theo. Gemini Gem không ghi được file, nên chỉ xuất bảng đề xuất để bạn tự cập nhật.

### Tra được gì

| Nhóm | Ví dụ nội dung tra được | Ví dụ câu hỏi |
|---|---|---|
| 1. Khởi sự và đầu tư | Chọn loại hình doanh nghiệp; hồ sơ đăng ký doanh nghiệp theo quy định 2025–2026; chủ sở hữu hưởng lợi; ngành nghề kinh doanh có điều kiện; nhà đầu tư nước ngoài theo Luật Đầu tư 2025; hộ kinh doanh chuyển lên doanh nghiệp; lệ phí môn bài đã bãi bỏ từ 2026 | "Nhà đầu tư nước ngoài góp thêm vốn vào công ty thì làm thủ tục gì trước?" |
| 2. Quản trị và vốn | Chuyển nhượng vốn và quyền ưu tiên mua; tăng, giảm vốn điều lệ; họp và biểu quyết HĐTV, ĐHĐCĐ; thay người đại diện theo pháp luật; tạm ngừng kinh doanh | "Thành viên công ty TNHH muốn bán vốn cho người ngoài thì phải làm gì?" |
| 3. Hợp đồng và thương mại | Phạt vi phạm, bồi thường, bất khả kháng; hợp đồng mẫu với người tiêu dùng và các điều khoản bị cấm; thương mại điện tử; quảng cáo, người có ảnh hưởng (KOL); khuyến mại; hợp đồng điện tử, chữ ký số; cạnh tranh | "Hợp đồng mẫu ghi 'không hoàn tiền trong mọi trường hợp' có hiệu lực không?" |
| 4. Lao động, BHXH, an toàn lao động | Hợp đồng lao động, thử việc; lương tối thiểu 2026 và từ 2027; kỷ luật, sa thải, chấm dứt hợp đồng; BHXH, BHYT, BHTN và mức phạt chậm đóng từ 10/09/2026; lao động nước ngoài; hợp đồng lao động điện tử; huấn luyện an toàn lao động | "Nhân viên nghỉ không phép 6 ngày, sa thải thế nào cho đúng trình tự?" |
| 5. Thuế, hóa đơn, kế toán | Hạn nộp tờ khai tháng, quý, năm, quyết toán; khai TNCN theo quý từ 01/07/2026; thuế GTGT, khấu trừ, hoàn thuế; thuế TNDN, chi phí được trừ, miễn thuế cho doanh nghiệp doanh thu nhỏ; hóa đơn điện tử và xử lý sai sót; xử phạt thuế, hóa đơn; giao dịch liên kết; chế độ kế toán mới từ 2026; khai bổ sung khi đang bị thanh tra | "Xuất hóa đơn sai đơn giá, khách đã kê khai rồi, xử lý sao?" |
| 6. Tuân thủ chuyên ngành | Bảo vệ dữ liệu cá nhân (luật mới từ 2026); đăng ký và bảo vệ nhãn hiệu; giấy phép môi trường; phòng cháy, chữa cháy | "Công ty thu thập dữ liệu khách hàng cần làm hồ sơ gì?" |
| 7. Tranh chấp và rút lui | Khởi kiện tại Tòa án nhân dân khu vực, trọng tài, hòa giải; khiếu nại, khởi kiện quyết định hành chính; thanh tra, xử phạt hành chính; thi hành án dân sự (luật mới từ 01/07/2026); giải thể; phục hồi, phá sản | "Công ty còn nợ thì có giải thể được không?" |
| 8. Hải quan và xuất nhập khẩu | Thủ tục thông quan; doanh nghiệp chế xuất mua bán với nội địa; xuất nhập khẩu tại chỗ; hàng cấm, hạn chế xuất nhập khẩu (quy định mới từ 9/2026); thuế xuất nhập khẩu; xử phạt hải quan (nghị định mới từ 01/07/2026) | "Doanh nghiệp chế xuất bán hàng cho công ty trong nước làm thủ tục gì?" |

Danh sách đầy đủ văn bản, kèm tình trạng hiệu lực và link nguồn: xem `references/danh-muc-can-cu.md`.

## Ghi công

Skill này được phát triển dựa trên skill **"Tư vấn pháp luật" của tác giả Nguyễn Duy Tùng**, tải miễn phí tại https://duytung.vn/tai-nguyen/tu-van-phap-luat (© 2026 Nguyễn Duy Tùng).

- **Kế thừa từ bản gốc:** ý tưởng và phương pháp tra cứu, gồm tra chéo văn bản theo 3 chiều, xây bảng căn cứ trích dẫn nguyên văn có tọa độ (Source of Truth), quy tắc xử lý xung đột văn bản, và cách lưu vết quá trình tra cứu.
- **Phần làm lại:** chuyển sang phạm vi doanh nghiệp; viết lại toàn bộ hướng dẫn; danh mục căn cứ duy nhất cập nhật đến năm 2026; nguyên tắc "chỉ nói khi có căn cứ" với nhãn tin cậy; kho trích dẫn đã xác minh; 8 nhóm nghiệp vụ; các tính năng lịch tuân thủ, rà soát văn bản, soạn văn bản theo mẫu, cập nhật căn cứ; bộ câu hỏi kiểm thử.
- Mọi quyền đối với phần thuộc tác phẩm gốc vẫn thuộc về tác giả gốc. Giấy phép MIT trong file `LICENSE` chỉ áp dụng cho phần do người phát hành skill này viết. Nếu tác giả gốc yêu cầu, người phát hành sẽ chỉnh sửa hoặc gỡ bỏ phần liên quan.

## Nguồn tham khảo

Skill **không chứa toàn văn** văn bản hay bài viết của bên thứ ba. Skill chỉ chứa các câu trích ngắn từ văn bản quy phạm pháp luật (kèm điều, khoản) và **đường link dẫn nguồn**. Các nguồn đã được dùng để tra cứu, xác minh khi xây dựng skill:

| Nhóm | Trang | Cách dùng trong skill |
|---|---|---|
| Cơ quan nhà nước | Cổng Thông tin điện tử Chính phủ và kho văn bản ký số (chinhphu.vn, datafiles.chinhphu.vn, xaydungchinhsach.chinhphu.vn), Công báo (congbao.chinhphu.vn), Cơ sở dữ liệu quốc gia về văn bản pháp luật (vbpl.vn), Bộ Tài chính, Bộ Tư pháp, cổng thông tin các tỉnh (Cần Thơ, Nghệ An, Khánh Hòa, Quảng Nam...), Báo Đại biểu Nhân dân, Tạp chí Tòa án | Nguồn ưu tiên để đọc nguyên văn và xác nhận hiệu lực |
| Ngành thuế | Cổng Cục Thuế (gdt.gov.vn), phần mềm HTKK, cổng thuế điện tử (thuedientu.gdt.gov.vn, canhan.gdt.gov.vn), dịch vụ công thuế, cổng hóa đơn điện tử, tra cứu hóa đơn, tra cứu người nộp thuế | Skill đưa link cho người dùng để lấy mẫu, nộp hồ sơ, tra cứu. Công văn hướng dẫn chỉ được trích kèm nhãn ⚠️ |
| Cơ sở dữ liệu pháp luật | Thư Viện Pháp Luật (thuvienphapluat.vn), LuatVietnam (luatvietnam.vn), Thư viện Nhà đất, caselaw.vn, legalzone.vn, hethongphapluat.com, trang văn bản của VCCI, WIPO Lex | Xác nhận số hiệu, tình trạng hiệu lực; đọc văn bản hợp nhất hoặc bản đăng lại |
| Hãng tư vấn, kiểm toán | KPMG, EY, PwC, Baker McKenzie, Crowe, Forvis Mazars, Grant Thornton | Chỉ dùng để tìm số hiệu, điểm mới; **không** dùng làm căn cứ |
| Báo chí, trang chuyên ngành, phần mềm | Tạp chí Luật sư Việt Nam (lsvn.vn), VnEconomy, Thị trường Tài chính Tiền tệ, Thời báo Tài chính, Tạp chí Thuế, MISA (amis.misa.vn, misaeshop.vn, meinvoice.vn), iHoaDon, Luật Việt An, Vietnam Journals Online | Chỉ dùng để tìm từ khóa; một số file văn bản có chữ ký số được tải từ các trang này |

Mọi nội dung, nhãn hiệu và tài liệu tại các trang trên **thuộc về chủ sở hữu tương ứng**. Việc nêu tên và đặt link chỉ nhằm dẫn nguồn. Skill **không có liên kết, không được tài trợ hay xác nhận** bởi bất kỳ trang, tổ chức nào kể trên. Tên Claude, Gemini, Antigravity chỉ dùng để mô tả nền tảng cài đặt.

## Không chịu trách nhiệm

- Người phát hành skill **không chịu trách nhiệm** về bất kỳ thiệt hại, tổn thất, chế tài hay tranh chấp nào phát sinh từ việc sử dụng skill hoặc câu trả lời do AI tạo ra bằng skill.
- Người phát hành **không chịu trách nhiệm** về tính chính xác, tính cập nhật hay tình trạng truy cập của nội dung tại các trang bên thứ ba được dẫn link.
- Danh mục căn cứ chỉ đúng đến ngày baseline ghi trong `references/danh-muc-can-cu.md`. Văn bản ban hành sau ngày đó không được phản ánh, trừ khi người dùng chạy lệnh cập nhật.
- Skill không phải dịch vụ pháp lý. Mọi quyết định áp dụng là của người dùng.
- Chủ sở hữu nội dung nào cho rằng skill sử dụng nội dung của mình chưa phù hợp, vui lòng mở Issue trên kho GitHub này. Người phát hành sẽ xem xét chỉnh sửa hoặc gỡ bỏ phần liên quan.

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
