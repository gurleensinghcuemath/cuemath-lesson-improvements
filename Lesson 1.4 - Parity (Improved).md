# Lesson 1.4 — Parity: Odd/Even to Cross Out Answers (Improved)

**ID:** `mk-f-parity-odd-even`
**Difficulty:** 3pt–4pt | **Time:** 25 min | **Status:** Improved
**Skills:** Number Theory · Parity

> ✏️ marks every content change. 🐛 marks critical code/schema bug fixes. 🆕 marks new additions.

---

## What changed and why — quick read

| Category | Count | Biggest wins |
|----------|-------|--------------|
| 🐛 Code bugs fixed | 8 | `cloze_drag`→`sort_order` (Steps 4, 6, 7); string-answer `fill_in_blank`→`mcq` (P2, MC1 — NaN crash); `mcq_multi`→`mcq` (WE2 Step 1); letter-expression `fill_in_blank`→`mcq` (WE1 Step 1); `problem.figure` bare strings throughout |
| ✏️ Answer-hints → CUEs | 11 | CF1 hint 2; CF2 hints 1–2; WE1 Steps 1–4 hints; WE2 Steps 2 and 4; CE1 hints 2–3; P8 hint 2 |
| ✏️ Language simplified | 12 | "sanity check" removed; ⇔/iff removed; ÷ symbol → "divided by"; curly braces removed; "eliminate"→"cross out"; "maximise"→plain words; mod-3 notation removed; "triples"→"groups of three" |
| ✏️ Content fixes | 7 | WE2 Step 4 no longer reveals answer before checkpoint; clearer bucket labels (Steps 3, 7); Step 0 onWrong simplified; 2-option MCQs capped at 1 attempt; WE1 insight simplified; P7/P3 asset bugs flagged |
| 🎥 Video production notes | 3 | Deformed kangaroo art; AI-sounding audio; mid-sentence scene cuts |

---

## 🎥 Video Notes — "The Pairing Story" (Block 2, Step 0b)

These are production/asset issues — flagged for the video team. The narration scripts are solid; only the delivery and visuals need fixing.

1. **Kangaroo visuals:** Current assets show deformed kangaroos with only one eye. Replace with corrected character art.
2. **Narration audio:** Voice is noticeably AI-generated. Record with a human voice or a higher-quality TTS model with natural prosody.
3. **Scene cuts:** Video cuts mid-sentence instead of completing a thought before switching. Each scene should finish its narration before transitioning.

---

## Block 1 — Challenge First

> Students attempt cold. Hint ladder unlocks after 2 minutes.

---

### CF1 — Anna's five odd numbers

**Type:** MCQ
**Question:** Anna writes down 5 different odd numbers. She adds them up. Can the sum be exactly 50?
**Options:** (A) Yes — many ways. (B) Yes — but only with very large odd numbers. **(C) No — the sum of 5 odd numbers is always odd. ✓** (D) Only if she allows zero.
**Answer:** C (index 2)
**Explanation:** odd + odd = even; even + odd = odd. Each odd added flips parity. After 5 odds the total is odd. 50 is even — impossible.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | What is odd + odd? Now what is (odd + odd) + odd? Track the parity as you add. | *No change — already a good CUE.* | ✅ keep |
| 2 | Sum of 5 odd numbers: count how many times the sum flips between even and odd. After 1 odd: odd. After 2: even. After 3: odd. After 4: even. After 5: odd. So 50 (even) is impossible. | **After 4 odd numbers the sum is even. What happens when you add one more odd number to an even sum?** | ❌→✅ CUE |

> 💡 **Why hint 2 changed:** The original walked through every step and named the final result — a full solution, not a prompt. The new version stops just before the conclusion so the student must finish the reasoning.

---

### CF2 — Anna, Ben, and Carla's marbles

**Type:** Fill in blank
**Question:** Anna, Ben, and Carla each have an odd number of marbles. Together they have 21. Anna has more than Ben, who has more than Carla. What is the largest number of marbles Anna could have?
**Answer:** 17

