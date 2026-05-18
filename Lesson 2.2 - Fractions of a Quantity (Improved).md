# Lesson 2.2 — Fractions of a Quantity & Reverse Problems (Improved)

**ID:** `mk-f-fractions-quantity-reverse`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved v2
**Skills:** Number Theory · Fractions

> ✏️ content change · 🐛 code/asset bug · 🆕 new addition

---

## What changed and why

| Category | Biggest wins |
|----------|-------------|
| 🐛 Code/asset bugs | `fraction-bar` applet unregistered; all `problem.figure` bare strings; PDF download button; P2/P4 answers in image; WE figure alt texts reveal answers |
| ✏️ Hints → true CUEs | ALL hints rewritten to ≤ 10 words. No hint names an answer, value, or full method. |
| ✏️ Narrations shortened | Step 2, Step 7 rewritten shorter than originals. All WE narrations stop before the final calculation. |
| ✏️ Algebraic notation removed | Step 1 formula (1/n, W); Step 6; Step 7 (m/n); Step 9 inline hint |
| 🆕 New content | CF1/CF2 hints added (none existed); Step 10 made interactive; 2 hints added to every practice problem |

---

## Block 1 — Challenge First

---

### CF1 — Sam's marbles ✏️🆕

**Type:** MCQ

✏️ "Kiran" → "Sam" (US-neutral name for Math Kangaroo audience)

**Question:** A bag holds 20 marbles. Sam takes 1/4 of them. How many marbles does Sam take?
**Options:** 4 / **5 ✓** / 10 / 15 / 20
**Answer:** index 1

🆕 **onWrong:** "Split the marbles into 4 equal groups."

🆕 **Hints:**

| # | Text | Word count |
|---|------|-----------|
| 1 | What does the bottom number of a fraction mean? | 9 |
| 2 | Make 4 equal groups from 20. | 6 |

> **Why these work:** Hint 1 points to a concept. Hint 2 gives the action without computing the answer. Neither names 5.

---

### CF2 — Reverse: find the whole ✏️🆕

**Type:** MCQ

**Question:** 1/3 of a certain number is 8. What is that number?
**Options:** 11 / 16 / **24 ✓** / 32 / 40
**Answer:** index 2

🆕 **onWrong:** "How many equal parts make one whole?"

🆕 **Hints:**

| # | Text | Word count |
|---|------|-----------|
| 1 | You have 1 part. How many parts in the whole? | 10 |
| 2 | Use 8 to find all 3 equal parts. | 8 |

> **Why these work:** Hint 1 points to counting parts. Hint 2 says "use 8" and "3 parts" but never names 24 or writes 8 × 3.

---

## Block 2 — Interactive Lesson

---

### Step 1 — Reveal: What "fraction of a quantity" means ✏️🐛

🐛 **PDF download button visible in lesson** — remove this UI element.

✏️ **Formula removed** (1/n, W — too abstract). Replace with:

> "The bottom number tells you how many equal groups to make.
> The top number tells you how many of those groups to take.
> Example: 1/4 of 20 → split into 4 groups → each group = 5."

---

### Step 2 — Explain: Find one part, then multiply ✏️

✏️ **Old text had numbered bullet steps** — felt like a manual. Simplified:

> "To find a fraction of a number, use two steps.
> Divide by the bottom number to get one equal part.
> Multiply that part by the top number.
> Try: 3/4 of 20 → 20 divided by 4 = 5 → 5 × 3 = 15."

✏️ **keyInsight:**
- Old: 2-sentence rule with "unit piece" jargon
- New: **"Find one equal part first. Then multiply to get the parts you need."**

---

### Step 3 — Predict: 1/4 of 20 ✏️

✏️ **onCorrect:** Remove "Yes!" → **"20 split into 4 equal groups gives 5 in each group."**

✏️ **onWrong:** Was giving the full calculation. Now:
**"Think: how many equal groups does 1/4 make?"**

---

### Step 4 — Applet: Equal groups ✏️🐛

🐛 **`appletType: "fraction-bar"` is not registered in CMS** — same class as "digit-card-builder" bug in L1.1. Will not load.

