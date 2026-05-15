# Lesson 1.2 — Digit Sums & Digit Counts (Improved Version)

**ID:** `mk-f-digit-sums-reversals`
**Difficulty:** 3pt–4pt | **Time:** 25 min
**Skills:** Number Theory · Digits
**PYQ Sources:** MK 2015 Q06 (WE1) · MK 2002 Q09 (WE2) · MK 2000 Q03 · MK 2016 Q09 · MK 2007 Q11

> ✏️ marks every change. 🔴 marks critical code bug fixes. ➕ marks new steps added to fix flow gaps.

---

## Block 1 — Challenge First

> Students attempt cold. Hint ladder unlocks after 2 minutes.

### CF1 — Anna's house

**Type:** Fill in blank
✏️ **Question:** "Anna's street has houses numbered 50 to 59. Here's her clue: when you add all the digits of her house number together, the total is 13. Which house is Anna's? 🏠"
**Answer:** 58
**Explanation:** All houses 50–59 start with a 5. So 5 + ones digit = 13 → ones digit = 8 → Anna lives at number 58.
✏️ **On Wrong:** "Every house on Anna's street starts with a 5. So 5 + something = 13. What's the something?"
✏️ **Suggested figure:** `/figures/mk-grade-3-4/lesson-1-2/MK_L12_CF1_house_strip_50_59.svg` — a strip showing houses 50–59 with blank digit boxes

| Hint | Text |
|------|------|
| 1 | Anna's house starts with 5 — the tens digit is 5. |
| 2 | If 5 + ? = 13, what is the ones digit? |

> ✏️ **Key change:** Original used "digit sum" before the term is defined anywhere. Reworded to plain language: "add all the digits together." A student seeing this lesson for the first time won't know "digit sum" — they will know "add."
> ✏️ **Added:** `onWrong` feedback with a warm concept-specific nudge.
> ➕ **Suggested:** Add a house strip figure so students can see the range visually, not just imagine it.

---

### CF2 — How many 3s from 1 to 50?

**Type:** MCQ
✏️ **Question:** "The numbers from 1 to 50 are painted on mailboxes. How many times does the digit 3 appear — count every single 3 you see, not just every mailbox that has one."
**Options:** 13 / 14 / **15** ✓ / 16 / 25
**Explanation:** Ones-place 3s: 3, 13, 23, 33, 43 → 5 times. Tens-place 3s: 30, 31, 32, 33, 34, 35, 36, 37, 38, 39 → 10 times. Total = 15. (Mailbox 33 has two 3s — it contributes to both counts.)
✏️ **On Wrong:** "Count every 3 you SEE, not every house that contains a 3. Mailbox 33 has two 3s — does your count include both?"
✏️ **Suggested figure:** `/figures/mk-grade-3-4/lesson-1-2/MK_L12_CF2_number_grid_1_50.svg` — a 1–50 number grid

| Hint | Text |
|------|------|
| 1 | How many numbers from 1 to 50 end with the digit 3? |
| 2 | ✏️ You found the ones-place 3s. Now look at the tens column — which group of ten numbers has 3 as their tens digit? |

> ✏️ **Hint 2 rewritten:** Original said "Watch out — 33 has two 3s." That names the exact trap that makes this a 4pt question and removes all the thinking. New hint points to the tens column without naming the trap.
> ✏️ **Question reworded:** "Mailboxes" framing makes it tangible. The phrase "count every 3 you see, not just every house" pre-empts the most common mistake (treating each house as contributing at most one 3) without teaching the method.
> ➕ **Suggested:** A 1–50 number grid figure would let students see what they're counting, turning an abstract question into a visual one.

---

## Block 2 — Interactive Lesson: "From Sum to Scan"

> **Section A** (Steps 1–4): Digit Sum — add all digits, ignore place value.
> **Section B** (Steps 5–8): Digit Count in a Range — scan each position separately, then add.

---

### Step 0 — Predict: How many 1s from 1 to 20?

**Type:** Predict
**Question:** "Without listing them — take a guess. How many times does the digit 1 appear in the numbers from 1 to 20?"
**Answer:** 12 *(proceed regardless)*
**Visual:** Number list 1–20 with digit 1 highlighted

- ✅ **Correct:** "Sharp — you spotted that 11 has two 1s, not one. That's the key insight of this whole section."
- ✏️ ❌ **Wrong:** "A common answer is 11 — but count again. How many 1s does the number 11 itself have?"

