# Lesson 2.2 — Fractions of a Quantity & Reverse Problems (Improved)

**ID:** `mk-f-fractions-quantity-reverse`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved
**Skills:** Number Theory · Fractions

> ✏️ marks every content change. 🐛 marks critical code/asset bugs. 🆕 marks new additions.

---

## What changed and why — quick read

| Category | Count | Biggest wins |
|----------|-------|--------------|
| 🐛 Code / asset bugs | 7 | `fraction-bar` applet unregistered; all `problem.figure` bare strings; PDF download button (UI); P2/P4 answers in image; WE figure alt texts reveal answers |
| ✏️ Answer-hints → CUEs | 11 | Steps 3, 5, 8, 9 onWrong; WE1 steps 2–4; WE2 steps 1–4; MC2/MC4 question text gives answer |
| ✏️ Algebraic notation removed | 5 | Step 1 formula (1/n, W); Step 6 formula; Step 7 dense text; Step 7 keyInsight; Step 9 inline hint |
| ✏️ Language simplified | 8 | Step 2 dense text; Step 7 reverse method; CF1 name changed; "!" removed; all hints shortened; Step 10 made interactive |
| 🆕 New content added | 4 | CF1 + CF2 hints added (none existed); onWrong nudges for CF1/CF2; hints added to all practice problems |

---

## Block 1 — Challenge First

> Students attempt cold. Hint ladder unlocks after 2 minutes.

---

### CF1 — Sam's marbles ✏️🆕

**Type:** MCQ

✏️ **Name changed:** "Kiran" → "Sam" — culturally neutral for a US Math Kangaroo audience.

**Question:** A bag holds 20 marbles. Sam takes 1/4 of them. How many marbles does Sam take?
**Options:** 4 / **5 ✓** / 10 / 15 / 20
**Answer:** index 1

🆕 **onWrong added** (was missing):
> "Think about splitting 20 marbles into 4 equal groups. How many go in each group?"

🆕 **Hints added** (none existed):

| Hint | Text |
|------|------|
| 1 | Split 20 into 4 equal groups. How many are in each group? |
| 2 | 20 divided into 4 groups = 20 ÷ 4. What is that? |

---

### CF2 — Reverse: find the number ✏️🆕

**Type:** MCQ

**Question:** 1/3 of a certain number is 8. What is that number?
**Options:** 11 / 16 / **24 ✓** / 32 / 40
**Answer:** index 2

🆕 **onWrong added** (was missing):
> "If 1/3 of a number is 8, think about how many thirds make a whole. What do you do to 8 to get the full number?"

🆕 **Hints added** (none existed):

| Hint | Text |
|------|------|
| 1 | 1/3 means the number was split into 3 equal parts. You have 1 part = 8. |
| 2 | To get all 3 parts, multiply: 8 × 3 = ? |

---

## Block 2 — Interactive Lesson: "Fractions of a Quantity"

---

### Step 1 — Reveal: What "fraction of a quantity" means ✏️🐛

🐛 **PDF download button showing in CMS** — remove this UI element. Students should not see a download option in the middle of an interactive lesson.

✏️ **Formula uses algebraic notation** (1/n, W) — too abstract for Grade 3-4:
- Old: `Part = Fraction × Whole → (1/n) of W = W ÷ n`
- New plain-language rule card:
  > **"A fraction of a number tells you one equal piece of a group.**
  > **The bottom number (denominator) says how many equal groups to make.**
  > **The top number (numerator) says how many of those groups you take.**
  > **Example: 1/4 of 20 — split 20 into 4 equal groups → each group has 5."**

Remove the formula line entirely. Keep the example. Students learn from examples, not formulas.

---

### Step 2 — Explain: Find the unit fraction first, then multiply ✏️

✏️ **Text is too dense and uses step-labels that feel like a manual.** Rewrite in plain, short sentences:

- Old: "To find any fraction of a quantity: • Step 1 — Find the unit fraction: divide the whole by the denominator. • Step 2 — Multiply by the numerator. Example: 3/4 of 20 → 1/4 of 20 = 20 ÷ 4 = 5 → 3/4 of 20 = 3 × 5 = 15"
- New:
  > **"To find a fraction of a number, do it in two moves.**
  > **First: divide the number by the bottom number. This gives you one equal part.**
  > **Then: multiply that part by the top number.**
  > **Try it: What is 3/4 of 20?**
  > **Step 1: 20 ÷ 4 = 5 (one part)**
  > **Step 2: 5 × 3 = 15 (three parts)**"**

