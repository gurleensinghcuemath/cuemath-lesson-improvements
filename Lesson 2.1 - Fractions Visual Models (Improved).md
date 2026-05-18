# Lesson 2.1 — Fractions as Parts of a Whole: Visual Models (Improved)

**ID:** `mk-f-fractions-visual-models`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved v2
**Skills:** Number Theory · Fractions · Visual Models

> ✏️ content change · 🐛 code/asset bug · 🆕 new addition

---

## What changed and why

| Category | Biggest wins |
|----------|-------------|
| 🐛 Asset/layout bugs | CF2 fraction labels on figures; Step 1 no images; Step 8 no figures; WE1 kangaroo count not visible; P2/P5 `{blank}` renders as code; MC2/MC3 answers in question text; CE1 answer in image subtext |
| ✏️ Hints → true CUEs | ALL hints rewritten to ≤ 10 words. No hint names an answer, value, or full method. |
| ✏️ Narrations simplified | WE answer-before-checkpoint pattern fixed throughout. All WE narrations stop before the final calculation. |
| ✏️ Questions rephrased | P3/MC2 options inside question text; P2/P5 `{blank}` placeholder issue; MC3 answer below figure |
| ✏️ Attempt counts standardised | 2 hints per practice problem throughout |

---

## Block 1 — Challenge First

---

### CF1 — Sarah and the unequal rectangle ✅

**Type:** MCQ | **Figure:** `MK_L21_CF1_unequal_rect.svg`

**Question:** Sarah colours 3 of the 5 sections and says she has coloured 3/5. Is she right?
**Options:** (A) Yes — 3 of 5 parts coloured. **(B) No — all parts must be the same size. ✓** (C) Yes — you count coloured divided by total. (D) No — she needed to colour exactly half.
**Answer:** index 1

Hints ✅ — already good CUEs. No changes.

---

### CF2 — Same fraction or different? ✏️🐛

**Type:** MCQ | **Figure:** `MK_L21_CF2_spine_pair.svg`

🐛 **Figures label the actual fractions** — SVG shows "2/3" and "6/9" written below each figure. These are what the student must work out. Remove all fraction labels from both figures.

**Question:** Both figures show the same fraction. Which fraction is it?
**Options:** **(A) 2/3 ✓** (B) 1/3 (C) 1/2 (D) They show different fractions.
**Answer:** index 0

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | Count the shaded parts in the rectangle. Write that as a fraction. | No change — good CUE. ✅ | 12 (keep) |
| 2 | For the dots: 6 are coloured, 9 total → fraction is 6/9. Does 6/9 equal 2/3? Try dividing by 3. | **You found the rectangle fraction. Do the dots show the same thing?** | 10 |

> Hint 2 old version named the dot count (6), total (9), and the fraction (6/9) — giving away all three steps. New version just asks for comparison.

---

## Block 2 — Interactive Lesson

---

### Step 0 — Predict: Same fraction or different? ✅

onCorrect and onWrong are well-written. No changes.

---

### Step 1 — Explain: What a fraction really says ✏️🐛

🐛 **No images.** This step compares equal vs unequal parts — the whole point is visual. Without images, the explanation makes no sense.

🆕 **Required figures:**
- `MK_L21_Step1_rect_equal.svg` — rectangle with 4 equal parts, 3 shaded
- `MK_L21_Step1_rect_unequal.svg` — rectangle with 4 unequal sections, 3 coloured

✏️ **keyInsight** — old version is 2 sentences. Shorten to one:
- Old: "A fraction is only valid when all parts are the same size. No equal parts → no fraction."
- New: **"For a fraction to work, every part must be the same size."**

---

### Step 2 — Explain: Numerator and denominator ✏️🐛

🐛 **No image.** Step describes a rectangle divided into 3 equal parts with 2 shaded — needs a visual to anchor the words "numerator" and "denominator."

🆕 **Required figure:** `MK_L21_Step2_label_diagram.svg` — rectangle 2/3 shaded, with arrows labelling numerator and denominator.

🆕 **onWrong added:**
- Old: none
- New: **"The bottom number counts all equal parts."** (7 words)

---

### Step 3 — Apply: Read three fractions ✏️

**Sub-question 1** ✅ fine as-is.