> ✏️ **Fixed:** Original said "Most folks guess 11" — a demographic claim that confuses students who guessed differently. Replaced with "A common answer is 11" and redirected to the double-digit trap specifically.

---

### Step 1 — Explain: What's a digit sum?

✏️ **Title:** "Meet the digit sum — the laziest operation in maths."
✏️ **Text:** "Add up every digit. Ignore place value. That's the whole rule. For 374: 3 + 7 + 4 = 14."
**Visual:** Digit-sum breakdown for 374
✏️ **Key Insight:** "Same digits = same digit sum, always. 374, 437, and 743 are different numbers — but all have digit sum 14."
**End Question:** Digit sum of 528 = ___. → **15**
*Hint:* ✏️ "Add the digits one at a time: start with 5."

> ✏️ **Title changed:** "Section A — Digit sum: definition" is a textbook chapter heading, not a child-facing title. New title creates a small smile and sets expectations.
> ✏️ **Text shortened:** Original was accurate but read like a definition in a dictionary. New version is a command ("Add up every digit") followed by a single example.
> ✏️ **Hint fixed:** Original: "5 + 2 + 8 = ?" writes the full operation — student just reads it. New hint starts them at 5 without completing the sum for them.

---

### Step 2 — Apply: You're the detective

✏️ **Title:** "You're the detective — find the digits."
✏️ **Text:** "I know the digit sum but not the number. A 2-digit number has digit sum 11, and one digit is 6. What's the other digit?"
**Visual:** Digit card row [6, ?], label "digit sum = 11"

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | The other digit is ___. | 5 | 6 + ? = 11. |

✏️ **Substep 2 (FIXED — moved from broken `followUp`):**
*"Both 56 and 65 have digit sum 11. Which of these numbers also use only the digit 6 and one other digit?"*

| Substep | Prompt | Options | Answer |
|---------|--------|---------|--------|
| 2 | Which of these have digit sum 11 AND use a 6? (Pick all.) | 56 / 65 / 50 / 61 / 11 | 56 and 65 |

**Explanation for Substep 2:** Both 56 and 65 work. The order of digits doesn't change the sum — but it completely changes the number.

- ✅ **All correct:** "Digit sum doesn't care about order. But the number itself does. Now — what if the constraint asks for the *smallest* number possible?"

> 🔴 **Code bug fixed:** Original had a `followUp` field containing a `cloze_drag` question. The `apply` step schema has no `followUp` field — this question silently never rendered. Every student skipped the "multiple valid numbers share a digit sum" insight entirely. The content has been moved into a proper second substep inside the `steps` array where it will actually render.
> ✏️ **Title changed:** "Section A — Reverse the operation" is adult language. "You're the detective" frames it as a puzzle, not a technique exercise.

---

### ➕ NEW Step 2.5 — Explain: Building the SMALLEST number

> **This step did not exist in the original.** It is essential — Step 3's applet assumes this rule but never teaches it.

✏️ **Title:** "Build small: which slot goes first?"
✏️ **Text:** "To make the SMALLEST 3-digit number with a given digit sum, put the smallest digit you can in the hundreds place. But hundreds can NEVER be 0 — that would make it a 2-digit number!"
**Visual:** 3-slot number builder: [1] [0] [4] = 104, label "digit sum = 5"
✏️ **Key Insight:** "Smallest hundreds = smallest number. But 0 can never go in hundreds!"
**End Question:** "Smallest 3-digit number with digit sum 7 = ___." → **106**
*Hint:* "Try putting 1 in hundreds. What's the smallest way to spread the remaining 6 across tens and ones?"

> ➕ **Why this step is needed:** The original Step 3 applet says in its instruction: "To minimise a 3-digit number, push the small digits to the leftmost slot." This rule appears exactly once, in instruction text that students typically skim. Without a dedicated explanation step, students arrive at Step 3's interactive exercise not knowing what they're being asked to do or why. This new step teaches the rule explicitly with a worked visual before asking students to apply it.

---

### Step 3 — Apply: Smallest 3-digit number with digit sum 5

✏️ **Title:** "Build the smallest — digit sum 5"
✏️ **Type changed from `applet` → `apply`** *(code bug fix — see below)*
✏️ **Text:** "Digit sum = 5. You need three digits that add up to 5. Make the number as small as possible."
**Visual:** 3-slot number builder for digit sum 5

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | Hundreds digit (smallest it can be) = ___ | 1 | If hundreds = 0, the number would only have 2 digits! |
| 2 | Tens digit (keep it as small as possible) = ___ | 0 | Hundreds took 1. You still need 4 more — where do you push it? |
| 3 | Ones digit = ___ | 4 | 1 + 0 + ___ = 5. |

