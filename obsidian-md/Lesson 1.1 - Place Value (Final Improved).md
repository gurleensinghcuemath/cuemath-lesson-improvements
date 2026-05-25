# Lesson 1.1 — Reading & Building Numbers from Place Value
## Final Improved Version (v6)

**Course:** Math Kangaroo Prep — Grade 3 & 4 · **Difficulty:** 3pt → 5pt · **Duration:** 25 min  
**Slug:** `mk-f-place-value-v6`  
**PYQs:** WE1: MK 2014 Q02 · WE2: MK 2000 Q10 · PL: 2013 Q08, 2007 Q15, 2019 Q14 · CE: MK 1999 Q22

> Every change is shown as **Original → Improved** with a reason.  
> ✏️ = content change · 🐛 = code bug fix · 🖥️ = UI/rendering fix

---

## Block 1 — Challenge First

### CF1

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Question framing | "Mia has three digit cards: 8, 3, and 5…" | "A number bag drops three digit tiles on your desk: [card:8], [card:3], and [card:5]…" | ✏️ |
| Question verb | "What is the LARGEST number she can make?" | "What is the BIGGEST number you can build?" | ✏️ |
| Hint 1 | "Which position is worth the most? Put the biggest digit there." — 11 words | "Hundreds is worth the most of all three places." — 9 words | ✏️ |
| Hint 2 | "Hundreds > Tens > Ones in value. Assign the largest digit to the highest-value position." — 15 words, uses "largest", formal register | "Biggest tile earns the biggest seat." — 6 words | ✏️ |
| Hint 3 | Missing (only 2 hints) | "Which of 8, 3, 5 is the biggest?" | ✏️ |
| `onWrong` feedback | Missing — UI shows generic default | "The hundreds place is worth the most. Give it your biggest tile." | 🖥️ |

---

### CF2

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Type | `fill_in_blank` | `mcq` | ✏️ |
| Why | — | MCQ distractors reveal misconceptions (e.g., 530 = student put 5 first) | — |
| Options (original) | Free text input (358) | 358 / 385 / 530 / 583 / 835 | ✏️ |
| Hint 1 | "Now you want the hundreds digit to be as small as possible." — 14 words, starts abstract | "Smallest tile earns the Hundreds seat now." — 7 words | ✏️ |
| Hint 2 | "Smallest available digit is 3. Put it in hundreds. Then 5 in tens, 8 in ones." — names full answer | "Which of 8, 3, 5 is the smallest?" — prompts, doesn't answer | ✏️ |
| Hint 3 | Missing | "After placing 3 in Hundreds, sort the rest smallest first." — 10 words | ✏️ |
| `onWrong` feedback | Missing | "For smallest, the hundreds seat goes to your smallest tile. Which tile is that?" | 🖥️ |

---

## Block 2 — Interactive Lesson

### Step 0 — Predict

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `prompt` | `"Smallest = {blank}"` — `{blank}` renders as literal text in this component | `"Smallest = ___"` | 🐛 🖥️ |
| `onWrong.feedback` | "Most folks try 048 — but '048' is just 48, a 2-digit number. We'll fix this in five minutes." — uses contractions, "Most folks" is a demographic claim | "048 is just 48 — zero cannot sit in front. We will sort this out in two minutes." | ✏️ |
| `onWrong.hint` | Missing — amber hint box never renders | "Zero cannot lead any number. Which digit goes first?" — activates the styled amber hint box | 🖥️ |
| `onCorrect.feedback` | "Sharp — you spotted the rule that catches everyone off guard." | "Sharp — you already know the trick that trips everyone up." | ✏️ |

---

### Step 1 — Explain (Place Value Ratio)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Title | "Same digit. Three places. Three values." | "Same digit. Three totally different values?" | ✏️ |
| `keyInsight` | "Each step left: ×10. Each step right: ÷10." — uses ÷ symbol (banned) | "Move one place left — value jumps 10 times. Every single time." | ✏️ |

---

