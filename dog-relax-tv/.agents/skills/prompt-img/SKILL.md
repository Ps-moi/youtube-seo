---
name: prompt-img
description: >
  Tạo các prompt ảnh chó thực tế, sống động, cân bằng ánh sáng và màu sắc cho AI image generation.
  Sử dụng skill này bất cứ khi nào người dùng yêu cầu viết prompt ảnh chó với nhiều giống, trang phục,
  đồ chơi và bối cảnh khác nhau — đặc biệt khi có yêu cầu về số lượng prompt, số lượng giống chó (2/3/4),
  bối cảnh châu Âu, hoặc không trùng lặp với các prompt đã tạo trước đó.
---

# Dog Photo Prompt Generator

Skill này giúp tạo ra các prompt ảnh chó chuyên nghiệp: chân thật, sống động, cân bằng ánh sáng, màu sắc hài hòa, bối cảnh đa dạng và không lặp lại.

---

## 1. CẤU TRÚC PROMPT CHUẨN

Mỗi prompt phải có đủ 7 lớp sau, theo thứ tự:

```
[SHOT TYPE] + [SETTING/BACKGROUND] + [DOG SUBJECTS] + [OUTFITS] + [TOYS/PROPS] + [ACTION] + [TECHNICAL TAGS]
```

### Ví dụ đầy đủ:
```
A vibrant, highly realistic action photograph on a sun-dappled lakeside dock in a lush European summer forest. A cheerful black-and-white Border Collie wearing a red chest harness and a smiling golden Cocker Spaniel wearing a teal bandana collar are playing an energetic game of tug-of-war with a thick braided rope toy. Their expressions are joyful and playful, mouths open in happy grins. Soft dappled sunlight filtering through the trees, natural color balance, no overexposure. Photorealistic, 8k resolution.
```

---

## 2. QUY TẮC SỐ LƯỢNG CHÓ THEO NHÓM PROMPT

Khi người dùng yêu cầu N prompt chia theo nhóm:

| Nhóm | Số chó | Cấu trúc |
|------|--------|-----------|
| Nhóm đầu (thường 2 prompt) | 2 chó | Chó chủ đạo + 1 chó khác |
| Nhóm giữa (thường 2 prompt) | 3 chó | Chó chủ đạo + 2 chó khác |
| Nhóm cuối (thường 2 prompt) | 4 chó | Chó chủ đạo + 3 chó khác |

- **Chó chủ đạo**: Giống chó do người dùng chỉ định (ví dụ: Border Collie)
- **Chó khác**: Lấy từ danh sách giống chó người dùng cung cấp, không được lặp lại cùng combo giống chó trong cùng batch

---

## 3. BỘ TRANG PHỤC CHO CHÓ (DOG OUTFITS)

Mỗi chú chó trong cùng prompt phải mặc **trang phục khác nhau**. Xoay vòng trong danh sách sau:

- Collar (vòng cổ): leather collar, studded collar, floral collar, bandana collar, pearl collar
- Harness (đai yếm): chest harness, sport harness, padded vest harness, mesh cooling harness
- Clothing (áo): striped t-shirt, hoodie, raincoat, life jacket, sailor outfit, floral dress, camo shirt, denim jacket
- Accessories: backwards cap, sun hat, bucket hat, sunglasses, goggles, bow tie, neckerchief

**Quy tắc**: Trong một prompt với 3 chó, không được để 2 chó mặc cùng loại phụ kiện chính.

---

## 4. BỘ ĐỒ CHƠI VÀ PROPS

Xoay vòng, không trùng lặp giữa các prompt trong cùng batch:

| Loại | Các lựa chọn |
|------|-------------|
| Tug rope | thick braided rope, colorful knotted rope, multi-colored rope toy |
| Ball & frisbee | tennis ball, rubber ball, colorful beach ball, foam frisbee, disc toy |
| Stuffed toy | plush duck, stuffed raccoon, squeaky hedgehog, plush fox |
| Chew toy | rubber chew ring, knotted chew rope, antler chew, colorful chew stick |

---

## 5. BỐI CẢNH CHÂU ÂU (EUROPEAN SETTINGS)

### Bối cảnh rừng + hồ (ưu tiên theo yêu cầu mặc định):
- Sun-dappled lakeside dock with a small wooden rowboat, wildflower meadow, wooden footbridge, summer European forest cabin
- Alpine meadow clearing beside a still mountain lake, wildflowers, rustic stone bridge, pine forest backdrop
- Bavarian forest path near a glassy lake, old wooden boathouse, mossy stone bridge, blooming elderflower bushes

### Các bối cảnh châu Âu khác (đa dạng hóa):
- Cobblestone village square with flower boxes, Amsterdam canal, Tuscany olive grove, Scottish coastal cliff, Provence lavender field, Swiss alpine pasture, Santorini whitewashed terrace, English countryside garden, Norwegian fjord meadow

### Quy tắc bối cảnh:
- Không lặp lại cùng bối cảnh trong cùng một batch 6 prompt
- Luôn bao gồm yếu tố ánh sáng tự nhiên (golden hour, soft dappled sunlight, bright noon sun)

---

## 6. KIỂM SOÁT ÁNH SÁNG & MÀU SẮC (CRITICAL)

Đây là yếu tố quan trọng nhất để ảnh không bị lỗi. **Luôn thêm** các tag sau vào cuối mỗi prompt:

### Tag ánh sáng cân bằng (chọn 1-2 phù hợp bối cảnh):
- `natural soft daylight, no overexposure`
- `warm golden hour lighting, balanced exposure`
- `bright sunny daylight with soft shadows`
- `soft diffused summer sunlight, true-to-life colors`
- `vivid yet natural color palette, no blown highlights`