- ✅ **All correct:** "104! The trick: smallest allowed digit in hundreds (that's 1), then pack the leftover sum into ones."

> 🔴 **Critical code bug fixed:** Original used `"appletType": "digit-card-builder"` — this applet type is NOT registered in the CMS. It rendered as "Unknown applet type" and students could not proceed. This blocked access to ALL content after Step 3: Steps 4–8, both Worked Examples, the Practice Lab, Mastery Check, and Challenge Extension — completely unreachable. Converted to a plain `apply` step with the same three fill-in-blank substeps. Content preserved, progression restored.

---

### Step 4 — Apply: Which has the BIGGEST digit sum?

✏️ **Title:** "No calculator needed — just look!"
✏️ **Text:** "One of these four numbers has the biggest digit sum. Can you spot it without adding anything?"
**Visual:** Digit cards [123, 540, 999, 765]
✏️ **End Question type:** MCQ (type: "mcq" added — see bug fix below)
**Question:** "Which 3-digit number has the largest digit sum?"
**Options:** 123 / 540 / **999** ✓ / 765
**Explanation:** 9+9+9 = 27 is the maximum possible digit sum for a 3-digit number. No other option can match three 9s.
*Hint:* ✏️ "Look at each digit of 999. Can any other option match all three of those digits?"

> 🔴 **Code bug fixed:** Original `endQuestion` had `"inputType": "choice"` but no `"type": "mcq"`. The CMS question router dispatches on the `type` field — without it, the choice question may not render. Added `"type": "mcq"`.
> ✏️ **Hint fixed:** Original: "All-9s beats anything else" — identifies 999 directly. New hint triggers the inspection without naming the answer.
> ✏️ **Title and text:** Made them feel like a puzzle challenge, not a procedure to follow.

---

### ➕ NEW Step 4.5 — Bridge: From one number to a whole range

> **This step did not exist in the original.** Without it, students jump from "digit sum of one number" to "count a digit across 50 numbers" with zero preparation.

✏️ **Title:** "Plot twist — the question flips."
✏️ **Type:** predict (proceedRegardless: true)
✏️ **Text:** "You've been adding digits inside ONE number. Now flip the question: instead of 'what's the digit sum of 374?' — imagine asking 'how many times does the digit 3 appear when you write ALL numbers from 1 to 50?'"
✏️ **Note to student:** "Sound familiar? That was CF2 at the very start. You had to guess. Now you'll get the exact method."
**Prompt:** "Take your best guess — how many 3s from 1 to 50? ___"
*(Answer: 15. proceedRegardless: true)*
- ✅ **Correct:** "You had the right answer at the start! Now let's see WHY."
- ❌ **Wrong:** "The answer is 15 — and you're about to see exactly why. Let's unlock the method."

> ➕ **Why this step is needed:** Step 4 ends Section A (digit sum of ONE number). Step 5 begins Section B (count a digit across a RANGE). These are fundamentally different operations. Without this bridge, the jump is disorienting — students don't know why the lesson has suddenly changed topic. This step creates the "aha" connection: CF2 at the start of the lesson was secretly a Section B question. Students who get here feel a satisfying loop closing.

---

### Step 5 — Explain: Scan by position, not by number

✏️ **Title:** "The position scan — your superpower for counting."
✏️ **Text (BROKEN INTO 3 BEATS — 55-word text wall replaced):**

**Beat 1:** "Start with the ones column. How many numbers from 1 to 20 have a 1 in the ones place?"
→ *Student fills in: 2* (numbers: 1 and 11)

**Beat 2:** "Now the tens column. How many numbers from 10 to 19 have a 1 in the tens place?"
→ *Student fills in: 10* (numbers: 10, 11, 12, 13, 14, 15, 16, 17, 18, 19)

**Beat 3:** "The number 11 appeared in both lists. Is that a mistake?"
→ *MCQ: (A) Yes, count it once / (B) No, count it twice — it has two 1s*
→ **Answer: (B)**

**Visual:** Digit-count breakdown visual for digit 1 in 1–20

✏️ **Key Insight:** "Scan ones first. Scan tens next. Then add. Numbers like 11 get counted in both scans — that's right, because 11 has two 1s!"