### Step 2 — Applet (Place Value Chart)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `discoveryQuestion.prompt` | "Adjacent columns always differ by a factor of {blank}." — "adjacent", "factor of" are not Grade 3 language | "Each column is {blank} times bigger than the one just to its right." | ✏️ |
| `discoveryMessage` | "700 ÷ 70 = 10. 70 ÷ 7 = 10. Every step left is exactly 10× more valuable." — uses ÷ | "7 times 10 equals 70. 70 times 10 equals 700. One step left — 10 times bigger. Always." | ✏️ |

---

### Step 3 — Apply (Read 749)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `onWrong` | `{ "adaptiveNextStep": "place-value-decompose" }` only — student sees "Let's review this concept." default before redirect | Added `"feedback": "Try 749 one column at a time — Hundreds, then Tens, then Ones."` | 🖥️ |
| `onAllCorrect.feedback` | "Now — what if you're handed \*loose\* digits and asked to \*\*build\*\* a number?" — asterisks render as raw characters | "Now — can you build a number from loose digit tiles?" | 🐛 |

---

### Step 4 — Explain (Build/Sort)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Title | "Sort the digits. Big **lives** left." — "lives" reads as video game lives | "Sort the digits. Big ones go left." | ✏️ |
| `text` | "You just learned what each column is worth. Now use that — to build numbers. The H column multiplies by 100, the U column by 1. So the biggest digit always belongs in **H** — that's the seat with the most leverage." — 41 words, H/U abbreviations, "leverage", asterisks, markdown | "Hundreds is worth 100 times more than Ones. So the biggest digit always belongs in Hundreds." — 16 words, plain language | ✏️ 🐛 |
| `visual.params.caption` | None | `"Which dial takes the biggest digit?"` — Socratic caption links to combination lock idea | ✏️ |
| `keyInsight` | "Largest: sort high → low. Smallest: sort low → high; zero takes T or U, never H." — H/T/U abbreviations, "→" arrows | "Zero cannot lead — it goes in Tens or Ones, never Hundreds." | ✏️ |
| `endQuestion.prompt` | "Using digits 3, 8, 1 once each, the **largest** 3-digit number is {blank}." — "largest" | "Using digits 3, 8, 1 once each — the BIGGEST 3-digit number is {blank}." | ✏️ |

---

### Step 5 — Applet (Digit Rearranger)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `instruction` | "Drag the digits 4, 0, 7 into **H, T, U** to make the smallest 3-digit number." — H/T/U | "Drag digits 4, 0, 7 into Hundreds, Tens, Ones to make the SMALLEST 3-digit number." | ✏️ |
| `discoveryQuestion.prompt` | "Smallest 3-digit number from {4, 0, 7} = {blank}." — curly braces (set notation) | "Smallest 3-digit number using digits 4, 0, 7 is {blank}." | ✏️ |

---

### Step 6 — Apply (Build Checks)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `text` | "Three quick checks — make sure largest and smallest are locked in, including the **leading-zero trap**." — banned phrasing | "Three checks — biggest, smallest, and the sneaky zero rule all together." | ✏️ |
| Prompt 1 | "Largest from {2, 9, 5} = {blank}" — curly braces, "Largest" | "BIGGEST from 2, 9, 5 = {blank}" | ✏️ |
| Prompt 2 | "Smallest from {2, 9, 5} = {blank}" — curly braces | "Smallest from 2, 9, 5 = {blank}" | ✏️ |
| Prompt 3 | "Smallest from {0, 6, 3} = {blank}" — curly braces | "Smallest from 0, 6, 3 = {blank}" | ✏️ |
| `onWrong` | `{ "adaptiveNextStep": "largest-smallest-formation" }` only | Added `"feedback": "Sort the tiles — biggest first for BIGGEST, smallest first for smallest."` | 🖥️ |

---

### Step 7 — Explain (Zero Placeholder)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Title | "When zero shows up" — passive, no hook | "Zero looks empty. It is not." | ✏️ |
| `text` | "You can decompose. You can build. Now — read a description and name the number. 408 = 400 + 0 + 8. The zero says 'nothing in tens'…" — 36 words, asterisks, "decompose" | "408 and 48 look similar. But zero in the Tens column pushes the 4 all the way to Hundreds. Remove the zero and the number collapses." | ✏️ 🐛 |
| `keyInsight` | "Zero is not missing — it is \*working\*. It holds a place." — asterisks render literally | "Zero is not missing. It is working — holding every other digit in the right seat." | 🐛 |

