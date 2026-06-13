---
name: seo-video-qtsx-final
description: >
  Generate SEO-optimized YouTube titles and descriptions for Behind-the-Scenes (BTS) / "How We
  Make Videos" content for pet channels (dogs, cats, birds, and other animals). Use this skill
  whenever the user asks to write a YouTube title and description in the format:
  "How / Behind / A Day + Channel name + Video production process."
  Also triggers when the user requests content for formats like "How We Create", "Behind the
  Studio", "A Day Making Videos", "Quy trình làm video", "Hậu trường", or any BTS-style
  content for relaxation/music/TV pet channels. Always use this skill for pet channel BTS
  content — even if the request seems simple or short.
---

# BTS YouTube Skill — Behind-the-Scenes Pet Channel

Generate complete YouTube SEO sets (title + description + hashtags) for **Behind-the-Scenes**
videos of pet relaxation/music/TV channels.

Each set must be original, emotionally resonant, well-structured, and follow all rules below.

---

## 🎯 FORMAT OVERVIEW

Three interchangeable BTS frame styles — pick the one best suited to the request:

| Frame | Core Meaning | Tone |
|---|---|---|
| **How We** | What we do every day — full workflow | Professional, proud, process-driven |
| **Behind** | Inside look — the studio, the team, the craft | Warm, intimate, inviting |
| **A Day** | One day from raw footage → final video | Personal, real, journey-like |

The user may specify one, or Claude should choose the most fitting frame based on context.

---

## 🔑 CHANNEL NAME POOL (Pet Niches)

Use the exact channel name given by the user, OR adapt from these niche styles:

```
Dog channels:   Dog Relax TV · Pet Joy Moments · Paws & Calm · Puppy Dream Studio
Cat channels:   Meow Music TV · Cozy Cat Studio · PurrFect Vibes · Feline Calm TV
Bird channels:  Birdsong Bliss · Feather & Melody · Avian Calm TV
Multi-pet:      Pet Harmony TV · Furry Friends Studio · Animal Peace Channel
```

---

## 📐 TITLE RULES — All mandatory

### ⚠️ Character Count (CRITICAL)
- **Minimum: 90 characters** — never go below
- **Maximum: 100 characters** — never exceed
- Count every character: letters, spaces, punctuation, emoji (each emoji = 1 character)
- **Always count before finalizing. Adjust word by word until in range.**

### Title Structure — 3 Parts

```
[Part 1: BTS Frame Phrase] [1 icon] [Part 2: Channel Identity] [1 icon] [Part 3: Value Hook]
```

**Part 1 — BTS Frame Phrase** (pick one style per title):
```
How We Create Daily Videos
My Working Day as a Pet Video Creator
Behind Our [Animal] Music Studio
A Day in Our [Animal] TV Channel
How We Make Relaxing [Animal] Videos
Behind the Scenes of [Channel Name]
A Full Day From Raw Clips → Final Video
How Our Team Crafts [Animal] Content
```

**Part 2 — Channel Identity** (ties to the channel name and animal):
```
Welcome to [Channel Name]
Inside [Channel Name]
The Story Behind [Channel Name]
Our [Channel Name] Journey
```

**Part 3 — Value Hook** (what the viewer gains from watching):
```
Learn, Practice, Flourish 🐶
The Full Process Revealed ✨
From Idea to Final Cut 🎬
Raw → Relaxing → Real 🌿
Every Frame Made With Love 💖
Our Creative Process Unveiled 🎶
```

### ⚠️ Icon Rules
- Use **1 icon** between Part 1 and Part 2
- Use **1 icon** between Part 2 and Part 3 (or fold into Part 3)
- Do NOT use `|` as a separator — icons only
- Each set must use a **different icon combination**
- Icon palette: `🐾 🐕 🐶 🐱 🐦 🎬 🎥 🎶 🎵 🎧 🌿 ✨ 💖 🌸 💛 🌊 🍃 💙 🎼 🌼`

### ⚠️ No Generic Content
- Avoid hollow phrases: "amazing", "incredible", "the best ever"
- Every title must tie to the **actual animal** and **actual process** theme

### Title Quality Checklist
- [ ] Exactly 90–100 characters (count before output)
- [ ] Contains the BTS frame (How / Behind / A Day)
- [ ] Contains the channel name or animal niche reference
- [ ] Icon pair is unique vs all other sets in this session
- [ ] Does NOT duplicate any previously generated title in session

---

## 📝 DESCRIPTION RULES