✏️ **End Question (FIXED — plain fill-in-blank):**
"Ones-place 1s + Tens-place 1s = Total 1s in 1–20 = ___."
→ **12**

> 🔴 **Code bug fixed:** Original `endQuestion` used a `sort_order` schema. The `explain` step renderer expects a `blank`-style schema. `sort_order` has no `blank` field and would likely not render. Changed to a simple fill-in-blank.
> ✏️ **Text wall broken up:** Original was 55 words delivering the complete technique before any student interaction. Rebuilt as 3 beats, each ending in a student action. Students *discover* the method rather than *receive* it.
> ✏️ **Removed:** Curly brace notation `{1, 11}` (set notation, not Grade 3 language). Now says "the numbers 1 and 11."
> ✏️ **Removed:** `keyInsight` that was a verbatim duplicate of the last sentence of `text`. New key insight is distinct and adds the synthesis.

---

### Step 6 — Apply: How many 7s from 1 to 50?

**Title:** "Use the scan — count every 7 from 1 to 50."
**Text:** "Same method — scan ones, then tens, then add."
**Visual:** Number grid 1–50, digit 7 highlighted

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | Ones-place 7s = ___ | 5 | ✏️ Which number between 1 and 50 ends in 7? Start at 7 and count up in tens. |
| 2 | Tens-place 7s = ___ | 0 | Range stops at 50. There are no numbers in the 70s. |
| 3 | Total 7s from 1 to 50 = ___ | 5 | ✏️ Add your ones count and your tens count. |

- ✅ **All correct:** "5 sevens. Clean and fast. Now try a digit where a double shows up — watch what happens at 44."

> ✏️ **All hints rewritten:** Original hints gave complete lists (7, 17, 27, 37, 47) and direct arithmetic (5 + 0). Replaced with directional CUEs that prompt the process without completing it.

---

### Step 7 — Apply: How many 4s from 1 to 50? (The trap!)

**Title:** "Same method — but 44 has a surprise."
**Text:** "Count every 4 from 1 to 50. Watch what happens when you reach 44."
**Visual:** Number grid 1–50, digit 4 highlighted, callout on 44: "Two 4s — both count!"

| Substep | Prompt | Answer | Hint |
|---------|--------|--------|------|
| 1 | Ones-place 4s = ___ | 5 | ✏️ Which numbers between 1 and 50 end in 4? Start at 4 and jump up in tens. |
| 2 | Tens-place 4s = ___ | 10 | ✏️ Which group of ten numbers has 4 as the tens digit? |
| 3 | Total 4s from 1 to 50 = ___ | 15 | ✏️ Add your ones count and your tens count. You counted 44 in both scans — that's intentional. It has two 4s. |

- ✅ **All correct:** "15 fours — and 44 contributed two of them. The position scan handled it automatically. If you got 14, you counted 44 once instead of twice."

> ✏️ **All hints rewritten:** Every original hint gave the full answer list (4, 14, 24, 34, 44 — entire list; 40–49 — entire list; 5+10 with full explanation). Replaced with directional CUEs.

---

### Step 8 — Reveal: Two techniques, one habit

**Title:** "Two techniques, one habit."

| Technique | Rule | Example |
|-----------|------|---------|
| ✏️ Digit sum | Add all digits. Ignore place value. | 374 → 3 + 7 + 4 = 14 |
| ✏️ Digit count in range | Scan ones, then tens. Add the counts. | 1s in 1–20 → 2 + 10 = 12 |
| ✏️ The double-digit trap | A digit can appear twice in one number (33, 44, 22). Count both. | 44 contributes 2 to the 4-count from 1–50 |

**Closing Checkpoint (match pairs):**

| Left | Right |
|------|-------|
| Add the digits | Digit sum problem |
| Scan by position | Digit count in a range |
| Both digits count | Numbers like 44, 33, 22 |

✏️ **Curiosity Bridge (FIXED — removed ÷ symbol):**
"Quick challenge: start at 5, add 3, then double the result. What do you get? ___"
→ **Answer: 16**
→ Reveal: "16! That's chaining — each step feeds into the next. Lesson 1.3 is all about chaining operations without losing track. Ready to test your chains? →"

> ✏️ **Curiosity bridge fixed:** Original used `(10 + 17) ÷ 9` — division symbol in a lesson that precedes any formal division content. Also felt arbitrary (no connection to digit sums). New bridge uses simple addition + multiplication, previews Lesson 1.3's chaining theme, and is doable by any Grade 3 student.