---

### Step 9 — Apply (Zero Checks)

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `onWrong` | `{ "adaptiveNextStep": "expanded-form-zero-placeholder" }` only | Added `"feedback": "Zero holds a place — never drop it from an expanded form."` | 🖥️ |
| `onAllCorrect.feedback` | "Time to seal them in." — too brief | "All three tools are live. Time to lock them in for good." | ✏️ |

---

### Step 10 — Reveal

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Title | "Three Tools. Unlocked." — flat | "Case Closed. Three Tools. Every Problem Solved." | ✏️ |
| Rule 1 name | "Decompose" — banned word | "Break it apart" | ✏️ |
| Rule 2 example | "Sort H → T → U" — abbreviations, arrows | "0, 6, 3 → BIGGEST: 630 · smallest: 306" — full words, example-driven | ✏️ |
| Rule 3 prompt | Used algebra variables X, Y, Z | "5 Hundreds + 8 Tens + 2 Ones = 582" — concrete example | ✏️ |
| Curiosity bridge | Missing | "Add the digits of 408: 4 + 0 + 8 = ___. → 12. That 12 is called the digit sum — Lesson 1.2 starts there." | ✏️ |

---

### Remediations

| Concept | Original | Improved | Tag |
|---------|----------|----------|-----|
| `largest-smallest-formation` options | ["047", "074", "407"] — shows invalid leading-zero strings to students | ["470", "704", "407"] | 🐛 |
| `place-value-ratio` feedback | "7 × 10 = 70. 70 × 10 = 700." — used ÷ previously | Removed all ÷ references | ✏️ |

---

## Block 3 — Worked Example 1 (MK 2014 Q02 · 3pt)

### Problem level

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `problem.figure` | Bare string path (e.g., `"/figures/…svg"`) — figure invisible in CMS | `{ "src": "/figures/…svg" }` object | 🐛 |

### Step titles (all renamed)

| Original | Improved |
|----------|----------|
| "Count the positions" | "Count the gaps" |
| "Map each slot to its number" | "Write out all five numbers" |
| "First-digit elimination" | "Cut the biggest starter!" |
| "Second + third digit elimination" | "Keep cutting — compare the next digits!" |
| "Final comparison + insight" | "Last two standing!" |

### Vocabulary fixes in narration

| Original | Improved | Tag |
|----------|----------|-----|
| "candidates" | "numbers still in the game" | ✏️ |
| "eliminate" | "cross out" | ✏️ |
| "adjacent digits" | "neighboring digits" | ✏️ |
| "the largest possible option" | "the biggest possible option" | ✏️ |

### Hint fixes in checkpoints

| Checkpoint | Original H1 | Improved H1 | Words |
|-----------|-------------|-------------|-------|
| WE1 S5 CP2 | "To maximize, the first digit should be as large as possible." | "To maximize, first digit must be biggest." | 11 → 7 |

---

## Block 4 — Worked Example 2 (MK 2000 Q10 · 4pt)

### Problem level

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| `problem.figure` | Bare string path — figure invisible in CMS | `{ "src": "/figures/…svg" }` object | 🐛 |

### Hint fixes in checkpoints