✏️ **Explanation fix:** Remove "Sanity check" — unfamiliar phrase for Grade 3-4.
- Old: "…To maximise Anna, minimise Ben and Carla: Carla = 1, Ben = 3 → Anna = 21 − 4 = 17. **Sanity check:** sum of 3 odds is odd; 21 is odd ✓."
- New: "…To give Anna the most, give Ben and Carla the least: Carla = 1, Ben = 3 → Anna = 21 − 4 = 17. **Quick check:** odd + odd + odd = odd, and 21 is odd ✓."

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | To maximise Anna, give Ben and Carla their smallest possible values. Carla has at least 1 (smallest positive odd). What is Ben's smallest possible value? | **To give Anna the most marbles, Ben and Carla each need the fewest. What is the smallest odd number Carla can have?** | ❌→✅ CUE |
| 2 | Carla = 1, Ben = 3 (next odd, must be > 1). Anna = 21 − 1 − 3 = ___. | **Carla has 1. The next odd number bigger than 1 is ___. That is Ben's share. Now Anna gets everything left from 21.** | ❌→✅ CUE |

> 💡 **Why hint 1 changed:** "Maximise" and "smallest possible values" are adult phrasing. Reworded in plain child language.
> 💡 **Why hint 2 changed:** The original named both values (Carla = 1, Ben = 3) — handing over the key numbers without the student earning them.

---

## Block 2 — Interactive Lesson: "Parity & Quick Elimination"

---

### Step 0 — Predict: "Can it work?" ✏️

**Question:** Can the sum of 7 different odd numbers be exactly 50?
**Options:** (A) Yes / (B) No / (C) Only if zero counts as odd
**maxAttempts:** 1 (proceedRegardless: true) — no change needed here.

✏️ **onWrong simplified:**
- Old: "Sum of 7 odd numbers — track the parity. After each odd, the sum flips between even and odd. After 7 odds: odd. 50 is even. Impossible."
- New: **"Start small: what is odd + odd? Now add a third odd number — what do you get? Keep going to 7."**

> 💡 **Why:** The old onWrong walked through the full solution in one block. A student who got it wrong should be nudged to TRY the reasoning, not have it handed to them.

---

### Step 0b — Animated Video: "The Pairing Story"

No content changes. See **Video Notes** section above for production issues.

---

### Step 1 — Explain: Even or odd? Look at the ones digit

endQuestion hint ("Look only at the ones digit: 3.") is already a good CUE — ✅ no changes.

---

### Step 2 — Apply: Sort the numbers

`sort_order` type works correctly. No changes needed.

---

### Step 3 — Explain: Sum rules ✏️

✏️ **Text:** Break into shorter sentences; remove variable "N" language:
- Old: "Three rules cover every two-number sum: even + even = EVEN, odd + odd = EVEN, odd + even = ODD. The big idea: adding an odd flips parity. So the sum of N odd numbers is odd if N is odd, even if N is even."
- New: **"There are three sum rules. Even + even = EVEN. Odd + odd = EVEN. Odd + even = ODD. Here is the key idea: every time you add an odd number, the parity flips. So count how many odd numbers you are adding. If that count is itself odd, the total is odd."**

✏️ **keyInsight:** Remove ⇔ symbol:
- Old: "Sum of N odd numbers is ODD ⇔ N is odd."
- New: **"If you add an odd count of odd numbers, the total is always odd."**

✏️ **endQuestion hint** — too compact:
- Old: "odd + even = odd."
- New: **"17 is odd. 28 is even. Which of the three sum rules covers odd + even?"**

---

### Step 4 — Apply: Predict the parity ✏️🐛

🐛 **Type changed:** `cloze_drag` → `sort_order`
Cloze-drag shows as a dropdown with no drop target in the CMS (nothing to drag onto). Sort-order achieves the same result and works correctly.

✏️ **Bucket labels:** items sorted into **"Odd total"** and **"Even total"** (was: dragging "even"/"odd" chips with nowhere to drop them)

✏️ **maxAttempts: 1** added — there are only 2 possible answers per item (even or odd). A second attempt is a guaranteed correct guess and adds no learning value.

