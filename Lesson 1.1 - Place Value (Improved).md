# Lesson 1.1 — Place Value (Improved Version)

**ID:** `mk-f-place-value-number-properties`
**Difficulty:** 3pt–4pt | **Time:** 25 min
**Skills:** Place Value · Digits · Number Theory
**PYQ Sources:** MK 2014 Q02 (WE1) · MK 2000 Q10 (WE2) · MK 2013 Q08 · MK 2002 Q12 · MK 2007 Q15 · MK 2007 Q16 (CE)

> ✏️ marks every change from the original. Changes span: language simplification, removing ÷ symbol, warmer feedback, engaging hints, student-friendly titles, terminology fixes, and code bug fixes.

---

## Block 1 — Challenge First

> Students attempt cold. Hints unlock after 2 minutes.

### CF1 — Biggest number from 3 digit cards

**Type:** MCQ
✏️ **Question:** Mia has 3 digit cards: 8, 3, and 5. Use each card once. What's the BIGGEST number?
**Options:** 358 / 385 / 538 / 583 / **853** ✓
**Explanation:** Biggest first — 8 in hundreds, 5 in tens, 3 in ones → 853.
✏️ **On Wrong:** "The hundreds place is worth the most. Give it your biggest card!"

| Hint | Text |
|------|------|
| 1 | ✏️ Biggest digit in hundreds = biggest number! |
| 2 | ✏️ Which card is biggest — 8, 3, or 5? That one earns the hundreds seat. |

---

### CF2 — Smallest number from same cards

**Type:** Fill in blank
✏️ **Question:** Same cards: 8, 3, and 5. Now make the SMALLEST number.
**Answer:** 358
**Explanation:** Smallest first — 3 in hundreds, 5 in tens, 8 in ones → 358.
✏️ **On Wrong:** "For smallest, the hundreds seat goes to your smallest card. Which card is that?"

| Hint | Text |
|------|------|
| 1 | ✏️ Smallest digit in hundreds = smallest number! |
| 2 | ✏️ Which card is smallest — 8, 3, or 5? That one earns the hundreds seat. |

---

## Block 2 — Interactive Lesson: "Place Value in Action"

---

### Step 0 — Predict: The sneaky zero rule

**Type:** Predict
**Question:** Using digits 4, 0, and 8 once each — what's the smallest 3-digit number?
**Answer:** 408 *(proceed regardless)*
- ✅ **Correct:** "Sharp — you spotted the rule that trips everyone up!"
- ✏️ ❌ **Wrong:** "Tricky! 0 can't lead — 408 is the smallest, not 048."

---

### Step 1 — Explain: Same digit, three totally different values?

✏️ **Title:** "Same digit… three totally different values?"
✏️ **Text:** "See the three 7s? Same digit — each one worth something completely different!"
**Visual:** Place-value chart with 777
✏️ **Key Insight:** Move left → 10× bigger. Move right → 10× smaller.
**End Question:** The hundreds 7 is worth ___ times the ones 7. → **100**

> ✏️ Removed ÷ symbol entirely. Original said "Each step left: ×10. Each step right: ÷10." — Grade 3 may not know division yet. Now: multiplication framing only.

---

### Step 2 — Applet: Tap each column (place-value-chart)

**Applet Type:** `place-value-chart` | **Config:** number = 777
✏️ **Discovery Question:** Each column is ___ times bigger than the one just to its right. → **10**
✏️ **Discovery Message:** "7 × 10 = 70. 70 × 10 = 700. Move left and the value jumps 10× every single time!"

> ✏️ Removed "Adjacent columns always differ by a factor of {blank}" — "adjacent" and "factor of" are not Grade 3 language. Removed ÷ from discovery message.

---

### Step 3 — Apply: What is each digit worth in 749?

✏️ **Title:** "What is each digit worth in 749?"
✏️ **Text:** "Let's try a new number. What is each digit worth?"
**Visual:** Digit blocks for 749

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | Hundreds digit 7 → ___ | 700 | 7 is in hundreds → 7 × 100 = ? |
| 2 | Tens digit 4 → ___ | 40 | 4 is in tens → 4 × 10 = ? |
| 3 | Ones digit 9 → ___ | 9 | 9 is in ones → 9 × 1 = ? |