✏️ **Replace applet with a static apply step:**
- Figure: `MK_L22_Step4_20dots_4rows.svg` — 20 dots in 4 equal rows
- Instruction: "Look at the dots. They are split into 4 equal rows."
- Question: "How many dots are in each row?"
- Answer: 5
- Hint: "Count the dots in just one row."

✏️ Remove "Tap each group" instruction — nothing to tap.

✏️ **discoveryMessage** shortened:
- Old: 3 sentences explaining why division works
- New: **"Each group has 5. So 1/4 of 20 = 5."**

---

### Step 5 — Apply: 3/4 of 20 ✏️

**Sub-step 1 (find 1/4 of 20):** Hint "Divide 20 by the denominator 4" ✅ — 7 words, good CUE, keep.

**Sub-step 2 (multiply by 3):**
- Old hint: "3/4 = 3 × (1/4) = 3 × 5." — gives full working
- New: **"You have 1 part. Now take 3 of those."** (8 words)

---

### Step 6 — Reveal: Working backwards ✏️

✏️ **Old formula (P × n) removed.** Replaced with:

> "If you know one part, you can find the whole.
> Multiply that part by the bottom number.
> Example: 1/4 of a number is 5 → whole = 5 × 4 = 20."

✏️ Remove the curiosity-reveal that computes the answer inline — show only after the student answers.

---

### Step 7 — Explain: The reverse method ✏️

✏️ **Old text used m/n and algebraic bullets.** Replaced with:

> "You are given a part of the number — not the whole.
> Divide the part by the top number to get one equal piece.
> Multiply that piece by the bottom number to get the whole.
> Example: 2/3 of a number is 14 → one piece = 14 divided by 2 = 7 → whole = 7 × 3 = 21."

✏️ **keyInsight:**
- Old: 2-sentence rule about "going the wrong direction"
- New: **"The whole is always bigger than the part you started with."**

🆕 **onWrong:** "What does dividing by the top number give you?" (9 words)

---

### Step 8 — Predict: 1/4 of a number is 7 ✏️

✏️ **onCorrect:** Remove check notation → **"7 × 4 = 28. Split 28 into 4 equal groups — each group is 7."**

✏️ **onWrong:** Was giving the full equation. Now:
**"You have 1 part. How many parts make the whole?"** (9 words)

---

### Step 9 — Apply: Reverse with a non-unit fraction ✏️

**Sub-step 1:**
✏️ Remove inline hint from prompt text. New prompt: **"2/3 of a number is 14. What is 1/3 of the same number?"**
- Old hint: "Divide the given part by the numerator: 14 ÷ 2 = 7." — gives full answer
- New: **"You have 2 equal parts. What is 1 part worth?"** (9 words)

**Sub-step 2:** Hint "Multiply 1/3 by 3 to build the whole" ✅ — 7 words, keep.

---

### Step 10 — Explain: Spotting fractions in MK problems ✏️

✏️ **Was text-only — passive card.** Add endQuestion:

🆕 **Question:** "Carl ate half the oranges. Then he ate half of what was left. For the second step, the 'whole' is:"
- (A) All the oranges at the start
- **(B) The oranges left after the first half ✓**
- (C) The same as the first half

---

## Block 3 — Worked Example 1 (MK 2009 Q6)

**Problem:** Mother bought 16 oranges. Carl ate half, Eva ate 2, Sophie ate the rest. How many did Sophie eat?

---

### WE1 — problem.figure 🐛

🐛 **Bare string** → `{ "src": "/figures/mk-grade-3-4/lesson-2-2/MK_L22_WE1_oranges_bar.svg" }`

---

### WE1 — Step 1: Identify the whole ✅

Narration does not reveal the answer. Checkpoint is clean. No changes.

---

### WE1 — Step 2: Carl's share ✏️🐛

🐛 **Alt text reveals answer:** "16 oranges split in half: left 8 are Carl's, right 8 remain"
- New alt: **"A bar showing 16 oranges split into two equal halves"**

