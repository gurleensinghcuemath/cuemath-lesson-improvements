# Lesson 2.1 — Fractions as Parts of a Whole: Visual Models (Improved)

**ID:** `mk-f-fractions-visual-models`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved
**Skills:** Number Theory · Fractions · Visual Models

> ✏️ marks every content change. 🐛 marks critical code/asset bugs. 🆕 marks new additions.

---

## What changed and why — quick read

| Category | Count | Biggest wins |
|----------|-------|--------------|
| 🐛 Asset/layout bugs | 8 | CF2 fractions labeled on figures; Step 1 no images; Step 8 no figures; WE1 kangaroos not visible; P2/P3 `{blank}` renders as code; MC2/MC3 options or answers embedded in question text; CE1 answer in image subtext |
| ✏️ Answer-hints → CUEs | 12 | Step 4 "!" hint; Step 5 wrong-answer reveal; Steps 6–7 hints; WE1 steps 3–4; WE2 steps 1–3; P7 redundant subtext; CE1 hint 3 |
| ✏️ Language simplified | 9 | Step 1 keyInsight; Step 3 incomplete statement; Step 4 "÷" in keyInsight; Step 6 abstract "whole" definition; P3 options in question text; P7 text below image; MC2 options in question text |
| ✏️ Question rephrased | 4 | Step 3 denominator question; P2 {blank} label; P3 self-answering options; MC3 answer given below figure |
| ✏️ Attempt counts standardised | 1 | All practice problems → 2 hints max |

---

## Block 1 — Challenge First

> Students attempt cold. Hint ladder unlocks after 2 minutes.

---

### CF1 — Sarah and the unequal rectangle

**Type:** MCQ | **Figure:** `MK_L21_CF1_unequal_rect.svg`

**Question:** Sarah colours 3 of the 5 sections of this rectangle and says she has coloured 3/5 of it. Is she right?
**Options:** (A) Yes — 3 of 5 parts are coloured, so the fraction is 3/5. **(B) No — a fraction only works when all the parts are the same size. ✓** (C) Yes — you always count coloured parts divided by total parts. (D) No — she should have coloured exactly half.
**Answer:** index 1

Hints — ✅ both are good CUEs, no changes needed.

---

### CF2 — Same fraction or different? ✏️🐛

**Type:** MCQ | **Figure:** `MK_L21_CF2_spine_pair.svg`

🐛 **Figures label the actual fractions:** The SVG for Figure A shows "2/3" written below it, and Figure B shows "6/9" — the two values the student is supposed to work out. Remove all fraction labels from both figures. The figures should show only the visual (shaded rectangle and dot grid) with no text annotations.

**Question:** Both of these figures show the same fraction. Which fraction is it?
**Options:** **(A) 2/3 ✓** (B) 1/3 (C) 1/2 (D) They show different fractions.
**Answer:** index 0

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Count the shaded parts in the rectangle and count all its equal parts. Write that as a fraction. | *No change — good CUE.* | ✅ keep |
| 2 | For the dots: 6 are coloured, 9 total → fraction is 6/9. Does 6/9 equal 2/3? Try dividing the top and bottom of 6/9 by 3. | **You found the rectangle fraction. Now count the coloured dots and the total dots. Can you simplify that fraction to match?** | ❌→✅ CUE |

> 💡 **Why:** Hint 2 named both numbers (6 coloured, 9 total) and explicitly stated the fraction 6/9 — handing over the key step the student needs to discover.

---

## Block 2 — Interactive Lesson: "What Is a Fraction, Really?"

---

### Step 0 — Predict: Same fraction or different?

No content changes. onCorrect and onWrong are well-written. ✅

---

### Step 1 — Explain: What a fraction really says ✏️🐛

🐛 **No images provided.** This step compares rectangle (a) with equal parts and rectangle (b) with unequal parts — the entire point is visual. Without images the explanation is meaningless.

🆕 **Suggested figures:**
- `MK_L21_Step1_rect_equal.svg` — rectangle split into 4 equal parts, 3 shaded
- `MK_L21_Step1_rect_unequal.svg` — rectangle split into 4 unequal sections, 3 coloured

