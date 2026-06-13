---
name: cattv-seo-youtube
description: >
  Generate SEO-optimized YouTube titles (92–100 characters) and matching descriptions for
  cat relaxation/music videos. Use this skill whenever the user asks to create, generate,
  or write YouTube titles and descriptions for cat music, cat TV, or cat relaxation videos.
  Also triggers when the user wants to build "bộ SEO" (SEO sets) for cat-themed YouTube content,
  or requests new non-duplicate title/description sets in the Meow Music TV style.
---

# Cat SEO YouTube Skill

Generate complete YouTube SEO sets (title + description + hashtags) for cat relaxation/music videos
in the **Meow Music TV** channel style. Each set must be unique, beautifully written, and follow the
strict structural and character-count rules below.

---

## 🔑 SEO Key Pool (use these as building blocks)

```
cat music, cat tv, music for cats, cat sleep music, cat relaxing music,
cat calming music, relaxing music for cats, healing cat music,
calming cat music, sleep music for cats, piano music, kitty music,
relaxing music
```

---

## 📐 TITLE RULES — Read carefully, all rules are mandatory

### Character Count (CRITICAL)
- **Minimum: 92 characters** — never go below
- **Maximum: 100 characters** — never exceed
- Count every character including spaces, icons, and punctuation
- Before outputting, count exactly and confirm the number

### Structure: 3 segments separated by icons (NOT `|`)
Use **2 icons between segments** instead of `|`. Example separators: `🐾🎵`, `💖🌿`, `🌸🎧`

```
[Segment 1] [2 icons] [Segment 2] [2 icons] [Segment 3]
```

### Segment 1 — FIXED (required, never change)
```
Cat TV for Cats to Watch
```
Followed by **1 or 2 icons** (e.g., `🐱🐾`, `🌿🐈`, `✨🐾`)

### Segment 2 — Choose one style per title:
**Style A:** `[1 SEO key from pool] + creative elaboration`
- Example: `Music for Cats with Gentle Melodies 🎧💖`
- Must naturally embed one SEO key

**Style B:** Creative phrase with strong embedded SEO key (must feel natural, not forced)
- Example: `Soft Piano Music to Calm Your Beloved Cat 🎵🌙`
- Must include a commonly searched keyword

### Segment 3 — Meaning/benefit statement
- Describes the purpose or emotional benefit of the video
- Examples: `Relax Cats & Support Cat Comfort`, `Deep Rest for Your Feline Friend`
- No icons needed (or 1 optional icon at end)

### Title Quality Checks
- [ ] Exactly 92–100 characters (count before finalizing)
- [ ] Contains at least 1 SEO key from the pool
- [ ] Segments separated by 2 icons (not `|`)
- [ ] Segment 1 is exactly `Cat TV for Cats to Watch`
- [ ] Reads naturally in English
- [ ] Does NOT duplicate any previously generated title in this conversation

---

## 📝 DESCRIPTION RULES

### Format template (follow this structure, expand each section):

```
Welcome to Meow Music TV 🌿🐾 — [1–2 sentences establishing the channel/video's purpose,
tied directly to the title's theme]

[Paragraph 2: Describe the music/sound characteristics — 3–4 sentences. Use sensory language.
Connect to the specific keyword/theme from Segment 2 of the title.]

[Paragraph 3: Describe the emotional benefit for the cat — 3–4 sentences. How does this
music support the cat's mood, comfort, sensitivity, or behavior?]

[Paragraph 4: Describe what the cat may experience over time as the music plays — 2–3 sentences.
Soft, poetic, observational language.]

🎵 Composed by Swallow Paur
[One sentence about the composition style, tied to the video theme]

📺 Enjoy uninterrupted calm with No Mid-Roll Ads ❌📢.

[Closing sentence — warm, gentle, poetic. Different each time.]

#hashtag1 #hashtag2 #hashtag3
```

### Description Quality Checks
- [ ] Opening line references the title theme directly
- [ ] Each paragraph is longer and richer than the sample
- [ ] Composer name `Swallow Paur` is unchanged
- [ ] No Mid-Roll Ads line is included verbatim
- [ ] Closing line is unique, warm, poetic
- [ ] Ends with exactly 3 hashtags

---

## #️⃣ HASHTAG RULES

- **Exactly 3 hashtags per set** — no more, no less
- Must be chosen from the SEO key pool
- Convert to hashtag format: remove spaces, camelCase or lowercase
  - `cat music` → `#catmusic`
  - `relaxing music for cats` → `#relaxingmusicforcats`
  - `calming cat music` → `#calmingcatmusic`
- **Rotate positions** — do not always put the same hashtag first
- **Do not repeat the same 3-hashtag combo** across sets in the same session

---

## 🚫 UNIQUENESS RULES

At the start of each generation request, mentally review all titles and descriptions already created
in this conversation. Then ensure:

- No segment 2 phrase is reused
- No segment 3 phrase is reused
- No opening description sentence is reused
- No closing description sentence is reused
- No hashtag combination is repeated

---

## ✅ OUTPUT FORMAT

For each SEO set, output exactly this structure:

```
---
**Bộ [N]**

**TITLE** ([X] ký tự):
[Full title here]

**MÔ TẢ:**
[Full description here]
```

---

## 📋 REFERENCE EXAMPLE (Bộ 0 — do not reproduce, use as style reference only)

**TITLE** (94 ký tự):
Cat TV for Cats to Watch 🐱🐾 Music for Cats with Gentle Melodies 🎧💖 Relax Cats & Support Cat Comfort

**MÔ TẢ:**
Welcome to Meow Music TV 🌿🐾 — a warm and comforting space where your cat can relax and feel emotionally safe. This video features soft piano music 🎧💖 that gently fills the environment with calm and reassurance.

The tones are light, smooth, and steady — designed to create a peaceful background that supports your cat's natural rhythm. The music does not interrupt or stimulate too much; instead, it quietly supports relaxation.

For cats who may feel uncertain or sensitive, this gentle atmosphere offers a sense of stability. It helps soften their reactions to small changes, allowing them to remain calm and comfortable.

As the music continues, your cat may settle more deeply into a relaxed state, moving with ease and observing with quiet curiosity.

🎵 Composed by Swallow Paur
Soft, comforting melodies crafted to support relaxation and emotional ease.

📺 Enjoy uninterrupted calm with No Mid-Roll Ads ❌📢.

May this peaceful sound bring your cat comfort, calmness, and a sense of gentle security. 🌸🐾

#calmingcatmusic #catcalm #musicforcats

---

## 🔄 WORKFLOW FOR EACH REQUEST

1. **Check conversation history** — note all titles and hashtag sets already generated
2. **For each new set:**
   a. Draft the title → count characters → adjust until 92–100 → confirm count
   b. Identify the SEO theme from Segment 2 → build description around that theme
   c. Choose 3 hashtags not used together before → rotate positions
3. **Output all sets** in the format above, labeled Bộ 1, Bộ 2, etc.
4. **After all sets:** list the character counts for verification

---

## ⚠️ COMMON MISTAKES TO AVOID

| Mistake | Correct approach |
|---|---|
| Title is 91 or 101 characters | Always count exactly; pad or trim carefully |
| Using `\|` as separator | Use 2 icons between segments |
| Segment 1 modified | Keep exactly: `Cat TV for Cats to Watch` |
| Changing composer name | Always: `Swallow Paur` |
| Reusing closing sentences | Write a fresh poetic closing each time |
| Only 2 hashtags or 4+ hashtags | Exactly 3, always |
| Description doesn't match title theme | Find the SEO keyword in title → build description around it |
