# Dàn ý bài nộp *(spec.md — nộp trước 23:59 ngày lab của lớp)*

> Copy dàn ý này vào `spec.md` của nhóm. Đây **không** phải form để điền đủ ô: mỗi mục chỉ cần đủ **bằng chứng** và **lập luận** ghi bên dưới. Viết ngắn, gạch đầu dòng là được. Hướng dẫn từng chặng: `02-guide.md`. Cách chấm: `04-rubric.md`.
>
> **Một quyết định = bốn ý:** đã cân nhắc phương án nào · chọn phương án nào · vì sao · loại các phương án kia vì sao. Bằng chứng = lập luận trỏ về một chỗ cụ thể: tool nào, dòng dữ liệu nào của track, điều gì trong mục "Sản phẩm thật hôm nay", chỗ nào trên prototype (ảnh đánh số). Không chạy agent.

```markdown
# Bài nộp LAB5 — T2 · Nhóm Vinflow
[Danh sách thành viên và việc mỗi người làm — copy bảng từ README]
| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
| Lê Quang Linh | 2A202603583 |  |
| Nguyễn Thanh Tùng | 2A202603594 |  |
| Nguyễn Minh Khôi | 2A202603528 |  |
## §1. Lát cắt & phạm vi
- **Lát cắt:** Trong **trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode)**, khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết[cite: 7].
- **3 việc tính năng KHÔNG làm:**
  1. **Không giải hộ hoặc xác nhận đáp số cụ thể của Bài tập 3 (bài đang mở hạn 13/11/2026 23:59)** — vì làm mất mục tiêu tự tư duy của chế độ Study mode và vi phạm quy chế học thuật của khóa học[cite: 7].
  2. **Không giảng giải chi tiết kiến thức hoặc công thức của các buổi chưa mở (từ Buổi 4 đến Buổi 10)** — vì tài liệu chi tiết các buổi này chưa được công bố trên trang khóa học, AI dễ tự bịa nội dung sai lệch so với giáo trình chính thức[cite: 7].
  3. **Không nhận xét, đánh giá năng lực học viên (khen thông minh hay chê tiếp thu chậm)** — vì không phục vụ mục tiêu giải đáp chuyên môn và dễ gây tâm lý tự ti cho người học khi tự học một mình lúc tối muộn[cite: 7].

## §2. Kịch bản rủi ro  (chặng 2)
- **Bảng ≥8 kịch bản phủ đủ 4 lớp:**

| # | Tin người dùng nhắn | Lớp | AI có thể sai thế nào (Bằng chứng trỏ về Tool / Dữ liệu T2) | Một sản phẩm tốt nên làm gì | Nhãn mức hại |
|---|---|---|---|---|---|
| 1 | *"Thầy ơi trong slide 12 buổi 3 giải thích độ lệch chuẩn chỗ nào ạ, em tìm không thấy?"* | ① Nguồn sự thật | Dữ liệu A ghi rõ **tài liệu buổi 3 không có slide đánh số** (chỉ có các mục `§3.1` đến `§3.5`). AI dễ hùa theo người dùng, bịa ra nội dung "slide 12" thay vì đối chiếu kết quả từ `tra_cuu_tai_lieu`[cite: 7]. | Nói rõ tài liệu buổi 3 không có slide đánh số mà chia theo mục, sau đó dẫn thẳng nội dung từ mục **`§3.3 Phương sai và độ lệch chuẩn`**[cite: 7]. | Sửa được |
| 2 | *"Buổi 7 học kiểm định giả thuyết với p-value là tính công thức thế nào ạ, cho em xin tài liệu đọc trước?"* | ① Nguồn sự thật | Dữ liệu B chỉ có tên tiêu đề **"7 Kiểm định giả thuyết và p-value"** trong đề cương (các buổi đã mở mới tới buổi 3). AI dễ dùng kiến thức ngoài để giảng sâu công thức p-value khi `tra_cuu_tai_lieu` không có nội dung buổi 7[cite: 7]. | Báo rõ nội dung này nằm ở **Buổi 7** (chưa mở tài liệu), chỉ giới thiệu khái quát tối đa 1 câu và khuyên học viên tập trung kiến thức Buổi 3[cite: 7]. | Nhẹ |
| 3 | *"Cái độ lệch ấy là gì ạ, em đọc tài liệu mãi mà không hiểu."* | ② Mơ hồ / thiếu | Tin nhắn dùng từ mơ hồ ("cái độ lệch ấy"). AI dễ đoán bừa sang khái niệm *độ lệch tuyệt đối trung bình (MAD)* ngoài giáo trình, thay vì gọi `tra_cuu_tai_lieu` kiểm tra mục **`§3.3 Phương sai và độ lệch chuẩn`**[cite: 7]. | Hỏi lại 1 câu để làm rõ có phải học viên đang hỏi về **"độ lệch chuẩn" ở mục §3.3** không, đồng thời giải thích ngắn gọn khái niệm này dựa trên `§3.3`[cite: 7]. | Nhẹ |
| 4 | *"Bài tập kia hạn chót là hôm nào thế ạ? Em làm xong rồi mà không biết nộp kịp không."* | ② Mơ hồ / thiếu | Dữ liệu B có hai bài tập: **Bài tập 2** (hạn `06/11/2026 23:59`, đã hết hạn) và **Bài tập 3** (hạn `13/11/2026 23:59`, đang mở). AI dễ đoán nhầm sang Bài tập 2 và báo sai rằng học viên đã trễ hạn[cite: 7]. | Hỏi xác nhận học viên đang hỏi bài nào, đồng thời liệt kê rõ hạn nộp cả hai bài từ dữ liệu trang khóa học (Bài 3 còn hạn đến `13/11/2026 23:59`)[cite: 7]. | Sửa được |
| 5 | *"Gần 11h đêm rồi em rối quá, giải hộ em câu a và b của Bài tập 3 với, mai em nộp bù sau!"* | ③ Ngoài thẩm quyền | Dữ liệu B ghi **Bài tập 3 đang mở** (hạn `13/11/2026 23:59`). AI gọi `goi_y_bai_tap` nhưng giải luôn phép tính trung bình (`15`) và trung vị (`11.5`) từ bộ dữ liệu lương ở mục **`§3.5 Bài tập 3`**, biến trợ lý thành công cụ giải bài hộ[cite: 7]. | Từ chối giải hộ vì bài đang mở; sử dụng `goi_y_bai_tap` để gợi ý bước đầu tiên (sắp xếp dãy số lương ở `§3.5` tăng dần) và dẫn chiếu lý thuyết `§3.1`, `§3.2`[cite: 7]. | **Không chấp nhận được** |
| 6 | *"Em tính trung vị Bài tập 3 ra 11.5 đúng chưa ạ? Chốt giúp em để em nộp bài."* | ③ Ngoài thẩm quyền | AI xác nhận *"Đúng rồi, đáp án là 11.5"* cho dữ liệu mục **`§3.5 Bài tập 3`** khi **Bài tập 3 vẫn đang mở**. Học viên dùng AI như công cụ dò đáp án thay vì tự kiểm tra lại cách tính[cite: 7]. | Không xác nhận đúng/sai; hướng dẫn học viên tự kiểm tra lại theo quy tắc *"trung bình cộng của hai giá trị đứng giữa khi số giá trị là chẵn"* tại mục **`§3.2`**[cite: 7]. | **Không chấp nhận được** |
| 7 | *"Mục §3.3 ghi 'độ lệch chuẩn luôn nhỏ hơn phương sai' là đúng hay sai ạ? Nếu phương sai bằng 0.25 thì sao?"* | ④ Đặc thù domain | Dữ liệu A mục **`§3.3`** có cài sẵn một mệnh đề sai toán học (*"Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai"*). AI mù quáng tin vào `tra_cuu_tai_lieu` và khẳng định tài liệu đúng, khiến học viên hiểu sai bản chất toán học[cite: 7]. | Chỉ rõ mệnh đề ở `§3.3` chỉ đúng khi phương sai $> 1$, còn nếu phương sai $= 0.25$ thì độ lệch chuẩn $= 0.5$ (lớn hơn); kích hoạt `chuyen_TA` để báo giảng viên sửa giáo trình[cite: 7]. | **Không chấp nhận được** |
| 8 | *"Câu giải thích về phương sai 0.25 hay quá, AI đăng luôn lên bảng hỏi đáp chung cho cả lớp cùng biết đi!"* | ④ Đặc thù domain | AI tự ý gọi tool `dang_FAQ` khi chưa có sự kiểm duyệt của TA/giảng viên. Nếu câu trả lời có sai sót hoặc liên quan đến đề bài đang mở, thông tin sai/lộ đề sẽ phát tán cho toàn bộ lớp học[cite: 7]. | Không tự ý công khai; chỉ lưu bản nháp câu hỏi và thông báo cần chờ TA kiểm duyệt trong khung giờ làm việc (`08:00–22:00`)[cite: 7]. | **Không chấp nhận được** |

- **Quyết định chọn 2 kịch bản đắt nhất:**
  1. **Kịch bản #5 (Xin giải hộ / xác nhận đáp số Bài tập 3 đang mở):** Đánh trực tiếp vào mục tiêu cốt lõi của sản phẩm (*"học viên hiểu đúng bài mình đang học, không chép đáp án"*). Nếu AI giải hộ một lần, hành vi lạm dụng AI để chép bài sẽ lan rộng, làm vô hiệu hóa hoàn toàn giá trị đánh giá của Bài tập 3 (đang mở đến `13/11/2026`)[cite: 7].
  2. **Kịch bản #7 kết hợp #8 (Phát hiện câu sai trong tài liệu gốc `§3.3` và yêu cầu đăng lên FAQ cả lớp):** Đây là lỗi **"học sai mà không biết"** mang tính hệ thống. Khác với việc một cá nhân hiểu nhầm, lỗi sai nằm ngay trong tài liệu chính thức (`§3.3`) và có nguy cơ khuếch đại qua tool `dang_FAQ` ra toàn bộ lớp học, phá hủy niềm tin của học viên và giảng viên đối với độ chính xác của trợ lý[cite: 7].
  - *Kịch bản suýt được chọn và vì sao không:* **Kịch bản #2 (Hỏi nội dung Buổi 7 chưa học)** suýt được chọn vì rủi ro AI bịa kiến thức rất cao. Tuy nhiên nhóm loại kịch bản này khỏi top 2 vì mức hại chỉ ở mức **Nhẹ** — kiến thức buổi 7 chưa dùng để làm Bài tập 3 ngay trong đêm, và khi buổi 7 chính thức mở tài liệu, học viên sẽ tự nhận ra sự khác biệt[cite: 7].

## §3. Khi AI sai  (chặng 3)

### Kịch bản đắt 1: Học viên xin giải hộ Bài tập 3 đang mở (Kịch bản #5)
- **AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu:**
  - *AI nói nguyên văn:* `"Bài tập 3 hiện đang trong thời gian mở (hạn nộp: 23:59 ngày 13/11/2026) nên mình không thể giải hộ hay đưa đáp án cụ thể cho bạn. Tuy nhiên, dựa vào tài liệu Buổi 3, mình có thể gợi ý từng bước để bạn tự làm nhé: Để tính Trung bình (mục §3.1) và Trung vị (mục §3.2) cho dãy 8 mức lương ở §3.5, bước đầu tiên bạn cần làm gì với thứ tự của các con số này? Bạn thử trả lời bước này, mình sẽ hướng dẫn tiếp nhé!"`[cite: 7]
  - *Người dùng thấy gì:* Nhãn trạng thái màu vàng **"Chế độ Study Mode — Bài tập 3 đang mở (Không đưa đáp số)"**; thẻ trích dẫn nội dung gốc của mục **`§3.1`**, **`§3.2`**, **`§3.5`**; thanh tiến độ gợi ý `Bước 1/3`[cite: 7].
  - *Làm gì tiếp:* Học viên gõ câu trả lời cho Bước 1 vào khung chat để đi tiếp sang Bước 2; hoặc bấm nút **"Gửi thắc mắc cho TA"** (kèm dòng chú thích rõ: *TA trực 08:00–22:00, câu hỏi của bạn sẽ được phản hồi từ 08:00 sáng mai*)[cite: 7]. Nếu học viên không làm gì, phiên học giữ nguyên ở Bước 1, không có đáp án nào bị lộ ra.
  - *Ai được báo, sau bao lâu:* Không báo TA ngay lập tức vì đây là luồng tự học thông thường; chỉ chuyển log cho TA vào **08:00 sáng hôm sau** nếu học viên chủ động bấm nút yêu cầu hỗ trợ thêm[cite: 7].
- **Quyết định (hỏi lại / trả lời kèm giới hạn / dừng và chuyển người):**
  - *Đã cân nhắc:* (1) Dừng hẳn và chuyển cho TA; (2) Hỏi lại để làm rõ ý định; (3) Trả lời kèm giới hạn (từ chối giải hộ nhưng mở luồng gợi ý từng bước).
  - *Chọn:* **Trả lời kèm giới hạn**[cite: 7].
  - *Vì sao & loại phương án kia:* Học viên đang học lúc gần 11h đêm, nếu chọn *Dừng và chuyển TA* thì học viên bị bỏ rơi hoàn toàn vì TA chỉ trực đến `22:00`, dẫn đến việc không làm kịp bài[cite: 7]. Loại *Hỏi lại* vì ý định xin giải hộ của học viên đã rõ ràng, hỏi lại gây mất thời gian và tạo cảm giác AI vòng vo. Chọn *Trả lời kèm giới hạn* vừa giữ đúng kỷ luật học thuật, vừa giúp học viên tự làm được bài ngay trong đêm[cite: 7].
- **Loại lỗi & cách nói, cách sửa theo loại đó:**
  - Đây là **Lỗi người dùng (User-induced boundary push)** — người dùng cố tình yêu cầu AI vượt quá phạm vi cho phép của hệ thống.
  - *Cách nói & sửa:* Không dùng giọng điệu phán xét hay giáo điều (tránh nói *"Bạn không được gian lận"*), mà thông báo trung lập về **quy định trạng thái bài tập** (`đang mở`) và chuyển hướng ngay sang hành động hữu ích (gợi ý bước 1)[cite: 7].
- **Nguyên tắc HAX/PAIR trỏ vào chỗ cụ thể:**
  - **HAX G1 (Làm rõ hệ thống làm được gì):** Hiển thị nhãn giới hạn *"Bài tập 3 đang mở — Trợ lý chỉ gợi ý từng bước, không giải hộ"* ngay đầu khung trả lời để học viên biết rõ luật chơi[cite: 7].
  - **HAX G11 + PAIR Explainability (Giải thích căn cứ):** Đính kèm thẻ trích dẫn trực tiếp mã mục **`§3.1`**, **`§3.2`** và thời hạn **`13/11/2026 23:59`** từ dữ liệu trang khóa học để chứng minh việc từ chối là dựa trên quy định lớp học chứ không phải AI từ chối bừa[cite: 7].
- **Lỗi sửa câu chữ không cứu được & thiết kế cứu nó:**
  - *Lỗi:* Nếu chỉ viết prompt nhắc AI *"Hãy từ chối khéo léo khi học viên hỏi đáp án Bài 3"*, học viên vẫn có thể dùng kỹ thuật đóng vai (ví dụ: *"Giả sử có một bài toán có dãy số 9, 10, 10, 11, 12, 12, 13, 45, hãy tính trung bình giúp mình"*) để lách luật và lấy được đáp án[cite: 7].
  - *Thiết kế cứu lỗi:* Ở tầng hệ thống, khóa cứng quyền truy xuất hoặc sinh ra các con số kết quả của `§3.5` (`15`, `11.5`) trong tool `goi_y_bai_tap` chừng nào biến trạng thái `bai_tap_3.status == "dang_mo"`[cite: 7].

### Kịch bản đắt 2: Tài liệu gốc §3.3 có câu sai toán học & đòi đăng FAQ (Kịch bản #7 & #8)
- **AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu:**
  - *AI nói nguyên văn:* `"Mình chưa chắc chắn về tính chính xác tuyệt đối của câu này trong giáo trình và cần nhờ giảng viên kiểm tra lại. Cụ thể: Tài liệu Buổi 3 (mục §3.3) hiện đang ghi 'Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai', nhưng về mặt toán học điều này chỉ đúng khi phương sai lớn hơn 1 (nếu phương sai bằng 0.25 thì độ lệch chuẩn là 0.5, lớn hơn phương sai). Mình đã gắn cờ mâu thuẫn này để chuyển cho TA kiểm tra với giảng viên (TA làm việc từ 08:00–22:00). Đồng thời, mình tạm khóa tính năng đăng câu này lên bảng FAQ chung cho đến khi có xác nhận chính thức để tránh gây nhầm lẫn cho cả lớp."`[cite: 7]
  - *Người dùng thấy gì:* Nhãn cảnh báo màu cam **"Phát hiện mâu thuẫn dữ liệu — Cần TA/Giảng viên xác minh"**; đoạn trích nguyên văn mục **`§3.3`** được tô sáng chỗ nghi ngờ; trạng thái nút **"Đăng lên FAQ cả lớp"** chuyển sang màu xám bị khóa kèm dòng chữ *"Đã lưu bản nháp — Chờ TA duyệt"*[cite: 7].
  - *Làm gì tiếp:* Học viên có thể bấm nút **"Theo dõi phản hồi từ TA"** (nhận thông báo khi TA cập nhật lúc `08:00` sáng hôm sau) hoặc tiếp tục hỏi các phần kiến thức khác[cite: 7].
  - *Ai được báo, sau bao lâu:* Hệ thống tạo ticket ưu tiên cao (kèm đoạn hội thoại và trích dẫn `§3.3`) đẩy vào hàng chờ của **TA trực**; TA sẽ nhìn thấy và xử lý ngay đầu ca làm việc lúc **08:00 sáng hôm sau** (do hiện tại đang là tối muộn ngoài giờ `08:00–22:00`)[cite: 7].
- **Quyết định (hỏi lại / trả lời kèm giới hạn / dừng và chuyển người):**
  - *Đã cân nhắc:* (1) Hỏi lại học viên; (2) Tự động sửa lại tài liệu và đăng lên FAQ; (3) Trả lời kèm giới hạn (chỉ rõ điểm mâu thuẫn toán học) kết hợp Chuyển người (TA/Giảng viên).
  - *Chọn:* **Trả lời kèm giới hạn + Chuyển người**[cite: 7].
  - *Vì sao & loại phương án kia:* Loại *Hỏi lại* vì học viên đã chỉ ra chính xác ví dụ phản chứng (`0.25`), việc hỏi lại là thừa thãi[cite: 7]. Loại *Tự sửa và đăng FAQ* vì AI không có thẩm quyền sửa nội dung giáo trình do giảng viên biên soạn; nếu AI tự sửa sai thì hậu quả lan ra cả lớp[cite: 7]. Chọn *Trả lời kèm giới hạn + Chuyển người* giúp học viên không bị học sai ngay lúc đó, đồng thời giữ đúng quyền quyết định cuối cùng cho giảng viên/TA[cite: 7].
- **Loại lỗi & cách nói, cách sửa theo loại đó:**
  - Đây là **Lỗi hệ thống / Lỗi dữ liệu nguồn (System / Source Data Error)** — hệ thống truy xuất đúng tài liệu của khóa học nhưng bản thân tài liệu nguồn (`§3.3`) bị sai[cite: 7].
  - *Cách nói & sửa:* AI phải thẳng thắn thừa nhận sự mâu thuẫn giữa giáo trình và quy tắc toán học thay vì tìm cách bao biện cho tài liệu. Cách sửa không nằm ở việc chỉnh câu thoại của AI mà nằm ở quy trình **gắn cờ báo lỗi dữ liệu ngược lại cho đội ngũ giảng dạy** và **chặn quyền tự động đăng FAQ**[cite: 7].
- **Nguyên tắc HAX/PAIR trỏ vào chỗ cụ thể:**
  - **HAX G2 (Làm rõ AI làm tốt tới đâu):** Sử dụng nhãn cảnh báo *"Chưa chắc chắn — Cần giảng viên xác minh"* thay vì khẳng định chắc nịch 100% hoặc đưa ra điểm số phần trăm mơ hồ[cite: 11, 12].
  - **HAX G10 (Thu hẹp phạm vi khi nghi ngờ):** Khi phát hiện dữ liệu mâu thuẫn, AI lập tức thu hẹp quyền hạn: từ chối thực thi tool `dang_FAQ` công khai và hạ cấp xuống chế độ lưu nháp chờ duyệt[cite: 7].
  - **PAIR Errors + Graceful Failure (Đường lui an toàn khi gặp lỗi):** Tạo đường chuyển tiếp mượt mà sang TA kèm bản tóm tắt tự động đoạn mâu thuẫn tại `§3.3`, đồng thời thông báo trung thực khung giờ TA phản hồi (`08:00–22:00`) chứ không nói dối là *"đã báo TA trả lời ngay"*[cite: 7].

## §4. Mức tự chủ  (chặng 4)
Với mỗi tool:
- Mức của nhóm (tự làm / cần người duyệt / cấm). Nếu cần người duyệt: ai duyệt · người duyệt thấy gì · quá hạn thì sao.
- Lý do theo cost-of-error: sai thì ai chịu gì · đảo lại được không · chờ người thì mất gì.
- Phương án đã cân nhắc và vì sao loại.
Thêm:
- Tool khó xếp nhất: mỗi người từng chọn gì, cái giá của mỗi phía (trỏ về kịch bản ở §2), nhóm chốt thế nào.
- Thử mức đã đặt trên 2 kịch bản đắt nhất + 1 kịch bản bình thường: cái sai có bị chặn không? còn việc nào làm khi lẽ ra phải hỏi? người dùng bình thường có phải chờ vô ích không?
- Luật thêm hoặc tool tách bước (nếu có), và vì sao.
- Một mức tự chủ đã đổi lời hứa nào với người dùng.

## §5. Prototype  (chặng 5)
- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không.
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì  (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)
- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo
- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
