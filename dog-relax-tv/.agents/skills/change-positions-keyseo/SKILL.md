---
name: change-positions-keyseo
description: Shuffle, rotate, and generate permutations of a fixed list of YouTube tags/keywords for dog music and relaxation videos. Use this skill whenever the user wants to reorder, remix, or generate new arrangements of their dog/relaxation keyword set — including requests like "đảo vị trí từ khóa", "xáo trộn tags", "tạo bộ tags mới", "shuffle keywords", or "generate keyword variations". The output must preserve all 16 keywords but vary their order across multiple sets so no two sets look identical. Always use this skill when the input contains the canonical dog-music keyword list or any subset of it.
---

# Dog Keyword Shuffle Skill

Tạo nhiều bộ sắp xếp (permutation) khác nhau từ danh sách từ khóa cố định, dùng cho YouTube tags của các video nhạc thư giãn cho chó.

---

## Danh sách từ khóa gốc (canonical list)

```
dog tv for dogs to watch, music for dogs, dogs, dog music,
relaxing dog music, dog tv, calm music for dogs, calming music,
Relaxing music, dog anxiety music, dog calming music, dog sleep music,
puppy calming music, puppy music, soothing music for dogs, dog relax tv
```

Tổng: **16 từ khóa**

> ⚠️ Giữ nguyên viết hoa/thường như trên — đặc biệt `Relaxing music` viết hoa chữ R, `dogs` viết thường.

---

## Phân nhóm logic

| Nhóm | Tên | Từ khóa |
|------|-----|---------|
| **A** | TV & Channel | `dog tv for dogs to watch`, `dog tv`, `dog relax tv` |
| **B** | Dog Music (general) | `music for dogs`, `dogs`, `dog music`, `relaxing dog music` |
| **C** | Calming & Anxiety | `calm music for dogs`, `calming music`, `dog anxiety music`, `dog calming music` |
| **D** | Sleep & Soothe | `dog sleep music`, `soothing music for dogs`, `Relaxing music` |
| **E** | Puppy | `puppy calming music`, `puppy music` |

---

## Chiến lược xoay vòng nhóm

| Bộ | Thứ tự nhóm |
|----|-------------|
| 1  | A → B → C → D → E |
| 2  | B → C → D → E → A |
| 3  | C → D → E → A → B |
| 4  | D → E → A → B → C |
| 5  | E → A → B → C → D |
| 6  | A → C → E → B → D |
| 7  | B → D → A → E → C |
| 8  | C → E → B → D → A |

Từ bộ 9 trở đi: kết hợp xen kẽ + đảo thứ tự **bên trong** từng nhóm.

---

## Ví dụ — 5 bộ mẫu

**Bộ 1** (A → B → C → D → E):
```
dog tv for dogs to watch, dog tv, dog relax tv, music for dogs, dogs, dog music, relaxing dog music, calm music for dogs, calming music, dog anxiety music, dog calming music, dog sleep music, soothing music for dogs, Relaxing music, puppy calming music, puppy music
```

**Bộ 2** (B → C → D → E → A):
```
music for dogs, dogs, dog music, relaxing dog music, calm music for dogs, calming music, dog anxiety music, dog calming music, dog sleep music, soothing music for dogs, Relaxing music, puppy calming music, puppy music, dog tv for dogs to watch, dog tv, dog relax tv
```

**Bộ 3** (C → D → E → A → B):
```
calm music for dogs, calming music, dog anxiety music, dog calming music, dog sleep music, soothing music for dogs, Relaxing music, puppy calming music, puppy music, dog tv for dogs to watch, dog tv, dog relax tv, music for dogs, dogs, dog music, relaxing dog music
```

**Bộ 4** (D → E → A → B → C):
```
dog sleep music, soothing music for dogs, Relaxing music, puppy calming music, puppy music, dog tv for dogs to watch, dog tv, dog relax tv, music for dogs, dogs, dog music, relaxing dog music, calm music for dogs, calming music, dog anxiety music, dog calming music
```

**Bộ 5** (E → A → B → C → D):
```
puppy calming music, puppy music, dog tv for dogs to watch, dog tv, dog relax tv, music for dogs, dogs, dog music, relaxing dog music, calm music for dogs, calming music, dog anxiety music, dog calming music, dog sleep music, soothing music for dogs, Relaxing music
```

---

## Định dạng đầu ra

```
**Bộ 1:**
dog tv for dogs to watch, dog tv, dog relax tv, ...

**Bộ 2:**
music for dogs, dogs, dog music, ...
```

- Các từ khóa cách nhau bằng dấu phẩy + khoảng trắng.
- Đánh số bộ rõ ràng.
- Nếu người dùng không chỉ định số lượng, mặc định tạo **4 bộ**.
- Không bao giờ tạo 2 bộ có thứ tự giống nhau.

---

## Quy tắc bất biến

1. **Luôn giữ đủ 16 từ khóa** — không thêm, không bớt, không sửa nội dung.
2. **Giữ nguyên chính tả gốc**, đặc biệt `Relaxing music` (viết hoa R).
3. **Mỗi bộ phải khác** thứ tự so với mọi bộ đã tạo trong cùng phiên.
4. Khi xáo trộn bên trong nhóm (từ bộ 6+), **không tách rời** nhóm A — `dog tv for dogs to watch`, `dog tv`, `dog relax tv` nên ở gần nhau vì liên quan về nghĩa.