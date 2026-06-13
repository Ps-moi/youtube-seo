---
name: cat-bird-garden-prompt
description: Tạo prompt ảnh nghệ thuật về mèo, chim, sóc/thỏ trong vườn thiên nhiên. Sử dụng skill này mỗi khi người dùng yêu cầu tạo prompt ảnh mèo cùng chim trong bối cảnh thiên nhiên, sân vườn, hoặc yêu cầu "thêm 5 prompt", "prompt mới không trùng lặp", "lấy bối cảnh ở...". Trigger ngay cả khi người dùng chỉ nói ngắn gọn như "cho tôi 5 prompt khác" hoặc "lấy bối cảnh ở trong nhà".
---

# Cat-Bird Garden Prompt Generator

Skill tạo các prompt ảnh nghệ thuật chất lượng cao, mô tả cảnh mèo – chim – sóc/thỏ trong thiên nhiên sân vườn đầy màu sắc và sinh động.

---

## Cách người dùng gọi skill này

Người dùng sẽ gõ lệnh ngắn theo mẫu:

```
Cho tôi thêm 5 prompt khác không trùng lặp. Lấy bối cảnh ở [bối cảnh]. [Chi tiết thêm nếu có]. [Yêu cầu đặc biệt nếu có].
```

**Claude cần tự điền các thông số còn lại** theo bộ quy tắc bên dưới — người dùng KHÔNG cần gõ lại toàn bộ yêu cầu.

---

## QUY TẮC BẤT BIẾN (Áp dụng cho MỌI prompt)

