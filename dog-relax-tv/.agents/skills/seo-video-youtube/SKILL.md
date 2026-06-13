---
name: seo-video-youtube
description: >
  Generate SEO-optimized YouTube titles (92–100 characters) and matching descriptions for
  dog relaxation/music/TV videos. Use this skill whenever the user asks to create, generate,
  or write YouTube titles and descriptions for dog music, dog TV, or dog relaxation/anxiety videos.
  Also triggers when the user wants to build "bộ SEO" (SEO sets) for dog-themed YouTube content,
  or requests new non-duplicate title/description sets in the Dog Relax TV style.
  ALWAYS use this skill for any request involving dog YouTube SEO, even casual phrasing like
  "thêm bộ SEO", "viết title cho video chó", or "làm SEO cho kênh chó".
---

# Dog SEO YouTube Skill — Dog Relax TV

Generate complete, high-impact YouTube SEO sets (title + description + hashtags) for the
**Dog Relax TV** channel. Each set must be unique, deeply written, structurally correct,
and strictly within character-count rules.

---

## ⚠️ FIRST STEP: COUNT CHARACTERS BEFORE OUTPUT

**Every title must be verified with a character count before being shown.**
Use Python mentally or step-by-step:
- Letters, spaces, punctuation: 1 char each
- Emoji: 2 characters each (as rendered in most systems)
- **Wait — this skill uses len() convention: each emoji = 1 character**
- Target: **92–100 characters inclusive**
- If outside range: adjust word by word. Never skip this check.

---

## 🔑 SEO KEY POOL — Segment 1 Phrases (Vế 1)

Use ONE as the variable phrase after "12 Hours of":

```
dog tv for dogs to watch
dog tv
dog music
music for dogs
dog calming music
dog tv for dogs to watch relax
dog channel for dogs to watch
dog tv for dogs to watch barking
tv for dogs with calming music
healing music for dogs
dog anxiety music
dog sleep music [BANNED — contains sleep element]
```

> **RULE: Never use "dog sleep music" or any sleep-adjacent phrase in Segment 1.**

---

## 🔑 SEO KEY POOL — Segment 2 Phrases (Vế 2)

Use ONE as the anchor phrase in Segment 2, or a creative phrase embedding one key:

```
relaxing music for dogs to calm down
puppy separation anxiety music
calming music for dogs with anxiety
calming music for dogs during storms
instrumental music for dogs
calming music for dogs after surgery
sleeping music for dogs and puppies [avoid — sleep adjacent]
deep healing music for dogs
anxiety music for dogs home alone
soothing music for dogs
calm music for dogs
dog music to calm them down
```

Creative Segment 2 examples (embed key naturally):
- `Gentle Calming Music That Dogs Love`
- `Soothing Piano for Dog TV`
- `Dog Channel Heal & Calm`
- `Dog TV Relax with Gentle Piano`
- `Relaxing Dog TV Piano Melodies`

---

## 📐 TITLE RULES — MANDATORY

### Structure: 3 Segments
```
[Segment 1] [ICON_A] [Segment 2] [ICON_B] [Segment 3]
```

### Segment 1
- Always starts: `12 Hours of`
- Followed by one phrase from Segment 1 pool (exact or SEO-preserving variant)
- Ends with **1 unique icon** (ICON_A)

### Segment 2
- A phrase from Segment 2 pool OR a creative phrase embedding 1 strong SEO key
- Ends with **1 unique icon** (ICON_B)
- Style A (direct): `Calming Music for Anxious Dogs 🎵`
- Style B (creative): `Soothing Piano for Dog TV 🎶`

### Segment 3
- Benefit/meaning statement describing emotional outcome
- Must differ in meaning from Segments 1 and 2
- No duplicate phrasing across sets
- Optional: 1 icon (not required)
- Examples: `Ease Fear & Build Deep Trust`, `Inner Peace & Daily Comfort`, `Restore Calm & Harmony`

### ⚠️ Character Count
- **Minimum: 92** — never go below
- **Maximum: 100** — never exceed
- Count every character; emoji = 1 char (Python len() convention)
- Adjust word by word until in range

### ⚠️ No Sleep Elements — ABSOLUTE
Never use: sleep, sleeping, lullaby, bedtime, nap, drift off, slumber, rest for the night, doze

### ⚠️ Icons
- ICON_A and ICON_B must be **different from each other**
- The pair (ICON_A + ICON_B) must be **unique across all sets in this session**
- Do NOT use `|` as a separator
- Icon palette (rotate freely):
  `🐕 🐾 🌿 🎧 🎵 🎶 🎹 🎼 🌸 💛 🌊 💙 🍃 ✨ 🌼 💚 🐶 💜 🎀 🌻`

---

## 📝 DESCRIPTION RULES

### Format Structure