---

## Block 3 — Worked Example 1 (MK 2015 Q06) ⭐ 3pt

**Problem:** A certain whole number has two digits. The product of the digits is 15. The sum of the digits is:
**Options:** 2 / 4 / 6 / 7 / **8** ✓

---

### ✏️ WE1 Step 1 — "Find the factor pair"

*(Was: "Read the constraint")*
**Narrative:** "Two digits, product = 15. Don't jump to the sum yet — find the digits first. Which pairs of single digits multiply to give 15?"

**Checkpoint (simplified):**
✏️ "Which pair of single-digit numbers multiplies to give 15?"
- **(A) 3 and 5** ✓
- (B) 1 and 15
- (C) 2 and 8
- (D) 5 and 5

*Hint:* "Single digits are 1 through 9. Test 3 × 5 — does it work?"
*Explanation:* "Only 3 × 5 = 15 works using two single digits. (1 × 15 doesn't count — 15 is not a single digit.)"

> ✏️ **Step redesigned:** Original had a `sort_order` drag with 4 items including BOTH `3 × 5` and `5 × 3` as separate chips. For a Grade 3–4 student, these look nearly identical and the need to classify both separately is confusing. Simplified to a direct MCQ that makes the key point cleanly: only 3 and 5 work as single-digit pairs.

---

### ✏️ WE1 Step 2 — "Which numbers could it be?"

*(Was: "Identify the candidates" — "candidates" is prohibited jargon)*
**Narrative:** "Digits are 3 and 5. So the two-digit number is either 35 or 53."

**Checkpoint (FIXED — type changed):**
✏️ "Which of these have a digit product of exactly 15? (Pick all that apply.)"
- **35** ✓ (3 × 5 = 15)
- **53** ✓ (5 × 3 = 15)
- 15 (1 × 5 = 5 ✗)
- 51 (5 × 1 = 5 ✗)
- 13 (1 × 3 = 3 ✗)

*Hint:* "Multiply the two digits of each number. Which ones give 15?"
*Explanation:* "3 × 5 = 15 ✓ (both 35 and 53). 1 × 5 = 5 ✗. 5 × 1 = 5 ✗. 1 × 3 = 3 ✗."

> 🔴 **Code bug fixed:** Original used `"type": "mcq_multi"` with `"answers": [0, 1]` (an array). `mcq_multi` does not appear elsewhere in the course — unconfirmed in the question router. If unregistered, this checkpoint would crash or render as unknown, blocking WE1 entirely. Changed to a standard `cloze_drag` or multi-select `mcq` using the confirmed schema. The `answers` field must be an array of the correct string values, not index integers.

---

### WE1 Step 3 — Compute the digit sum

**Narrative:** "Both 35 and 53 use digits 3 and 5 → digit sum = 3 + 5 = 8. The order doesn't matter for the sum."
**Checkpoint:** Digit sum of 35 (or 53) = ___. → **8**
*Hint:* 3 + 5 = ?

---

### WE1 Step 4 — The big idea

**Narrative:** "You never needed to know whether the number was 35 or 53. Both share the same digit sum. That's the digit-sum mindset: think about the digits, not the number."
**Checkpoint:** "Why do 35 and 53 have the same digit sum?"
- (A) Coincidence — it usually works out differently.
- **(B) Digit sum doesn't depend on the order of digits.** ✓
- (C) 35 and 53 are equal.

*Hint:* "Adding 3 + 5 vs adding 5 + 3 — same operation?"
**Insight:** "Digit sum is order-independent. Find the digits first; the sum follows."

---

## Block 4 — Worked Example 2 (MK 2002 Q09) ⭐⭐ 4pt

**Problem:** The houses on the street where John lives are numbered from 1 to 24. How many times does the digit 2 appear in the numbering of these houses?
**Options:** 2 / 4 / **8** ✓ / 16 / 32

> 🔴 **Code bug fixed:** Original `problem.figure` was a bare string path: `"/figures/.../MK_L12_WE2_houses_1_24_grid.svg"`. The CMS renderer reads `figure.src` — a bare string has no `.src` property, so the house grid was invisible when students first saw the problem. Fixed to `{ "src": "/figures/..." }` object format.

---

### WE2 Step 1 — Set up the position scan