### 🐱 Mèo
| Thông số | Quy tắc |
|----------|---------|
| Giống mèo | Theo từng prompt (xem bảng bên dưới) |
| Lông | Ngắn, KHÔNG xù, mịn |
| Tư thế | KHÔNG nằm — ngồi, đứng, đang chơi, đang với tay, đang nghiêng đầu, đang nhún mình |
| Biểu cảm | Dễ thương, đáng yêu, vui vẻ, tò mò — KHÔNG cool ngầu, KHÔNG hung dữ |
| Mắt | Tròn to, sáng, nhìn có mục đích rõ ràng (nhìn đồ chơi / nhìn chim / nhìn thức ăn...) |
| Góc nhìn | KHÔNG nhìn thẳng chính diện vào ống kính |
| Góc chụp | KHÔNG chụp từ trên cao xuống (no bird's eye view) |

### 🐦 Chim (Mặc định 4 loài — trừ khi prompt chỉ định khác)
Ưu tiên phối 4 loài 4 màu khác nhau:
- **Cardinalis cardinalis** — đỏ rực
- **Oriole** — cam sáng
- **Cyanistes caeruleus** (Blue Tit) — xanh dương & vàng
- **White-rumped Shama** — đen, trắng & nâu hạt dẻ

> ⚠️ KHÔNG dùng các loài chim ăn cá (kingfisher, heron, pelican...).

### 🌿 Bối cảnh
- **Nền chính là cỏ xanh** — sau đó mới đến đất, cát, sỏi, rêu, lá rụng...
- Ánh sáng: ban mai hoặc chiều tà mềm mại — TUYỆT ĐỐI KHÔNG ngược sáng
- Ảnh có **chiều sâu** (depth of field rõ ràng), màu sắc sinh động
- Có thể thêm hoa nhưng số lượng VỪA ĐỦ — không để hoa lấn át nhân vật chính

### 🐿️ Sóc / Thỏ
- Mỗi prompt có 1 con sóc HOẶC 1 con thỏ (theo chỉ định)
- Sóc có thể đứng sau vật gì đó (đá, thân cây, chậu hoa...) hoặc đứng tự do gần mèo / bầy chim
- Kích thước NHỎ HƠN chú mèo

---

## BẢNG THÔNG SỐ 5 PROMPT MẶC ĐỊNH

| Prompt | Giống mèo | Màu mèo | Chim | Động vật phụ | Ghi chú |
|--------|-----------|---------|------|--------------|---------|
| 1 | Munchkin lông ngắn | Trắng | Cardinal, Blue Tit, African Grey | 1 sóc | — |
| 2 | Munchkin lông ngắn | Cam trắng | Cardinal, Blue Tit, White-rumped Shama | 1 thỏ trắng | — |
| 3 | Munchkin lông ngắn | Đen trắng | Cardinal, Blue Tit, Oriole | 1 sóc + 2 bướm trắng | — |
| 4 | Mèo Anh lông ngắn | Xám trắng | Cardinal, Blue Tit, Oriole, Budgerigar | 1 thỏ trắng | 4 chim |
| 5 | Toyger lông ngắn | Vằn hổ | Cardinal, Blue Tit, Oriole, Budgerigar | 1 thỏ trắng | 4 chim |

> Khi người dùng yêu cầu "5 prompt mới", hãy THAY ĐỔI giống mèo & màu mèo, nhưng giữ bộ chim theo bảng trên hoặc xoay vòng hợp lý.

---

## ĐỒ CHƠI CHO MÈO

Chọn **1 trong 2 nhóm** mỗi prompt (xoay vòng để không trùng):

**Option A — Treo/Trên cao:**
- Thú bông hình chim treo trên cành cây / giá gỗ
- Chổi lông treo
- Chuông gió nhỏ
- Chuông / lục lạc treo

**Option B — Đặt dưới đất:**
- Thú bông con chuột
- Cuộn len màu sắc
- Banh lồng chuột
- Cá nhồi bông
- Tháp bóng 3 tầng

> Đồ chơi phải **phù hợp với hành động của mèo**: mèo đang vươn tay lên → đồ chơi treo cao; mèo đang vồ → đồ chơi dưới đất.

---

## ĐỒ ĐỰNG THỨC ĂN CHO CHIM

Chọn **1 kiểu** mỗi prompt (xoay vòng):

**Option A — Đặt dưới đất:**
- Tô gỗ tròn
- Đĩa gỗ phẳng
- Tấm đá tự nhiên phẳng
- Tấm gỗ tròn rustic
- Thùng gỗ nhỏ

**Option B — Treo:**
- Hộp gỗ treo trên cành cây
- Giá đỡ gỗ có khay đựng thức ăn

**Option C — 2 tầng:**
- Tầng trên: bát nước uống cho chim
- Tầng dưới: đựng thức ăn

> ⚠️ Kích thước đồ đựng thức ăn phải **NHỎ HƠN chú mèo**.

---

## THỨC ĂN (Tối thiểu 4 loại, đa dạng mỗi prompt)

Chọn từ danh sách — ưu tiên xoay vòng qua các prompt:

| Thức ăn | Cách trình bày |
|---------|---------------|
| Chùm nho xanh nhỏ | Nguyên chùm hoặc tách hạt |
| Táo | Cắt đôi, thấy rõ ruột |
| Dâu tây | Cắt đôi |
| Kiwi | Cắt đôi, thấy ruột xanh |
| Hạt ngô | Rải hoặc thành cụm |
| Hạt dẻ | Nguyên hạt |
| **Hạt đậu** | ⚠️ BẮT BUỘC cắt đôi — thấy rõ bên trong |

> Hạt đậu phải được cắt ra làm đôi trong mọi prompt có hạt đậu.

---

## CẤU TRÚC PROMPT TIẾNG ANH

Mỗi prompt cần bao gồm đủ các thành phần sau theo thứ tự:

```
[OPENING — bối cảnh tổng thể & ánh sáng]
[GROUND — nền cỏ + đất/cát/sỏi + chi tiết bối cảnh]
[FLORA — cây cối, hoa (vừa đủ), yếu tố đặc trưng của bối cảnh]
[CAT — giống, màu, tư thế, hành động, biểu cảm, hướng nhìn]
[TOY — đồ chơi & cách mèo tương tác]
[FEEDER — đồ đựng thức ăn, kiểu dáng, vật liệu]
[BIRDS — từng loài, màu sắc, đang ăn / đang đậu]
[FOOD — liệt kê chi tiết thức ăn trong đồ đựng]
[WILDLIFE — sóc/thỏ, vị trí, hành động]
[BUTTERFLY — nếu có]
[LIGHTING & TECHNICAL — ánh sáng, depth of field, màu sắc, góc chụp]
```

---

## VÍ DỤ PROMPT HOÀN CHỈNH (Tham khảo)

> **Prompt 1 — Munchkin trắng, sân vườn Nhật:**

*A beautifully lit garden scene in soft morning sunlight, set in a traditional Japanese-style backyard with a stone lantern and small mossy stepping stones. The primary ground is lush green grass blending into fine earthy soil. Nearby, a cluster of soft white Hydrangea blooms adds gentle color without overwhelming the scene.*

*In the midground, a short-legged white Munchkin cat with smooth, sleek short fur sits upright with its head tilted curiously to one side. Its large round eyes are bright and warm, gazing attentively at a small feathered toy bird hanging from a low wooden branch above — its tiny paw gently raised as if about to bat at it. Expression: utterly adorable and playful, not aloof.*

*To the side, a rustic two-tiered wooden bird feeder (noticeably smaller than the cat) sits on the grass: the upper tier holds fresh water, the lower tier holds a colorful spread of halved strawberries, sliced kiwi (revealing bright green flesh), small green grape clusters, and split peas (cut cleanly in half showing the interior). A small squirrel peeks out curiously from behind the stone lantern near the feeder.*

*Perched around the feeder are three birds: a vibrant red Northern Cardinal, a blue-and-yellow Cyanistes caeruleus (Eurasian Blue Tit), and a sleek African Grey parrot. Each bird is distinct and colorful.*

*The image is bathed in warm, even morning light with no backlight. Sharp foreground, rich depth of field, vivid and lively colors. Camera angle is at ground level or slight low angle — never top-down.*

---

## KHI NGƯỜI DÙNG GỌI SKILL

**Input mẫu:**
```
Cho tôi thêm 5 prompt khác không trùng lặp. Lấy bối cảnh ở trong sân vườn. Có cây hoa, hồ nước nuôi cá cảnh. Sử dụng đồ chơi dành cho mèo.
```

**Claude cần làm:**
1. Xác định bối cảnh từ input (ví dụ: sân vườn có hồ cá cảnh)
2. Xác định các yêu cầu đặc biệt (ví dụ: có đồ chơi mèo)
3. Tạo 5 prompt tiếng Anh hoàn chỉnh theo cấu trúc trên
4. Mỗi prompt thay đổi: giống/màu mèo, bộ chim, đồ chơi, đồ đựng thức ăn, thức ăn, vị trí sóc/thỏ
5. KHÔNG lặp lại combo đã dùng trong các lần trước cùng cuộc hội thoại

---

## CHECKLIST TRƯỚC KHI XUẤT PROMPT

Trước khi hoàn tất mỗi prompt, kiểm tra:

- [ ] Mèo KHÔNG nằm
- [ ] Mèo KHÔNG nhìn thẳng vào ống kính
- [ ] Mèo KHÔNG có biểu cảm lạnh lùng / hung dữ
- [ ] Ánh mắt mèo nhìn vào vật cụ thể (đồ chơi / chim / thức ăn)
- [ ] Góc chụp KHÔNG từ trên cao xuống
- [ ] Nền chính là cỏ xanh
- [ ] Ánh sáng KHÔNG ngược sáng
- [ ] Hạt đậu được cắt đôi (nếu có)
- [ ] Kích thước đồ đựng thức ăn nhỏ hơn mèo
- [ ] Có ít nhất 4 loại thức ăn
- [ ] Hoa vừa đủ, không lấn át nhân vật chính
- [ ] Prompt viết bằng tiếng Anh, đủ các thành phần cấu trúc