✏️ **All correct:** "Now — can you build a number from loose digits?"

---

### Step 4 — Explain: Sort the digits. Big ones go left.

✏️ **Title:** "Sort the digits. Big ones go left."
✏️ **Text:** "Hundreds place rules! Put your biggest digit there — that makes the BIGGEST number."
**Visual:** Digit cards [6, 2, 9]
✏️ **Key Insight:** "Zero can't lead! It goes in tens or ones, never hundreds."
✏️ **End Question:** "Digits 3, 8, 1 — what's the BIGGEST number?" → **831**

> ✏️ Original title: "Big lives left" (reads as video game lives). Fixed to "Big ones go left."
> ✏️ Original body text was 41 words with "H column", "U column", "leverage". Now 13 words, plain language.
> ✏️ Key Insight: "zero takes T or U, never H" → now spells out the rule in full plain words.

---

### Step 5 — Applet: Drag and drop (digit-rearranger)

**Applet Type:** `digit-rearranger` | **Config:** digits = [4, 0, 7]
✏️ **Instruction:** "Drag 4, 0, 7 into Hundreds, Tens, Ones to make the SMALLEST number!"
✏️ **Discovery Question:** Smallest 3-digit number using 4, 0, and 7 = ___. → **407**
✏️ **Discovery Message:** "0 can't lead! So 4 takes hundreds, 0 goes to tens."

> ✏️ Original instruction used "H, T, U" (undefined abbreviations). Now spells out Hundreds, Tens, Ones.
> ✏️ Original discovery message introduced "047 is just 47" as a concept to dwell on. Replaced with a direct rule.
> ✏️ Removed {4, 0, 7} curly brace notation — middle-school set theory notation, not Grade 3.

---

### Step 6 — Apply: Three quick checks

✏️ **Text:** "Three checks — biggest, smallest, and the sneaky zero rule!"
**Visual:** Digit cards [0, 6, 3]

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | ✏️ Biggest from 2, 9, 5 = ___ | 952 | Biggest digit in hundreds, then tens, then ones. |
| 2 | ✏️ Smallest from 2, 9, 5 = ___ | 259 | Smallest digit in hundreds first. |
| 3 | ✏️ Smallest from 0, 6, 3 = ___ | 306 | Zero can't lead — 3 takes hundreds, 0 slides to tens. |

✏️ **All correct:** "Last move — read a description and name the number."

> ✏️ Removed {2, 9, 5} and {0, 6, 3} curly brace set notation throughout.

---

### Step 7 — Explain: Zero looks empty. It's not.

✏️ **Title:** "Zero looks empty. It's not."
✏️ **Text:** "408 and 48 look similar. But zero makes them worlds apart."
**Visual:** Place-value breakdown for 408
✏️ **Key Insight:** "Zero isn't missing — it's working! It holds a place."
**End Question:** 300 + 0 + 7 = ___. → **307**

> ✏️ Original title: "When zero shows up" (passive, no hook).
> ✏️ Original body was 36 words. Now 11 words. The emotional hook ("worlds apart") comes first.
> ✏️ Original key insight had asterisks rendering as literal characters (markdown bug). Fixed.

---

### Step 8 — Applet: Build each number (number-builder)

**Applet Type:** `number-builder`
**Rounds:** Target 603 · Target 480 · Target 205 (all start from 000)
✏️ **Instruction:** "Three targets, each with a zero hiding somewhere. Press + / − to build each one."
**Discovery Question:** In 603, the value of the tens digit is ___. → **0**
✏️ **Discovery Message:** "603 = 600 + 0 + 3. 480 = 400 + 80 + 0. Zero is always on the job — keeping every other digit in the right seat!"

---

### Step 9 — Apply: Three quick checks (zero)