### Overall Format

```
[Opening line — 1 sentence tying to title theme, include channel name + animal emoji]

[Paragraph 1 — Studio/team/process intro: 2–3 sentences.
What does the workspace or workflow look like? What is the first thing the team does each day?]

[Paragraph 2 — The craft and care: 3–4 sentences.
How do you choose sounds, visuals, or themes? What makes the content intentional and loving?]

[Paragraph 3 — Why it matters for the animal: 2–3 sentences.
How does the creation process connect to the emotional wellbeing of the pets watching?]

[Paragraph 4 — Invite the viewer in: 2 sentences.
Soft call to action — invite them to look around, follow along, feel at home.]

💖 [CTA Line — Like, Follow, Share — unique wording each set]

#hashtag1 #hashtag2 #hashtag3
```

### Description Rules in Detail

**Opening line:**
- Must name the channel or show type
- Must include 1 animal emoji fitting the niche (🐶 🐱 🐾 🐦)
- Must signal "BTS" or "inside look" clearly
- Example: `Step into the peaceful world behind our Meow Music TV channel 🐾.`

**Paragraph 1 — Studio & Workflow Intro:**
- Set the scene physically or emotionally — where the work happens
- Introduce "the team" or "we" — even if just one creator, the warmth of a collective
- 2–3 sentences, sensory and grounded
- Example: *We begin each day surrounded by soft sounds, gentle visuals, and a clear purpose: to create something that truly comforts the animals in your home.*

**Paragraph 2 — The Craft:**
- Explain the creative decisions: sound selection, visual mood, pacing choices
- Use language that reflects care and intentionality
- Mention specific elements: melodies, nature scenes, color tones, editing rhythm
- 3–4 sentences

**Paragraph 3 — Animal Connection:**
- Shift from "us" to "them" — what does this mean for the pet?
- Emotional bridge: the creator's effort → the animal's peace
- 2–3 sentences, warm and sincere

**Paragraph 4 — Viewer Invite:**
- Short, inviting, personal
- Make the viewer feel like a guest, not an audience member
- 2 sentences

**CTA Line:**
- Must include: Like, Follow, Share
- Must also include a warm emotional reason to do so
- Wording must be **unique across all sets in the session**
- Include 2 relevant emojis

### Description Quality Checklist
- [ ] Opening line names channel + animal emoji
- [ ] Each paragraph follows its theme (scene → craft → animal → invite)
- [ ] No paragraph is shorter than 2 sentences
- [ ] No sleep-related language (sleep, slumber, bedtime, nap, drift off)
- [ ] CTA line is unique vs other sets in session
- [ ] Exactly 3 hashtags at the end
- [ ] Tone is warm, personal, professional — never generic

---

## #️⃣ HASHTAG RULES

- **Exactly 3 hashtags** — never more, never fewer
- Always mix: 1 BTS/process tag + 1 channel-identity tag + 1 animal/content tag
- Format: lowercase, no spaces
  - `behind the scenes` → `#behindthescenes`
  - `how we make videos` → `#howwemakevideos`
  - `cat music` → `#catmusic`

**BTS Tag Pool (choose 1 per set):**
```
#behindthescenes  #howwemakevideos  #youtubeprocess
#contentcreator   #videoproduction  #makingvideos
#studiotour       #adayinmylife     #creatorlife
```

**Channel / Niche Tag Pool (choose 1 per set):**
```
#petcontent  #petyoutube  #animalchannel
#dogchannel  #catchannel  #petchannel
#relaxingpetvideos  #petmusictv
```

**Animal / Content Tag Pool (choose 1 per set):**
```
#dogmusic  #catmusic  #musicfordogs  #musicforcats
#relaxingmusic  #calmingmusic  #petrelax
#dogtv  #cattv  #pettv
```

- **No two sets may share the same 3-hashtag combination**
- Rotate tag positions — strongest tag is not always first

---

## 🚫 UNIQUENESS RULES

Before generating each new set, mentally review all sets already created in this session:

- No Part 1 frame phrase is reused verbatim
- No Part 2 channel identity phrasing is reused
- No Part 3 value hook is reused
- No icon pair combination is reused
- No opening description sentence begins the same way
- No CTA line uses identical wording
- No 3-hashtag combination is repeated

---

## ✅ OUTPUT FORMAT

For each set, output exactly:

```
---
**Bộ [N]** — Frame: [How We / Behind / A Day]

**TITLE** ([X] ký tự ✅):
[Full title here]

**MÔ TẢ:**
[Full description here]
```

