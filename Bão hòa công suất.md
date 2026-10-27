Kết luận chính: **sai pha không phải do bão hòa.** Sai pha phụ thuộc vào mã gain, không phụ thuộc mức tín hiệu vào.

Bài đo dùng file Through lúc 11:13, chỉ đo dải 1. Mức trôi pha đầu và cuối phiên của CH1, CH2, CH4 dưới 4°, nên số đo dùng được.

**1. Quét mức vào (CH1 còn ADTR)**

| Gain | Mức vào | Công suất ra board | Độ lợi so với −45 dBm | Pha TB lệch | Sai pha RMS |
|---|---|---|---|---|---|
| 127 | −45 dBm | −25,5 dBm | 0 | 0 | 18,5° |
| 127 | −30 dBm | −10,2 dBm | +0,3 dB | −0,3° | 18,3° |
| 127 | −15 dBm | +4,8 dBm | +0,4 dB | −0,9° | 18,2° |
| 96 | −45 → −15 dBm | −27,4 → +3,0 dBm | ≤ +0,4 dB | ≤ 1,2° | 14,7° ở cả 7 mức |

- Tăng mức vào 30 dB thì công suất ra tăng đúng 30 dB, pha gần như không đổi. Sai pha giữ nguyên 18° ở gain 127 và 15° ở gain 96.
- Như vậy đến +5 dBm đầu ra, CH1 chưa có dấu hiệu nén hay phi tuyến. Sai pha lớn ở gain cao không phải do tín hiệu mạnh.

**2. Công suất theo gain, mức vào −30 dBm** (trả lời câu anh Quân hỏi về gain 0 và 127)

| Kênh | Ra ở gain 0 | Ra ở gain 127 | Tăng từ 96→112→127 | Sai pha ở gain 16 / 64 / 127 |
|---|---|---|---|---|
| CH1 | −41,7 dBm | −10,8 dBm | +1,1 / +0,6 dB | 4,8 / 9,4 / 17,4° |
| CH2 | −46,6 dBm | −13,2 dBm | +1,3 / +0,8 dB | 5,4 / 4,4 / 6,3° |
| CH4 | −44,0 dBm | −12,0 dBm | +1,2 / +0,8 dB | 4,8 / 6,1 / 11,3° |
| CH3 (bỏ ADTR) | −55,3 dBm | −42,2 dBm | +1,5 / +0,4 dB | tín hiệu quá yếu, không dùng được |

- **Gain gần như không tăng từ mã 96 lên 127, ở cả CH3 đã bỏ ADTR.** Đây là đặc tính của mã gain ADAR, không phải ADTR bị nén. Hôm 15/10 tao còn nghi là nén, số đo hôm nay loại được khả năng đó.
- **CH2 cũng còn ADTR nhưng sai pha giữ 4–6° ở mọi gain.** CH1 tăng từ 5° lên 17°, CH4 từ 5° lên 11°. Vậy có ADTR và gain cao chưa đủ gây sai pha lớn; lý do CH1 và CH4 khác CH2 thì chưa xác nhận.
- Ở gain thấp (16–32), cả 3 kênh còn ADTR đều sai pha khoảng 4–5°, ngang CH3 khi đo được.

**3. CH3 (bỏ ADTR) bị giới hạn bởi nhiễu trên ZVL**
- CH3 ra yếu: ở mức vào −30 dBm chỉ khoảng −42 đến −55 dBm. Vì vậy bài công suất theo gain của CH3 và các mức vào −45 đến −25 dBm toàn nhiễu (trôi pha tới 88–160°).
- Chỉ từ mức vào −20 dBm trở lên mới đọc được. Ở −15 dBm, CH3 sai pha 6,0° ở gain 96 và 5,4° ở gain 127, gain 127 không xấu hơn gain 96. Kết quả này khớp với số đo E5080B hôm 23/10 (3,5–4,9°, không đổi theo gain).

**Tin nhắn gửi anh Quân** (mày xem trước rồi gửi):

> Em gửi anh kết quả đo ngày 27/10 trên ZVL (dải 12,77–12,97 GHz, module có CH3 đã bỏ ADTR):
> 1. Quét mức vào từ −45 đến −15 dBm ở gain 96 và 127, CH1 (còn ADTR): công suất ra tăng đúng theo mức vào, tối đa khoảng +5 dBm. Độ lợi lệch dưới 0,5 dB, pha lệch dưới 1,2°, sai pha giữ nguyên 15° (gain 96) và 18° (gain 127). Trong dải này em chưa thấy ADTR bị nén hay phi tuyến.
> 2. Công suất ra ở mức vào −30 dBm: gain 0 khoảng −42 đến −47 dBm, gain 127 khoảng −11 đến −13 dBm (CH1, CH2, CH4). Từ gain 96 lên 127 công suất chỉ tăng thêm khoảng 2 dB, kể cả ở CH3 không có ADTR, nên đây là đặc tính mã gain của ADAR.
> 3. Sai pha tăng theo mã gain ở CH1 (5° lên 17°) và CH4 (5° lên 11°), còn CH2 giữ 4–6°. Nguyên nhân em chưa xác nhận được.
> 4. CH3 không có ADTR ra yếu nên ZVL chỉ đo được ở mức vào từ −20 dBm. Ở −15 dBm sai pha 5–6°, không tăng theo gain.

Tao đã lưu các kết quả xác nhận hôm nay vào ghi chú dự án để lần sau phân tích tiếp. Mày muốn thì tao đưa các bảng này vào báo cáo Word.