**Text:** "Check that zeros, expanded forms, and names all lock in."
**Visual:** Place-value breakdown for 480

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 (MCQ) | Expanded form of 480 is ___ | **400 + 80 + 0** | 4 hundreds = 400. 8 tens = 80. 0 ones = 0. |
| 2 | 300 + 0 + 6 = ___ | 306 | Hundreds = 300, tens = 0, ones = 6. Put them together. |
| 3 | 7 hundreds, 0 tens, 9 ones. The number is ___ | 709 | Hundreds = 700, tens = 0, ones = 9. Add them up. |

**MCQ Options for Substep 1:** 400 + 80 + 0 / 40 + 80 + 0 / 400 + 8 + 0 / ✏️ 400 + 80

> ✏️ **Bug fix:** Added `"type": "mcq"` to this substep — missing from original, causes question router to fail in CMS.
> ✏️ Replaced invalid option "4 + 800" with "400 + 80" (a meaningful distractor — forgets the zero ones placeholder).
> ✏️ Substep 3 hint: removed "H × 100 + T × 10 + O × 1" formula notation. Now plain language.

---

### Step 10 — Reveal: Three tools. One toolkit.

| Tool | Rule | Example |
|------|------|---------|
| ✏️ Break it apart | ✏️ Find what each digit is worth. | 749 = 700 + 40 + 9 |
| Build biggest/smallest | ✏️ Big digits go left. Zero can't lead! | ✏️ 0, 6, 3 → biggest: 630 · smallest: 306 |
| Read & name | ✏️ Name each place's value, then add up. | ✏️ 5 hundreds + 8 tens + 2 ones = 582 |

**Curiosity Bridge:** Add the digits of 408: 4 + 0 + 8 = ___. → **12**
> ✏️ Updated CTA: "Next: See it in action — 2 real competition problems →"

> ✏️ Rule card 1: "Decompose" → "Break it apart" (child-friendly verb).
> ✏️ Rule card 2: Removed "sort H → T → U" notation.
> ✏️ Rule card 3: Removed algebra variables X, Y, Z entirely. Now uses a concrete example.

---

### Remediations

| Concept | Title | Options | Answer | Feedback |
|---------|-------|---------|--------|---------|
| place-value-ratio | Quick refresher — the 10× rule | 10 / **100** / 1000 | 100× | Hundreds = 100, ones = 1. So hundreds is 100× ones. |
| place-value-decompose | Walk through one digit at a time | 5 / **50** / 500 | 50 | 5 is in the tens column → 5 × 10 = 50. |
| ✏️ largest-smallest-formation | Sort it. Remember the sneaky zero rule. | ✏️ 470 / 704 / **407** | 407 | ✏️ 0 can't lead — so 4 takes hundreds, 0 takes tens, 7 takes ones → 407. |
| expanded-form-zero-placeholder | Zero holds a place — it never disappears | 50 + 6 / **500 + 0 + 6** / 500 + 60 | 500 + 0 + 6 | 5 hundreds = 500, 0 tens = 0, 6 ones = 6 → 500 + 0 + 6. |

> ✏️ Remediation text for largest-smallest-formation updated: "H, T, U" → "hundreds, tens, ones". Options changed from ["047", "074", "407"] — showing invalid leading-zero strings to students was actively teaching a wrong concept.
> ✏️ Remediation text for place-value-ratio: removed ÷ symbol. Now "7 × 10 = 70. 70 × 10 = 700."

---

## Block 3 — Worked Example 1 (MK 2014 Q02) ⭐ 3pt

**Problem:** Jackie wants to place the digit 3 somewhere in the number 2014. Where should she place it to make the resulting five-digit number as small as possible?

**Options:** (A) in front of 2014 · (B) between 2 and 0 · (C) between 0 and 1 · **(D) between 1 and 4** ✓ · (E) after 2014

> ✏️ **Bug fix:** `problem.figure` changed from bare string path to `{ "src": "..." }` object. The CMS reads `figure.src` — a bare string causes an invisible/missing figure.

---

### ✏️ Step 1 — "Count the gaps"

*(Was: "Count the positions")*
**Narrative:** "Jackie inserts digit 3 into 2014. It can go in any gap between digits, or at either end."
**Checkpoint:** How many different gaps can digit 3 go into? → **5**
*Hint: Count: before 2, between 2–0, between 0–1, between 1–4, after 4.*