✏️ **Narration computed the answer before the checkpoint:**
- Old: "1/2 of 16 = 16 ÷ 2 = 8."
- New: **"Carl ate half of all the oranges. Use the bar model to find how many that is."**

---

### WE1 — Step 3: Subtract Eva's share ✏️🐛

🐛 **Alt text reveals Sophie's count** — remove numbers from alt.
- New alt: **"Remaining oranges after Carl, with some crossed out for Eva"**

✏️ **Narration computed the answer:**
- Old: "After Carl took 8, there are 16 − 8 = 8 left. Eva ate 2. Sophie gets 8 − 2 = 6."
- New: **"Carl took his half. Eva then ate 2 of what was left. Use the bar to find Sophie's share."**

---

### WE1 — Step 4: Verify ✏️

✏️ **Narration named the answer and option before checkpoint:**
- Old: "Carl ate 8, Eva ate 2, Sophie ate 6. Total = 16 ✓ Answer: B."
- New: **"Check: Carl's share + Eva's 2 + Sophie's share should equal 16. Then pick the matching option."**

---

## Block 4 — Worked Example 2 (MK 2014 Q10)

**Problem:** Sally, Tom, Clara each took half the remaining candy. 6 pieces were left. How many were there at the start?

---

### WE2 — problem.figure 🐛

🐛 **Bare string** → `{ "src": "/figures/mk-grade-3-4/lesson-2-2/MK_L22_WE2_chain.svg" }`

---

### WE2 — Step 1: Undo Clara's step ✏️🐛

🐛 **Alt text reveals 12:** "6 pieces → ×2 → 12 pieces before Clara"
- New alt: **"A chain diagram starting from 6, with an arrow going backwards"**

✏️ **Narration computed the answer:**
- Old: "6 × 2 = 12 pieces before Clara."
- New: **"Clara took half, leaving 6. The half she took was the same size. How many pieces were there before Clara?"**

---

### WE2 — Step 2: Undo Tom's step ✏️🐛

🐛 **Alt text reveals 24** — remove numbers from alt.
- New alt: **"The chain diagram extended one step back, before Tom"**

✏️ **Narration computed the answer:**
- Old: "Tom left 12, so before Tom: 12 × 2 = 24."
- New: **"You found 12 pieces before Clara. Tom took half before that, leaving those 12. How many were there before Tom?"**

---

### WE2 — Step 3: Undo Sally's step ✏️

✏️ **Narration computed the answer:**
- Old: "24 × 2 = 48 pieces before Sally."
- New: **"You found 24 before Tom. Sally took half before that, leaving those 24. How many were there at the very start?"**

---

### WE2 — Step 4: Verify forward ✏️

✏️ **Narration named "48 (option E)" before the MCQ:**
- Old: "48 → Sally takes half (24) → 24 → Tom takes half (12) → 12 → Clara takes half (6) ✓ Answer: 48 (option E)."
- New: **"Check by going forwards: start with your answer. Have Sally take half, then Tom, then Clara. Do you end up with 6? Now pick the matching option."**

---

## Block 5 — Practice Lab

> 🆕 All problems: 2 hints added (none existed). All `figure` bare strings fixed.

---

### P1 — 1/3 of 12 🐛🆕

🐛 `figure` bare string → `{ "src": "..." }`

| Hint | Text | Words |
|------|------|-------|
| 1 | Split 12 into 3 equal groups. | 6 |
| 2 | How many are in each group? | 7 |

---

### P2 — 1/4 of 24 🐛✏️🆕

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Answer written in image** — remove all number labels from group sizes in SVG.

| Hint | Text | Words |
|------|------|-------|
| 1 | Split 24 into 4 equal groups. | 6 |
| 2 | How many are in each group? | 7 |

---

### P3 — 3/4 of 20 🆕

| Hint | Text | Words |
|------|------|-------|
| 1 | Start by finding 1/4 of 20. | 7 |
| 2 | You need 3 of those equal parts. | 7 |

---

### P4 — 2/5 of 15 🐛✏️🆕

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Answer written in image** — remove number labels from SVG group sizes.

