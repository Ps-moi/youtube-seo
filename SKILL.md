---
name: seo-youtube
description: >
  Generate SEO-optimized YouTube titles (93–100 characters) and matching descriptions
  for dog sleep/relaxation music videos on the dog sleep channel. Use this skill whenever
  the user asks to create, generate, or write YouTube titles and descriptions for dog sleep
  music, dog calming music, or dog anxiety music videos. Also triggers when the user wants
  to build "bộ SEO" (SEO sets) for dog sleep/relaxation YouTube content, or requests
  non-duplicate title/description sets in the dog sleep channel style. Bắt buộc dùng skill
  này khi người dùng yêu cầu tạo bộ SEO cho kênh chó ngủ hoặc video nhạc thư giãn cho chó.
---

# Dog Sleep YouTube SEO Skill

Tạo bộ SEO hoàn chỉnh (title + description + hashtags) cho video nhạc thư giãn/ngủ dành cho
chó trên kênh dog sleep. Mỗi bộ phải **độc đáo, viết hay, cảm xúc**, và tuân thủ tuyệt đối
các quy tắc về ký tự, cấu trúc, và không trùng lặp.

---

## 🔑 VẾ 1 — Phần mở đầu bắt buộc (Segment 1 Phrase Pool)

Sau "12 Hours of", **bắt buộc** dùng đúng một trong các cụm từ sau, KHÔNG tự sáng tạo thêm:

```
Dog Music
Healing Sleep Music for Dogs
Dog Calming Music
Music for Dogs
Dog Anxiety Music
Dog Sleep Music
Soothing Music for Dogs
```

**Ví dụ Vế 1 hoàn chỉnh:**
- `12 Hours of Music for Dogs 🐶💤`
- `12 Hours of Dog Sleep Music 🐾🎵`
- `12 Hours of Soothing Music for Dogs 🎶✨`

---

## 🔑 VẾ 2 — Cụm từ SEO sáng tạo (Segment 2 Phrase Pool)

Vế 2 phải nhúng tự nhiên 1 KEY SEO từ danh sách dưới đây **nhưng KHÔNG được trùng cụm từ
đã dùng ở Vế 1**. Sáng tạo diễn giải xung quanh key SEO để tạo cụm từ hay, tự nhiên, đa dạng.

**KEY SEO chính:**
```
dog calming music
dog music
music for dogs
dog sleep music
relaxing dog music
sleepy dog music
dog anxiety music
dog music to calm them
dogs
calming music
puppy calming music
calm music for dogs
music for dogs to calm down
```

**Ví dụ Vế 2 sáng tạo:**
- `Sleep Music for Dogs with Anxiety 🎧`
- `Calming Music for Anxious Dogs 🐕`
- `Puppy Calming Music for Restless Nights 🌙`
- `Relaxing Dog Music to Ease Separation Anxiety 🎼`
- `Calm Music for Dogs During Thunderstorms 🌿`
- `Sleepy Dog Music for Peaceful Dreams 💤`
- `Dog Anxiety Music for Lonely Puppies 🎵`

⚠️ **Quy tắc quan trọng:** Nếu Vế 1 đã dùng "Music for Dogs" thì Vế 2 không được dùng lại
cụm "Music for Dogs". Hạn chế tối đa việc lặp lại cùng 1 cụm từ giữa các vế.

---

## 🔑 VẾ 3 — Câu kết cảm xúc tự do (Segment 3 Free Creative)

Vế 3 diễn giải lợi ích cảm xúc hoặc trạng thái kết quả. **Tự do sáng tạo, viết hay, có hồn,
không trùng lặp giữa các bộ.**

**Ví dụ Vế 3:**
- `Calm Puppies into Peaceful Sleep`
- `Peaceful Tunes for Healing Dog Sleep`
- `Relaxing Music for Stress Relief`
- `Help Your Dog Feel Safe and Loved`
- `Drift into Deep and Dreamy Rest`
- `Gentle Comfort for Tired Little Paws`
- `Soothe a Restless Heart into Stillness`
- `Wrap Your Pup in Warmth and Peace`

---

## 📐 QUY TẮC TITLE — Bắt buộc tuyệt đối

### ⚠️ Độ dài ký tự (CRITICAL)
- **Tối thiểu: 93 ký tự** — không được dưới
- **Tối đa: 100 ký tự** — không được vượt
- Đếm MỌI ký tự: chữ cái, dấu cách, dấu câu, icon (mỗi icon = 1 ký tự theo `len()` Python)
- **Bắt buộc đếm trước khi hoàn thiện. Chỉnh từng chữ cho đến khi đạt 93–100.**

### ⚠️ Cấu trúc 3 vế

```
[Vế 1: 12 Hours of + Phrase] [Icon] [Vế 2: SEO phrase] [Icon] [Vế 3: Creative close]
```

- Vế 1 luôn bắt đầu bằng `12 Hours of`
- Dùng **đúng 1 icon** giữa Vế 1 và Vế 2
- Dùng **đúng 1 icon** giữa Vế 2 và Vế 3
- **Không dùng** dấu `|` hay ký tự đặc biệt khác làm ngăn cách — chỉ dùng icon