✏️ **hint:** Remove ⇔ symbol:
- Old: "Count the odd terms. Sum is odd ⇔ count of odds is odd."
- New: **"Count the odd numbers in each expression. If that count is itself odd, the total is odd."**

---

### Step 5 — Explain: Product rules ✏️

✏️ **keyInsight:** Remove ⇔ symbol:
- Old: "Odd product ⇔ ALL factors odd."
- New: **"A product is odd only when every single number multiplied together is odd."**

endQuestion hint ("All four factors are odd.") is already a good CUE — ✅ no change.

---

### Step 6 — Apply: Even or odd product? 🐛

🐛 **Type changed:** `cloze_drag` → `sort_order`
Same reason as Step 4.

✏️ **Bucket labels:** items sorted into **"Odd product"** and **"Even product"**

---

### Step 7 — Apply: Cross out the impossibles ✏️🐛

🐛 **Type changed:** `cloze_drag` → `sort_order`

✏️ **Bucket labels** — "✓ stay" / "✗ eliminate" are too vague and "eliminate" is on the vocabulary ban list:
- Old: `choices: ["✓ stay", "✗ eliminate"]`
- New buckets: **"Can be the answer"** / **"Cannot be the answer"**

✏️ **hint** — same text regardless of which item the student is stuck on; doesn't guide specifically:
- Old: "Sum of 3 odds is always odd. Even options are impossible."
- New: **"Three odd numbers always add up to an odd total. Which of these options are even? Those cannot be the answer."**

---

### Step 8 — Reveal: Three rules, one habit ✏️

✏️ **Rules text:** Remove ⇔ symbols:

| Rule | Old statement | ✏️ New statement |
|------|--------------|-----------------|
| Sum | "odd + odd = even. Sum of N odds is odd ⇔ N is odd." | **"Odd + odd = even. If you add an odd count of odd numbers, the total is odd."** |
| Product | "A product is even if any factor is even; odd if all are odd." | **"A product is even if any number in it is even. It is odd only when every number in it is odd."** |
| Habit | No change needed. | ✅ keep |

closingCheckpoint and curiosity section — ✅ no changes needed.

---

## Block 3 — Worked Example 1 (MK 2012 Q13)

**Question:** Among Nikolay's classmates there are twice as many girls as boys. Which number can equal the total number of children in the class?

---

### WE1 — Problem figure 🐛

🐛 `problem.figure` is a bare string — must be an object:
- Old: `"figure": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_WE1_nikolay_class_diagram.svg"`
- New: `"figure": { "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_WE1_nikolay_class_diagram.svg" }`

---

### WE1 — Step 1: Read carefully ✏️🐛

🐛 **Type changed:** `fill_in_blank` → `mcq`
The original asks the student to type "2B" — an algebraic expression. The CMS fill-in-blank only accepts numbers. Changed to MCQ.

✏️ **New checkpoint question:**
> "If there are B boys among Nikolay's classmates, how many girls are there?"
- (A) B + 2
- **(B) 2B ✓**
- (C) B
- (D) 3B
- Answer: index 1

✏️ **hint:**
- Old: "'Twice as many girls as boys' → girls = 2 × boys."
- New: **"'Twice as many girls as boys' — what does twice as many mean? If there are 4 boys, how many girls would there be?"**

---

### WE1 — Step 2: Set up the total ✏️

✏️ **Question wording:** The original prompt "Total class = ?" is confusing — the answer (3B + 1) is already in the narration directly above it.
- Old: `"question": "Total class = ?"`
- New: **"The total class size — counting Nikolay himself — equals:"**

✏️ **hint:**
- Old: "Add Nikolay (1 boy) to the 3B classmates."
- New: **"The 3B counts Nikolay's classmates only. Is Nikolay himself included in that number?"**

---

### WE1 — Step 3: Test each option ✏️