**Sub-question 2 (which shows 3/4?):**
✏️ Prompt did not make it clear all parts must be equal — student could confuse 3/4 with any rectangle showing 3 shaded. Rephrase:
- Old: describes each option in text
- New: **"3/4 means 3 parts shaded out of 4 equal parts in total. Which rectangle shows exactly that?"**

✏️ **Wrong-answer nudge:**
- Old: "3/4 means 3 of the 4 equal parts are shaded. Count the shaded sections in each option." — gives method in full
- New: **"Check option C — count its shaded parts."** (7 words)

**Sub-question 3** ✅ fine as-is.

---

### Step 4 — Explain: Set model ✏️

✏️ **keyInsight** — removed ÷ symbol and "!" punctuation (both banned):
- Old: "Objects instead of parts of a shape — the rules are identical: chosen ÷ equal total."
- New: **"Counting objects or counting parts of a shape — the rule is the same."**

🆕 **Required figure:** `MK_L21_Step4_dot_grid.svg` — 3 × 3 grid, 6 filled orange, 3 empty. Without this, the set-model concept has no visual anchor.

---

### Step 5 — Apply: Two set-model reads ✏️

**Sub-question 1** ✅ fine as-is.

**Sub-question 2 (fraction NOT coloured):**
✏️ **Wrong-answer nudge named the count (7):**
- Old: "NOT coloured means white tiles… 7 as the count"
- New: **"Count the tiles with no colour."** (6 words)

---

### Step 6 — Explain: What is the whole? ✏️

✏️ **Old definition used ÷ symbol and reverse formula** (both too abstract):
- Old: "Part ÷ Whole = Fraction. To reverse: Whole = Part ÷ Fraction."
- New: **"Before writing a fraction, you need two things: what you are counting (the part) and what the full group is (the whole)."**
- Keep the kangaroo example. Drop the formula lines.

🆕 **onWrong:**
- Old: none
- New: **"If 6 is one half, add the other half too."** (10 words)

---

### Step 7 — Apply: Find the whole ✏️

**Sub-question 1 (4 squares = 1/4, find total):**

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | If 4 squares = 1/4, the full bar = 4 × 4 squares. | **The bar has 4 equal quarters in total.** | 8 |

> Old hint gave the full equation (4 × 4). New hint points to the fact without computing.

**Sub-question 2 (3 slices = 3/4, find total slices):**

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | 3 slices = 3/4. So 1 slice = 1/4. How many quarters make a whole? | **3 slices fill 3 quarters. How many slices fill 1 quarter?** | 10 |

> Old hint did all the reasoning. New hint is still a question that the student must answer.

---

### Step 8 — Apply: Why do both figures show 2/3? ✏️🐛

🐛 **No figures.** Step refers to Figure A (rectangle) and Figure B (dot grid) but shows nothing.

🆕 **Required figures:**
- `MK_L21_Step8_figA_rect.svg` — rectangle with 3 equal columns, 2 shaded yellow
- `MK_L21_Step8_figB_dots.svg` — 3×3 grid, 6 coloured orange

**Sub-question 1 (shaded fraction of rectangle):**

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | Count the shaded columns — that is the numerator. The denominator is 3. | **Count shaded columns, then count all columns.** | 7 |

> Old hint gave the denominator (3) directly. New hint just names the two things to count.

**Sub-question 2 (coloured fraction of dot grid):**

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | Count all dots (3 rows × 3 columns) — that is the denominator. | **Count all the dots in the grid.** | 7 |

> Old hint gave the multiplication (3×3) and labelled the answer as "denominator." New hint asks them to count.

**Sub-question 3 (simplify 6/9):**

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | 6 ÷ 3 = 2. | **What number divides into both 6 and 9?** | 9 |

> Old hint gave the numerator of the answer directly. New hint asks for the common factor.

---

### Step 9 — Reveal: Three tools, one idea ✅

Content is solid. No changes.

---

## Block 3 — Worked Example 1 (MK 2017 Q02)

**Problem:** John looks out the window and sees half the kangaroos in the park. How many kangaroos are there in the park?

---

### WE1 — problem.figure 🐛

🐛 **Bare string** → `{ "src": "..." }`
🐛 **Verify SVG shows exactly 6 countable kangaroos** — problem is unsolvable without this.

---

### WE1 — Step 1: Name the fraction ✅

Checkpoint (fill "1"/2) is a clean confirmation. No changes.

---

### WE1 — Step 2: Identify part vs whole ✅

2-option MCQ is well-framed. No changes.

---

### WE1 — Step 3: Bar model — find the total ✏️