✏️ **keyInsight simplified** — current version is a full two-sentence rule. Grade 3-4 needs one sharp line:
- Old: "A fraction is only valid when all parts are the same size. No equal parts → no fraction."
- New: **"For a fraction to work, every part must be exactly the same size."**

---

### Step 2 — Explain: Numerator and denominator ✏️🐛

🐛 **No image provided.** The step describes a rectangle divided into 3 equal parts with 2 shaded — this needs a visual to anchor the vocabulary "numerator" and "denominator."

🆕 **Suggested figure:** `MK_L21_Step2_label_diagram.svg` — a rectangle showing 2 shaded / 3 total, with arrows pointing to "2 = numerator (parts chosen)" and "3 = denominator (total equal parts)"

✏️ **endQuestion:** The `{blank}` prompt style works here — no change needed. But add a gentle wrong-answer nudge:
- 🆕 **onWrong:** "The denominator is the bottom number. It tells you how many equal parts the shape was cut into — not how many are shaded."

---

### Step 3 — Apply: Read three fractions ✏️

**Sub-question 1 (rectangle, 2 of 5 shaded):** ✅ fine as-is.

**Sub-question 2 (which shows 3/4?):** ✏️ **Statement is incomplete and the denominator question needs rephrasing.**

- Old prompt: "Four rectangles, each with 4 equal parts: (A) all 4 shaded, (B) only 1 shaded, (C) exactly 3 shaded, (D) only 2 shaded. Which shows 3/4?"
- Issue: The prompt describes the figures in text but doesn't show them. Also "can't 2/3 mean there are multiples of 3 total parts?" — the denominator concept hasn't been locked down yet. Rephrase to remove ambiguity:
- New prompt: **"3/4 means 3 parts are shaded out of 4 equal parts in total. Which rectangle shows exactly that?"**

✏️ **Hint after wrong answer reveals the answer:**
- Old wrong-answer hint: "3/4 means 3 of the 4 equal parts are shaded. Count the shaded sections in each option."
- This is fine as a first hint, but if it follows a wrong answer it needs to guide without naming the answer. New:
- **"Look at option (C). Count its shaded parts. Count its total equal parts. Does that match 3/4?"**

**Sub-question 3 (circle, 4 of 6 shaded):** ✅ fine as-is.

---

### Step 4 — Explain: Same idea, different look — set model ✏️

✏️ **keyInsight:** Remove "÷" symbol and "!" punctuation — both are confusing for Grade 3-4:
- Old: "Objects instead of parts of a shape — the rules are identical: chosen ÷ equal total."
- New: **"Whether you're counting parts of a shape or separate objects, the rule is the same: how many did you choose out of how many equal ones in total?"**

✏️ **"!" hint is strangely written** — the onAllCorrect or inline hint that uses "!" mid-sentence feels abrupt. Review all exclamation marks in this step and remove or soften them.

🆕 **Suggested figure:** `MK_L21_Step4_dot_grid.svg` — a 3×3 grid of 9 circles, top 6 filled orange, bottom 3 empty. Without this, the set-model concept floats with no visual anchor.

---

### Step 5 — Apply: Two set-model reads ✏️

**Sub-question 1 (5 gold stars of 8):** ✅ fine as-is.

**Sub-question 2 (fraction NOT coloured):** ✏️ **Wrong-answer follow-up reveals the answer:**
- Old onWrong / next hint: Tells student "NOT coloured means white tiles" and names 7 as the count — this is the answer.
- New: **"NOT coloured means you're counting the tiles that have no colour. How many tiles are white?"** — stops before naming 7.

---

### Step 6 — Explain: What is the whole? ✏️

✏️ **Definition is not concrete enough for Grade 3-4:**
- Old: "John sees 6 kangaroos through his window. Those 6 are the PART — the whole park holds more. Before writing a fraction, always ask: what is the WHOLE? Once you name the whole, the fraction follows: Part ÷ Whole = Fraction. To reverse: Whole = Part ÷ Fraction."
- Issues: "Part ÷ Whole = Fraction" uses ÷ symbol (banned); the formula is abstract and confusing for 8-year-olds; "To reverse: Whole = Part ÷ Fraction" is algebra-level reasoning.
- New: **"John looks through his window and sees 6 kangaroos. But the park has more kangaroos than he can see. The 6 he sees are only a PART of the whole group. Before writing a fraction, you need to know two things: what you are counting (the part) and what the full group is (the whole). The fraction is: part out of whole."**