✏️ **Narration:** Replace ÷ symbol (on the banned list):
- Old: "30÷3 = 10 r0 (no), 20÷3 = 6 r2 (no), 24÷3 = 8 r0 (no), 25÷3 = 8 r1 (yes!), 29÷3 = 9 r2 (no)."
- New: **"30 divided by 3 = 10 with no remainder (no). 20 divided by 3 = 6 remainder 2 (no). 24 divided by 3 = 8 no remainder (no). 25 divided by 3 = 8 remainder 1 (yes!). 29 divided by 3 = 9 remainder 2 (no)."**

✏️ **Bucket labels** — "is 3B+1" / "isn't" unclear for Grade 3-4:
- New: **"Fits the rule"** / **"Does not fit"**

✏️ **hint:**
- Old: "A number N satisfies 3B+1 iff (N − 1) is divisible by 3. Check each."
- New: **"Take each option. Subtract 1. Is the result a multiple of 3? Try it: 25 − 1 = 24. Is 24 a multiple of 3?"**

---

### WE1 — Step 4: Pick the answer ✏️

✏️ **insight:** Remove modular arithmetic notation — too advanced for Grade 3-4:
- Old: "We didn't compute every product. We eliminated 4 of 5 options using one quick property: 'must be ≡ 1 (mod 3).' Parity is the same idea with mod 2. The lesson is bigger than just odd/even — it's 'find the quick property of the answer and use it to eliminate.'"
- New: **"We did not try all the options from scratch. We found one rule — 'the total must be 1 more than a multiple of 3' — and used it to cross out 4 of the 5 choices. Parity is the same move: find a quick rule about the answer, then cross out anything that breaks it."**

✏️ **hint:**
- Old: "The only option that's 1 more than a multiple of 3."
- New: **"For each option, subtract 1. Which result is a multiple of 3?"**

---

## Block 4 — Worked Example 2 (MK 2014 Q12)

**Question:** Paula shoots two arrows at a target with rings worth 30, 50, and 70 points. Which sum CANNOT be her score?

---

### WE2 — Problem figure 🐛

🐛 `problem.figure` is a bare string — must be an object:
- Old: `"figure": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_WE2_target_30_50_70.svg"`
- New: `"figure": { "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_WE2_target_30_50_70.svg" }`

---

### WE2 — Step 1: What can a single arrow score? ✏️🐛

🐛 **Type changed:** `mcq_multi` → `mcq`
`mcq_multi` is not confirmed in the question router and was rendering as a text input field in the CMS. Replaced with a single-answer MCQ that tests the same understanding.

✏️ **New question:**
- Old: "Which of these is NOT a possible score for one arrow? (Pick all that apply.)" — 6 options
- New: **"Which of these could a single arrow NOT score?"**
  - (A) 0 points
  - (B) 30 points
  - **(C) 40 points ✓**
  - (D) 70 points
  - Answer: index 2

✏️ **hint:**
- Old: "Look at the target: rings score 30, 50, 70. Plus 0 if missed."
- New: **"Look at the target rings. Which scores appear on the rings? Does 40 appear anywhere?"**

---

### WE2 — Step 2: List every 2-arrow sum ✏️

✏️ **Bucket labels:** "possible" / "impossible" too abstract as labels:
- New: **"Can happen"** / **"Cannot happen"**

✏️ **hint** — gives the entire enumeration (full answer, not a prompt):
- Old: "Possible 2-arrow sums from {0, 30, 50, 70}: 0+0, 0+30, 0+50, 0+70, 30+30, 30+50, 30+70, 50+50, 50+70, 70+70 = {0, 30, 50, 60, 70, 80, 100, 120, 140}."
- New: **"Start with the smallest pairs: 0 + 0, 0 + 30, 0 + 50. Keep going through all the ring values. Can you make 90 from any two?"**

✏️ **explanation:** Remove curly brace notation (Grade 6+ set notation):
- Old: "Possible: {0, 30, 50, 60, 70, 80, 100, 120, 140}. 90 is the only listed value not in the achievable set."
- New: **"Possible 2-arrow totals: 0, 30, 50, 60, 70, 80, 100, 120, 140. The only answer choice that does not appear in this list is 90."**

---

### WE2 — Step 3: Did parity help here?