**Narrative:** "Don't list every 2 by hand — that's slow and easy to miss. Instead, scan by position. First: which houses have a 2 in the ones place?"
**Figure:** House grid 1–24
**Checkpoint (cloze_drag):** Drag house numbers with a 2 in the ones place.
**Chips:** 2 / 7 / 12 / 14 / 22 / 23
**Correct:** 2, 12, 22
*Hint:* "Ones place = rightmost digit. Which chips end in 2?"

---

### WE2 Step 2 — Count ones-place 2s

**Narrative:** "Three houses have 2 in the ones place: 2, 12, 22."
**Checkpoint:** Ones-place 2s in houses 1–24 = ___. → **3**
*Hint:* "Count the chips you just placed."

---

### WE2 Step 3 — Switch to the tens-place scan

**Narrative:** "Now scan the tens column. Houses with a 2 in the tens place are in the 20s — but the street only goes up to 24."
**Checkpoint (cloze_drag):** Drag house numbers with a 2 in the tens place.
**Chips:** 12 / 20 / 21 / 22 / 23 / 24 / 25
**Correct:** 20, 21, 22, 23, 24
✏️ *Hint:* "Cover the ones digit of each chip with your finger. Which chips show a 2 when you do that? (And the street only goes to 24 — so 25 doesn't exist!)"

> ✏️ **Hint improved:** Original hint said "Tens digit = the digit before ones. Which chips have 2 right before their ones digit?" — "right before" is ambiguous for Grade 3–4. New hint uses a physical action (cover the ones digit) which is concrete and unambiguous.

---

### WE2 Step 4 — Count tens-place 2s and confront the trap

**Checkpoint 1:** Tens-place 2s in houses 1–24 = ___. → **5**
*Hint:* "Count the chips you just placed."

**Narrative:** "Now — house 22 has a 2 in BOTH the ones place AND the tens place. How do we count it?"

**Checkpoint 2:** "House 22 has two 2s. How many times should we count it?"
- (A) Once — it's the same house.
- **(B) Twice — it has two 2s, one in each position.** ✓
- (C) Don't count it — it's confusing.

*Hint:* "We're counting digit appearances, not house appearances. How many '2' digits does the number 22 have written in it?"
*Explanation:* "The number 22 is written with two '2' characters. Our position scan already handles this correctly — it counted 22 once in the ones scan and once in the tens scan."

> ⚠️ **Note on option figures:** Original referenced three SVG files for this checkpoint's options (once/twice/neither). If these files don't exist, options render with broken images. Verify: `MK_L12_WE2_opt_22_once.svg`, `MK_L12_WE2_opt_22_twice.svg`, `MK_L12_WE2_opt_22_neither.svg`.

---

### WE2 Step 5 — Add the scans

**Narrative:** "Total = ones (3) + tens (5) = 8. House 22 was counted once in each scan — correctly, because it has two 2s."
**Checkpoint:** Total digit-2 count from house 1 to house 24 = ___. → **8**
*Hint:* "3 + 5."
*Explanation:* "Sanity check by listing: 2, 12, 20, 21, 22 (×2), 23, 24 → 1+1+1+1+2+1+1 = 8. ✓"
**Insight:** "Position scan turns 'count occurrences' into two simple sub-counts — and handles double-digit numbers (22, 33, 44) automatically."

---

## Block 5 — Practice Lab

| # | Type | Question summary | Answer | Difficulty |
|---|------|-----------------|--------|------------|
| P1 | Fill in blank | Digit sum of 478 | 19 | 3pt |
| P2 | MCQ | Which number has digit product > digit sum? | 222 (D) | 3pt |
| P3 | MCQ | Which 3-digit number has the largest digit sum? | 988 (C) — 9+8+8=25 | 3pt |
| P4 | MCQ | Next year after 2016 with digit sum 9 | 2025 (B) | 4pt |
| P5 | MCQ | Smallest number > 2007 with same digit sum as 2007 | 2016 (A) | 4pt |
| P6 | Fill in blank | How many times does digit 7 appear from 1 to 100? | 20 | 4pt |
| P7 | Sort order | Order 624, 333, 587, 901 by digit sum | 333, 901, 624, 587 | 4pt |
| P8 | MCQ | How many times does digit sum = 1 on a 24h digital clock? | 4 (D) | 4pt ★ |

---

### P1 Hints
1. Add the three digits on the cards.

---

### P2 Hints
1. Compute the digit product AND the digit sum for each option.
2. ✏️ Before you multiply all three digits of an option, check: does any digit make the product very easy to figure out?

