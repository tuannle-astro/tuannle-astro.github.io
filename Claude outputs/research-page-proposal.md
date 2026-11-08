# Gợi ý cho trang Research

## 1. Rút ra gì từ 2 trang tham khảo

**Trang của Hải (hainn.clbtvusac.com/research.html)**
- Kể theo *câu chuyện*: hero → 4 chủ đề (thẻ có ảnh, 50–70 chữ, dòng "Highlights") → **Approach** (một sơ đồ pipeline) → **Open Questions** → **Facilities** → proposals.
- Viết ở ngôi thứ nhất, mở bằng ngôn ngữ đời thường rồi mới vào thuật ngữ, có dùng câu hỏi tu từ ("How do we weigh a black hole we cannot see?").
- Danh sách bài báo đẩy sang trang Publications, không lặp lại ở đây.

**Trang của Jacob (jacobpilawa.github.io/projects/)**
- Trang này không phải trang research: đó là trang *Projects* gồm tool tương tác, course notes, ảnh thiên văn. Mỗi mục có 1 thumbnail và 1 câu mô tả. (Trang /research/ của anh ấy chỉ có 2 đoạn văn.)
- Bài học: những thứ **CV không chứa được** (sản phẩm tự làm, ghi chú, sở thích) mới là thứ làm website "có người thật".

**Lưu ý quan trọng:** Hải cùng nhóm và cùng hướng với bạn. Hội đồng có thể xem cả hai trang (cùng lab, cùng tác giả trên nhiều bài). Nếu bạn cũng làm "4 themes + approach + facilities" thì hai trang sẽ trông như một khuôn. Nên học *cách kể* từ Hải, nhưng chọn **một trục kể khác**.

---

## 2. Trục kể đề xuất: "khi ánh sáng cản đường"

Đọc lại CV, ba bài bạn làm chính đều cùng một kiểu khó:

| Bài | Thứ che khuất / làm nhiễu | Bạn xử lý bằng cách |
|---|---|---|
| IC 342 (+ Maffei 2) | Bụi của mặt phẳng Ngân Hà | AO K-band, CO bandheads, gradient M/L của NSC trẻ |
| M81 | Continuum AGN phi nhiệt át ánh sáng sao | Tách continuum AGN, ensemble 24 mô hình JAM |
| NGC 3862 | Jet synchrotron, AGN, vành bụi quanh nhân | Mask jet/AGN, hiệu chỉnh bụi bằng color map F475W–F814W |

→ Một câu chủ đề mà CV không nói được: **"Đo khối lượng hố đen ở những nơi mà ánh sáng của chính thiên hà (bụi, AGN, jet) che mất tín hiệu"**. Đây là câu chuyện *của bạn*, khác với trục "theo dải khối lượng / theo thiết bị" của Hải.

(Bạn nên tự kiểm tra xem câu này có đúng với cách bạn nhìn công việc của mình không. Mình chỉ rút ra từ CV.)

---

## 3. Bố cục đề xuất

1. **Mở đầu (2–3 câu).** Nêu vấn đề, chưa nêu kết quả. Ví dụ hướng:
   > The model is rarely the hardest part of weighing a black hole. The hard part is that the galaxy's own light (dust, an active nucleus, a jet) gets in the way of the stars and gas we need to see.

2. **"The method in one picture".** Một sơ đồ do bạn tự vẽ (không cần xin phép ai):
   ảnh HST/JWST → MGE → mô hình khối lượng sao; phổ IFU → pPXF → động học; JAM/KinMS + MCMC → M_BH.
   Kèm 3–4 câu giải thích ý tưởng *trước*, tên công cụ *sau*. Phần này thay cho mục "Tools" khô khan hiện tại.

3. **Case studies (3 mục, mỗi mục ~100–150 chữ + 1 hình).** Mỗi mục trả lời 4 ý:
   *Vì sao khó → Tôi đã làm gì → Điều mình học được / bất ngờ → Kết quả + link.*
   Tiêu đề viết dạng câu chuyện, không ghi tên bài báo. Ví dụ:
   - *Behind the dust of the Milky Way*: IC 342, nối sang Maffei 2 (ongoing)
   - *When the nucleus outshines its stars*: M81
   - *A jet in the way*: NGC 3862

4. **The bigger picture (ngắn).** Vì sao các phép đo này quan trọng: đầu khối lượng thấp (seeding, IMBH), đầu khối lượng cao (UMBH ↔ sóng hấp dẫn nền), và ELT. Mục này gom các bài đồng tác giả (NGC 315, NGC 4258, NGC 4736, NGC 4061, ELT papers) thành **1 đoạn có link**, không liệt kê.

5. **Questions I want to pursue.** Phần này CV không có, và rất hợp với hồ sơ PhD. Phải là câu hỏi *của bạn* (mình không viết hộ). Bạn có thể tự hỏi:
   - Có bao nhiêu IMBH bị bỏ sót chỉ vì nằm sau bụi?
   - Giả định M/L không đổi gây sai lệch bao nhiêu cho các phép đo cũ?
   - Muốn đi tiếp hướng nào ở PhD?

6. *(Tùy chọn, học từ Jacob)* **Trang "Projects / Notes" riêng** cho những thứ ngoài bài báo: ISYA flare project, dự án ML với Gaia, ghi chú học tập, kính thiên văn tự làm hồi lớp 11. Không bắt buộc, nhưng làm trang web "có người".

---

## 4. Mẫu một case study (để xem giọng văn)

> ### When the nucleus outshines its stars: M81
>
> To weigh a black hole with stars, we first need to see the stars. In M81, the active nucleus adds a bright, non-thermal glow on top of the starlight at the very centre, exactly where the black hole's influence is strongest. If left in, it distorts both the stellar mass model and the measured motions.
>
> Using JWST/NIRSpec integral-field spectra, I separated the AGN continuum from the stellar light, then extracted two-dimensional stellar kinematics. Rather than trusting a single "best" model, we ran an ensemble of 24 Jeans models, varying the mass-to-light gradient, the PSF, the AGN mask and the orbital anisotropy, so the final mass carries these systematics honestly.
>
> **Result:** M<sub>BH</sub> = (4.77 ± 0.37) × 10<sup>7</sup> M<sub>⊙</sub>, resolving long-standing disagreement between earlier measurements. [ApJ 2026 →](https://doi.org/10.3847/1538-4357/ae64f0)
>
> *[Hình: bản đồ động học hoặc so sánh mô hình–dữ liệu, lấy từ bài (ApJ, CC BY) và ghi nguồn]*

Mọi thông tin trong mẫu đều lấy từ CV. Câu "điều mình học được / bất ngờ" thì mình để trống có chủ ý: đó là phần bạn tự viết, và chính phần đó làm trang khác CV.

---

## 5. So với bản hiện tại

| | Hiện tại | Đề xuất |
|---|---|---|
| Đơn vị kể | Chủ đề → danh sách bài | Vấn đề → case study |
| Vai trò của bạn | Nhãn "My role" | Hiện ra qua việc bạn đã làm |
| Bài đồng tác giả | Ngang hàng với bài của bạn | Gom vào "bigger picture" |
| Hình | Chưa có | 1 sơ đồ tự vẽ + 1 hình/case |
| Phần CV không có | Không | Phương pháp bằng lời, câu hỏi mở, (Projects) |