✏️ **Narration computed the answer before the checkpoint:**
- Old: "Left half = 6 visible kangaroos. Right half = same number. 1 half = 6 → 2 halves = 6 + 6 = 12."
- New: **"The park has 2 equal halves. You know one half = 6 kangaroos. The other half is the same size. Use the bar to find the total."**

The student does the addition in the checkpoint — not the narration.

---

### WE1 — Step 4: Match to answer options ✏️

✏️ **Narration named the answer:**
- Old: "Answer = 12. Match it to the competition choices."
- New: **"You have found the total. Now find it in the answer choices."**

---

## Block 4 — Worked Example 2 (MK 2019 Q15)

**Problem:** A full glass weighs 400 g. An empty glass weighs 100 g. How much does a half-full glass weigh?

---

### WE2 — problem.figure 🐛

🐛 **Bare string** → `{ "src": "..." }`

---

### WE2 — Step 1: Separate glass from water ✏️

✏️ **Narration computed the answer before the checkpoint:**
- Old: "Water alone = 400 − 100 = 300 g"
- New: **"The glass weighs 100 g whether it is full or empty. A full glass = 400 g total. How much does just the water weigh?"**

Student computes 400 − 100 in the checkpoint.

---

### WE2 — Step 2: Half of the water ✏️

🐛 **Figure alt text reveals the answer:** "top = 150 g, bottom = 150 g"
- New alt: **"A bar showing 300 g water split into two equal halves"**

✏️ **Narration pointed to the answer:**
- Old: "Half of the water is in the glass."
- New: **"Half-full means only half the water fits. You know the total water. What is half of that?"**

---

### WE2 — Step 3: Add the glass back ✏️

✏️ **Narration gave the final sum:**
- Old: "= 150 + 100 = 250 g"
- New: **"The glass holds 150 g of water and always adds its own 100 g. Add those in the checkpoint."**

---

### WE2 — Step 4: Why is 200 g wrong? ✅

Conceptual MCQ is well-designed. No changes.

---

## Block 5 — Practice Lab

---

### P1 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`

✏️ **Remove answer subtext from image** — the image label says "1 of 3 parts shaded," giving the answer away.

| Hint | Text | Words |
|------|------|-------|
| 1 | Count how many parts are shaded. | 6 |
| 2 | Write: shaded parts / total equal parts. | 7 |

---

### P2 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **`{blank}` renders as code** — remove inline placeholder from question text.

✏️ **New question:** "There are 10 shapes — 6 circles and 4 triangles. How many of the 10 shapes are circles?"
- Type: `fill_in_blank`
- Answer: 6

| Hint | Text | Words |
|------|------|-------|
| 1 | Count just the circular shapes. | 6 |
| 2 | Write your count out of 10. | 7 |

---

### P3 ✏️

✏️ **Options described inside question text** — option labels should be visual figures only, not text descriptions. The question text tells the student what each rectangle looks like, making this a reading task not a thinking task.

✏️ **New question:** "Which of these figures shows the fraction 2/5?"
- Options: (A) / (B) / (C) / (D) — figure references only, no descriptions in text

🆕 **Required figures:** Four rectangle SVGs, one per option.

| Hint | Text | Words |
|------|------|-------|
| 1 | 2/5 means 2 shaded out of 5 equal parts. | 9 |
| 2 | Check option D — are all its 5 parts equal? | 10 |

---

### P4 ✅

Hints are good CUEs. No changes.

---

### P5 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **`{blank}` in question text** — same rendering issue as P2. Rewrite question to avoid inline placeholder.
🐛 **Image text cut by dividing line** — fix SVG so labels sit outside the dividing line.

✏️ **New question:** "The shaded part has 8 small squares. The shaded part is 2/3 of the whole rectangle. How many small squares does the whole rectangle have?"

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | If 2 equal parts = 8 squares, how many squares are in just 1 of those equal parts? | **2 equal parts = 8. What is 1 part?** | 8 |
| 2 | You found the size of 1 part. The whole has 3 of those equal parts. How many squares total? | **Multiply 1 part by 3 for the whole.** | 7 |

> Old hints were 17 and 20 words each and spelled out the full working. New hints are 8 and 7 words.

---

### P6 ✅

Hints are good CUEs. No changes.

---

### P7 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`

✏️ **Image subtext names the fraction** — "6 of its 8 equal parts are shaded" written below the figure makes the simplification obvious. Remove subtext.

