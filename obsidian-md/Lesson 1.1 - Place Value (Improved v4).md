# Lesson 1.1 — Reading & Building Numbers from Place Value

**Course:** Math Kangaroo Prep — Grade 3 & 4 · **Phase:** 1 (NT Part 1) · **Difficulty:** 3pt → 5pt · **Duration:** 25 min
**Technique:** Read any digit's value by its place. Build the BIGGEST and smallest number from digit tiles. Name a number from "X hundreds, Y tens, Z ones."

> **v4 changes from v3 (marked ✏️v4):**
> 1. **CF1** — scenario freshened to code-breaker / number-bag framing
> 2. **IL Step 4 visual** — combination lock figure replaces plain digit cards
> 3. **IL Step 10 reveal** — "Case Closed" detective toolkit framing
> 4. **P1** — format changed from MCQ to sort_order (drag digit tiles)
> 5. **P4** — replaced with 2004 Q13 (Angie ×10 vs ÷10, directly tests the lesson's core ×10 rule)
> 6. **P7** — replaced with 2019 Q14 (Steven's digit boxes for max sum, tests place value priority)
> 7. **P8** — format changed from MCQ to sort_order (drag digit tiles)
> 8. **CE** — replaced with 1999 Q22 (5pt ✓ — insert 0 between digits of 51–55)

> All v3 language fixes, code bug fixes, and hint rewrites are carried forward.

---

## Block 1 — Challenge First

> Students attempt cold. Hints unlock after 2 minutes.

---

### CF1 — Biggest number from 3 digit tiles

**Type:** MCQ
✏️v4 **Scenario:** A number bag drops 3 digit tiles on your desk: **8, 3, and 5**. Use each tile exactly once. What's the BIGGEST number you can build?
**Options:** 358 / 385 / 538 / 583 / **853** ✓
**Explanation:** Biggest digit first — 8 in hundreds, 5 in tens, 3 in ones → 853.
✏️ **On Wrong:** "The hundreds place is worth the most. Give it your biggest tile!"

| Hint | Text |
|------|------|
| 1 | Biggest digit in hundreds = biggest number! |
| 2 | Which tile is biggest — 8, 3, or 5? That one earns the hundreds seat. |

---

### CF2 — Smallest number from same tiles

**Type:** MCQ
✏️ **Question:** Same tiles: 8, 3, and 5. Now make the SMALLEST number.
**Options:** **358** ✓ / 385 / 530 / 583 / 835
**Explanation:** Smallest digit first — 3 in hundreds, 5 in tens, 8 in ones → 358.
✏️ **On Wrong:** "For smallest, the hundreds seat goes to your smallest tile. Which tile is that?"

| Hint | Text |
|------|------|
| 1 | Smallest digit in hundreds = smallest number! |
| 2 | Which tile is smallest — 8, 3, or 5? That one earns the hundreds seat. |

> ✏️v4 **CF2 changed from fill_in_blank to MCQ.** fill_in_blank is fine for numbers, but MCQ provides distractors that reveal common misconceptions (e.g., 530 = "I put 5 first because it was the middle card"). MCQ is also explicitly preferred for WE/Practice/MC per lesson design standard.

---

## Block 2 — Interactive Lesson: "Crack the Code — Place Value in Action"

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

> ✏️ Removed ÷ symbol. Original: "Each step right: ÷10." Grade 3 may not know division yet. Now: multiplication framing only.

---

### Step 2 — Applet: Tap each column (place-value-chart)

**Applet Type:** `place-value-chart` | **Config:** number = 777
✏️ **Discovery Question:** Each column is ___ times bigger than the one just to its right. → **10**
✏️ **Discovery Message:** "7 × 10 = 70. 70 × 10 = 700. Move left and the value jumps 10× every single time!"

> ✏️ Removed "Adjacent columns always differ by a factor of {blank}" — "adjacent" and "factor of" are not Grade 3 language.

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
✏️v4 **Visual:** A 3-dial combination lock. Each dial shows digits 0–9. The three dials are set to 6, 2, 9. Caption: "Set the biggest digit on the left dial first!"
✏️ **Key Insight:** "Zero can't lead! It goes in tens or ones, never hundreds."
✏️ **End Question:** "Digits 3, 8, 1 — what's the BIGGEST number?" → **831**

> ✏️v4 **Combination lock figure:** The lock's three rotating dials map directly to Hundreds, Tens, Ones. This is more visceral than a flat digit-card image — students have turned combination locks and know the left dial matters most. Reinforces the "sort from left" rule without words.
> ✏️ Original title: "Big lives left" (reads as video game lives). Fixed to "Big ones go left."
> ✏️ Original body text was 41 words with "H column", "U column", "leverage". Now 13 words, plain language.

---

### Step 5 — Applet: Drag and drop (digit-rearranger)

**Applet Type:** `digit-rearranger` | **Config:** digits = 4, 0, 7
✏️ **Instruction:** "Drag 4, 0, 7 into Hundreds, Tens, Ones to make the SMALLEST number!"
✏️ **Discovery Question:** Smallest 3-digit number using 4, 0, and 7 = ___. → **407**
✏️ **Discovery Message:** "0 can't lead! So 4 takes hundreds, 0 goes to tens."

> ✏️ Original instruction used "H, T, U" (undefined abbreviations). Now spells out Hundreds, Tens, Ones.
> ✏️ Removed {4, 0, 7} curly brace notation — middle-school set theory, not Grade 3.

---

### Step 6 — Apply: Three quick checks

✏️ **Text:** "Three checks — biggest, smallest, and the sneaky zero rule!"
**Visual:** Digit cards 0, 6, 3

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | ✏️ Biggest from 2, 9, 5 = ___ | 952 | Biggest digit in hundreds, then tens, then ones. |
| 2 | ✏️ Smallest from 2, 9, 5 = ___ | 259 | Smallest digit in hundreds first. |
| 3 | ✏️ Smallest from 0, 6, 3 = ___ | 306 | Zero can't lead — 3 takes hundreds, 0 slides to tens. |

✏️ **All correct:** "Last move — read a description and name the number."

> ✏️ Removed curly brace set notation throughout.

---

### Step 7 — Explain: Zero looks empty. It's not.

✏️ **Title:** "Zero looks empty. It's not."
✏️ **Text:** "408 and 48 look similar. But zero makes them worlds apart."
**Visual:** Place-value breakdown for 408
✏️ **Key Insight:** "Zero isn't missing — it's working! It holds a place."
**End Question:** 300 + 0 + 7 = ___. → **307**

> ✏️ Original title: "When zero shows up" (passive, no hook).
> ✏️ Original body was 36 words. Now 11 words.

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

> ✏️ **Bug fix:** Added `"type": "mcq"` to this substep — missing from original.
> ✏️ Replaced invalid option "4 + 800" with "400 + 80" (forgets the zero ones placeholder — a meaningful distractor).

---

### Step 10 — Reveal: Case Closed. Three Tools. Every Problem Solved.

✏️v4 **Framing:** "Every problem in this lesson cracked by the same three tools. File them away."

| Tool | Rule | Example |
|------|------|---------|
| ✏️ Break it apart | Find what each digit is worth. | 749 = 700 + 40 + 9 |
| Build biggest/smallest | Big digits go left. Zero can't lead! | 0, 6, 3 → biggest: 630 · smallest: 306 |
| Read and name | Say each place's value, then add up. | 5 hundreds + 8 tens + 2 ones = 582 |

✏️v4 **Tone:** "Detective's toolkit — stamped SOLVED on every contest problem you'll meet on place value."

**Curiosity Bridge:** Add the digits of 408: 4 + 0 + 8 = ___. → **12**
✏️ **CTA:** "Next: See these tools in action on 2 real competition problems →"

> ✏️v4 "Case Closed" framing: replaces plain summary table with a sense of accomplishment and narrative payoff. The "detective's toolkit" metaphor ties back to the code-breaker CF framing, making the lesson feel like one coherent story arc.
> ✏️ Rule card 1: "Decompose" → "Break it apart."
> ✏️ Rule card 2: Removed "sort H → T → U."
> ✏️ Rule card 3: Removed algebra variables. Now uses a concrete example.

---

### Remediations

| Concept | Title | Options | Answer | Feedback |
|---------|-------|---------|--------|---------|
| place-value-ratio | Quick refresher — the 10× rule | 10 / **100** / 1000 | 100 | Hundreds = 100, ones = 1. So hundreds is 100× ones. |
| place-value-decompose | Walk through one digit at a time | 5 / **50** / 500 | 50 | 5 is in the tens column → 5 × 10 = 50. |
| ✏️ largest-smallest-formation | Sort it. Remember the sneaky zero rule. | ✏️ 470 / 704 / **407** | 407 | ✏️ 0 can't lead — so 4 takes hundreds, 0 takes tens, 7 takes ones → 407. |
| expanded-form-zero-placeholder | Zero holds a place — it never disappears | 50 + 6 / **500 + 0 + 6** / 500 + 60 | 500 + 0 + 6 | 5 hundreds = 500, 0 tens = 0, 6 ones = 6 → 500 + 0 + 6. |

> ✏️ Remediation options changed from ["047", "074", "407"] — showing invalid leading-zero strings was teaching a wrong concept.

---

## Block 3 — Worked Example 1 (MK 2014 Q02) ⭐ 3pt

**Problem:** Jackie wants to place the digit 3 somewhere in the number 2014. Where should she place it to make the resulting five-digit number as small as possible?

**Options:** (A) in front of 2014 · (B) between 2 and 0 · (C) between 0 and 1 · **(D) between 1 and 4** ✓ · (E) after 2014

> ✏️ **Bug fix:** `problem.figure` changed from bare string path to `{ "src": "..." }` object.

---

### ✏️ Step 1 — "Count the gaps"

**Narrative:** "Jackie inserts digit 3 into 2014. It can go in any gap between digits, or at either end."
**Checkpoint:** How many different gaps can digit 3 go into? → **5**
*Hint: Count: before 2, between 2–0, between 0–1, between 1–4, after 4.*

---

### ✏️ Step 2 — "Write out all five numbers"

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

- A → 32014, first digit = 3
- B, C, D, E → first digit = 2
- 3 > 2 → ✏️ cross out A

✏️ **Checkpoint:** After crossing out A, how many numbers are left? → **4**
*Hint: Started with 5. Crossed out 1.*

---

### ✏️ Step 4 — "Keep cutting — compare the next digits!"

- B → 23014, second digit = 3 → ✏️ cross out B
- C → 20314, third digit = 3 → ✏️ cross out C
- ✏️ D and E are still in the game: 20134 and 20143

**Checkpoint 1:** Second digit of 23014 is ___. → **3**
✏️ **Checkpoint 2:** Two numbers are still in the game. Which are they?
- **(A) 20134 and 20143** ✓
- (B) 20314 and 20143
- (C) 20134 and 20314

> ✏️ "candidates" → "numbers still in the game." "eliminate" → "cross out."

---

### ✏️ Step 5 — "Last two standing!"

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

**Narrative:** "7 digits. Remove exactly 4. Keep 3. The 3 kept digits must stay in their original left-to-right order — no rearranging."
**Checkpoint:** Keeping positions 4, 6, 7 gives digits 1, 0, 8. What number? → **108**

---

### ✏️ Step 2 — "Pick the hundreds digit"

- Positions 1–5 work — there are still 2+ digits after each
- Position 6 (digit 0) won't work — only 1 digit left after it
- Position 7 (digit 8) won't work — no digits left after it

✏️ **Narrative:** "The five digits we can pick for hundreds: 4, 9, 2, 1, 5."

**Checkpoint 1:** How many digits are to the right of position 5? → **2**
**Checkpoint 2:** Smallest digit among 4, 9, 2, 1, 5 is ___. → **1**

---

### ✏️ Step 3 — "Pick the tens digit"

- Position 5 (digit 5): 2 digits after it — works
- Position 6 (digit 0): 1 digit after it — works
- Position 7 (digit 8): 0 digits after it — no

**Checkpoint 1:** Which tens digit gives the smaller final number?
- (A) 5 → gives 158
- **(B) 0 → gives 108** ✓

**Checkpoint 2:** The smallest 3-digit number from 4921508 is ___. → **108**

---

### ✏️ Step 4 — "Name the removed digits"

- Kept: 1, 0, 8 (positions 4, 6, 7)
- Removed: 4, 9, 2, 5 (positions 1, 2, 3, 5)

**Checkpoint:** Which answer lists the four removed digits? → **(D) 4, 9, 2, 5**
*Hint: Kept digits are 1, 0, 8. Everything else in 4 9 2 1 5 0 8 was removed.*

---

## Block 5 — Practice Lab

| # | Type | Question | Answer | Difficulty |
|---|------|---------|--------|------------|
| P1 | ✏️v4 sort_order | Sam has digit tiles 4, 7, and 9. Drag them into Hundreds, Tens, Ones to make the BIGGEST number. | 974 | 3pt |
| P2 | MCQ | Which boy is wrong about 325? (Andy/Barry/Charlie/Danny/Eddie) | Eddie — digit 2 is even, not odd | 3pt |
| P3 | ✏️ fill_in_blank | What's the BIGGEST digit in 6\_3 that keeps it less than 670? | 6 | 3pt |
| P4 | ✏️v4 MCQ | Angie multiplied the wrong way — she divided her number by 10 instead. She got 600. What should the answer have been? | 60,000 (E) | 4pt |
| P5 | ✏️ fill_in_blank | In 528, how much MORE is the 5 worth than the 2? | 480 | 4pt |
| P6 | MCQ | David wrote a one-digit number. He put another digit to its right to make a two-digit number. He added 19. He got 72. What was David's first digit? | 5 (B) | 4pt |
| P7 | ✏️v4 MCQ | Steven writes digits 2, 0, 1, and 9 in the boxes: □□□ + □. He wants the BIGGEST total. Which digit goes in the separate box? | Either 0 or 1 (A) | 4pt |
| P8 | ✏️v4 sort_order | Tom has digit tiles 7, 0, 3, 5. Drag them to make the BIGGEST 4-digit number (0 can't go first). | 7530 | 4pt |

> **Format variety:** sort_order (P1, P8) · MCQ (P2, P4, P6, P7) · fill_in_blank (P3, P5)
> **Figure-based:** P1 (digit tile drag), P2 (number 325 / five boys), P5 (digit breakdown for 528), P7 (box diagram), P8 (digit tile drag) = 5/8 = 62.5% ≥ 50% ✓

---

### P4 — Full question (MK 2004 Q13, 4pt)

**Question:** Angie multiplied the wrong way. She divided her number by 10 instead of multiplying it by 10. As a result she got 600. What would the correct answer have been?

**Options:** (A) 6 / (B) 60 / (C) 600 / (D) 6,000 / **(E) 60,000** ✓

**Explanation:** Her number divided by 10 = 600, so her number = 6,000. The right answer: 6,000 × 10 = 60,000.

> ✏️v4 **Why P4 was replaced:** The original P4 ("add 17 to smallest 2-digit, divide by largest 1-digit") used the ÷ symbol in hint 2 and tested general arithmetic rather than place value. MK 2004 Q13 directly tests the lesson's core rule: each step left × 10. Going the wrong way (right instead of left) is the exact misconception this lesson targets.

---

### P7 — Full question (MK 2019 Q14, 4pt)

**Question:** Steven wants to write each of the digits 2, 0, 1, and 9 in one of the boxes of the addition: □□□ + □. He wants to get the BIGGEST possible total. Which digit goes in the separate box?

**Options:** **(A) Either 0 or 1** ✓ / (B) Either 0 or 2 / (C) Only 0 / (D) Only 1 / (E) Only 2

**Explanation:** To maximize, put 9 in hundreds. Then try: 921 + 0 = 921 and 920 + 1 = 921. Both give 921 — the max! So either 0 or 1 can go in the separate box.

> ✏️v4 **Why P7 was replaced:** The original P7 ("Leo inserts digit 5 into 37") was a custom problem that repeated the WE1 concept without adding new insight. MK 2019 Q14 pushes deeper: students must realize the hundreds place is 100× more valuable than the ones place, so the single box should hold the smallest digit. It's a much more revealing test of whether the lesson's concept landed.

---

### Hints

**P1** (sort_order)
1. Which tile is biggest — 4, 7, or 9? That one goes in hundreds.
2. 9 is in hundreds. Now sort the other two from biggest to smallest.
3. After 9 in hundreds and 7 in tens, only one tile is left — where does it go?

**P2**
1. Check each boy's claim one at a time.
2. Are all digits of 325 odd? What are the three digits?
3. The digits are 3, 2, and 5. Is 2 odd or even?

**P3**
1. Try a digit in the blank. Does it keep 6\_3 below 670?
2. Try digit 6: is 663 less than 670? Try digit 7: is 673 less than 670?
3. You tried 6 and 7. Only one of them kept the number below 670.

**P4**
1. She went the wrong direction on the place value ladder. She got 600.
2. What number, moved one place right, gives 600?
3. You found her original number. Now move it one place left.

**P5**
1. What is digit 5 worth in 528? What is digit 2 worth?
2. 5 is in hundreds → 500. 2 is in tens → 20. Now find the difference.
3. You have both values. Subtract the smaller from the larger.

**P6**
1. Work backwards: two-digit number = 72 − 19. What is that?
2. The first digit David wrote is the tens digit of that two-digit number.
3. What is the tens digit of the number you just found?

**P7**
1. Which place is worth more — hundreds or ones?
2. Put 9 in hundreds. What's the next best arrangement?
3. Try 920 + 1 and 921 + 0. Compare the totals.

**P8** (sort_order)
1. Which tile is biggest? That one goes in thousands.
2. 7 is first. Now sort the remaining tiles 5, 3, 0 from biggest to smallest.
3. With 7 in thousands, arrange 5, 3, 0 from biggest to smallest in the next three spots.

---

## Block 6 — Mastery Check

> 4 questions · No hints · Pass 3/4 to unlock Lesson 1.2

| # | Type | Question | Answer |
|---|------|---------|--------|
| MC1 | MCQ | ✏️ Digit tiles 6, 0, 4 are on your desk. What's the BIGGEST 3-digit number? | 640 (E) |
| MC2 | MCQ | ✏️ Digit tiles 3, 8, 1 are on your desk. What's the SMALLEST 3-digit number? | 138 (A) |
| MC3 | MCQ | ✏️ Maya arranges tiles 3, 6, 1. Which gives the SMALLEST number? | Hundreds=1, Tens=3, Ones=6 → 136 (A) |
| MC4 | MCQ | ✏️ David writes digit 4 next to digit 7, forming 74. What is 74 − (7 × 7)? | 25 (C) |

> ✏️ **MC3:** All 5 options updated from "U=X" to "Ones=X" (U is non-standard in US curriculum).
> ✏️ **MC4:** Now explicitly says "(7 × 7)" so there's zero ambiguity about which 7 to use.
> **Figure quota:** MC1 (digit tile figure), MC2 (digit tile figure), MC3 (arrangement figure) = 3/4 = 75% ≥ 50% ✓

---

## Block 7 — Challenge Extension (MK 1999 Q22) ⭐⭐⭐ 5pt

✏️v4 **Question:** One number was chosen from the numbers 51, 52, 53, 54, and 55. The digit 0 was placed between the two digits of that number. What is the difference between the new number and the original number?

**Options:** (A) 500 · (B) 50 · (C) 550 · **(D) 450** ✓ · (E) The difference depends on which number was chosen.

**Explanation:** Take 53 as an example. Insert 0 → 503. Difference: 503 − 53 = 450. Try 51: 501 − 51 = 450. Every number from the list gives the same answer — 450. Why? Original = 50 + ones. New = 500 + 0 + ones. Difference = 500 − 50 = 450. Always.

| Hint | Text |
|------|------|
| 1 | ✏️v4 Pick one number from the list. Insert 0 between its digits. |
| 2 | ✏️v4 Subtract the original from your new number. What do you get? |
| 3 | ✏️v4 Try a second number from the list. Do you get the same difference? |

> ✏️v4 **CE replaced:** MK 2007 Q16 was 4pt — violates Non-Negotiable Rule 5 (CE must be 5pt). MK 1999 Q22 is 5pt and is the most pedagogically powerful CE choice for this lesson: it directly tests what happens when 0 pushes a tens digit into hundreds (×10 shift), which is the exact core insight of Lesson 1.1. The twist — the difference is always 450 regardless of which number you pick — rewards deep place value thinking with a satisfying surprise.

---

## Summary of All Changes (v3 → v4)

| Location | Change | Why |
|----------|--------|-----|
| CF1 scenario | "number bag drops tiles" / code-breaker framing | More tactile and story-driven |
| CF2 type | fill_in_blank → MCQ | MCQ preferred; distractors reveal misconceptions |
| IL Step 4 visual | plain digit cards → combination lock | Left dial = most valuable; visceral + memorable |
| IL Step 10 reveal | plain table → "Case Closed" detective toolkit | Narrative payoff; ties back to CF framing |
| P1 type | MCQ → sort_order | Drag interaction is more engaging for digit arrangement |
| P4 question | MK 2002 Q12 (arithmetic, uses ÷ in hints) → MK 2004 Q13 | Directly tests the ×10 per column rule |
| P7 question | Custom insertion question → MK 2019 Q14 | Tests place-value priority more deeply |
| P8 type | MCQ → sort_order | Drag interaction; better for 4-digit arrangement |
| CE question | MK 2007 Q16 (4pt) → MK 1999 Q22 (5pt) | Fixes Non-Negotiable Rule 5 violation; more pedagogically rich |

### Code Bugs Fixed (carried from v3)
| Location | Bug | Fix |
|----------|-----|-----|
| WE1 `problem.figure` | Bare string path — figure invisible | Changed to `{ "src": "..." }` object |
| WE2 `problem.figure` | Bare string path — figure invisible | Changed to `{ "src": "..." }` object |
| IL Step 9 substep 1 | Missing `"type": "mcq"` | Added `"type": "mcq"` |
| Remediation options | ["047", "074", "407"] — shows invalid leading-zero strings | Changed to ["470", "704", "407"] |

### Language Fixes (carried from v3)
| Original | Improved | Why |
|----------|----------|-----|
| ÷ symbol | "×" framing only, or words ("divided by") | Grade 3 may not know division yet |
| H, T, U | Hundreds, Tens, Ones (full words) | U is undefined and non-standard |
| {set} curly braces | Plain comma-separated list | Middle-school notation, not Grade 3 |
| "adjacent" | "next to" | Adult vocabulary |
| "candidates" | "numbers still in the game" | Formal vocabulary |
| "eliminate" | "cross out" | More concrete action word |
| "decompose" | "break it apart" | Child-friendly |
| "leading-zero trap" | "the sneaky zero rule" | Playful and memorable |
| "Big lives left" | "Big ones go left" | "lives" reads as video game lives |
| Algebra variables X, Y, Z | Concrete example | Grade 6+ notation |
| Hints that reveal the answer | Directional nudges only | CUE format — ≤10 words, no answer |