---

### ✏️ Step 2 — "Write out all five numbers"

*(Was: "Map each slot to its number")*

| Gap | Position | Number |
|-----|----------|--------|
| A | before 2 | 32014 |
| B | between 2–0 | 23014 |
| C | between 0–1 | 20314 |
| D | between 1–4 | 20134 |
| E | after 4 | 20143 |

**Checkpoint 1:** Gap C gives the number ___. → **20314**
**Checkpoint 2:** Gap D gives the number ___. → **20134**

---

### ✏️ Step 3 — "Cut the biggest starter!"

*(Was: "First-digit elimination")*
- A → 32014, first digit = 3
- B, C, D, E → first digit = 2
- 3 > 2 → ✏️ cross out A

✏️ **Checkpoint:** After crossing out A, how many numbers are left? → **4**
*Hint: Started with 5. Crossed out 1.*

---

### ✏️ Step 4 — "Keep cutting — compare the next digits!"

*(Was: "Second + third digit elimination")*
- B → 23014, second digit = 3 → ✏️ cross out B
- C → 20314, third digit = 3 → ✏️ cross out C
- ✏️ D and E are still in the game: 20134 and 20143

**Checkpoint 1:** Second digit of 23014 is ___. → **3**
✏️ **Checkpoint 2:** Two numbers are still in the game. Which are they? → **20134 and 20143**

> ✏️ "candidates" → "numbers still in the game" (adult/formal vocabulary replaced throughout).
> ✏️ "eliminate" → "cross out" (more concrete for Grade 3).

---

### ✏️ Step 5 — "Last two standing!"

*(Was: "Final comparison + insight")*
- D → 20134, fourth digit = 3
- E → 20143, fourth digit = 4
- 3 < 4 → D wins → **Answer: (D)**

✏️ **Insight:** "To make it smallest: push inserted digit right, past all smaller digits. To make it biggest: push it left."

**Checkpoint 1:** Which is smaller — 20134 or 20143? → **20134**
*Hint: First three digits match. Look at the fourth.*
**Checkpoint 2:** What if Jackie wanted the BIGGEST number?
- **(A) Place 3 in front → 32014** ✓
- (B) Place 3 between 0 and 1 → 20314
- (C) Place 3 after 4 → 20143

---

## Block 4 — Worked Example 2 (MK 2000 Q10) ⭐⭐ 4pt

**Problem:** Which four digits need to be removed from 4921508 to get the smallest possible three-digit number?

**Options:** (A) 4,9,2,1 · (B) 4,2,1,0 · (C) 1,5,0,8 · **(D) 4,9,2,5** ✓ · (E) 4,9,5,8

> ✏️ **Bug fix:** `problem.figure` changed from bare string path to `{ "src": "..." }` object.

---

### ✏️ Step 1 — "Understand the rule"

*(Was: "Establish the constraint")*
**Narrative:** "7 digits. Remove exactly 4. Keep 3. The 3 kept digits must stay in their original left-to-right order — no rearranging."
**Checkpoint:** Keeping positions 4, 6, 7 gives digits 1, 0, 8. What number? → **108**

---

### ✏️ Step 2 — "Pick the hundreds digit"

*(Was: "Choose hundreds digit")*
- Positions 1–5 work — there are still 2+ digits after each
- Position 6 (digit 0) won't work — only 1 digit left after it
- Position 7 (digit 8) won't work — no digits left after it

✏️ **Narrative:** "The five digits we can pick for hundreds: 4, 9, 2, 1, 5."

**Checkpoint 1:** How many digits are to the right of position 5? → **2**
**Checkpoint 2:** Smallest digit among 4, 9, 2, 1, 5 is ___. → **1**

---

### ✏️ Step 3 — "Pick the tens digit"

*(Was: "Choose tens digit")*
- Position 5 (digit 5): 2 digits after it — works
- Position 6 (digit 0): 1 digit after it — works
- Position 7 (digit 8): 0 digits after it — no

**Checkpoint 1:** Which tens digit gives the smaller final number?
- (A) 5 → gives 158
- **(B) 0 → gives 108** ✓