✏️ **endQuestion progression is flat** — the single question (1/2 of park = 6, find whole) is the right difficulty. But add a 🆕 **onWrong nudge:**
- **"If 6 kangaroos are half the park, think of the park as two equal groups. How many kangaroos are in both groups together?"**

---

### Step 7 — Apply: Find the whole ✏️

**Sub-question 1 (4 squares = 1/4, find total):**
- Hint: "If 4 squares = 1/4, the full bar (all 4 quarters) = 4 × 4 squares." → Gives the full working. ✏️
- New: **"If 4 squares make up 1 quarter of the bar, how many squares make up all 4 quarters?"**

**Sub-question 2 (3 slices = 3/4, find total):**
- Hint: "3 slices = 3/4. So 1 slice = 1/4. How many quarters make a whole pizza?" → The first two sentences do all the reasoning; the question is trivial.
- New: **"3 slices are 3 out of how many equal slices? If 3 slices fill 3 quarters, how many slices fill 1 quarter?"**

✏️ **Question difficulty doesn't increase** between sub-questions 1 and 2 — both follow the same "part = fraction → find whole" pattern. Consider making sub-question 2 slightly harder by not naming the fraction explicitly, e.g. "Maria eats 3 slices. The whole pizza had 4 equal slices. She ate ___ quarters of the pizza." That introduces the link between counting and fractions.

---

### Step 8 — Apply: Prove it — why do both figures show 2/3? ✏️🐛

🐛 **No figures provided.** This step refers to Figure A (rectangle) and Figure B (dot grid) but provides no SVGs. Students are asked to work from visuals that aren't shown.

🆕 **Required figures:**
- `MK_L21_Step8_figA_rect.svg` — rectangle with 3 equal columns, 2 shaded yellow
- `MK_L21_Step8_figB_dots.svg` — 3×3 grid of 9 dots, 6 coloured orange

**Sub-question 1 (shaded fraction of rectangle):**
- Hint: "Count the shaded columns in Figure A — that is the numerator. The denominator is 3." → Tells the student what the denominator is.
- New: **"Count the shaded columns. Count all the columns. Write shaded out of total."**

**Sub-question 2 (coloured fraction of dot grid):**
- Hint: "Count all dots (3 rows × 3 columns) — that is the denominator." → Gives the denominator (9) and the method.
- New: **"Count all the dots in the grid. That total is the denominator."**

**Sub-question 3 (simplify 6/9):**
- Hint: "6 ÷ 3 = 2." → Gives the numerator of the answer directly.
- New: **"Both the top and bottom of 6/9 can be divided by the same number. What number goes into both 6 and 9?"**

---

### Step 9 — Reveal: Three tools, one idea

Content is solid. ✅ No changes needed.

---

## Block 3 — Worked Example 1 (MK 2017 Q02)

**Question:** John looks out the window. He sees half of the kangaroos in the park. How many kangaroos are there in the park?

---

### WE1 — Problem figure 🐛

🐛 **`problem.figure` is a bare string** → must be `{ "src": "..." }` object.
🐛 **6 visible kangaroos not shown in image:** The problem says John can see some kangaroos — the figure must clearly show exactly 6 kangaroos visible through a window frame. Without seeing the 6, students cannot solve the problem from the figure. Verify the SVG shows a countable group of 6.

---

### WE1 — Step 1: Name the fraction ✅

Checkpoint (fill "1"/2) is a good confirmation question. No changes.

---

### WE1 — Step 2: Identify part vs whole ✅

2-option MCQ is well-framed. No changes.

---

### WE1 — Step 3: Bar model — find the total ✏️

🐛 **Step figure is correct format** `{ "src": "..." }` ✅ — keep.