> ✏️ **H2 rewritten:** Original: "Watch out for any option containing a 0 — its digit product is automatically 0." Directly eliminates option B (209) by naming the rule. New hint prompts the student to notice zero without naming it or the conclusion.

---

### P3 Hints
1. Add the digits for each option. Which total is biggest?
2. 991 has a 1 in it — that's a small digit dragging the sum down.

---

### P4 Hints
*(P4 is a wonderful real-world question — digit sums of years!)*
1. Test each option after 2016: add its digits. Which gives 9?
2. ✏️ We want the SMALLEST year AFTER 2016 with digit sum 9. If two options both have digit sum 9, which comes earlier?

---

### P5 Hints
1. ✏️ First, work out the digit sum of 2007. Then test each option — which ones match that sum AND are bigger than 2007?
2. ✏️ Two conditions: digit sum matches AND the year is after 2007. Among all options that pass both tests, pick the smallest.

> ✏️ **Hints improved for P4 and P5:** Originals were fine but didn't remind students of the "two filter" nature of the problem. Added clarity.

---

### P6 Hints
1. Scan ones-place first: which numbers from 1–100 end in 7? Count them.
2. Now scan tens-place: which numbers have 7 in the tens spot? Watch out — 77 belongs in both scans.

---

### P7 Hints
1. Compute the digit sum of each number first. Don't compare the numbers themselves.
2. ✏️ Compute the digit sum of 333. Does it beat any of the other three?

> ✏️ **H2 rewritten:** Original: "Smallest sum: 333 → 3+3+3=9. Largest: 587 → 5+8+7=20." Reveals both endpoints of a 4-item sort — leaves only 2 items for the student to figure out. New hint starts them at one endpoint without completing the ordering.

---

### P8 Hints
*(P8 is the most creative problem in the lab — a real gem)*
1. Digit sum of all four clock digits = 1 means exactly one digit is 1 and the other three are 0.
2. ✏️ Try putting the digit 1 in each of the four positions of HH:MM — one at a time. For each, check: is it a valid clock time?

> ✏️ **H2 improved:** Original was essentially the same idea but less directed. New hint gives the systematic method (try each position in turn) and adds the validation check.

---

## Block 6 — Mastery Check

> 3 questions · No hints · Pass 2/3 to unlock Lesson 1.3

| # | Question | Answer |
|---|---------|--------|
| MC1 | Digit sum of 3628 | 19 |
| MC2 | In which range does digit 5 appear exactly 6 times? | 1 to 50 (C) |
| MC3 | 2-digit number: digits multiply to 12 AND add to 7. Smallest such number? | 34 |

**MC3 working:** Digit pairs with product 12: (3,4), (4,3), (2,6), (6,2). Filter by sum = 7: only (3,4) qualifies. Numbers: 34 and 43. Smallest = 34. ✓

---

## Block 7 — Challenge Extension ⭐⭐⭐ 5pt

**Problem:** "I'm thinking of a 3-digit number. Its hundreds digit is twice its tens digit. Its tens digit is 1 more than its ones digit. The digit sum equals 11. What is the number?"
**Answer:** 632

### CE1 Hints (COMPLETELY REWRITTEN)

| Hint | Text |
|------|------|
| 1 | ✏️ Start by guessing the ones digit — try 1. If ones = 1, what would tens be? What would hundreds be? |
| 2 | ✏️ Ones = 1 → tens = 2 → hundreds = 4. Add them: 1 + 2 + 4 = 7. Too small! Try ones = 2. |
| 3 | ✏️ If ones = 2: tens = 3, hundreds = 6. Add: 2 + 3 + 6 = ? |

**Explanation (REWRITTEN):**
Try ones = 1: tens = 2, hundreds = 4. Sum = 7. Too small.
Try ones = 2: tens = 3, hundreds = 6. Sum = 11. ✓ Check: hundreds is twice tens (6 = 2×3 ✓). Tens is 1 more than ones (3 = 2+1 ✓). Answer: 632.

> 🔴 **CE1 completely redesigned:** All three original hints and the explanation used algebra (`let x`, `4x + 3 = 11`, `solve for x`) — this is CCSS 6.EE.B.7, Grade 6 content, entirely out of scope for Grade 3–4. A high-performing Grade 3–4 student does not need algebra to solve this problem. Trial-and-check (try ones = 1, try ones = 2, …) solves it in two steps. The hints now walk through exactly that — no letters, no equations, just systematic guessing with checking.
> ✏️ The problem itself is excellent — keep it. Only the hints and explanation needed a rethink.