```
Welcome to Dog Relax TV 🐶💖 — [1–2 sentences tied directly to the title's Segment 1 theme]

[Paragraph 2: Music character — 3–4 sentences.
Sensory and emotional. What does the music sound like and how does it work?
Connect to the specific theme of Segment 1.]

[Paragraph 3: Emotional benefit for the dog — 3–4 sentences.
How does this address the named anxiety, stress, or situation?
Be specific, not generic.]

[Paragraph 4: Visual/poetic image — 2–3 sentences.
Paint a picture of the dog at ease. Soft, observational, warm.]

💞 Benefits for Your Dog
• [Benefit 1 — specific to this video's theme]
• [Benefit 2]
• [Benefit 3]
• [Benefit 4 — optional]

🎧 Listening Tips
• [Tip 1]
• [Tip 2]
• [Tip 3]

🌿 Music Flow
00:00 – [Opening phase]
[MM:SS] – [Mid phase — vary timestamps each set]
[MM:SS] – [Deeper phase]
[MM:SS] – [Closing phase]

🎼 This composition by Ethan Caldwell is crafted with [short style note tied to video theme].

PLEASE SUBSCRIBE to be the first to discover the newest products!

#hashtag1 #hashtag2 #hashtag3
```

### Description Quality Rules
- Opening sentence must reference the Segment 1 theme directly
- Each prose paragraph longer and richer than the reference example
- Benefits section tailored to this video's specific theme (not copy-paste)
- Music Flow timestamps **unique per set** — vary the times
- Composer name **always: `Ethan Caldwell`** — never change
- SUBSCRIBE line **verbatim** — never change
- Exactly **3 hashtags** at the end
- No sleep-adjacent language anywhere

---

## #️⃣ HASHTAG RULES

- **Exactly 3 hashtags** — never more, never fewer
- Source from main SEO key pool only:
  ```
  dog calming music → #dogcalmingmusic
  dog music → #dogmusic
  music for dogs → #musicfordogs
  dog anxiety music → #doganxietymusic
  relaxing dog music → #relaxingdogmusic
  calming music for dogs → #calmingmusicfordogs
  soothing music for dogs → #soothingmusicfordogs
  puppy music → #puppymusic
  calm music for dogs → #calmmusic
  tv for dogs → #tvfordogs
  dog tv → #dogtv
  dog tv for dogs to watch → #dogtvfordogstowatch
  puppy calming music → #puppycalmingmusic
  ```
- **Rotate positions** — strongest hashtag should not always be first
- **No two sets may share the same 3-hashtag combination**

---

## 🚫 UNIQUENESS RULES

Before generating, review all titles already created in this session. Then verify:

- No Segment 1 phrase is reused
- No Segment 2 phrase/anchor is reused
- No Segment 3 benefit phrase is reused
- No icon pair (ICON_A + ICON_B) combination is reused
- No opening description sentence is reused
- No hashtag trio (as a set of 3) is repeated
- Music Flow timestamps are unique per set

---

## ✅ OUTPUT FORMAT

For each SEO set:

```
---
**Bộ [N]**

**TITLE** ([X] ký tự ✅):
[Full title here]

**MÔ TẢ:**
[Full description here]
```

After all sets, include verification table:

```
| Bộ | Ký tự | Trạng thái | Icon A | Icon B | Hashtags |
|----|-------|------------|--------|--------|----------|
| 1  | XX    | ✅ / ❌    | ...    | ...    | ...      |
```

---

## 📋 REFERENCE EXAMPLE (Bộ 0 — style reference, do NOT reproduce)

**TITLE** (95 ký tự):
12 Hours of Dog Relax Music 🐕 Calm Piano Sounds for Dogs 🎧 Stress Relief & Anxiety Calm Support

**MÔ TẢ:**
Welcome to Dog Relax TV 🐶💖 — where relaxing piano music helps your dog feel calm, secure, and emotionally balanced 🎶
This calming music supports dogs experiencing stress or anxiety and creates a peaceful environment at home.
[... etc. — descriptions in production sets must be longer and richer than this reference ...]

#dogmusic #relaxingdogmusic #dogcalmingmusic

---

## 🔄 WORKFLOW PER REQUEST

1. **Review session history** — note all phrases, icon pairs, hashtag combos used
2. **For each new set:**
   a. Select unique Segment 1 phrase → draft full title → **count characters** → adjust to 92–100
   b. Verify: no sleep words, unique icon pair, unique Segment 2 anchor
   c. Build description fully tied to Segment 1 theme — every paragraph references it
   d. Choose 3 hashtags not used together before → vary their order
3. **Output all sets** labeled Bộ 1, Bộ 2, etc.
4. **Output verification table** at end

---

## ⚠️ COMMON MISTAKES TO AVOID

| Mistake | Fix |
|---|---|
| Title under 92 or over 100 chars | Count exactly; add/remove words one at a time |
| Using `\|` as segment separator | Use 1 emoji icon only |
| Same icon pair as another set | Check full session history; pick a fresh pair |
| Sleep words in title or description | Replace with: calm, ease, relax, comfort, settle, restore |
| Description doesn't match title theme | Extract Segment 1 keyword → build all paragraphs around it |
| Repeating the same hashtag trio | Write down used combos; pick 3 different keys |
| Changing composer name | Always: `Ethan Caldwell` |
| Skipping SUBSCRIBE line | Include verbatim every time |
| Generic benefits list | Tailor each bullet to the specific theme of this set |