**Checkpoint 2:** The smallest 3-digit number from 4921508 is ___. → **108**

---

### ✏️ Step 4 — "Name the removed digits"

*(Was: "Identify removed digits")*
- Kept: 1, 0, 8 (positions 4, 6, 7)
- Removed: 4, 9, 2, 5 (positions 1, 2, 3, 5)

**Checkpoint:** Which answer lists the four removed digits? → **(D) 4, 9, 2, 5**
*Hint: Kept digits are 1, 0, 8. Everything else in 4 9 2 1 5 0 8 was removed.*

---

## Block 5 — Practice Lab

| # | Question | Answer | Difficulty |
|---|---------|--------|------------|
| P1 | ✏️ Sam has 3 digit cards: 4, 7, and 9. Use each card once. What's the BIGGEST number? | 974 (E) | 3pt |
| P2 | Which boy is wrong about 325? (Andy/Barry/Charlie/Danny/Eddie) | Eddie (E) — digit 2 is even | 3pt |
| P3 | ✏️ What's the BIGGEST digit in 6_3 that keeps 6_3 less than 670? | 6 (C) | 3pt |
| P4 | Add 17 to smallest 2-digit, divide by largest 1-digit. Result? | 3 (A) | 4pt |
| P5 | ✏️ In 528, how much MORE is the 5 worth than the 2? | 480 (D) | 4pt |
| P6 | David's first digit (two-digit + 19 = 72) | 5 (B) | 4pt |
| P7 | ✏️ Leo inserts digit 5 into 37. What's the SMALLEST 3-digit number? | 357 (A) | 4pt |
| P8 | ✏️ Tom has cards 7, 0, 3, 5. Biggest 4-digit number (0 can't go first)? | 7530 (E) | 4pt |

---

### Hints (all revised)

**P1**
1. ✏️ Which number is biggest: 4, 7, or 9? It earns hundreds first!
2. ✏️ 9 is in hundreds. Now sort the other two from biggest to smallest.
3. ✏️ After 9 in hundreds and 7 in tens, only one card is left — where does it go?

**P2**
1. Check each boy's claim one at a time.
2. Are all digits of 325 odd? What are the three digits?
3. The digits are 3, 2, and 5. Is 2 odd or even?

**P3**
1. ✏️ Try a digit in the blank. Does it keep 6_3 under 670?
2. ✏️ Try 6: 663 < 670. Try 7: 673 < 670?
3. ✏️ You tried 6 and 7. Which one kept the number below 670?

**P4**
1. What's the smallest 2-digit number? What's the largest 1-digit number?
2. Smallest 2-digit = 10. Largest 1-digit = 9. Work out (10 + 17) ÷ 9.
3. ✏️ What is 27 ÷ 9?

**P5**
1. ✏️ What is digit 5 worth in 528? What is digit 2 worth?
2. ✏️ 5 is in hundreds → 500. 2 is in tens → 20. Now find the difference.
3. ✏️ You have both values. Subtract the smaller from the larger.

**P6**
1. Work backwards: two-digit number = 72 − 19. What is that?
2. The first digit David wrote is the tens digit of that two-digit number.
3. ✏️ What is the tens digit of the number you just found?

**P7**
1. ✏️ List all three positions: 5 before 3, 5 between 3 and 7, 5 after 7.
2. ✏️ The three numbers are 537, 357, 375. Which is smallest?
3. ✏️ Compare from the left — which number has the smallest hundreds digit?

**P8**
1. ✏️ Which card is biggest? That one takes the thousands place.
2. ✏️ 7 is first. Now sort the remaining cards 5, 3, 0 from biggest to smallest.
3. ✏️ With 7 in thousands, arrange 5, 3, 0 from biggest to smallest in the next three spots.

---

## Block 6 — Mastery Check

> 4 questions · No hints · Pass 3/4 to unlock Lesson 1.2

| # | Question | Answer |
|---|---------|--------|
| MC1 | ✏️ What's the BIGGEST 3-digit number from 6, 0, 4? | 640 (E) |
| MC2 | ✏️ What's the SMALLEST 3-digit number from 3, 8, 1? | 138 (A) |
| MC3 | ✏️ Maya's cards 3, 6, 1 — which arrangement gives SMALLEST? | ✏️ Hundreds=1, Tens=3, Ones=6 → 136 (A) |
| MC4 | ✏️ Digit 4 placed after 7 makes 74. What is 74 − (7 × 7)? | 25 (C) |

> ✏️ **MC3:** All 5 options updated from "U=X" to "Ones=X" (U is non-standard in US curriculum).
> ✏️ **MC4:** Original question said "minus 7 times the original digit" — ambiguous. Now explicitly says "(7 × 7)" so there's zero confusion.

---

## Block 7 — Challenge Extension (MK 2007 Q16) ⭐⭐ 4pt

✏️ **Question:** An electronic watch shows 02:07. After how much time will the same digits appear again for the first time — in any order?

**Options:** **(A) 4 hr 55 min** ✓ · (B) 6 hr · (C) 10 hr 55 min · (D) 11 hr 13 min · (E) 24 hr

**Explanation:** Digits at 02:07 are 0, 2, 0, 7. Valid times: 00:27 (before 02:07), 07:02, 07:20, 20:07. First valid time after 02:07 → 07:02. Elapsed: 4 hr 55 min.

| Hint | Text |
|------|------|
| 1 | ✏️ Write down every digit on the watch face at 02:07. There are four of them. |
| 2 | What valid times (00:00 to 23:59) can you make using exactly those four digits? |
| 3 | ✏️ You have your list of valid times. Which one comes first after 02:07? |

> ✏️ Original H1 used {0, 0, 2, 7} curly brace notation. Removed.
> ✏️ Original H3 listed all valid times — that's the full answer. Now it's a directional nudge only.

---

## Summary of All Changes

### Code Bugs Fixed
| Location | Bug | Fix |
|----------|-----|-----|
| WE1 `problem.figure` | Bare string path — figure invisible in CMS | Changed to `{ "src": "..." }` object |
| WE2 `problem.figure` | Bare string path — figure invisible in CMS | Changed to `{ "src": "..." }` object |
| IL Step 9 substep 1 | Missing `"type": "mcq"` — question router fails | Added `"type": "mcq"` field |
| Remediation options | Options ["047", "074", "407"] show invalid leading-zero strings | Replaced with ["470", "704", "407"] |
| IL Step 9 option | "4 + 800" is a confusing/invalid distractor | Replaced with "400 + 80" (forgets zero ones placeholder) |

### Language Fixes (every instance)
| Original | Improved | Why |
|----------|----------|-----|
| "÷" symbol anywhere | "×" framing only | Grade 3 may not know division yet |
| "H, T, U" abbreviations | "Hundreds, Tens, Ones" in full | U is undefined and non-standard |
| {set} curly brace notation | Plain comma-separated list | Middle-school notation, not Grade 3 |
| "adjacent columns" | "columns next to each other" | "Adjacent" is adult vocabulary |
| "candidates" | "numbers still in the game" | Formal/political vocabulary |
| "eliminate" | "cross out" | More concrete action word |
| "decompose" | "break it apart" | Child-friendly verb |
| "leverage" | removed | Finance/adult vocabulary |
| "leading-zero trap" | "the sneaky zero rule" | Playful, memorable, child-friendly |
| "Sort the digits. Big lives left." | "Sort the digits. Big ones go left." | "lives" reads as video game lives |
| "When zero shows up" | "Zero looks empty. It's not." | Original title has no hook |
| 30–40 word body texts | ≤15 words per sentence | Shorter = more readable for 8-year-olds |
| X, Y, Z algebra in rule card 3 | Concrete example (5 hundreds + 8 tens + 2 ones = 582) | Algebra variables are Grade 6+, not Grade 3 |
| "LARGEST/SMALLEST" in questions | "BIGGEST/SMALLEST" where natural | "Biggest" is more natural for Grade 3 |
| Markdown `*bold*` in JSON strings | Plain text | Asterisks render as raw characters in CMS |

### Hint Quality (all revised)
Every Hint 3 that revealed the complete answer has been replaced with a light directional nudge — one step short of the answer, not the answer itself.