✏️ **keyInsight** simplified:
- Old: "Always find '1/n of the whole' first. Every other fraction of the same whole is just a multiple of that unit piece."
- New: **"Always find one equal part first. Then multiply to get the number of parts you need."**

---

### Step 3 — Predict: Quick check ✏️

**Question:** What is 1/4 of 20?

✏️ **onCorrect:** Remove "Yes!" — replace with calm confirmation:
- Old: "Yes! 20 ÷ 4 = 5."
- New: **"20 ÷ 4 = 5. You split 20 into 4 equal groups and took one."**

✏️ **onWrong reveals the answer:**
- Old: "1/4 of 20 = 20 ÷ 4 = 5. Dividing by the denominator gives you one equal part."
- New: **"Think about splitting 20 into 4 equal groups. How many go in each group?"**

---

### Step 4 — Applet: Explore equal groups ✏️🐛

🐛 **appletType: "fraction-bar" is not registered in the CMS** — this applet will not load. Same class of bug as "digit-card-builder" in Lesson 1.1. Replace with a static visual + question:

✏️ **Replace applet with a simple apply step:**
- Show a static image: `MK_L22_Step4_20_dots_4groups.svg` — 20 dots arranged in 4 equal rows of 5
- **Instruction:** "Look at the dots. They are sorted into 4 equal groups."
- **Question:** "How many dots are in each group?"
- Answer: 5
- **Hint:** "Count the dots in just one row."

✏️ **"Tap each group to see how many items are in it"** — instruction is confusing because there is nothing to tap (applet broken). Remove this instruction entirely once the applet is replaced.

✏️ **discoveryMessage** is too long. Shorten:
- Old: "Each of the 4 equal groups has exactly 5 items. 1/4 of 20 = 5. This is why dividing by the denominator works — you are splitting the whole into equal parts."
- New: **"Each group has 5. So 1/4 of 20 = 5. Dividing by the bottom number splits the whole into equal groups."**

---

### Step 5 — Apply: Find 3/4 of 20 ✏️

**Sub-step 1 (find 1/4 of 20):**
- Hint: "Divide 20 by the denominator 4." → ✅ good CUE, keep.

**Sub-step 2 (multiply by 3):**
- Old hint: "3/4 = 3 × (1/4) = 3 × 5." → Gives the full working.
- New: **"You found 1 part = 5. Now you need 3 of those parts."** | ❌→✅ CUE

---

### Step 6 — Reveal: Thinking in reverse ✏️

✏️ **Formula uses algebraic notation:**
- Old: `If (1/n) of W = P, then W = P × n`
- New plain-language card:
  > **"Going backwards: if you know one part, you can find the whole.**
  > **Multiply the part by the bottom number.**
  > **Example: 1/4 of a number is 5 → the whole = 5 × 4 = 20.**
  > **Check: 1/4 of 20 = 5 ✓"**

✏️ **curiosity reveal** gives the answer before the student tries:
- The prompt asks "If 1/4 of a number is 5, what is the number?" then the reveal says "Multiply to undo the division: 5 × 4 = 20."
- Move the explanation AFTER the student answers, not inline with the reveal.

---

### Step 7 — Explain: The reverse method step by step ✏️

✏️ **Text is the most complex in the lesson** — algebraic bullet form with `m/n`, `P`, parentheses:
- Old: "• 'If 1/n of a number is P' → the whole is P × n • 'If m/n of a number is P' → find 1/n first: (P ÷ m), then the whole: (P ÷ m) × n"
- New:
  > **"If a fraction of a number is given, find the whole in two steps.**
  > **Step 1: Find 1 equal part. Divide the number you are given by the top number.**
  > **Step 2: Find the whole. Multiply 1 part by the bottom number.**
  > **Example: 2/3 of a number is 14.**
  > **Step 1: 1 part = 14 ÷ 2 = 7**
  > **Step 2: Whole = 7 × 3 = 21"**

✏️ **keyInsight (the "green formula")** is hard to follow:
- Old: "The whole is always larger than any proper fractional part. If your answer is smaller than the given part, you went the wrong direction."
- New: **"Your answer for the whole must always be bigger than the part you started with. If it is smaller, try again."**