| Hint | Text | Words |
|------|------|-------|
| 1 | Start by finding 1/5 of 15. | 7 |
| 2 | You need 2 of those equal parts. | 7 |

---

### P5 — Reverse: 1/3 of a number = 9 ✏️🐛🆕

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Image subtext reveals the answer** — remove all number/calculation labels from SVG.

✏️ **Question simplified:**
- Old: "The bar shows 1/3 of a number = 9 (one segment is filled). What is the whole number?"
- New: **"One part of this bar equals 9. The bar has 3 equal parts. What is the whole bar?"**

| Hint | Text | Words |
|------|------|-------|
| 1 | The whole bar has 3 equal parts. | 7 |
| 2 | Use 9 to find all 3 parts. | 8 |

---

### P6 — Reverse: 1/4 of a number = 7 🆕

| Hint | Text | Words |
|------|------|-------|
| 1 | How many equal parts make one whole here? | 8 |
| 2 | Use 7 to find all 4 parts. | 8 |

---

### P7 — Reverse: 3/4 of a number = 12 🆕

| Hint | Text | Words |
|------|------|-------|
| 1 | 3 parts = 12. What is 1 part? | 8 |
| 2 | Now find all 4 equal parts. | 6 |

---

### P8 — Anna's apples 🆕

| Hint | Text | Words |
|------|------|-------|
| 1 | Count Anna and all her friends together. | 7 |
| 2 | Two people share exactly 1 whole apple. | 7 |

---

## Block 6 — Mastery Check

> No hints allowed in mastery check.

---

### MC1 ✅

Clean question, no figure. No changes.

---

### MC2 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Figure labels each group with its size** — remove group-size numbers from SVG.

✏️ **Question text gives away the answer:**
- Old: "The bar model shows 5 equal groups totalling 20. What is 3/5 of 20?"
- New: **"The bar is split into 5 equal parts and shows 20 in total. What is 3/5 of 20?"**
- Remove "5 equal groups totalling 20" — let the figure show this visually.

---

### MC3 ✅

Clean fill-in-blank. No changes.

---

### MC4 ✏️🐛

🐛 `figure` bare string → `{ "src": "..." }`
🐛 **Figure labels shaded segments with the answer number** — remove from SVG.

✏️ **Question text sets up the method:**
- Old: "The bar model shows 2 of 3 equal segments shaded, totalling 18. What is the whole?"
- New: **"The shaded part of the bar equals 18. The shaded part is 2/3 of the whole bar. What is the whole?"**

---

## Block 7 — Challenge Extension

### CE — Adam and Bart's chestnuts ✏️🆕

🆕 **Hints added** (none existed):

| Hint | Text | Words |
|------|------|-------|
| 1 | Try starting with 10 chestnuts each. | 7 |
| 2 | Compare Bart's total to Adam's total. | 7 |

> Hint 1 points to the "try a number" strategy without naming the answer. Hint 2 points to the comparison step.

---

## All figure field fixes (summary)

| Location | Issue | Fix |
|----------|-------|-----|
| WE1 `problem.figure` | Bare string | → `{ "src": "..." }` |
| WE1 Step 2 figure | Alt text names "8" | Remove numbers from alt |
| WE1 Step 3 figure | Alt text names Sophie's count | Remove numbers from alt |
| WE2 `problem.figure` | Bare string | → `{ "src": "..." }` |
| WE2 Step 1 figure | Alt text names "12" | Remove numbers from alt |
| WE2 Step 2 figure | Alt text names "24" | Remove numbers from alt |
| P1 figure | Bare string | → `{ "src": "..." }` |
| P2 figure | Bare string + answer in image | → `{ "src": "..." }` + remove label |
| P4 figure | Bare string + answer in image | → `{ "src": "..." }` + remove label |
| P5 figure | Bare string + answer in subtext | → `{ "src": "..." }` + remove label |
| MC2 figure | Bare string + group size labels | → `{ "src": "..." }` + remove labels |
| MC4 figure | Bare string + segment labels | → `{ "src": "..." }` + remove labels |