✏️ **Narration gives away the answer before the checkpoint:**
- Old narration: "…Left half = 6 visible kangaroos. Right half = the same number (both halves are equal)." followed by list: "1 half = 6 kangaroos. 2 halves = 6 + 6 = 12 kangaroos."
- The checkpoint then asks "The whole park has ___ kangaroos" — but the narration just computed 12.
- New narration (remove the list): **"The whole park = 2 equal halves. You know one half = 6 kangaroos. The other half is the same size. Use the bar model to find the total."**
- Let the student do the addition in the checkpoint.

---

### WE1 — Step 4: Match to answer options ✏️

✏️ **Narration reveals the answer before the checkpoint:**
- Old: "Answer = 12. Match it to the competition choices."
- New: **"You have found the total. Now find it in the answer choices below."**

---

## Block 4 — Worked Example 2 (MK 2019 Q15)

**Question:** A full glass weighs 400 g. An empty glass weighs 100 g. How many grams does a half-full glass weigh?

---

### WE2 — Problem figure 🐛

🐛 **`problem.figure` is a bare string** → must be `{ "src": "..." }` object.

---

### WE2 — Step 1: Separate glass from water ✏️

✏️ **Narration explains the answer, then asks the checkpoint:**
- Old narration list: "Water alone = 400 − 100 = 300 g" — immediately followed by "The water alone weighs ___ grams."
- New narration (stop before the calculation): **"The glass itself weighs the same in every picture — 100 g. A full glass = 400 g total. That total includes the glass AND the water. How could you find out how much just the water weighs?"**
- Let the student compute 400 − 100 in the checkpoint.

---

### WE2 — Step 2: Half of the water ✏️

✏️ **Image and explanation give the answer before the checkpoint:**
- Old: Figure alt text says "top = 150 g, bottom = 150 g" — the answer (150) is in the alt text.
- New figure alt: **"Vertical bar for 300 g water, divided into two equal halves"** — no numbers in the alt text.
- Old narration: "'Half-full' means half of the water is in the glass." — this is fine, but the checkpoint ("Half of 300 g = ___") is then trivial.
- New narration: **"'Half-full' means only half of the water fits in the glass. You know the total water is 300 g. What is half of that?"** — framed as a question the student answers in the checkpoint.

---

### WE2 — Step 3: Add the glass back ✏️

✏️ **Narration list computes the final answer before the checkpoint:**
- Old list: "= 150 + 100 = 250 g"
- New narration (stop before the sum): **"The half-full glass holds 150 g of water. But the glass itself still weighs 100 g. Add those two together in the checkpoint below."**

---

### WE2 — Step 4: Why is 200 g wrong? ✅

Conceptual MCQ is well-designed. No changes.

---

## Block 5 — Practice Lab

---

### P1 ✏️🐛

**Type:** MCQ | **Figure:** `MK_L21_P1_rect_1of3.svg`

🐛 **`figure` bare string** → `{ "src": "..." }`

✏️ **No subtext needed on the image** — the image should speak for itself. Remove any label text printed directly on or below the SVG (e.g. "1 of 3 parts shaded"). The question asks what fraction is shaded — the answer label defeats the purpose.

Hint — ✅ good CUE, no change.

---

### P2 ✏️🐛

**Type:** Fill in blank | **Figure:** `MK_L21_P2_shapes_set.svg`

🐛 **`figure` bare string** → `{ "src": "..." }`

🐛 **`{blank}` rendering as code:** The question text reads "The fraction of shapes that are circles = {blank}/10" — the `{blank}` placeholder is visible as literal text in the CMS. Rewrite the question to avoid inline blanks:

✏️ **New question:** **"There are 10 shapes in the row — 6 circles and 4 triangles. How many of the 10 shapes are circles?"**
- Type: `fill_in_blank`
- Answer: 6
- Follow-up display: "So the fraction that are circles = your answer / 10."

Hint — ✅ no change.

---

### P3 ✏️

**Type:** MCQ

✏️ **Options are given inside the question text itself** — the question describes every option in plain language ("(A) Rectangle with 5 equal parts, 3 shaded. (B) Rectangle with 5 equal parts, exactly 2 shaded…") making this a read-and-match rather than a think-and-choose. The figure SVGs should carry the visual information; the question should only ask:

✏️ **New question:** **"Which of these figures shows the fraction 2/5?"**
- Options: (A) / (B) / (C) / (D) — visuals only, no descriptions in option text

🆕 **Required figures:** One SVG per option showing the four rectangles described, referenced as `optionFigures`.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | 2/5 means 2 shaded out of 5 equal parts. Count the parts and the shaded ones in each option. | *No change — good CUE.* | ✅ keep |
| 2 | Watch option (D) carefully — are its 5 parts equal in size? | *No change — good CUE.* | ✅ keep |

---

### P4 ✅

Hints are good CUEs. No changes.

---

### P5 ✏️🐛

**Type:** Fill in blank | **Figure:** `MK_L21_P5_labeled_portion.svg`

🐛 **`figure` bare string** → `{ "src": "..." }`

🐛 **`{blank}` in question text** — same rendering issue as P2. Rewrite:
✏️ **New question:** **"The shaded part of this rectangle contains 8 small squares. The shaded part is 2/3 of the full rectangle. How many small squares does the whole rectangle contain?"**

🐛 **Image text cut by dividing line:** The label text on the figure is overlapping or being cut off by the line separating the shaded and unshaded sections. Fix the SVG so labels sit outside the dividing line.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | If 2/3 of the whole = 8, then 1/3 of the whole = 8 ÷ 2 = 4. | **If 2 equal parts = 8 squares, how many squares are in just 1 of those equal parts?** | ❌→✅ CUE |
| 2 | Three thirds = the whole. Whole = 3 × 4 = ? | **You found the size of 1 part. The whole rectangle has 3 of those equal parts. How many squares is that in total?** | ❌→✅ CUE |

---

### P6 ✅

Hints are good CUEs. No changes.

---

### P7 ✏️🐛

**Type:** MCQ | **Figure:** `MK_L21_P7_rect_6of8.svg`

🐛 **`figure` bare string** → `{ "src": "..." }`

✏️ **Question text below image is redundant and reveals the answer:** The figure shows 6 of 8 parts shaded, and the question text (or image subtext) restates "6 of its 8 equal parts shaded" — this makes the simplification step (6/8 = 3/4) obvious. Remove the subtext from the image and simplify the question:

✏️ **New question:** **"What fraction of the rectangle is shaded? Which dot set below shows the same fraction?"**
- (A) / (B) / (C) / (D) — dot sets shown as figures only

The student must first read the rectangle fraction themselves, then match it — no numbers given in the question text.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Simplify the rectangle fraction: 6/8 = ? (divide both numbers by 2). | **Count the shaded parts and total parts in the rectangle. Can you write that as a simpler fraction?** | ❌→✅ CUE |
| 2 | 6/8 = 3/4. Which option shows 3 out of every 4 dots coloured? | **You simplified the rectangle fraction. Now look at each dot set — which one matches that same fraction?** | ❌→✅ CUE |

---

### P8 ✅

Hints are good CUEs. No changes.

---

### Attempt count standardisation ✏️

✏️ **Inconsistent hint counts across practice problems** — some problems have 1 hint (1 extra attempt), some have 2 hints (2 extra attempts). Standardise to **2 hints per problem** for consistency. P1 currently has only 1 hint — add a second:

🆕 **P1 hint 2:** **"The denominator is the total number of equal parts. The numerator is how many are shaded. Write numerator/denominator."**

---

## Block 6 — Mastery Check

> No hints allowed.

---

### MC1 🐛

🐛 **`figure` bare string** → `{ "src": "..." }`

✏️ **Question phrasing is awkward:** "How many of the 6 equal parts are shaded? ___ (The fraction shaded is that number /6.)" — the parenthetical tells the student the denominator and the format, reducing this to a counting task.
- New: **"Look at the rectangle. What fraction of it is shaded? Write the numerator only — the denominator is 6."**

---

### MC2 ✏️

✏️ **Options described in question text:** Same issue as P3 — the question lists all four options as text descriptions of figures. The options field should contain "(A) / (B) / (C) / (D)" as figure references only.