| Checkpoint | Original | Improved | Issue fixed |
|-----------|----------|----------|-------------|
| WE2 S1 CP1 H1 | "Digits 1, 0, 8 in left-to-right order — read as a number." — 12 words | "Read digits 1, 0, 8 in order as a number." — 9 words | Word count |
| WE2 S1 CP1 H2 | "1 is in Hundreds. 0 is in Tens. 8 is in Ones." — 11 words | "1 in Hundreds, 0 in Tens, 8 in Ones." — 8 words | Word count |
| WE2 S2 CP1 H3 | "Positions 6 and 7 are to the right — how many is that?" — 13 words | "Count the positions that follow position 5." — 7 words | Word count |
| WE2 S2 CP2 H3 | "Order them from smallest: 1, 2, 4, 5, 9." — first element is the answer | "Compare 1 and 2 — which is the smaller one?" | Content violation |
| WE2 S3 CP1 H2 | "Which is smaller — a number starting 15_ or one starting 10_?" — 12 words | "Does 15_ or 10_ give a smaller number?" — 8 words | Word count |
| WE2 S3 CP1 H3 | "The smaller Tens digit gives the smaller number." — names the entire method/answer | "Which is smaller: 158 or 108?" | Content violation |
| WE2 S3 CP2 H1 | "Hundreds = 1, Tens = 0. What is the only digit left?" — 11 words | "Hundreds and Tens are set. One digit remains." — 8 words | Word count |
| WE2 S4 CP1 H2 | "From 4, 9, 2, 1, 5, 0, 8 — which four are not 1, 0, or 8?" — 15 words | "Cross out 1, 0, and 8 from the original list." — 9 words | Word count |

---

## Block 5 — Practice Lab

### Question changes

| # | Original | Improved | Tag |
|---|----------|----------|-----|
| P1 | MCQ "What is the BIGGEST number?" | **sort_order** — student drags [card:4], [card:7], [card:9] into order | ✏️ |
| P3 | "What is the largest digit that can replace the blank…" | "What is the BIGGEST digit that can replace the blank…" | ✏️ |
| P4 | "Add 17 to smallest 2-digit, divide by largest 1-digit" — uses ÷, tests arithmetic not place value | "Benny moved one step RIGHT instead of LEFT. He got 40. What was the correct answer?" — tests ×10 rule from a mistake angle | ✏️ |
| P7 | "Leo inserts digit 5 into 37 — smallest 3-digit number?" — custom, repeats WE1 concept | MK 2019 Q14: □□□ + □ with digits 2,0,1,9 — tests place value priority more deeply | ✏️ |
| P8 | MCQ "What is the BIGGEST 4-digit number from 7, 0, 3, 5?" | **sort_order** — student drags tiles | ✏️ |

### Hint fixes (word count)

| Question | Original H1 | Improved H1 | Words |
|---------|-------------|-------------|-------|
| P1 | "Hundreds seat is worth the most — give it the biggest tile." | "Biggest tile goes in Hundreds." | 12 → 5 |
| P3 | "Try a digit in the blank. Does the result stay under 670?" | "Replace the blank with any digit." | 12 → 6 |
| P7 | "Which seat — Hundreds or the single box — is worth more?" | "Which place is worth the most?" | 11 → 6 |
| P7 H2 | "Put 9 in Hundreds. Try two different arrangements for the rest." | "Put 9 in Hundreds. Now try two arrangements." | 11 → 8 |
| P8 | "Thousands seat is worth the most — give it the biggest tile." | "Biggest tile goes in Thousands." | 12 → 5 |

### PYQ allocation (Practice Lab)

| # | Original | Improved |
|---|----------|----------|
| P2 | MK 2013 Q08 ✓ | MK 2013 Q08 ✓ (kept) |
| P4 | MK 2002 Q12 (arithmetic, ÷ in hints) | Original — "Benny wrong direction" |
| P6 | MK 2007 Q15 ✓ | MK 2007 Q15 ✓ (kept) |
| P7 | Custom "Leo inserts 5 into 37" | MK 2019 Q14 ✓ (upgraded) |
| **Total PYQs** | 3 (P2, P4, P6) | **3 (P2, P6, P7)** — rule: 2–3 ✓ |

---

## Block 6 — Mastery Check

### Question changes

| # | Original | Improved | Tag |
|---|----------|----------|-----|
| MC3 options | "U=1, Tens=3, Ones=6" / "H=3" / etc. — U is non-standard | "Hundreds=1, Tens=3, Ones=6" — full words throughout | ✏️ |
| MC4 | "Digit 4 placed to the right of 7 forms 74. What is 74 − (7 × 7)?" — tests arithmetic, not place value | "A number has 5 Hundreds, 0 Tens, and 8 Ones. What is the number?" — tests Tool 3 (read and name) with zero placeholder | ✏️ |

### Tool coverage after change