### ⚠️ Icon — Đa dạng không trùng lặp
- Mỗi bộ phải dùng **cặp icon khác nhau** so với tất cả bộ trong cùng phiên
- Xoay vòng từ bộ icon liên quan: chó, âm nhạc, thú cưng, thiên nhiên, cảm xúc
- **Bộ icon gợi ý** (không lặp lại cùng 1 cặp):
  `🐶 🐾 🐕 🎵 🎶 🎼 🎹 🎧 💤 🌙 🌿 🍃 🌸 ✨ 💖 💙 💚 💛 🌊 🌼 🐩`

### ✅ Checklist Title
- [ ] Đúng 93–100 ký tự (đã đếm xong)
- [ ] Bắt đầu bằng `12 Hours of`
- [ ] Vế 1 dùng đúng phrase từ pool quy định
- [ ] Vế 2 nhúng ít nhất 1 KEY SEO, không trùng cụm Vế 1
- [ ] Vế 3 sáng tạo, có cảm xúc, không trùng vế khác
- [ ] 2 icon ngăn cách, cặp icon chưa dùng trong phiên này
- [ ] Không trùng bất kỳ title nào đã tạo

---

## 📝 QUY TẮC MÔ TẢ VIDEO

### Độ dài
- **Tối thiểu: 1.500 ký tự** — không được nhỏ hơn
- **Tối đa: 4.000 ký tự** — không được vượt quá
- Viết đủ dài, đủ sâu, đủ cảm xúc — không đếm từng ký tự một cách gượng ép

### Phong cách
- Viết hay, sáng tạo, tự nhiên, có cảm xúc
- Không trùng lặp ý với các bộ khác trong phiên
- Không ghi tên tác giả / composer
- Mỗi đoạn văn phải gắn trực tiếp với chủ đề của title

### Cấu trúc mô tả (theo thứ tự)

```
[Đoạn mở — 2-3 câu: Giới thiệu video, gắn với chủ đề cụ thể của title]

[Đoạn 2 — 3-4 câu: Mô tả âm thanh/nhạc. Cảm giác khi nghe. Cụ thể, giàu hình ảnh.]

[Đoạn 3 — 3-4 câu: Lợi ích cảm xúc và hành vi cho chó. Nối với tình huống cụ thể
của title (lo lắng / khó ngủ / cô đơn / bão tố...).]

[Đoạn 4 — 2-3 câu: Hình ảnh thơ mộng về chú chó đang thư giãn. Mềm, dịu, quan sát.]

💖 Benefits
• [Lợi ích 1 — gắn với chủ đề video]
• [Lợi ích 2]
• [Lợi ích 3]
• [Lợi ích 4]
• [Lợi ích 5 — tùy chọn]

🎧 How to Use
• [Mẹo 1]
• [Mẹo 2]
• [Mẹo 3]
• [Mẹo 4]
• [Mẹo 5]

🌼 Timeline
00:00 [Mô tả giai đoạn mở]
05:xx [Giai đoạn giữa]
10:xx [Giai đoạn sâu hơn]
15:xx [Giai đoạn cuối]
20:00 [Kết thúc nhẹ nhàng]

[Câu kết — 1-2 câu: Kêu gọi like/subscribe/share nhẹ nhàng, cảm xúc]

#hashtag1 #hashtag2 #hashtag3 [#hashtag4 — tùy chọn]
```

### ✅ Checklist Mô tả
- [ ] Độ dài 1.500–4.000 ký tự
- [ ] Đoạn mở gắn với chủ đề title
- [ ] Văn xuôi sáng tạo, không gượng ép
- [ ] Có đủ Benefits, How to Use, Timeline
- [ ] Timeline có ít nhất 4 mốc thời gian, unique mỗi bộ
- [ ] Không ghi tên tác giả
- [ ] Có lời kêu gọi cuối tự nhiên
- [ ] 3–4 hashtag ở cuối
- [ ] Không trùng nội dung với các bộ khác trong phiên

---

## #️⃣ QUY TẮC HASHTAG

- **Tối thiểu: 3 hashtag — Tối đa: 4 hashtag**
- Lấy từ KEY SEO pool, viết liền không dấu, chữ thường hoặc camelCase
  - `dog sleep music` → `#dogsleepmusic`
  - `relaxing dog music` → `#relaxingdogmusic`
  - `calming music for dogs` → `#calmingmusicfordogs`
- **Không hai bộ nào dùng cùng bộ 3 hashtag** trong một phiên
- Xoay vị trí hashtag mạnh (không luôn đặt cùng 1 tag đầu tiên)

**Ví dụ hashtag:**
```
#soothingmusicfordogs #doganxietymusic #dogsleepmusic
#dogcalmingmusic #relaxingdogmusic #musicfordogs
#dogsleepmusic #puppycalmingmusic #calmingmusicfordogs #dogmusic
```

---

## 🚫 QUY TẮC KHÔNG TRÙNG LẶP

Trước khi tạo, **xem lại tất cả các bộ đã tạo trong phiên** và đảm bảo:

| Thành phần | Quy tắc |
|---|---|
| Phrase Vế 1 | Không lặp lại cụm đã dùng ở bộ khác |
| Phrase Vế 2 | Không lặp lại anchor phrase đã dùng |
| Câu Vế 3 | Không lặp lại ý hoặc cụm từ |
| Cặp icon | Không dùng cùng 2 icon theo thứ tự |
| Câu mở mô tả | Không trùng cấu trúc hoặc ý |
| Bộ hashtag | Không trùng cả 3 hashtag |
| Mốc Timeline | Timestamps và mô tả khác nhau |

---

## ✅ ĐỊNH DẠNG ĐẦU RA

Với mỗi bộ SEO, xuất đúng theo format sau:

```
---
**Bộ [N]**

**TITLE** ([X] ký tự ✅):
[Toàn bộ title]

**MÔ TẢ:**
[Toàn bộ mô tả]
```

Sau tất cả các bộ, thêm bảng kiểm tra:

```
| Bộ | Ký tự Title | Ký tự Mô tả | Trạng thái |
|----|-------------|-------------|------------|
| 1  | XX          | XXXX        | ✅ / ❌    |
...
```

---

## 📋 VÍ DỤ THAM KHẢO (Bộ 0 — chỉ để tham khảo phong cách, không sao chép)

**TITLE** (97 ký tự ✅):
`12 Hours of Music for Dogs 🐶 Sleep Music for Dogs with Anxiety 🎧 Calm Puppies into Peaceful Sleep`

**MÔ TẢ** (tham khảo):
Create a peaceful and comforting bedtime atmosphere for your dog with this 12-hour soothing
relaxation music 🐶💤. Gentle piano melodies and calming ambient sounds flow softly together
to help reduce stress, quiet nervous energy, and encourage emotional comfort throughout the night.

This relaxing dog music is specially designed for puppies and dogs who experience anxiety,
restlessness, loneliness, or difficulty settling down before sleep. The slow emotional pacing
helps create a calm environment where your furry companion can feel safe, secure, and deeply relaxed.

💖 Benefits
• Helps reduce anxious behavior
• Encourages calm emotional balance
• Supports deeper sleep and relaxation
• Creates a peaceful nighttime atmosphere
• Helps dogs feel comforted and secure

🎧 How to Use
• Play during naps or bedtime
• Keep the volume soft and gentle
• Use in a quiet resting area
• Repeat daily for calming routines
• Pair with blankets or favorite toys

🌼 Timeline
00:00 Gentle dreamy piano begins
05:18 Soft emotional melodies flow
10:12 Relaxing nighttime atmosphere
15:04 Deep calming comfort builds
20:00 Peaceful sleep ending

If this relaxing music helps your dog sleep peacefully, feel free to like the video, subscribe
for more calming dog music, and share your dog's favorite relaxing moments in the comments 🐾💖

#soothingmusicfordogs #doganxietymusic #dogsleepmusic

---

## 🔄 QUY TRÌNH LÀM VIỆC CHO MỖI YÊU CẦU

1. **Xem lại lịch sử** — ghi nhớ tất cả title, cặp icon, bộ hashtag đã dùng trong phiên
2. **Với mỗi bộ mới:**
   a. Chọn phrase Vế 1 từ pool → Draft Vế 2 (không trùng) → Sáng tạo Vế 3
   b. Ghép title đầy đủ → **Đếm ký tự** → Chỉnh đến khi đạt 93–100
   c. Chọn cặp icon chưa dùng → Xác nhận không trùng title nào
   d. Viết mô tả gắn với chủ đề Vế 1 → Kiểm tra độ dài 1.500–4.000 ký tự
   e. Chọn 3–4 hashtag chưa dùng cùng nhau
3. **Xuất tất cả bộ** theo format chuẩn (Bộ 1, Bộ 2, ...)
4. **Xuất bảng kiểm tra** ở cuối

---

## ⚠️ CÁC LỖI THƯỜNG GẶP CẦN TRÁNH

| Lỗi | Cách xử lý đúng |
|---|---|
| Title 92 ký tự hoặc 101 ký tự | Đếm chính xác; thêm/bớt từng chữ một |
| Dùng `\|` làm ngăn cách | Chỉ dùng 1 icon giữa các vế |
| Lặp cặp icon ở bộ khác | Kiểm tra tất cả bộ trước; chọn cặp mới |
| Vế 1 và Vế 2 trùng cụm từ | Đọc lại cả 2 vế; thay đổi ngay |
| Mô tả dưới 1.500 ký tự | Mở rộng từng đoạn; thêm chi tiết cảm xúc |
| Mô tả không gắn với chủ đề title | Chiết xuất keyword Vế 1 → xây toàn bộ mô tả xung quanh nó |
| Bộ hashtag lặp lại | Ghi lại các combo đã dùng; chọn 3 key khác |
| Ghi tên tác giả trong mô tả | Không cần, bỏ hoàn toàn |
| Vế 3 nhạt, không cảm xúc | Viết lại: thêm hình ảnh, cảm giác, từ ngữ gợi tả |