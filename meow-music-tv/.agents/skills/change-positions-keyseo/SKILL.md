---
name: change-positions-keyseo
description: Shuffle, rotate, and generate permutations of a fixed list of YouTube tags/keywords for cat music and relaxation videos. Use this skill whenever the user wants to reorder, remix, or generate new arrangements of their cat/relaxation keyword set — including requests like "đảo vị trí từ khóa", "xáo trộn tags", "tạo bộ tags mới", "shuffle keywords", or "generate keyword variations". The output must preserve all keywords but vary their order across multiple sets so no two sets look identical. Always use this skill when the input contains the canonical cat-music keyword list or any subset of it.
---

# Cat Keyword Shuffle Skill

Tạo nhiều bộ sắp xếp (permutation) khác nhau từ danh sách từ khóa cố định, dùng cho YouTube tags của các video nhạc thư giãn cho mèo.

---

## Danh sách từ khóa gốc (canonical list)

```
music for cats, cat tv, piano music, cat relaxing music, cat music,
calming music for cats, stress relief, cat sleep music,
relaxing music for stress relief, relaxation, deep sleep,
relaxing music for cats, anxiety, cat calming music, squirrel,
bird feeder, parrot sounds, 잠잘때듣는음악, 고양이가좋아하는음악,
고양이 편안한 음악, 스트레스해소음악
```

Tổng: **21 từ khóa**

---

## Quy tắc xáo trộn

1. **Giữ nguyên tất cả 21 từ khóa** — không thêm, không bớt, không sửa chính tả.
2. **Mỗi bộ phải khác thứ tự** so với bộ trước — không lặp lại arrangement đã dùng.
3. **Phân nhóm logic khi xáo trộn** để tránh cảm giác hoàn toàn ngẫu nhiên:
   - Nhóm A (hành vi mèo): `cat tv`, `cat music`, `cat relaxing music`, `cat calming music`, `cat sleep music`, `relaxing music for cats`, `calming music for cats`
   - Nhóm B (trạng thái con người): `stress relief`, `relaxation`, `deep sleep`, `anxiety`, `relaxing music for stress relief`
   - Nhóm C (âm thanh/nhạc cụ): `piano music`, `music for cats`, `parrot sounds`, `bird feeder`, `squirrel`
   - Nhóm D (tiếng Hàn): `잠잘때듣는음악`, `고양이가좋아하는음악`, `고양이 편안한 음악`, `스트레스해소음악`
4. **Chiến lược xoay vòng nhóm**:
   - Bộ 1: A → B → C → D
   - Bộ 2: B → C → D → A
   - Bộ 3: C → D → A → B
   - Bộ 4: D → A → B → C
   - Bộ 5: Xáo trộn trong từng nhóm + xoay vòng
   - Bộ 6+: Kết hợp xen kẽ nhóm (A, C, B, D hoặc D, B, A, C...)
5. **Trong mỗi nhóm**, cũng thay đổi thứ tự nội bộ qua các bộ khác nhau.

---

## Định dạng đầu ra

Khi người dùng yêu cầu N bộ, xuất ra N bộ theo định dạng sau:

```
**Bộ 1:**
music for cats, cat tv, piano music, ...

**Bộ 2:**
calming music for cats, stress relief, relaxation, ...
```

- Mỗi bộ trên một dòng riêng, các từ khóa cách nhau bằng dấu phẩy + khoảng trắng.
- Đánh số bộ rõ ràng.
- Nếu người dùng không chỉ định số lượng, mặc định tạo **4 bộ**.

---

## Ví dụ — 4 bộ mẫu

**Bộ 1** (A → B → C → D):
```
cat tv, cat music, cat relaxing music, cat calming music, cat sleep music, relaxing music for cats, calming music for cats, stress relief, relaxation, deep sleep, anxiety, relaxing music for stress relief, piano music, music for cats, parrot sounds, bird feeder, squirrel, 잠잘때듣는음악, 고양이가좋아하는음악, 고양이 편안한 음악, 스트레스해소음악
```

**Bộ 2** (B → C → D → A):
```
stress relief, relaxation, deep sleep, anxiety, relaxing music for stress relief, piano music, music for cats, parrot sounds, bird feeder, squirrel, 잠잘때듣는음악, 고양이가좋아하는음악, 고양이 편안한 음악, 스트레스해소음악, cat tv, cat music, cat relaxing music, cat calming music, cat sleep music, relaxing music for cats, calming music for cats
```

**Bộ 3** (C → D → A → B):
```
piano music, music for cats, parrot sounds, bird feeder, squirrel, 잠잘때듣는음악, 고양이가좋아하는음악, 고양이 편안한 음악, 스트레스해소음악, cat tv, cat music, cat relaxing music, cat calming music, cat sleep music, relaxing music for cats, calming music for cats, stress relief, relaxation, deep sleep, anxiety, relaxing music for stress relief
```

**Bộ 4** (D → A → B → C):
```
잠잘때듣는음악, 고양이가좋아하는음악, 고양이 편안한 음악, 스트레스해소음악, cat tv, cat music, cat relaxing music, cat calming music, cat sleep music, relaxing music for cats, calming music for cats, stress relief, relaxation, deep sleep, anxiety, relaxing music for stress relief, piano music, music for cats, parrot sounds, bird feeder, squirrel
```

---

## Mở rộng (bộ thứ 5 trở đi)

Khi cần nhiều hơn 4 bộ, áp dụng thêm:
- Xáo trộn thứ tự **bên trong** từng nhóm (ví dụ: trong nhóm A, đổi `cat tv` lên cuối, `cat sleep music` lên đầu...).
- Xen kẽ nhóm theo pattern: A₁, C₁, B₁, D₁ hoặc D₁, B₂, A₂, C₂...
- Tách đôi nhóm lớn và xen giữa nhóm nhỏ.

Mục tiêu: **không bao giờ có 2 bộ giống nhau**, kể cả khi người dùng yêu cầu hàng chục bộ.