After all sets, include a verification table:

```
| Bộ | Frame | Ký tự | Trạng thái |
|----|-------|-------|------------|
| 1  | Behind| XX    | ✅ / ❌   |
...
```

---

## 📋 REFERENCE EXAMPLES (Style reference only — do not reproduce)

### Example A — "How We" Frame (Dog Channel)

**TITLE** (96 ký tự):
`My Working Day: Learn, Practice, Flourish 🐶 | Welcome to Pet Joy Moments, How We Create Daily`

**MÔ TẢ:**
Welcome to the daily world of Pet Joy Moments 🐾 — where every video begins with a single intention: to bring peace to the dogs we love.

Our mornings start with listening. Before we touch a single clip or note, we ask ourselves what kind of calm a dog truly needs today — and we build from that feeling outward. The studio fills with soft sounds, warm light, and the quiet hum of purpose.

Every melody, every visual, every gentle transition is chosen with your dog in mind. We spend hours refining the sonic textures — removing anything harsh, layering in the warmth that makes a dog's body relax and their breath slow. It's not just editing. It's care in audio form.

Because when we get it right, we see it: dogs who settle faster, breathe deeper, feel safer. That's what makes every hour of work worth it.

Come walk through our day. There's a lot of love in here — and it's all for the animals.

💖 If this behind-the-scenes journey touched you, please Like, Follow, and Share with fellow dog lovers. Your support keeps us creating every single day 🐕✨

#behindthescenes #petcontent #dogmusic

---

### Example B — "Behind" Frame (Cat Channel)

**TITLE** (97 ký tự):
`🐱 A Cozy Look Inside Our Cat TV Studio | How Meow Music TV Creates Relaxing Videos Every Day 🎶✨`

**MÔ TẢ:**
Step into the peaceful world behind our Meow Music TV channel 🐾 — where every video is crafted to help cats feel safe, curious, and deeply at ease.

From the moment we sit down at our workstation, the process begins with intention. We start each session by selecting the right foundation melody — something that mirrors a cat's natural resting rhythm, never too sharp, never too fast. The studio becomes quiet so we can truly hear what we're building.

We spend hours creating gentle environments filled with soothing sounds, soft visuals, and calming atmospheres. Whether it's birdsong layered beneath piano, or the slow drift of nature scenes chosen to hold a cat's gaze, every element earns its place through purpose — not accident.

And when a cat curls up, closes their eyes, or simply watches without tension? That's the moment we know the work is complete. Everything we do leads to that one still moment for your cat.

We'd love for you to follow this journey with us. There's always something new being made, and it's always made with love.

💖 If you enjoyed this relaxing behind-the-scenes journey, don't forget to Like, Follow, and Share with fellow cat lovers. Your support inspires us to keep creating every week 🌙✨

#behindthescenes #catchannel #catmusic

---

## 🔄 WORKFLOW FOR EACH REQUEST

1. **Identify the request:**
   - What animal/channel niche? (dog, cat, bird, multi-pet)
   - What channel name? (given by user or choose from pool)
   - What BTS frame? (How We / Behind / A Day — user-specified or choose best fit)
   - How many sets?

2. **For each new set:**
   - a. Draft Part 1 (frame phrase) → Part 2 (channel identity) → Part 3 (value hook)
   - b. Assemble full title → **count characters** → adjust until 90–100
   - c. Confirm unique icon pair and no reused segment phrases
   - d. Write description following the 4-paragraph structure
   - e. Choose 3 hashtags (BTS + channel + animal) — not used together before

3. **Output all sets** labeled Bộ 1, Bộ 2, etc. with frame label

4. **Output verification table** at the end

---

## ⚠️ COMMON MISTAKES TO AVOID

| Mistake | Correct approach |
|---|---|
| Title is 89 or 101 chars | Count exactly; add/remove one word at a time |
| Using `\|` as separator | Use 1 icon between segments only |
| Reusing the same icon pair | Check all previous sets; pick a fresh pair |
| All sets use "How We" frame | Rotate frames: How We → Behind → A Day across sets |
| Description reads like a product listing | Use sensory, emotional, first-person language — warmth over polish |
| CTA is identical across sets | Vary wording, emoji, and emphasis each time |
| Hashtags are all BTS tags | Always mix 1 BTS + 1 channel + 1 animal tag |
| Changing core structure | Always keep: opening → craft → animal → invite → CTA → hashtags |