✏️ **endQuestion hint** added for wrong answers:
🆕 onWrong: **"If 1/3 = 9, think: how many thirds make a whole? Multiply 9 by that number."**

---

### Step 8 — Predict: Practice the reverse ✏️

**Question:** 1/4 of a number is 7. What is the number?

✏️ **onCorrect:** keep as-is but remove the check notation — too math-symbol heavy for Grade 3-4:
- Old: "7 × 4 = 28. And 1/4 of 28 = 7 ✓"
- New: **"7 × 4 = 28. You can check: split 28 into 4 equal groups — each group is 7."**

✏️ **onWrong reveals the answer:**
- Old: "If 1/4 of the number is 7, the whole is 7 × 4 = 28."
- New: **"You have 1 out of 4 equal parts. How many parts make the whole? Multiply 7 by that."** | ❌→✅ CUE

---

### Step 9 — Apply: Reverse with a non-unit fraction ✏️

**Sub-step 1:**
- Old prompt embeds the hint inline: "Step 1 — Find 1/3 of the number. If 2/3 = 14, what is 1/3? (Hint: 14 ÷ 2)"
- ✏️ Remove the inline hint from the prompt. Move it to the hint field.
- New prompt: **"2/3 of a number is 14. What is 1/3 of the same number?"**
- Old hint: "Divide the given part by the numerator: 14 ÷ 2 = 7." → Gives full answer.
- New hint: **"You have 2 equal parts = 14. What is 1 part worth?"** | ❌→✅ CUE

**Sub-step 2:**
- Old hint: "Multiply 1/3 by 3 to build the whole." → ✅ good CUE, keep.

---

### Step 10 — Explain: Spotting fractions in MK problems ✏️

✏️ **This step is text-only with no interaction** — a passive card violates the "no-passive-cards" design principle from the lesson's own designPrinciples field.

🆕 **Add an endQuestion:**
> "Carl ate half the oranges. Then he ate half of what was left. The 'whole' for the second half is:"
- (A) All the oranges at the start
- **(B) The oranges that were left after the first half ✓**
- (C) The same as the first half

This locks in the key concept that "the whole changes at each step."

---

## Block 3 — Worked Example 1 (MK 2009 Q6)

**Question:** Mother bought 16 oranges. Carl ate half, Eva ate 2, and Sophie ate the rest. How many did Sophie eat?

---

### WE1 — Problem figure 🐛

🐛 **`problem.figure` bare string** → `{ "src": "/figures/mk-grade-3-4/lesson-2-2/MK_L22_WE1_oranges_bar.svg" }`

---

### WE1 — Step 1: Identify the whole ✅

Narration doesn't reveal the answer. Checkpoint is clean. ✅ No changes.

---

### WE1 — Step 2: Find Carl's share ✏️

🐛 **Figure alt text reveals the answer:** alt: "16 oranges split in half: left 8 are Carl's, right 8 remain" — names the answer (8) before the student tries.
- New alt: **"A bar showing 16 oranges split into two equal halves"**

✏️ **Narration computes the answer before the checkpoint:**
- Old: "Carl ate half of them. Half means 1/2 of 16. Use the rule: 1/2 of 16 = 16 ÷ 2 = 8."
- New: **"Carl ate half of all the oranges. Half means 1 out of 2 equal groups. Use the bar model to find how many that is."**

---

### WE1 — Step 3: Subtract Carl's and Eva's shares ✏️

🐛 **Figure alt text reveals Sophie's count:** alt: "8 remaining oranges: 2 crossed out (Eva), 6 green (Sophie)"
- New alt: **"The oranges remaining after Carl, with some crossed out for Eva"**

✏️ **Narration computes the full answer before the checkpoint:**
- Old: "After Carl took 8, there are 16 − 8 = 8 oranges left. Then Eva ate 2 of those." + "Oranges remaining for Sophie: 8 − 2 = 6."
- New: **"After Carl took his share, some oranges are left. Eva then ate 2 of those. Use the bar model to find how many are left for Sophie."**

---

### WE1 — Step 4: Verify and match ✏️

✏️ **Narration names the answer before the MCQ:**
- Old: "Check: Carl ate 8, Eva ate 2, Sophie ate 6. Total: 8 + 2 + 6 = 16 ✓ Sophie ate 6 oranges → answer B."
- New: **"Check your answer adds up: Carl's share + Eva's 2 + Sophie's share should equal 16. Now pick the matching answer option."**