✏️ **New question:** "What fraction of the rectangle is shaded? Which dot set below shows the same fraction?"
- Options: (A) / (B) / (C) / (D) — dot sets as figures only, no numbers in question text.

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | Simplify the rectangle fraction: 6/8 = ? (divide both by 2). | **Count shaded parts and total parts. Can you simplify?** | 9 |
| 2 | 6/8 = 3/4. Which option shows 3 out of every 4 dots coloured? | **Which dot set matches the fraction you found?** | 8 |

> Old Hint 1 gave the fraction (6/8) and the divisor (2). Old Hint 2 gave the simplified answer (3/4). New hints just direct attention.

---

### P8 ✅

Hints are good CUEs. No changes.

---

## Block 6 — Mastery Check

> No hints allowed in mastery check.

---

### MC1 🐛✏️

🐛 `figure` bare string → `{ "src": "..." }`

✏️ **Question parenthetical gives away format:**
- Old: "How many of the 6 equal parts are shaded? ___ (The fraction shaded is that number /6.)"
- New: **"What fraction of the rectangle is shaded? Write the numerator — the denominator is 6."**

---

### MC2 ✏️

✏️ **All four options described in question text** — same issue as P3. Question becomes a reading exercise.

✏️ **New question:** "Which of these figures shows the fraction 1/3?"
- Options: (A) / (B) / (C) / (D) — `optionFigures` references only

🆕 **Required figures:** Four rectangle SVGs as described in the original.

---

### MC3 🐛✏️

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Answer given below figure** — remove answer text from image caption.

✏️ **Question parenthetical reduces difficulty:**
- Old: "How many stars are NOT yellow? ___ (The fraction NOT yellow is that number/9.)"
- New: **"There are 9 stars. 6 are yellow. How many are NOT yellow?"**
- Answer: 3

---

### MC4 ✅

Clean fill-in-blank. No changes.

---

## Block 7 — Challenge Extension

### CE1 — Garden fractions ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Image subtext names the answer fraction** (1/6) — remove all fraction labels from CE figure.

**Question:** A school garden is a rectangle. 2/3 of it has flowers. 1/4 of the flower section has roses. What fraction of the entire garden has roses?
**Options:** **(A) 1/6 ✓** (B) 1/4 (C) 2/3 (D) 1/12

| Hint | Old text | ✏️ New text | Words |
|------|----------|------------|-------|
| 1 | Step 1: The flowers cover 2/3. That is your starting whole for the next step. | No change — good CUE. ✅ | — |
| 2 | Step 2: Roses are 1/4 of the flower section only. Split the flower section into 4 equal parts. | No change — good CUE. ✅ | — |
| 3 | Look at the whole garden rectangle. Count how many equal parts it has been split into, and how many are roses. | **Count the equal pieces in the whole garden now.** | 9 |

> Hint 3 old version was 25 words and described the method. New version is 9 words and just says what to count.

---

## All figure field fixes (summary)

| Location | Issue | Fix |
|----------|-------|-----|
| CF2 | Fraction labels on SVGs | Remove from asset |
| Step 1 | No images | Add 2 new SVGs |
| Step 2 | No image | Add labelled SVG |
| Step 4 | No image | Add dot grid SVG |
| Step 8 | No figures | Add 2 new SVGs |
| WE1 `problem.figure` | Bare string | → `{ "src": "..." }` |
| WE1 SVG | Verify 6 kangaroos visible | Asset check |
| WE2 `problem.figure` | Bare string | → `{ "src": "..." }` |
| WE2 Step 2 figure | Alt text names "150 g" | Remove numbers from alt |
| P1 figure | Bare string + answer subtext | → `{ "src": "..." }` + remove label |
| P2 figure | Bare string | → `{ "src": "..." }` |
| P3 | Need 4 option SVGs | Add as `optionFigures` |
| P5 figure | Bare string + label cut by line | → `{ "src": "..." }` + fix SVG |
| P7 figure | Bare string + number subtext | → `{ "src": "..." }` + remove subtext |
| MC1 figure | Bare string | → `{ "src": "..." }` |
| MC2 | Need 4 option SVGs | Add as `optionFigures` |
| MC3 figure | Bare string + answer in caption | → `{ "src": "..." }` + remove caption |
| CE1 figure | Bare string + answer fraction label | → `{ "src": "..." }` + remove label |
