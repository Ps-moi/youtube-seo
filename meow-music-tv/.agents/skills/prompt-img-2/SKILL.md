---
name: prompt-img-2
description: >
  Tạo các prompt ảnh AI chuyên nghiệp về mèo dễ thương trong sân vườn tương tác với chim, sóc/thỏ và đồ chơi. 
  Kích hoạt khi người dùng yêu cầu "cho tôi thêm N prompt", "tạo prompt ảnh mèo", "viết prompt sân vườn mèo chim",
  hoặc câu lệnh dạng: "Cho tôi thêm 5 prompt khác không trùng lặp. Lấy bối cảnh ở [...]".
  Luôn dùng skill này khi tạo prompt ảnh có mèo + chim + bối cảnh thiên nhiên.
---

# Skill: Cat × Bird Garden Prompt Generator

Tạo các prompt ảnh AI sinh động, đầy màu sắc về mèo dễ thương trong sân vườn, tương tác với chim muông và động vật nhỏ.

---

## Cú pháp lệnh của người dùng

```
Cho tôi thêm 5 prompt khác không trùng lặp. Lấy bối cảnh ở [bối cảnh]. [Chi tiết thêm]. [Yêu cầu đồ chơi/không].
```

Ví dụ:
```
Cho tôi thêm 5 prompt khác không trùng lặp. Lấy bối cảnh ở trong sân vườn. Có cây hoa, hồ nước nuôi cá cảnh. Sử dụng đồ chơi dành cho mèo.
```

---

## Ngân hàng tài nguyên

### 🐱 Giống mèo được phép dùng
- Mèo Munchkin lông ngắn (màu trắng, cam trắng, đen trắng, xám trắng, tam thể, vàng,...)
- Mèo Anh lông ngắn (British Shorthair) — màu xám trắng, xanh xám, nâu tabby,...

### 🐦 Danh sách chim được dùng
| Tên | Màu sắc |
|-----|---------|
| Cardinalis cardinalis | Vibrant red |
| Oriole | Bright orange |
| Cyanistes caeruleus | Blue and yellow |
| White-rumped Shama | Black, white, and chestnut |
| Budgerigar | Xanh lá & vàng hoặc xanh dương |
| African Grey | Xám với đuôi đỏ |

> ⛔ **Không dùng các loài chim ăn cá** (kingfisher, heron, pelican,...)

### 🐿️ Động vật nhỏ đi kèm
- Sóc (squirrel) — có thể núp sau vật hoặc đứng gần mèo/chim
- Thỏ trắng (white rabbit)
- Bướm trắng (white butterfly) — tối đa 2 con

### 🧸 Đồ chơi cho mèo

**Option 1 — Treo trên giá gỗ / cành cây:**
- Thú bông hình con chim
- Chổi lông (feather wand)
- Chuông gió
- Chiếc chuông nhỏ
- Lục lạc

**Option 2 — Đặt dưới đất:**
- Thú bông con chuột
- Cuộn len
- Banh lồng chuột (ball-in-ring toy)
- Cá nhồi bông
- Đồ chơi tháp bóng 3 tầng

### 🍽️ Đồ đựng thức ăn cho chim/sóc/thỏ

> ⚠️ Kích thước đồ đựng thức ăn **PHẢI nhỏ hơn chú mèo**

**Option 1 — Đặt dưới đất:**
- Tô gỗ / đĩa gỗ
- Tấm đá phẳng
- Tấm gỗ tròn
- Thùng gỗ nhỏ

**Option 2 — Treo trên giá / cành cây:**
- Hộp treo xinh xắn

**Option 3 — Kiểu 2 tầng đặt dưới đất:**
- Tầng trên: đựng nước uống cho chim
- Tầng dưới: đựng thức ăn

### 🍓 Thức ăn trong đồ đựng (phải đủ tất cả)
- Chùm nho xanh
- Táo cắt đôi
- Hạt dẻ
- Trái kiwi cắt đôi
- Hạt ngô
- Trái dâu tây cắt đôi

---

## Quy tắc bắt buộc (KHÔNG được vi phạm)

### 🐱 Về chú mèo
- ✅ Lông ngắn, không xù
- ✅ Mặt dễ thương, vui vẻ, đáng yêu, cute
- ✅ Mắt hướng về đúng đối tượng (đồ chơi → nhìn đồ chơi; chim → nhìn chim)
- ✅ Tư thế ngồi hoặc đứng — có thể đang vươn tay với đồ chơi
- ❌ Không nằm
- ❌ Không nhìn chính diện vào camera
- ❌ Không mặt cool ngầu / hung dữ
- ❌ Không nhìn vô hướng / không mục đích