---

## Block 4 — Worked Example 2 (MK 2014 Q10)

**Question:** Sally, Tom, then Clara each took half the remaining candy. 6 pieces were left. How many were there at the start?

---

### WE2 — Problem figure 🐛

🐛 **`problem.figure` bare string** → `{ "src": "/figures/mk-grade-3-4/lesson-2-2/MK_L22_WE2_chain.svg" }`

---

### WE2 — Step 1: Work backwards from the end ✏️

🐛 **Figure alt text reveals the answer:** alt: "6 pieces left → ×2 → 12 pieces before Clara"
- New alt: **"A chain diagram starting from 6 pieces left, with an arrow going backwards"**

✏️ **Narration computes the answer before the checkpoint:**
- Old: "After Clara took half, 6 pieces were left. So before Clara took half, there were 6 × 2 = 12 pieces."
- New: **"Clara took half, so 6 pieces are what was left after her. The half she took was the same size. Use the diagram — how many pieces were there before Clara took her share?"**

---

### WE2 — Step 2: Undo Tom's step ✏️

🐛 **Figure alt text reveals the answer:** alt: "12 pieces before Clara → ×2 → 24 pieces before Tom"
- New alt: **"The chain diagram extended one step further back, before Tom"**

✏️ **Narration computes the answer before the checkpoint:**
- Old: "Before Tom took half, twice as many pieces were there. Tom left 12, so before Tom: 12 × 2 = 24 pieces."
- New: **"You found there were 12 before Clara. Tom took half before that, leaving those 12. How many were there before Tom took his share?"**

---

### WE2 — Step 3: Undo Sally's step ✏️

✏️ **Narration computes the answer before the checkpoint:**
- Old: "Before Sally took half, twice as many pieces were there. Sally left 24, so before Sally: 24 × 2 = 48 pieces."
- New: **"You found there were 24 before Tom. Sally took half before that, leaving those 24. How many were in the bowl at the very beginning?"**

---

### WE2 — Step 4: Verify forward ✏️

✏️ **Narration gives the full forward chain and names "answer: 48 (option E)" before the MCQ:**
- Old: "Check forward: 48 → Sally takes half (24) → 24 left. 24 → Tom takes half (12) → 12 left. 12 → Clara takes half (6) → 6 left ✓ Answer: 48 (option E)."
- New: **"Check your answer by going forwards: start with your number, have Sally take half, then Tom, then Clara. Do you end up with 6? Now pick the matching answer option."**

---

## Block 5 — Practice Lab

> 🆕 **Hints added to all problems** — none of the original problems had hints. Added 2 hints per problem. All figure bare strings fixed.

---

### P1 — 1/3 of 12 🐛🆕

🐛 **`figure` bare string** → `{ "src": "..." }`

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | Split 12 into 3 equal groups. How many are in each group? |
| 2 | 12 ÷ 3 = ? |

---

### P2 — 1/4 of 24 🐛✏️

🐛 **`figure` bare string** → `{ "src": "..." }`
🐛 **Answer written in image** — the SVG shows "6" somewhere in the figure. Remove all number answers from the image. The figure should show only the bar divided into 4 groups with no labels on the group sizes.

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | Split 24 into 4 equal groups. How many are in each group? |
| 2 | 24 ÷ 4 = ? |

---

### P3 — 3/4 of 20 🆕

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | First find 1/4 of 20. Divide 20 by 4. |
| 2 | You found 1 part. You need 3 parts. Multiply your answer by 3. |

---

### P4 — 2/5 of 15 🐛✏️🆕

🐛 **`figure` bare string** → `{ "src": "..." }`
🐛 **Answer written in image** — the SVG for P4 shows the answer. Remove all number labels from the group sizes in the figure.

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | First find 1/5 of 15. Divide 15 by 5. |
| 2 | You need 2 of those equal parts. Multiply your 1 part by 2. |

---

### P5 — Reverse: 1/3 of a number = 9 ✏️🐛🆕

🐛 **`figure` bare string** → `{ "src": "..." }`
🐛 **Image subtext hints at the answer** — the figure caption or label on the bar shows "9" or "×3 = 27". Remove all answer-revealing text from the SVG.