hint ("0, 30, 50, 70 — what's their parity?") is already a good CUE — ✅ no change.

---

### WE2 — Step 4: Pick the answer ✏️

✏️ **Narration gives away the answer before the checkpoint:**
- Old: "Only 90 has no valid pair."
- New: **"Look back at your list of possible 2-arrow totals. One of the answer choices is missing from that list."**

The checkpoint MCQ now asks the student to find it themselves rather than confirm what was just stated.

---

## Block 5 — Practice Lab

---

### P1 🐛✏️

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_P1_five_numbers.svg" }`

✏️ **hint:** Remove curly brace notation:
- Old: "Look at the ones digit of each number. Which one is from {0, 2, 4, 6, 8}?"
- New: **"Look at the ones digit of each number. Even ones digits are: 0, 2, 4, 6, 8. Which option matches?"**

---

### P2 🐛✏️

🐛 **Type changed:** `fill_in_blank` (answer: "odd") → `mcq`
A fill-in-blank with a text answer crashes the CMS renderer with NaN. Any time the answer is "even" or "odd", the question must be MCQ.

✏️ **New format:**
- Question: "What is the parity of 17 + 19 + 21 + 23 + 25?"
- Options: **(A) Odd ✓** / (B) Even
- answer: index 0

✏️ **hint:**
- Old: "Five odd numbers — count them. Sum of N odds is ___ when N is odd?"
- New: **"Count how many odd numbers are being added. If that count is itself odd, what is the total?"**

---

### P3 🐛✏️

🐛 **optionFigures not rendering in CMS** — asset bug. The five option SVGs are referenced but not displaying. Until resolved, the text options (A)–(E) must be fully readable standalone so students can still answer.

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_P3_options.svg" }`

✏️ **hint 1:** "eliminate" → "cross out":
- Old: "Use parity first — eliminate any option whose ones digit is odd."
- New: **"Start with parity: cross out any option whose ones digit is odd."**

✏️ **Answer display note:** User reported answer shown incorrectly in test view. Verify that answer index 1 (B: 3874) maps correctly after the optionFigures asset fix — visual position of options may shift.

---

### P4 🐛

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_P4_long_street.svg" }`

Hints are good CUEs — ✅ no changes.

---

### P5

No changes needed.

---

### P6 🐛✏️

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_P6_evens_1_to_50.svg" }`

✏️ **hint 2:** Replace ÷ symbol:
- Old: "2, 4, 6, …, 50 — that's 50 ÷ 2 = ___ numbers."
- New: **"2, 4, 6, …, 50 — that's 50 divided by 2 = ___ numbers."**

---

### P7 🐛✏️

🐛 **figure not showing in CMS** — critical asset bug. Without the dot-pattern images for options A–D, students cannot answer this question at all. Text labels ("4×3 grid", "13 dots in irregular cluster", etc.) must be clear enough to stand alone until the asset is fixed.

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_P7_dots.svg" }`

✏️ **hint:**
- Old: "Count carefully. A pattern with an even count would be e.g. a perfect rectangle of dots."
- New: **"Count the dots in each option. Any rectangle of rows and columns gives an even count. Which option is not a rectangle?"**

---

### P8 ✏️

✏️ **explanation:** Replace "Triples" with "groups of three"; remove curly braces; remove ✗ symbol:
- Old: "Triples of distinct positive integers summing to 9: {1,2,6}, {1,3,5}, {2,3,4}. Apply parity-of-product rule (even iff any factor is even). {1,2,6}: 2 is even → product even ✓. {1,3,5}: all odd → product odd ✗. {2,3,4}: 2 and 4 even → product even ✓. So 2 sets."
- New: **"Groups of three different counting numbers that sum to 9: (1, 2, 6), (1, 3, 5), (2, 3, 4). Check each: (1, 2, 6) has a 2, so its product is even ✓. (1, 3, 5) are all odd, so its product is odd — does not count. (2, 3, 4) has a 2, so its product is even ✓. Answer: 2 groups."**

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | List all triples of distinct positive integers summing to 9. Then check which have an even product. | **List all ways to pick three different counting numbers that add up to 9. Start with 1 as the smallest.** | ✏️ simplified |
| 2 | Triples: {1,2,6}, {1,3,5}, {2,3,4}. Apply the parity-of-product rule (even iff any factor is even). Eliminate the all-odd triple. | **Your three groups are (1, 2, 6), (1, 3, 5), and (2, 3, 4). Which group has all odd numbers? Cross that one out.** | ❌→✅ CUE |