✏️ **New question:** **"Which of these figures shows the fraction 1/3?"**
- Options: (A) / (B) / (C) / (D) — visuals via `optionFigures`

🆕 **Required figures:** Four rectangle SVGs as described in the original.

---

### MC3 🐛✏️

🐛 **`figure` bare string** → `{ "src": "..." }`

🐛 **Answer given below figure:** The image subtext or caption reads the answer (3 not-yellow stars, or the fraction 3/9) — remove all answer text from the figure and its caption.

✏️ **Question phrasing:** "How many stars are NOT yellow? ___ (The fraction NOT yellow is that number/9.)" — the parenthetical again reduces difficulty by naming the denominator and format.
- New: **"There are 9 stars. 6 are yellow. How many are NOT yellow?"**
- Answer: 3
- (The follow-on fraction concept is implicit — if needed, a second checkpoint can ask "write that as a fraction out of 9.")

---

### MC4 ✅

Clean fill-in-blank with no hints. No changes.

---

## Block 7 — Challenge Extension

---

### CE1 — Garden fractions ✏️🐛

**Type:** MCQ | **Figure:** `MK_L21_CE1_garden.svg`

🐛 **`figure` bare string** → `{ "src": "..." }`

🐛 **Answer revealed in image subtext:** The figure caption or subtext names the answer fraction (1/6). Remove all text annotations from the CE figure — it should show only the garden rectangle divided into sections, with no fraction labels.

**Question:** A school garden is a rectangle. 2/3 of the garden has flowers. 1/4 of the flower section has roses. What fraction of the entire garden has roses?
**Options:** **(A) 1/6 ✓** (B) 1/4 (C) 2/3 (D) 1/12
**Answer:** index 0

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Step 1: The flowers cover 2/3 of the garden. That is your starting 'whole' for the next step. | *No change — good CUE.* | ✅ keep |
| 2 | Step 2: Roses are 1/4 of the FLOWER SECTION only. Split the flower section into 4 equal parts. | *No change — good CUE.* | ✅ keep |
| 3 | Step 3: Look at the whole garden rectangle. Count how many equal parts it has been split into, and how many are roses. | **Look at the whole garden shape. After splitting it for flowers and then splitting the flower part for roses, how many equal pieces is the whole garden now divided into? How many of those pieces are roses?** | ❌→✅ CUE |

> 💡 **Why hint 3 changed:** The original hint 3 essentially described the diagram and told the student to count — but without naming the answer, it was close to a CUE already. The new version asks the same question more concretely for a Grade 3-4 student.

---

## Summary of all figure field fixes

| Block | Item | Fix needed |
|-------|------|-----------|
| CF2 | Remove fraction labels from SVG | Asset fix |
| Step 1 | Add two rectangle SVGs (equal vs unequal) | 🆕 new asset |
| Step 2 | Add labeled numerator/denominator diagram | 🆕 new asset |
| Step 4 | Add dot grid SVG | 🆕 new asset |
| Step 8 | Add Figure A (rect) and Figure B (dots) | 🆕 new assets |
| WE1 | `problem.figure` bare string → `{src:...}` | 🐛 schema fix |
| WE1 | Verify 6 kangaroos visible in SVG | 🐛 asset check |
| WE2 | `problem.figure` bare string → `{src:...}` | 🐛 schema fix |
| WE2 Step 2 | Remove numbers from figure alt text | 🐛 asset fix |
| P1 | Remove answer subtext from SVG | 🐛 asset fix |
| P1 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| P2 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| P3 | Add 4 option SVGs as `optionFigures` | 🆕 new assets |
| P5 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| P5 | Fix label cut by dividing line in SVG | 🐛 asset fix |
| P7 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| P7 | Remove number subtext below image | 🐛 asset fix |
| MC1 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| MC2 | Add 4 option SVGs as `optionFigures` | 🆕 new assets |
| MC3 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| MC3 | Remove answer from figure caption | 🐛 asset fix |
| CE1 | `figure` bare string → `{src:...}` | 🐛 schema fix |
| CE1 | Remove answer fraction from image subtext | 🐛 asset fix |