✏️ **Question text gives away the method:**
- Old: "The bar shows 1/3 of a number = 9 (one segment is filled). What is the whole number?"
- The phrase "one segment is filled" describes the image and "1/3 = 9" directly sets up the multiplication.
- New: **"One part of this bar is filled in and equals 9. The bar has 3 equal parts. What does the whole bar equal?"**

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | The whole bar has 3 equal parts. You know 1 part = 9. |
| 2 | Multiply: 9 × 3 = ? |

---

### P6 — Reverse: 1/4 of a number = 7 🆕

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | 1/4 of the number is 7. How many quarters make a whole? |
| 2 | Multiply: 7 × 4 = ? |

---

### P7 — Reverse: 3/4 of a number = 12 🆕

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | You have 3 equal parts = 12. What is 1 part worth? Divide 12 by 3. |
| 2 | Now you know 1 part. Multiply by 4 to get the whole. |

---

### P8 — Anna's apples 🆕

🆕 **Hints added:**

| Hint | Text |
|------|------|
| 1 | Count everyone who gets apples — Anna plus her 5 friends. How many people is that? |
| 2 | Each person gets 1/2 apple. Two people together need 1 whole apple. How many whole apples for all 6 people? |

---

## Block 6 — Mastery Check

> No hints allowed.

---

### MC1 ✅

Clean question, no figure. No changes.

---

### MC2 ✏️🐛

🐛 **`figure` bare string** → `{ "src": "..." }`
🐛 **Figure likely shows group sizes** — if the SVG labels each of the 5 groups with "4", the answer (3 × 4 = 12) is visible. Remove group-size labels from the SVG.

✏️ **Question text gives away the answer:** "The bar model shows 5 equal groups totalling 20. What is 3/5 of 20?"
- Stating "5 equal groups totalling 20" means each group = 4, and 3 groups = 12 — the student just multiplies.
- New: **"The bar is split into 5 equal parts and shows the number 20 in total. What is 3/5 of 20?"**
- Remove the "5 equal groups totalling 20" preamble — the figure should communicate the groups visually.

---

### MC3 ✅

Clean fill-in-blank, no figure. No changes.

---

### MC4 ✏️🐛

🐛 **`figure` bare string** → `{ "src": "..." }`
🐛 **Figure likely labels the shaded segments with "18"** — if so, the student can read off "2 parts = 18, so 1 part = 9, whole = 27" directly from the image. Remove number labels from shaded areas.

✏️ **Question text gives away the method:**
- Old: "The bar model shows 2 of 3 equal segments shaded, totalling 18. What is the whole number?"
- "2 segments shaded, totalling 18" directly sets up ÷2 then ×3.
- New: **"The shaded part of the bar equals 18. The shaded part is 2/3 of the whole bar. What is the whole?"**

---

## Block 7 — Challenge Extension ✅

**CE1 — Adam and Bart's chestnuts** (MK 2001 Q14)

Content and hint structure are fine. No changes needed.

> 🆕 **Suggested hints** (none exist currently):

| Hint | Text |
|------|------|
| 1 | Try a simple number. Say they each start with 10 chestnuts. Adam gives Bart half of his 10. How many does each person end up with? |
| 2 | Now compare Bart's total to Adam's total. How many times bigger is Bart's? Does this change if you start with a different number? |

---

## Summary of all figure field fixes

| Block | Item | Fix |
|-------|------|-----|
| WE1 | `problem.figure` bare string | → `{ "src": "..." }` |
| WE1 Step 2 | Figure alt text names answer | Remove numbers from alt |
| WE1 Step 3 | Figure alt text names Sophie's count | Remove numbers from alt |
| WE2 | `problem.figure` bare string | → `{ "src": "..." }` |
| WE2 Step 1 | Figure alt text names 12 | Remove numbers from alt |
| WE2 Step 2 | Figure alt text names 24 | Remove numbers from alt |
| P1 | `figure` bare string | → `{ "src": "..." }` |
| P2 | `figure` bare string + answer in image | → `{ "src": "..." }` + remove label |
| P4 | `figure` bare string + answer in image | → `{ "src": "..." }` + remove label |
| P5 | `figure` bare string + answer in subtext | → `{ "src": "..." }` + remove label |
| MC2 | `figure` bare string + group labels | → `{ "src": "..." }` + remove labels |
| MC4 | `figure` bare string + segment labels | → `{ "src": "..." }` + remove labels |
