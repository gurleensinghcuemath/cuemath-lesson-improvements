# Lesson 1.3 — Multi-Step Arithmetic: Chaining Operations (Improved)

**ID:** `mk-f-multi-step-arithmetic`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved
**Skills:** Number Theory · Operations

---

## What changed and why — quick read

| Category | Count | Biggest wins |
|----------|-------|--------------|
| 🐛 Code bugs fixed | 6 | Step 4 blocked progression; MC3 NaN crash; WE2 figure invisible |
| ✏️ Answer-hints → CUEs | 12 | CF1 both hints, Step 1 hint, ALL Step 3 hints, Step 5 hint, P3/P4/P5/P6/P7 hint 2 |
| ✏️ Language simplifications | 11 | "sequence"→ plain words; ↔/≠ symbols removed; backticks removed; "pill"/"Ops:" removed |
| 🆕 New steps added | 2 | Step 3.5 (forward→backward bridge); MC3 split into MC3a + MC3b |
| ✏️ Narrative threading | 1 | Tom removed — CF2 now uses Mira (same character as CF1) |
| ✏️ Step 0 spoiler fixed | 1 | onCorrect no longer reveals 60,000 before WE2 |

---

## Block 1 — Challenge First

> Students attempt cold. Hint ladder appears after 2 minutes.

---

### CF1 — Mira's Marbles ✏️

**Type:** Fill in blank
**Question:** Mira starts with 8 marbles. She doubles them, gives away 5, then doubles again. How many marbles does Mira have now?
**Answer:** 22

✏️ **onWrong added** (was missing):
> "Good try! Write down just the first step: 8 × 2 = ___. Once you have that, write the answer in a new box and move on."

**Explanation:** 8 × 2 = 16 → 16 − 5 = 11 → 11 × 2 = 22.

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | ~~Step 1: 8 × 2 = ___. Step 2: that answer − 5 = ___. Step 3: that answer × 2 = ___.~~ → **Draw three boxes. What number goes in the first box after 8 × 2?** | ❌→✅ CUE |
| 2 | ~~Don't try to do all three in your head. Write down 16 after step 1, then 11 after step 2, then double 11 for step 3.~~ → **After step 1 you have more than 10. After step 2 you have less than 15. Can you find both?** | ❌→✅ CUE |

> 💡 **Why:** The old hints mapped out every step (Hint 1) then gave both intermediate values (Hint 2). Both were full answers, not prompts.

---

### CF2 — Mira's secret number ✏️

> ✏️ **Character changed: Tom → Mira.** Using one character across CF1 and CF2 builds a story arc. Students feel like they're following Mira's journey, not jumping between strangers.

**Type:** Fill in blank
**Question:** ✏️ ~~Tom thought of a number~~ → **Mira thought of a number. She multiplied it by 3, then added 7. She got 22. What was Mira's starting number?**
**Answer:** 5
**Explanation:** Reverse: 22 − 7 = 15 → 15 ÷ 3 = 5.

✏️ **onWrong added** (was missing):
> "To find the start, you need to walk backward. What was the LAST thing Mira did? Undo that step first."

| Hint | Text | Status |
|------|------|--------|
| 1 | What was the last thing Mira did? It was '+7.' Reverse that first: 22 − 7 = ___. | ✅ CUE |
| 2 | Now you have 15 = number × 3. Reverse the ×3 to find the number. | ✅ CUE |

---

## Block 2 — Interactive Lesson: "Walk Forward, Then Walk Back"

---

### Step 0 — Predict: "What went wrong for Angie?" ✏️

**Type:** Predict
**Question:** Angie divided some number by 10 — but she should have multiplied by 10. She got 600 instead. What was she supposed to get?
**Answer:** 60,000 *(proceed regardless)*

✏️ **onCorrect fixed** (old version revealed 60,000 before WE2 — spoiled all tension):
> ~~"You spotted it: 600 came from ÷10, so the input was 6,000. Multiply that by 10 → 60,000. Off by 100×!"~~
> → **"You're right — the mistake cost Angie far more than she expected. Let's find out exactly how much in Worked Example 2."**