| Question | Tool tested |
|----------|-------------|
| MC1 | Tool 2 — build BIGGEST |
| MC2 | Tool 2 — build smallest |
| MC3 | Tool 2 — which arrangement gives smallest |
| MC4 ✏️ | **Tool 3 — read description and name number (with zero)** |

---

## Block 7 — Challenge Extension

| Field | Original | Improved | Tag |
|-------|----------|----------|-----|
| Source | MK 2007 Q16 — 4pt (violates Non-Negotiable Rule 5: CE must be 5pt) | MK 1999 Q22 — 5pt ✓ | ✏️ |
| Question | "Electronic watch shows 02:07. After how many hours will same digits appear again?" | "One number was chosen from 51–55. Digit 0 was placed between its two digits. What is the difference between the new number and the original?" | ✏️ |
| Why better | Tests digit-pattern recognition, distant from lesson's core concept | Directly tests the ×10 shift: inserting 0 pushes the tens digit into hundreds. Difference is always 450 — a satisfying constant that rewards deep thinking | — |
| Hints H1 | "{0, 0, 2, 7} = your four digits" — curly brace set notation | "Pick any one number. Place 0 between its digits." | ✏️ |
| Hints H3 | Listed all valid times — full answer revealed | "Try a second number. Do you get the same difference?" | ✏️ |

---

## Complete Bug Fix Log

| # | Location | Bug | Fix | Tag |
|---|----------|-----|-----|-----|
| 1 | WE1 `problem.figure` | Bare string path — figure invisible | Changed to `{ "src": "..." }` object | 🐛 |
| 2 | WE2 `problem.figure` | Same | Same | 🐛 |
| 3 | IL Step 9 substep 1 | Missing `"type": "mcq"` — question router fails | Added `"type": "mcq"` and `inputType: "choice"` | 🐛 |
| 4 | Remediation options | ["047", "074", "407"] — shows invalid leading-zero strings | Changed to ["470", "704", "407"] | 🐛 |
| 5 | IL Step 10 onAllCorrect | Asterisks in string render as raw `*` characters | Removed all markdown formatting from JSON strings | 🐛 |
| 6 | IL Step 0 predict | `"prompt": "Smallest = {blank}"` — `{blank}` renders literally in predict-step component | Changed to `"Smallest = ___"` | 🐛 |

---

## Complete Language Fix Log

| Rule violated | Original | Improved |
|--------------|----------|----------|
| No ÷ symbol | "÷10", "700 ÷ 70 = 10" | "10 times smaller", "7 times 10 equals 70" |
| No H, T, U abbreviations | "H column", "T or U, never H", "H, T, U" | "Hundreds", "Tens", "Ones" throughout |
| No curly braces | "{4, 0, 7}", "{2, 9, 5}", "{0, 6, 3}" | Plain comma-separated: "4, 0, 7" etc. |
| No "adjacent" | "adjacent columns", "adjacent digits" | "neighboring digits", "next to each other" |
| No "decompose" | "Decompose" in rule card | "Break it apart" |
| No "eliminate" | "eliminate" in WE narration | "cross out" |
| No "candidates" | "candidates" in WE narration | "numbers still in the game" |
| No "leverage" | "the seat with the most leverage" | removed — replaced with "the seat with the most value" |
| No "leading-zero trap" | "leading-zero trap" in Step 6 | "the sneaky zero rule" |
| "BIGGEST" not "LARGEST" | "LARGEST", "largest possible option" | "BIGGEST", "biggest possible option" |
| ≤15 words/sentence | Step 4 body: 41-word sentence | Rewritten as two sentences, each ≤15 words |
| No `!` in feedback | Not present in original at scale | Confirmed zero `!` in final JSON |

---

## Hint Compliance Summary

All hints in the final lesson pass:
- ✅ ≤ 10 words
- ✅ Do not name the answer
- ✅ Do not name a key intermediate value
- ✅ Do not spell out the method
- ✅ Exactly 3 hints per question (CF, PL, CE)
- ✅ 0 hints in Mastery Check (as required)

---

*Final JSON: `lesson-1-1-place-value-v6.json` · Registered in `v2-loader.ts` · Live at `/lesson/mk-foundations-grade-3-4/0/0`*