---

## Block 6 — Mastery Check

> No hints allowed. `hintsAllowed: false` ✅

🐛 **CMS display issue:** Mastery check is showing "0/3 correct?" — flagged as a CMS rendering bug. Verify that `passCount: 2` is being read correctly before launch.

---

### MC1 🐛✏️

🐛 **Type changed:** `fill_in_blank` (answer: "odd") → `mcq`
Same NaN crash as P2. Any "even"/"odd" answer must be MCQ.

✏️ **New format:**
- Question: "Without computing, what is the parity of (1 + 2 + 3 + ... + 10) × 7?"
- Options: (A) Even / **(B) Odd ✓**
- answer: index 1

---

### MC2 🐛

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_MC2_options.svg" }`
🐛 **optionFigures:** same bare-string pattern as P3/P7 — wrap each in `{ "src": "..." }` if schema requires objects here.

---

### MC3 🐛

🐛 **figure:** bare string → `{ "src": "/figures/mk-grade-3-4/lesson-1-4/MK_L14_MC3_five_balls.svg" }`

---

## Block 7 — Challenge Extension (CE1)

**Question:** Anna writes down 5 different odd numbers, each between 1 and 15 (inclusive). Their sum is exactly 35. How many such sets are possible?
**Answer:** 5

✏️ **explanation:** Remove curly brace notation; replace "triples":
- Old: "Three-element subsets summing to 29: {1,13,15}, {3,11,15}, {5,9,15}, {5,11,13}, {7,9,13} — five triples. So 5 sets."
- New: **"Groups of three that sum to 29: (1, 13, 15), (3, 11, 15), (5, 9, 15), (5, 11, 13), (7, 9, 13) — five groups. So 5 sets."**

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | List all the odd numbers between 1 and 15. How many are there? What's their total sum? | *No change — already a good CUE.* | ✅ keep |
| 2 | Sum of all 8 odds = 64. Anna picks 5 summing to 35, so the 3 she leaves out must sum to 64 − 35 = 29. Find all 3-subsets summing to 29. | **All 8 odd numbers from 1 to 15 add up to 64. Anna keeps 5 that sum to 35. What must the other 3 add up to?** | ❌→✅ CUE |
| 3 | Triples summing to 29 from {1,3,5,7,9,11,13,15}: include 15 → other two sum to 14: (1,13), (3,11), (5,9). Include 13 (not 15) → other two sum to 16: (5,11), (7,9). Total: 3 + 2 = 5. | **Start with groups that include 15. The other two numbers must add up to 29 − 15 = 14. How many pairs from your list add up to 14?** | ❌→✅ CUE |

> 💡 **Why hints 2 and 3 changed:** Hint 2 gave away the complementary-sum insight (the key aha moment) and hint 3 gave the complete enumeration — both were full answers. New versions stop at the next step so the student takes the next move.

---

## All figure field fixes — summary

Every `figure` that was a bare string path needs to become a `{ "src": "..." }` object. Affected locations:

| Block | Item | Status |
|-------|------|--------|
| WE1 | `problem.figure` | 🐛 fix |
| WE2 | `problem.figure` | 🐛 fix |
| P1 | `figure` | 🐛 fix |
| P3 | `figure` + `optionFigures` | 🐛 fix + asset bug |
| P4 | `figure` | 🐛 fix |
| P6 | `figure` | 🐛 fix |
| P7 | `figure` + `optionFigures` | 🐛 fix + critical asset bug |
| MC2 | `figure` + `optionFigures` | 🐛 fix |
| MC3 | `figure` | 🐛 fix |