### Tag chất lượng ảnh (luôn có):
- `photorealistic, 8k resolution`
- `award-winning pet photography, sharp focus`
- `cinematic depth of field, vibrant but natural colors`

### KHÔNG dùng:
- ❌ "vivid HDR" (gây overexposed)
- ❌ "ultra bright" (mất chi tiết)
- ❌ "neon colors" (không tự nhiên)

---

## 7. BIỂU THỨC & HÀNH ĐỘNG CHÓ

Luôn mô tả biểu cảm vui vẻ. Xoay vòng các hành động:

| Hành động | Mô tả trong prompt |
|-----------|-------------------|
| Tug of war | enthusiastically pulling, leaning back with all their weight, paws planted firmly |
| Chase/keep away | running playfully, looking back over shoulder with teasing expression |
| Jumping/splashing | leaping incredibly high, massive water droplets splashing dynamically |
| Skating/riding | zooming fast downhill, ears flapping in the wind |
| Fetch | mid-leap catching, mouth open wide, eyes locked on toy |
| Swimming | paddling energetically, splashing joyfully |

**Biểu cảm luôn dùng**: joyful expressions, happy open-mouthed grins, bright alert eyes, playful and energetic demeanor

---

## 8. QUY TRÌNH TẠO BATCH PROMPT

Khi nhận yêu cầu, thực hiện theo thứ tự:

1. **Đọc yêu cầu**: Xác định (a) danh sách giống chó, (b) bối cảnh, (c) đồ chơi, (d) trang phục, (e) số prompt cần tạo
2. **Lập bảng phân công**: Trước khi viết, lên danh sách phân công giống chó / bối cảnh / đồ chơi / trang phục cho từng prompt để tránh trùng
3. **Viết prompt**: Theo cấu trúc 7 lớp, đảm bảo mỗi prompt dài 80-150 từ
4. **Kiểm tra chéo**: Đảm bảo không prompt nào trùng về (a) combo giống chó, (b) hành động chính, (c) bối cảnh, (d) đồ chơi chính
5. **Đánh số**: Đánh số thứ tự liên tiếp theo batch (Prompt 6, 7, 8... nếu đã có 5 prompt mẫu)

---

## 9. TEMPLATE PROMPT THEO SỐ LƯỢNG CHÓ

### Template 2 chó:
```
A [SHOT_TYPE] in [EUROPEAN_SETTING]. A [DOG1_BREED] wearing [OUTFIT1] and a [DOG2_BREED] wearing [OUTFIT2] are [ACTION] with a [TOY]. [EXPRESSION_DESC]. [LIGHTING_TAG]. Photorealistic, 8k resolution.
```

### Template 3 chó:
```
A [SHOT_TYPE] in [EUROPEAN_SETTING]. A [DOG1_BREED] wearing [OUTFIT1], a [DOG2_BREED] wearing [OUTFIT2], and a [DOG3_BREED] wearing [OUTFIT3] are [ACTION] with [TOY/PROPS]. [EXPRESSION_DESC]. [SETTING_DETAIL]. [LIGHTING_TAG]. Photorealistic, 8k resolution.
```

### Template 4 chó:
```
A [SHOT_TYPE] in [EUROPEAN_SETTING]. A [DOG1_BREED] wearing [OUTFIT1], a [DOG2_BREED] wearing [OUTFIT2], a [DOG3_BREED] wearing [OUTFIT3], and a [DOG4_BREED] wearing [OUTFIT4] are [ACTION]. [TOY/PROPS_DESC]. [EXPRESSION_DESC]. [SETTING_DETAIL]. [LIGHTING_TAG]. Photorealistic, 8k resolution.
```

---

## 10. QUY TẮC KHÔNG TRÙNG LẶP

Duy trì danh sách nội bộ trong toàn bộ cuộc trò chuyện:

- ✅ Ghi nhớ TẤT CẢ combo giống chó đã dùng
- ✅ Ghi nhớ TẤT CẢ bối cảnh cụ thể đã dùng
- ✅ Ghi nhớ TẤT CẢ hành động chính đã dùng trong cùng batch
- ✅ Mỗi batch mới phải khác biệt hoàn toàn so với prompt mẫu gốc (5 prompt mẫu) và mọi batch trước

---

## 11. VÍ DỤ OUTPUT CHUẨN

### Prompt 2 chó (Border Collie + Golden Retriever):
```
A vibrant, highly realistic action photograph on a sun-dappled wooden dock beside a glassy Alpine lake in a lush European summer forest. A joyful black-and-white Border Collie wearing a red sport harness and a cheerful golden Golden Retriever wearing a navy blue bandana collar are playing an intense game of tug-of-war with a thick colorful braided rope toy. Both dogs are leaning back with all their weight, paws planted firmly on the dock, mouths stretched in happy open grins. A rustic wooden rowboat is moored nearby, and wildflowers bloom along the mossy banks. Soft warm sunlight filtering through the pine canopy, balanced natural exposure, vivid true-to-life colors. Photorealistic, 8k resolution.
```

### Prompt 4 chó (Border Collie + 3 khác):
```
A breathtaking, dynamic action shot on a sun-lit cobblestone path beside a scenic Norwegian fjord meadow with a small stone bridge and summer wildflowers. A playful black-and-white Border Collie wearing a teal mesh cooling harness, an enthusiastic Shetland Sheepdog wearing an orange life jacket, a smiling Cocker Spaniel in a yellow striped t-shirt, and a happy Boston Terrier wearing a floral collar are all chasing a large colorful foam frisbee together through the air. Their expressions are wildly joyful, ears flying, eyes bright and alert. Bright warm summer daylight, soft natural shadows, no overexposure, vivid yet true-to-life color palette. Award-winning pet photography, photorealistic, 8k resolution.
```