---

## Summary of All Changes

### Code Bugs Fixed (6)

| Location | Bug | Effect | Fix |
|----------|-----|--------|-----|
| IL Step 3 | `appletType: "digit-card-builder"` not registered in CMS | "Unknown applet type" — blocks ALL content after Step 3 | Convert to `apply` step with same 3 fill-in-blank substeps |
| IL Step 2 | `followUp` field not in `apply` step schema | cloze_drag question silently never renders — students miss key insight | Move content into a second substep inside `steps` array |
| IL Step 5 | `endQuestion` uses `sort_order` schema | `explain` renderer expects `blank` schema — end question likely doesn't render | Convert to fill-in-blank |
| IL Step 4 | `endQuestion` has `inputType: "choice"` but no `type: "mcq"` | CMS question router may not render the choice question | Add `"type": "mcq"` field |
| WE1 Step 2 | `type: "mcq_multi"` unconfirmed in question router | May crash or show as unknown — blocks WE1 Step 2 | Convert to confirmed question type with equivalent functionality |
| WE2 problem | `figure` is bare string, not `{ "src": "..." }` object | Problem figure invisible when question first shown | Change to `{ "src": "/figures/..." }` |

### New Steps Added (2)

| Step | Position | Purpose |
|------|----------|---------|
| Step 2.5 — "Build small: which slot goes first?" | Between Step 2 and Step 3 | Teaches the minimisation rule that Step 3 assumes but never explains |
| Step 4.5 — "Plot twist — the question flips." | Between Step 4 and Step 5 | Bridges Section A (digit sum) and Section B (digit count in range); reconnects to CF2 |

### Language Fixes (every instance)

| Original | Improved | Why |
|----------|----------|-----|
| "digit sum" in CF1 (undefined term) | "when you add all the digits together" | Term hasn't been taught yet — plain language first |
| 55-word text wall in Step 5 | 3 short beats, each with a student action | Students receive a lecture instead of discovering — rebuilt as interactive |
| "Section A — Digit sum: definition" | "Meet the digit sum — the laziest operation in maths." | Chapter heading vs engaging hook |
| "candidates" (WE1 Step 2 title) | "Which numbers could it be?" | Formal jargon, not Grade 3–4 language |
| `{1, 11}` curly brace notation in Step 5 | "the numbers 1 and 11" | Set notation is middle-school level |
| `keyInsight` duplicating `text` verbatim | Distinct insight added | Duplication wastes the insight box |
| CE1 hints using `let x`, algebra equations | Trial-and-check hints (try ones = 1, 2, 3…) | CCSS 6.EE.B.7 is Grade 6 — out of scope |
| Curiosity bridge using `÷` symbol | Chain arithmetic with × only (5 + 3, then ×2) | Division may not be formally introduced yet |
| "Most folks guess 11" (demographic claim) | "A common answer is 11 — but count again" | If student guessed 8 or 15, original feedback is confusing |

### Hints Audited and Fixed (9 of 19 were answers → now CUEs)

| Location | Was | Now |
|----------|-----|-----|
| CF2 H2 | Named the 33 double-digit trap | Points to tens column without naming the trap |
| IL Step 1 endQ hint | "5 + 2 + 8 = ?" (full operation) | "Add one at a time: start with 5." |
| IL Step 4 endQ hint | "All-9s beats anything else." (names answer) | "Can any option match all three digits of 999?" |
| IL Step 6 substep 1 | Listed 7, 17, 27, 37, 47 in full | "Start at 7 and count up in tens." |
| IL Step 6 substep 3 | "5 + 0." | "Add your ones count and your tens count." |
| IL Step 7 substep 1 | Listed 4, 14, 24, 34, 44 in full | "Start at 4 and jump up in tens." |
| IL Step 7 substep 2 | Listed 40–49 in full (10 numbers) | "Which group of ten has 4 as the tens digit?" |
| IL Step 7 substep 3 | "5 + 10. 44 was counted in both…" (full answer + explanation) | "Add counts. Did you count 44 twice? That's intentional." |
| P2 H2 | Named the zero-product rule for option B | "Does any digit make multiplication very easy?" |
| P7 H2 | Revealed both endpoints of 4-item sort | "Compute 333's sum first. Does it beat the others?" |