### 📸 Về góc chụp & ánh sáng
- ✅ Góc ngang (eye-level) hoặc hơi thấp
- ✅ Ánh sáng buổi sáng nhẹ nhàng, tươi sáng
- ✅ Depth of field rõ ràng (foreground-midground-background)
- ❌ Không chụp từ trên cao xuống (bird's eye view)
- ❌ Không backlight / ngược sáng
- ❌ Không ánh sáng gắt / lóa
- ❌ Không ánh nắng lờ mờ gây ảnh hưởng chất lượng

### 🌿 Về bối cảnh
- ✅ Nền chính là **cỏ xanh** (grass-dominant ground)
- ✅ Có thể kết hợp đất, cát, đá nhỏ — nhưng cỏ phải là chủ đạo
- ✅ Hoa: số lượng vừa đủ, tạo điểm nhấn — không quá nhiều
- ✅ Màu sắc sinh động, đầy sức sống
- ✅ Bức ảnh có chiều sâu (depth)

### 🌟 Về điểm nhấn tổng thể
- Mèo và chim là **nhân vật chính**
- Sóc/thỏ/bướm là phụ, tạo thêm sức sống
- Không có yếu tố nào lấn át nhân vật chính

---

## Cấu trúc prompt chuẩn

```
[SHOT & STYLE] Clear, well-lit, [angle] shot with detailed background and clear depth of field. Soft morning sunlight, no backlight, no harsh light.

[GROUND/SETTING] Primary ground is lush green grass [+ secondary elements: clean dirt / fine sand / small pebbles]. [Background scenery per user request].

[FLORA] [Nếu có hoa: A beautiful cluster of [loài hoa] blooming nearby — quantity kept tasteful, not overwhelming.]

[CAT] A [màu sắc] short-haired [giống mèo] cat with smooth, non-fluffy coat is [tư thế đứng/ngồi + hành động]. The cat has an adorable, cheerful, and curious expression with sweet eyes gazing [toward đối tượng cụ thể].

[CAT TOY — nếu có] [Mô tả đồ chơi + cách mèo tương tác — eyes directed at the toy].

[FOOD CONTAINER] A [mô tả đồ đựng] — notably smaller than the cat — holds [danh sách đủ 6 loại thức ăn: green grape clusters, halved apples, chestnuts, halved kiwi, corn kernels, halved strawberries].

[BIRDS] [Số lượng] birds are eating from it: [Tên chim 1 (màu)], [Tên chim 2 (màu)], [Tên chim 3 (màu)][, Tên chim 4 nếu có].

[SMALL ANIMAL] [Mô tả sóc/thỏ + vị trí — peeking from behind / near the feeder / close to the cat].

[BUTTERFLY — nếu có] Two white butterflies flutter gracefully nearby.
```

---

## Ví dụ prompt mẫu hoàn chỉnh

```
Clear, well-lit, ground-level shot with a detailed garden background and clear depth of field. Soft morning sunlight casting a fresh, gentle glow — strictly no backlight or harsh lighting.

Primary ground is lush green grass mixed with fine clean dirt. A small wooden garden fence lines the background, with climbing roses in soft pink adding gentle color accents — kept tasteful and not overwhelming.

A white short-haired Munchkin cat with a smooth, non-fluffy coat sits upright on the grass, one paw gently raised and reaching toward a hanging feather wand toy suspended from a small wooden stand. The cat's expression is utterly adorable and joyful, with big round sweet eyes gazing attentively at the feather toy.

A round wooden tray — noticeably smaller than the cat — rests on the grass nearby, holding green grape clusters, halved apples, chestnuts, halved kiwi, corn kernels, and halved strawberries.

Three birds eat from the tray: a Cardinalis cardinalis (vibrant red), a Cyanistes caeruleus (blue and yellow), and an African Grey (grey with a red tail).

A small squirrel peeks out curiously from behind a mossy garden stone near the food tray, its tiny eyes wide with interest.

The entire scene is bathed in soft, clear morning light with vivid, lively colors and beautiful depth from foreground to background.
```

---

## Checklist trước khi xuất prompt

- [ ] Mèo đúng giống & màu yêu cầu
- [ ] Mèo không nằm, không nhìn thẳng camera, không mặt hung
- [ ] Mắt mèo hướng đúng đối tượng
- [ ] Đủ 3–4 chú chim đúng loài yêu cầu (không dùng chim ăn cá)
- [ ] Đồ đựng thức ăn nhỏ hơn mèo
- [ ] Đủ 6 loại thức ăn trong đồ đựng
- [ ] Nền cỏ là chủ đạo
- [ ] Không backlight / ánh sáng gắt / lờ mờ
- [ ] Không góc từ trên cao
- [ ] 5 prompt không trùng lặp nhau (giống mèo, màu, đồ chơi, chim, bối cảnh, đồ đựng)