✏️ **onWrong fixed** (old version didn't address the most common wrong answer: 6,000):
> ~~"Watch what Angie's mistake costs her. ÷10 and ×10 differ by a factor of 100, not 10. We'll prove it together."~~
> → **"If you got 6,000 — that's actually Angie's starting number, not her correct answer. She still needed to multiply by 10 after finding the start. Let's trace it together."**

---

### Step 1 — Explain: "One step, one box — never skip ahead" ✏️

**Title:** ✏️ ~~"One step at a time"~~ → **"One step, one box — never skip ahead"**

**Body:** ✏️ (old version used "sequence" — Grade 5+ vocabulary)
> ~~"A chain of operations is a sequence of mini-puzzles. Solve one step, write the answer, move on. Don't try to hold all four operations in your head — write the running total at every stop."~~
> → **"A chain is like a row of boxes. Solve the first puzzle, write the answer in the box. Then use that answer for the next box. Never try to hold two steps in your head at once."**

**Visual:** Chain-flow: 4 → +5 → 9 → ×3 → 27 → −2 → 25

**Key Insight:** Write the running value at every stop. Never combine steps in your head.

✏️ **endQuestion prompt** (removed backticks — render as literal characters):
> ~~"If we start with 6 instead and do the same `+5, ×3, −2` chain, what's the result?"~~
> → **"Start with 6. Do the same chain: add 5, then multiply by 3, then subtract 2. What is the final answer?"**
> **Answer: 31**

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | ~~6+5=11, 11×3=33, 33−2=?~~ → **After the first step (+5), your new number is more than 10. What is it? Write it down, then move to the next step.** | ❌→✅ CUE |

---

### Step 2 — Apply: "Try the chain on a new number" ✏️

**Title:** ✏️ ~~"Trace the chain"~~ → **"Try the chain on a new number"**

**Body:** ✏️ (removed "pill" — design jargon; removed "Ops:" abbreviation; added story frame)
> ~~"Fill in each pill as you go. Start = 10. Ops: −4, ×2, +1."~~
> → **"Let's try a new chain. Start at 10. First: subtract 4. Then: multiply by 2. Then: add 1. Fill in each step."**

**Visual:** Chain-flow: 10 → −4 → [ ] → ×2 → [ ] → +1 → [ ]

| Substep | ✏️ Improved Prompt | Answer | ✏️ Improved Hint | Status |
|---------|-------------------|--------|-------------------|--------|
| 1 | 10 − 4 = ___ | 6 | ~~"10 − 4 = ?"~~ → **You're at your first stop. What is 10 take away 4?** | ❌→✅ CUE |
| 2 | ✏️ ~~"(previous) × 2"~~ → **6 × 2 = ___** | 12 | ~~"6 × 2 = ?"~~ → **You just wrote 6. Now double it.** | ❌→✅ CUE |
| 3 | ✏️ ~~"(previous) + 1"~~ → **12 + 1 = ___** | 13 | ~~"12 + 1 = ?"~~ → **One more step to the finish. What is 12 and 1 more?** | ❌→✅ CUE |

> ✏️ **"(previous)" removed** — after a student answers correctly, the next prompt should show the ACTUAL number, not the word "(previous)". This is abstract and confusing for Grade 3-4.

✏️ **onAllCorrect:** ~~"Chain works one step at a time. Now make it harder — the first step has a carrying trap."~~ → **"Perfect chain! You wrote each answer and used it in the next step — that's exactly the right habit. Now let's try one with a hidden trap."**

---

### Step 3 — Apply: "Watch the ones column!" ✏️

**Title:** ✏️ ~~"Add a carrying trap"~~ → **"Watch the ones column!"**

**Body:** ✏️ (removed pre-warning — telling students where they'll slip removes the discovery)
> ~~"Start = 18. Ops: +47, −9, ×2. Watch the first step — adding 47 to 18 is where most students slip."~~
> → **"New chain. Start at 18. Add 47. Then subtract 9. Then multiply by 2. Take it one box at a time."**

| Substep | ✏️ Improved Prompt | Answer | ✏️ Improved Hint | Status |
|---------|-------------------|--------|-------------------|--------|
| 1 | 18 + 47 = ___ | 65 | ~~"Ones column: 8 + 7 = 15. Write 5, carry 1. Tens: 1 + 1 + 4 = 6. Result is 65 (not 55)."~~ → **Add the ones column first: 8 + 7. Do you get more than 9? If yes, write the ones digit and carry 1 to the tens.** | ❌→✅ CUE |
| 2 | ✏️ **65 − 9 = ___** | 56 | ~~"65 − 9 = 56."~~ → **Count back 9 steps from 65. What do you land on?** | ❌→✅ CUE |
| 3 | ✏️ **56 × 2 = ___** | 112 | ~~"56 × 2 = 112."~~ → **Double 56. Try: double 50, then double 6, then add both together.** | ❌→✅ CUE |

✏️ **onWrong for substep 1 added** (55 is the most common wrong answer — needs targeted feedback):
> **"If you got 55, check the ones column again. 8 + 7 doesn't fit in one digit — what do you do with the extra?"**

✏️ **onAllCorrect:** ~~"Carry caught. The carry on step 1 is the slip-zone. Get that right and the rest follows."~~ → **"You caught the carry! That ones-column trap catches a lot of students. Now you know where to look."**

---

### 🆕 Step 3.5 — Predict: "You know the end. Can you find the start?" [NEW STEP]

> **Why this step exists:** Steps 0–3 are all forward chains. Step 5 introduces backward chains. Without a bridge, the shift feels sudden. This predict step recalls CF2 (which students already struggled with) and builds natural motivation for the backward method. It makes students *want* the rule before it's given.

**Type:** Predict (proceed regardless)
**Title:** "You know the answer — but not the start"
**Body:** "Mira ran a chain: she multiplied her number by 3, then added 7. She ended up with 22. You saw this earlier! Can you find what Mira started with?"

**Answer:** 5 *(proceed regardless)*

**onCorrect:** "You got it — Mira started with 5! You just ran a chain backward. Now let's learn the rule so you can do this on ANY chain."

**onWrong:** "Let's figure it out together. The trick is to undo each step — but you have to start from the LAST step, not the first. Let's see why."

---

### Step 4 — Apply: "Order changes the answer" ✏️

**Body:** "Start = 5. You have two operations: ×2 and +6. Which order gives the bigger final number?"

**Visual:** Two parallel chains — 5 → ×2 → 10 → +6 → 16 vs 5 → +6 → 11 → ×2 → 22

> 🐛 **CODE BUG FIXED:** Old `endQuestion` had `"inputType": "choice"` but no `"type": "mcq"`. The CMS question router dispatches on `"type"`. Without it, no renderer is found — the step stops and students can't proceed.
> Fix: Add `"type": "mcq"` to the endQuestion.

**endQuestion (MCQ):**
- (A) Doing ×2 first → 16
- **(B) Doing +6 first → 22** ✓
- (C) The order doesn't matter

✏️ **onWrong for option C added** (most common wrong answer — needs targeted feedback):
> **"If the order didn't matter, both paths would give the same answer. But look at the two chains — do they end at the same number?"**

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | ~~"Compute both. ×2 first: 5→10→16. +6 first: 5→11→22."~~ → **When you multiply first, the +6 gets added to a small number. When you add first, ×2 stretches a bigger number. Try both paths and compare.** | ❌→✅ CUE |

---

### Step 5 — Explain: "To find the start, flip and go backward" ✏️

**Title:** ✏️ ~~"Walk it back: undo the last step first"~~ → **"To find the start, flip and go backward"**

**Body:** ✏️ (replaced ↔ symbol — not Grade 3-4 vocabulary)
> ~~"When you know the result but need the start, walk the chain backward. Two rules: reverse the last operation first, and each operation gets flipped: + ↔ −, × ↔ ÷."~~
> → **"When you know the answer but need the start, walk backward. Two rules to remember:**
> **Rule 1: Undo the LAST step first.**
> **Rule 2: Every operation gets flipped.**
>
> | Forward | Backward |
> |---------|----------|
> | + | becomes − |
> | − | becomes + |
> | × | becomes ÷ |
> | ÷ | becomes × |"

**Visual:** Two rows — forward (start → ×3 → +7 → 22) and backward (5 ← ÷3 ← −7 ← 22)

**Key Insight:** Reverse the LAST step first. Each operation flips to its opposite.

**endQuestion:** "A number had ×4 done to it, then −5. The result is 23. What was the starting number?"
**Answer: 7**

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | ~~"Reverse −5 first: 23 + 5 = 28. Reverse ×4: 28 ÷ 4 = ?"~~ → **What was the very last step done to the number? Use Rule 1: undo THAT one first.** | ❌→✅ CUE |

---

### Step 6 — Apply: "Find the starting number" ✏️

**Body:** "A number had −2, then +3, then ×5 done to it. The result was 40. Find the starting number."

**Visual:** Chain flowing backward from 40.

| Substep | ✏️ Improved Prompt | Answer | Hint | Status |
|---------|-------------------|--------|------|--------|
| 1 | Reverse ×5: 40 ÷ 5 = ___ | 8 | 40 ÷ 5 = ? | ✅ CUE |
| 2 | ✏️ ~~"Reverse +3: (previous) − 3 = ___"~~ → **Reverse +3: 8 − 3 = ___** | 5 | 8 − 3 = ? | ✅ CUE |
| 3 | ✏️ ~~"Reverse −2: (previous) + 2 = ___ (this is the start)"~~ → **Reverse −2: 5 + 2 = ___ (this is your starting number)** | 7 | 5 + 2 = ? | ✅ CUE |

✏️ **onAllCorrect elevated to keyInsight** (was buried as a throwaway sentence):
> ~~"Start = 7. Reversing the chain reverses the order of operations too."~~
> → 🔑 **Key Insight: "Start = 7. When you reverse a chain, you also reverse the ORDER of the steps. The last step forward becomes the FIRST step backward."**

---

### Step 7 — Apply: "Don't undo with the wrong inverse" ✅ (minimal changes)

> ✅ **Best-designed step in the lesson.** The Aria vs Bilal character debate is excellent pedagogy. The callback to Angie from Step 0 is strong narrative continuity. Keeping this almost entirely as-is.

**Body:** "A number had ÷10 done to it. The result is 6,000. Aria says: 'reverse ÷10 with ×10. Start = 6,000 × 10 = 60,000.' Bilal says: 'reverse ÷10 with ÷10. Start = 6,000 ÷ 10 = 600.' Who is right?"

**endQuestion (MCQ):**
- **(A) Aria — start was 60,000** ✓
- (B) Bilal — start was 600
- (C) Both are right depending on the chain

| Hint | Text | Status |
|------|------|--------|
| 1 | ÷10 reverses to ×10, not ÷10. Bilal made Angie's mistake from Step 0. | ✅ CUE (great callback) |

---

### Step 8 — Reveal ✏️

| Rule | ✏️ Improved Statement | Example |
|------|----------------------|---------|
| Forward | Do each step in order. Write the running value at every stop. | 8 → ×2 → 16 → +5 → 21 → ×2 → 42 |
| Backward (undo) | Reverse the LAST step first. Flip each op to its opposite. | Result 22, steps were ×3 then +7 → 22−7=15 → 15÷3=5 |
| Common traps | ✏️ ~~"+6 then ×2 ≠ ×2 then +6"~~ → **Carry trap (18+47=65, not 55). Wrong flip (÷10 reverses to ×10, not ÷10). Different order gives a different answer.** | — |

> ✏️ **≠ symbol removed** — not Grade 3-4 vocabulary. Replaced with plain description.

✏️ **Closing Checkpoint (match_pairs)** — removed algebraic variables X and Y:
> ~~"Start with X, apply ops, find result"~~
> ~~"Result is Y, find start"~~
> → **"You know the start — find the result"** → Forward — go in order
> → **"You know the result — find the start"** → Backward — reverse the last step first

✏️ **Curiosity Bridge** — removed "eliminate" (adult vocabulary):
> ~~"Lesson 1.4 introduces a faster move: eliminate wrong answers BEFORE you compute."~~
> → **"Lesson 1.4 teaches a faster move: rule out wrong answers BEFORE you compute. Here's a taste: Can 5 odd numbers add up to 50? Type yes or no."**
> **Answer: no**
> **Reveal:** "No — every odd number ends in 1, 3, 5, 7, or 9. Add five of them and the result is always odd. But 50 is even, so it's impossible. That's the kind of shortcut Lesson 1.4 is all about."

---

## Block 3 — Worked Example 1 (MK 2013 Q06) ⭐ 3pt

> 🔔 **Note on alignment:** This problem is about divisibility — not directly about chaining operations. However, the DISCIPLINE is the same: test every option, one by one, write down what you find. The bridge framing below makes this connection explicit.

✏️ **Bridge framing added** (connects WE1 to the lesson habit):
> "You've been tracing chains step by step without skipping. Now apply that same discipline to a multiple-choice problem: test each option, one by one, and write what you find."

**Problem:** Daniel had 36 pieces of candy. He divided them equally among his friends. Which of the following was definitely NOT the number of his friends?
**Options:** (A) 2 / (B) 3 / (C) 4 / (D) **5** ✓ / (E) 6

---

### WE1 Step 1 — Read the rule ✏️

**Narration:** ✏️ (simplified language)
> ~~"Daniel divided 36 candies equally — so the number of friends must divide 36 with no remainder. The question asks which number CANNOT be the friend-count."~~
> → **"Daniel split 36 candies so every friend got the same amount. That means 36 must divide evenly — no leftovers. The question asks which number of friends makes that IMPOSSIBLE."**

**Checkpoint (MCQ):** If 36 ÷ N has a remainder, then N is NOT a possible number of friends. True or false?
- **(A) True** ✓
- (B) False

**Hint:** If candies don't divide evenly, some friends get more than others — not a fair share.
**Explanation:** Equal sharing means zero remainder. Any number that leaves a remainder is impossible.

---

### WE1 Step 2 — Test each option ✏️

**Narration:** ✏️
> ~~"Don't guess. Compute each division. Write the quotient and any remainder."~~
> → **"Don't guess — test each one. Compute the division. If it comes out perfectly, the option works. If there's a leftover, the option is impossible."**

**Checkpoint (sort_order):** Drag each division to the correct bucket.

| Division | Correct Bucket |
|----------|---------------|
| 36 ÷ 2 | Divides evenly |
| 36 ÷ 3 | Divides evenly |
| 36 ÷ 4 | Divides evenly |
| 36 ÷ 5 | Has a remainder |
| 36 ÷ 6 | Divides evenly |

**Hint:** Compute each one. Mark the division that doesn't come out as a whole number.
**Explanation:** 36 ÷ 2 = 18, ÷3 = 12, ÷4 = 9, ÷6 = 6 — all exact. 36 ÷ 5 = 7 with 1 left over.

---

### WE1 Step 3 — Compute 36 ÷ 5 ✏️

> 🐛 **CODE BUG FIXED:** Old `"answers": [7, 1]` is a plural array. The CMS `fill_in_blank` renderer reads `question.answer` (singular). Accessing `.answer` on an object that only has `.answers` returns `undefined`, which displays as **NaN**. Fix: split into two separate checkpoint questions.

**Narration:** "Only one division has a remainder: 36 ÷ 5. Let's confirm exactly what the remainder is."

**Checkpoint A:** 36 ÷ 5 = ___
**Answer:** 7
**Hint:** How many times does 5 fit into 36? Think: 5 × 7 = 35.

**Checkpoint B:** How many are left over? ___
**Answer:** 1
**Hint:** 5 × 7 = 35. How far is 35 from 36?

**Explanation:** 5 fits into 36 seven times (5 × 7 = 35), with 1 piece left over. That leftover means 5 friends is impossible.

---

### WE1 Step 4 — Pick the answer ✏️

**Narration:** "The answer is whichever option does NOT divide 36. That's 5."

**Checkpoint (MCQ):** Which is the correct answer?
- (A) 2 / (B) 3 / (C) 4 / **(D) 5** ✓ / (E) 6

**Hint:** The only one with a leftover is the impossible friend-count.
**Explanation:** 5 is the only option that doesn't divide 36 evenly. Answer: D.

✏️ **Insight rewritten** (connected back to lesson discipline):
> ~~"Work through every option systematically — don't skip."~~
> → **"The same habit as tracing a chain: do each step, write the answer, don't skip. When one option leaves a remainder, you've found your answer."**

---

## Block 4 — Worked Example 2 (MK 2004 Q13) ⭐⭐ 4pt

> ✏️ **Bridge framing added:** "This is Angie's problem from Step 0. You already predicted an answer. Now let's prove it — step by step."

**Problem:** Angie divided a certain number by 10 instead of multiplying by 10. She got 600. What would the result have been if she hadn't made this mistake?
**Options:** (A) 6 / (B) 60 / (C) 600 / (D) 6,000 / **(E) 60,000** ✓

> 🐛 **CODE BUG FIXED:** `"figure": "/figures/..."` is a bare string. The CMS renderer reads `figure.src`. A bare string has no `.src` property, so the figure is invisible when the problem appears.
> Fix: Change to `"figure": { "src": "/figures/mk-grade-3-4/lesson-1-3/MK_L13_WE2_angie_two_paths.svg" }`

---

### WE2 Step 1 — Find the original number

**Narration:** "Angie did ÷10 to a number and got 600. To find the original number, reverse ÷10 — multiply by 10."

**Checkpoint:** Original number = 600 × ___ = ___
**Answers:** 10 and 6,000

> 🐛 **CODE BUG NOTE:** This also uses `"answers": [10, 6000]` array format. Same NaN bug as WE1 Step 3. Fix: split into two checkpoints.
> Checkpoint A: "600 × ___ gives back the original number." → Answer: 10
> Checkpoint B: "600 × 10 = ___" → Answer: 6,000

**Hint:** ÷10 reverses to ×10. So take 600 and multiply it by 10.
**Explanation:** To undo ÷10, multiply by 10. 600 × 10 = 6,000.

---

### WE2 Step 2 — Find the intended operation

**Narration:** "Angie's starting number was 6,000. Now what was she SUPPOSED to do to it?"

**Checkpoint (MCQ):** Angie meant to…
- (A) ÷10
- **(B) ×10** ✓
- (C) +10
- (D) −10

**Hint:** Read the question again: "instead of multiplying it by 10."
**Explanation:** She was supposed to multiply by 10. She divided instead.

---

### WE2 Step 3 — Apply the correct operation

**Checkpoint:** 6,000 × 10 = ___
**Answer:** 60,000

**Hint:** Multiplying by 10 adds one zero to the right. What does 6,000 become?
**Explanation:** 6,000 × 10 = 60,000.

---

### WE2 Step 4 — Why 6,000 is the trap

**Narration:** "Some students compute 600 × 10 = 6,000 and stop. But 6,000 is the ORIGINAL number, not the correct result."

**Checkpoint (MCQ):** What does 600 × 10 = 6,000 represent?
- **(A) The original number Angie started with** ✓
- (B) The result Angie should have got
- (C) Angie's actual answer

**Hint:** 600 was Angie's wrong result after she did ÷10. Multiplying it by 10 gets you back to where she started — not to where she should have ended.
**Explanation:** 6,000 is the original input. The correct result is one more ×10: 60,000.

---

### WE2 Step 5 — Why the gap is 100×, not 10× ✏️

> ✏️ **Redesigned.** The original question (60,000 ÷ 600 = ?) is too hard for mental calculation at Grade 3-4. The hint gave a technique ("divide both by 100") that hasn't been taught. Reframed as a comparison question — same insight, more accessible.

**Narration:** ✏️
> ~~"The answer is 60,000 — exactly 100× Angie's wrong result. ÷10 and ×10 differ by a factor of 100, not 10."~~
> → **"Angie got 600. The right answer is 60,000. That's not just 10 times bigger — it's 100 times bigger. Why? Because she needed TWO steps of ×10: one to undo her mistake, and one to do the right thing."**

**Checkpoint:** ✏️
> ~~"60,000 ÷ 600 = ___"~~ → **"How many times bigger is 60,000 than 600?"**
> **Answer:** 100

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | ~~"Divide both by 100 mentally: 600 → 6, 60,000 → 600. 600 ÷ 6 = 100."~~ → **Count the zeros: 600 has 2 zeros. 60,000 has 4 zeros. How many more zeros does 60,000 have? Each extra zero means ×10.** | ❌→✅ CUE |

**Insight:** Two factors of 10 separate Angie's wrong result from the correct one — one ×10 to undo the mistake, plus one more ×10 to do the right thing.

---

## Block 5 — Practice Lab

---

### P1 ✏️

✏️ **Story context added** (was "pure notation" — no context):
> ~~"Start = 12. Ops: +8, ÷4, ×3. What is the result?"~~
> → **"Priya starts with 12 stickers. She gets 8 more. Then she splits all of them equally into 4 groups. Then every sticker in each group gets tripled. How many stickers are in one group now?"**
> **Answer:** 15

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | Step 1: 12 + 8 = ___. | ✅ CUE |
| 2 | ~~"Then divide that by 4. Then multiply by 3."~~ → **After step 1 you have 20. Can you take the next two steps?** | ❌→✅ CUE |

**Explanation:** 12 + 8 = 20. 20 ÷ 4 = 5. 5 × 3 = 15.

---

### P2 ✅ (already well-designed — minimal changes)

**Question:** During a party each of two identical cakes was divided into four equal pieces. Then each piece was divided into three equal pieces. Each person got one piece and three pieces were left over. How many people were at the party?
**Options:** (A) 13 / (B) 18 / **(C) 21** ✓ / (D) 24 / (E) 27

| Hint | Text | Status |
|------|------|--------|
| 1 | Compute total sub-pieces: 2 × 4 × 3. | ✅ CUE |
| 2 | Subtract the 3 leftover pieces from the total. | ✅ CUE |

**Explanation:** 2 cakes × 4 = 8 pieces. 8 × 3 = 24 sub-pieces. 24 − 3 = 21 people.

---

### P3 ✏️

**Question:** Each of the kangaroo's eleven children has eleven children. Each of THOSE also has eleven children. How many great-grandchildren does the kangaroo have?
**Options:** (A) 111 / (B) 121 / (C) 11211 / **(D) 1331** ✓ / (E) 12321

> 💡 **Framing note:** This is a chain of multiplications: 11 × 11 × 11. Three generations, each branching 11 ways. A tree diagram visual would help — kangaroo → 11 children → 121 grandchildren → 1331 great-grandchildren.

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | Three generations of 11. Compute 11 × 11 × 11. | ✅ CUE |
| 2 | ~~"11 × 11 = 121. Then 121 × 11."~~ → **11 × 11 gives you the number of grandchildren. Now do that one more time with 11 to get great-grandchildren.** | ❌→✅ CUE |

**Explanation:** 11 × 11 = 121. 121 × 11 = 1,331.

---

### P4 ✏️

**Question:** In the animal school, 3 kittens, 4 ducklings, 2 baby geese, and several lambs are taking lessons. All pupils have 44 legs altogether. How many lambs are there?
**Options:** **(A) 6 / (B) 5** ✓ / (C) 4 / (D) 3 / (E) 2

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | Add up the known legs first: 3 kittens, 4 ducklings, 2 geese. Then subtract from 44. | ✅ CUE |
| 2 | ~~"Kittens 3×4=12. Ducklings 4×2=8. Geese 2×2=4. Total=24. Lambs=(44−24)÷4."~~ → **You found the total known legs. Now: how many legs are left for the lambs? Each lamb has 4 legs. How many lambs fit?** | ❌→✅ CUE |

**Explanation:** Kittens: 3 × 4 = 12. Ducklings: 4 × 2 = 8. Geese: 2 × 2 = 4. Total = 24. Remaining for lambs: 44 − 24 = 20. Lambs: 20 ÷ 4 = 5.

---

### P5 ✏️

✏️ **Story context added**:
> ~~"Start = 26. Ops: +57, −18, ÷5. What is the result?"~~
> → **"Riya starts at 26 on a number line. She jumps forward 57. Then she steps back 18. Then she divides her position into 5 equal parts and takes one. Where does she end up?"**
> **Answer:** 13

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | Watch the first jump's carry: 26 + 57. Ones column: 6 + 7. What do you write and what do you carry? | ✅ CUE |
| 2 | ~~"After step 1 you have 83. Then 83 − 18 = ___, then ÷5 = ___."~~ → **After the first step you pass 80. What exact number do you reach? Then take the next two steps.** | ❌→✅ CUE |

**Explanation:** 26 + 57 = 83 (carry from ones). 83 − 18 = 65. 65 ÷ 5 = 13.

---

### P6 ✏️

**Question:** After applying −4, then ×3, then +1 (in that order) to a starting number, the result is 25. What was the starting number?
**Answer:** 12

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | The last forward step was +1. Reverse it first: 25 − 1 = ___. | ✅ CUE |
| 2 | ~~"Now you have 24 = (start − 4) × 3. Reverse the ×3, then reverse the −4."~~ → **After reversing +1, you have 24. Now look at the step that came just before +1. What do you need to reverse next?** | ❌→✅ CUE (algebra removed) |

**Explanation:** Reverse: 25 − 1 = 24. 24 ÷ 3 = 8. 8 + 4 = 12. Check: 12 − 4 = 8, 8 × 3 = 24, 24 + 1 = 25 ✓

---

### P7 ✏️

**Question:** Start = 4. The two operations are ×3 and +5. Which order gives the bigger final result?
- (A) ×3 first → 17
- **(B) +5 first → 27** ✓

> 🐛 **CODE BUG FLAG:** `optionFigures` references SVG files at `MK_L13_P7_optA_chain.svg` and `MK_L13_P7_optB_chain.svg`. If these files don't exist, both options render as broken image placeholders. Remove `optionFigures` and `figuresInOptions: true` until the SVGs are confirmed to exist.

| Hint | ✏️ Improved Text | Status |
|------|-----------------|--------|
| 1 | Compute both orderings. Don't guess. | ✅ CUE |
| 2 | ~~"×3 then +5: 4→12→17. +5 then ×3: 4→9→27."~~ → **When you multiply first, +5 is added to a small number. When you add first, ×3 stretches a bigger number. Which gives more?** | ❌→✅ CUE |

**Explanation:** ×3 then +5: 4 → 12 → 17. +5 then ×3: 4 → 9 → 27. Adding first wins.

---

### P8 ✅ + ✏️ (good question, bonus insight elevated)

**Question:** A frog starts at 0 on a number line. It hops +7, +7, −5, +7, −5, −5. Where does it land?
**Answer:** 6

| Hint | Text | Status |
|------|------|--------|
| 1 | Track each hop. Hop 1: 0 + 7 = 7. Hop 2: ___. | ✅ CUE |
| 2 | Six hops total. Add up: 7 + 7 − 5 + 7 − 5 − 5 = ___. | ✅ CUE |

**Explanation:** 0 → 7 → 14 → 9 → 16 → 11 → 6.

✏️ **Bonus insight elevated to featured callout** (was buried in footnote):
> 🔑 **Shortcut:** Group the same hops together: (7 + 7 + 7) + (−5 − 5 − 5) = 21 − 15 = 6. When hops repeat, grouping saves time!

---

## Block 6 — Mastery Check ✏️

> No hints. Pass 2/3 to unlock Lesson 1.4.

---

### MC1 ✏️

> ✏️ Story context added. "Ops:" notation removed.

**Question:** ✏️
> ~~"Start = 9. Ops: ×4, −6, ÷6. What is the result?"~~
> → **"Liam starts with 9 coins. He earns 4 times as many. Then he loses 6. Then he shares them equally among 6 friends. How many coins does each friend get?"**
> **Answer:** 5

**Explanation:** 9 × 4 = 36. 36 − 6 = 30. 30 ÷ 6 = 5.

---

### MC2 ✏️

> ✏️ Story context added. "Ops:" notation removed.

**Question:** ✏️
> ~~"After applying ops +8, ÷5, −1 in that order, the result is 4. What was the starting number?"~~
> → **"A machine adds 8, then divides by 5, then subtracts 1. The output is 4. What number went into the machine?"**
> **Options:** (A) 11 / (B) 13 / **(C) 17** ✓ / (D) 25 / (E) 33

**Explanation:** Reverse −1: 4 + 1 = 5. Reverse ÷5: 5 × 5 = 25. Reverse +8: 25 − 8 = 17.

---

### MC3 ✏️ [SPLIT INTO TWO QUESTIONS]

> 🐛 **THREE CODE BUGS FIXED:**
> 1. Backtick formatting in prompt (`` `start → ×3 → +12 → result` ``) — renders as literal characters
> 2. `"answers": [24, 6]` array format — renderer reads `answer` singular, returns NaN
> 3. "Type two answers separated by a comma, like 'a,b'" — ambiguous and confusing for Grade 3-4
>
> Fix: Split into two separate, clearly labelled fill_in_blank questions.

**MC3a — Forward chain:**
> **"Aman starts at 4. He multiplies by 3, then adds 12. What does Aman get?"**
> **Answer:** 24
> **Explanation:** 4 × 3 = 12. 12 + 12 = 24.

**MC3b — Backward chain:**
> **"Beena uses the same chain (multiply by 3, then add 12) and ends at 30. What did Beena start with?"**
> **Answer:** 6
> **Explanation:** Reverse: 30 − 12 = 18. 18 ÷ 3 = 6.

---

## Block 7 — Challenge Extension ✏️

> ✏️ **×N algebraic variable removed** (CCSS 6.EE.A.2 — Grade 6 scope). Redesigned as trial-and-check using the chain-tracing skill from this very lesson.
> ✏️ **All 3 hints redesigned** — old hints used full algebraic equations and gave the answer. New hints guide trial-and-check.

**Problem:** ✏️
> ~~"Asha builds a chain of three operations: ×N, +5, −7, applied in that order."~~
> → **"Asha has a mystery chain: multiply by a secret number, then add 5, then subtract 7. When she starts with 2, she gets 16. When she starts with 5, what does she get?"**
> **Answer:** 43

| Hint | ✏️ Improved Text (trial-and-check) | Status |
|------|-----------------------------------|--------|
| 1 | ~~"From the first run, find N. Set up: (2 × N) + 5 − 7 = 16. Solve."~~ → **Use the first run to find the secret number. Try: if the secret number is 5, what does 2 → ×5 → +5 → −7 give you? Too small? Try a bigger secret number.** | ❌→✅ CUE |
| 2 | ~~"2N − 2 = 16, so 2N = 18, so N = 9."~~ → **The secret number is somewhere between 7 and 12. Try each one with start = 2 until you hit 16.** | ❌→✅ CUE |
| 3 | ~~"Now plug N = 9 into the second run with start = 5. Result = (5 × 9) + 5 − 7."~~ → **Once you know the secret number, run the chain one more time — but now start with 5 instead of 2.** | ❌→✅ CUE |

**Explanation:** ✏️
> ~~"From the first run: (2 × N) + 5 − 7 = 16 → 2N − 2 = 16 → 2N = 18 → N = 9."~~
> → **Trial and check with start = 2: try multiplier = 7: 2×7=14, +5=19, −7=12. Too small. Try 8: 2×8=16, +5=21, −7=14. Still small. Try 9: 2×9=18, +5=23, −7=16. That's it! Secret number = 9. Now apply: 5×9=45, +5=50, −7=43.**

---

## Summary Tables

### 🐛 Code Bugs Fixed (6 total)

| Location | Bug | Fix |
|----------|-----|-----|
| IL Step 4 endQuestion | `"inputType": "choice"` with no `"type": "mcq"` — step blocks progression | Add `"type": "mcq"` |
| WE1 Step 3 checkpoint | `"answers": [7, 1]` array — renderer reads `.answer` singular → NaN | Split into two separate checkpoint questions |
| WE2 problem | `"figure": "..."` bare string — renderer reads `.src` → figure invisible | Change to `"figure": { "src": "..." }` |
| WE2 Step 1 checkpoint | `"answers": [10, 6000]` array — same NaN bug | Split into two separate checkpoint questions |
| MC3 | Backtick formatting + `"answers": [24, 6]` array + comma-separated input | Split into MC3a + MC3b, each single fill_in_blank |
| P7 optionFigures | SVG files may not exist — renders as broken image placeholders | Remove `optionFigures` and `figuresInOptions: true` until SVGs confirmed |

---

### 🆕 New Steps Added (2 total)

| Step | Title | Why added |
|------|-------|-----------|
| Step 3.5 | "You know the answer — but not the start" | Bridges forward (Steps 0–4) and backward (Steps 5–7). Recalls CF2 to create natural motivation for Step 5's explanation. |
| MC3 split → MC3a + MC3b | Forward and backward in separate questions | Fixes three code bugs. Removes comma-separated input confusion. Clearer for Grade 3-4. |

---

### ✏️ Answer-Hints → CUEs (12 total)

| Location | Old (answer) | New (CUE) |
|----------|-------------|----------|
| CF1 Hint 1 | Maps out all 3 steps with blanks | "Draw three boxes. What number goes in the first box?" |
| CF1 Hint 2 | Gives intermediate values 16 and 11 | "After step 1 you have more than 10. After step 2 less than 15." |
| IL Step 1 Hint | Gives 11 and 33 | "After +5, your number is more than 10. What is it?" |
| IL Step 3 Hint 1 | Full carry walkthrough + result 65 | "Add ones column first. Do you get more than 9?" |
| IL Step 3 Hint 2 | "65 − 9 = 56" (literal answer) | "Count back 9 from 65. Where do you land?" |
| IL Step 3 Hint 3 | "56 × 2 = 112" (literal answer) | "Double 56: double 50, double 6, then add." |
| IL Step 4 Hint | Both complete computations | "When you add first, ×3 stretches a bigger number. Try both." |
| IL Step 5 Hint | Gives intermediate value 28 | "What was the very last step? Undo THAT one first." |
| P3 Hint 2 | Gives intermediate value 121 | "11×11 gives grandchildren. Do that again with 11." |
| P4 Hint 2 | Complete solution with ÷ | "How many legs left for lambs? Each has 4 — how many fit?" |
| P5 Hint 2 | Gives intermediate value 83 | "After the first step you pass 80. What exact number?" |
| P6 Hint 2 | Algebraic notation (Grade 6) | "After reversing +1, you have 24. What step comes before it?" |
| P7 Hint 2 | Both full computations | "Adding first stretches a bigger number. Which gives more?" |

---

### ✏️ Language + Design Fixes

| Location | Issue | Fix |
|----------|-------|-----|
| IL Step 1 body | "sequence" — Grade 5+ vocab | → "a row of boxes" |
| IL Step 1 endQ | Backtick formatting | Removed, wrote out plain text |
| IL Step 2 body | "pill" (design jargon) / "Ops:" abbreviation | → "step" / write out operations in full |
| IL Step 2 substeps | "(previous)" placeholder — abstract | → Show actual number after each correct answer |
| IL Step 3 body | Pre-warns where students slip | Removed — let onWrong handle it |
| IL Step 3 substeps | "(previous)" placeholder | → Show actual number |
| IL Step 5 body | ↔ symbol — not Grade 3-4 | → Simple 4-row flip table |
| IL Step 6 substeps | "(previous)" placeholder | → Show actual number |
| IL Step 8 Common Traps | ≠ symbol | → "gives a different answer than" |
| IL Step 8 match_pairs | "Start with X" / "Result is Y" — algebraic | → Plain language ("you know the start" / "you know the result") |
| IL Step 8 curiosity | "eliminate" — adult vocab | → "rule out" |
| MC3 prompt | Backtick formatting | → Plain text |
| CE1 problem | ×N algebraic variable (Grade 6) | → "secret number" / trial-and-check |

---

### ✏️ Character / Narrative Thread

| Change | Reason |
|--------|--------|
| CF2: Tom → Mira | CF1 and CF2 both star Mira. Students follow one character's story across both challenges. |
| Step 3.5: Recalls Mira from CF2 | Creates emotional continuity before introducing backward chains. |
| WE2 bridge: links to Step 0 Angie | Students already predicted the answer. WE2 becomes confirmation, not a cold problem. |
| P8 shortcut featured as callout | Most interesting insight in the whole practice block — was buried in footnote. |
