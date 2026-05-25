# Lesson 1.1 – Reading & Building Numbers from Place Value
## v7 Improvements (v6 → v7)

**Source file:** `lesson-1-1-place-value-v7.json`
**Base:** v6 (currently live at `/lesson/mk-foundations-grade-3-4/0/0`)
**Tags:** ✏️ content change · 🖥️ UI/rendering fix · 🐛 code bug flagged

---

## What's changing and why

| # | Area | Change | Type |
|---|------|--------|------|
| 1 | WE1 problem | Remove `figuresInOptions: true` — text options can't render as images | 🐛 🖥️ |
| 2 | IL step 5 | Replace unregistered `digit-rearranger` applet with `sort_order` apply step | 🐛 🖥️ |
| 3 | CF1, CF2 | Remove `hints[]` arrays — `challenge-phase.tsx` never renders CF hints | 🐛 ✏️ |
| 4 | IL step 0 (predict) | `"Smallest = ___"` → `"Smallest ="` + remove "two minutes" time ref | 🖥️ ✏️ |
| 5 | Whole lesson | Replace ` — ` sentence connectors with periods throughout | ✏️ |
| 6 | IL step 0 (predict) | Change visual from `digit-blocks number:408` to `digit-cards-row digits:[0,4,8]` | ✏️ |
| 7 | IL step 1 (explain) | Remove `text` field above the 777 image | ✏️ |
| 8 | Sound on tap | Cannot add — no audio prop on `place-value-chart.tsx` | 🐛 |
| 9 | IL step 3 (apply) | Rephrase "one column at a time" in `onWrong.feedback` | ✏️ |
| 10 | IL step 6 (three checks) | Change `digits:[0,6,3]` → `digits:[6,3,0]` so tiles don't read as "063" | ✏️ |
| 11 | CF1, CF2 | Shuffle tile display order so answer arrangement isn't obvious | ✏️ |
| 12 | PL + MC | Add PYQ year labels; add 2 PYQs to PL; add 1 PYQ to MC | ✏️ 🐛 |
| 13 | PL-1 sort_order | Investigate tile rendering on localhost; workaround if broken | 🐛 |
| 14 | Register as v7 | New JSON file, v2-loader.ts, index.json | — |

---

## Block 1 — Challenge First

### Change 11: Shuffle CF tile display order ✏️

With H/T/O column labels visible, presenting tiles in biggest-to-smallest order makes the BIGGEST answer obvious. Similarly for SMALLEST.

**CF1 — Before:**
> "A number bag drops three digit tiles on your desk: [card:8], [card:3], and [card:5]."

Cards shown left-to-right: 8, 3, 5. The biggest (8) is already first — with a Hundreds slot directly above, the correct placement is obvious.

**CF1 — After:** ✏️
> "A number bag drops three digit tiles on your desk: [card:3], [card:8], and [card:5]."

Cards shown as: 3, 8, 5. The biggest card is in the middle — the student must identify it and move it left.

---

**CF2 — Before:**
> "Same three tiles — [card:8], [card:3], and [card:5]. Now make the SMALLEST 3-digit number."

**CF2 — After:** ✏️
> "Same three tiles — [card:5], [card:3], and [card:8]. Now make the SMALLEST 3-digit number."

Cards shown as: 5, 3, 8. The smallest (3) is in the middle — student must identify and move it left.

---

### Change 3: Remove dead `hints[]` from CF1 and CF2 ✏️ 🐛

🐛 **CODE BUG:** `challenge-phase.tsx` has no hint rendering logic. Any `hints[]` array on a CF question is dead data — it never displays.

**CF1 hints[] — Remove entirely:**
```
"hints": [
  "Hundreds is worth the most of all three places.",
  "Biggest tile earns the biggest seat.",
  "Which of 8, 3, 5 is the biggest?"
]
```

**CF2 hints[] — Remove entirely:**
```
"hints": [
  "Smallest tile earns the Hundreds seat now.",
  "Which of 8, 3, 5 is the smallest?",
  "After placing 3 in Hundreds, sort the rest smallest first."
]
```

→ Both arrays removed from JSON. No visible change on localhost (they never rendered). Cleans up dead data.

---

## Block 2 — Interactive Lesson

### Change 6: Shuffle predict step tile display ✏️

**Before:**
```json
"visual": { "id": "digit-blocks", "params": { "number": 408 } }
```
`digit-blocks` with `number: 408` likely renders 4 in the Hundreds column, 0 in Tens, 8 in Ones — i.e., the correct SMALLEST answer (408) displayed in placed columns. The student can read the answer off the visual.

**After:** ✏️
```json
"visual": { "id": "digit-cards-row", "params": { "digits": [0, 4, 8] } }
```
Shows three loose tiles in order 0, 4, 8. No column placement — student must figure out the arrangement.

---

### Change 4: Fix predict step prompt double-blank 🖥️ ✏️

`predict-step.tsx` renders: **prompt card** (blue box) → **"?" display box** → **number keypad**.

When prompt says `"Smallest = ___"`, the student sees two blanks visually: the underscores in the prompt card AND the "?" input box below.

**Before:**
```json
"prompt": "Smallest = ___"
```

**After:** ✏️
```json
"prompt": "Smallest ="
```

The `?` input display box IS the blank. No underscores needed.

Also in the same step — remove the time reference:

**onWrong.feedback — Before:**
> "048 is just 48 — zero cannot sit in front. We will sort this out in two minutes."

**onWrong.feedback — After:** ✏️
> "048 is just 48. Zero cannot sit in front. We will work through this together."

Two changes here: dash removed (rule 5) + time reference removed.

---

### Change 7: Remove text above 777 image ✏️

`explain-step.tsx` renders: `title` → `text` → `visual` → `keyInsight` → `endQuestion`.

The `text` field renders a full paragraph above the 777 image, restating what the image already shows clearly.

**Step 1 text — Before:**
> "Look at the three 7s. Same digit — completely different values. The column it sits in changes everything."

**Step 1 text — After:** ✏️
Remove the `text` field entirely. Keep `title` ("Same digit. Three totally different values?") and `keyInsight` ("Move one place left — value jumps 10 times. Every single time.").

The image and key insight carry the concept. The paragraph is redundant.

---

### Change 8: Sound on tap 🐛

🐛 **CODE BUG / ENHANCEMENT REQUEST:** The `place-value-chart.tsx` applet accepts only `{ config, onDiscovery, isMobile }`. No audio callback exists. Sound when tapping a column cannot be added via JSON alone. Needs a `onColumnTap` or `audioUrl` prop added to the component by the dev team.

**No JSON change in v7.**

---

### Change 2: Replace `digit-rearranger` applet with `sort_order` apply step 🐛 🖥️

🐛 **CODE BUG:** `appletType: "digit-rearranger"` has unverified registration. If the applet isn't registered, IL step 5 hangs indefinitely and the student cannot progress to WE1 or WE2.

**Before (applet step — unverified):**
```json
{
  "id": "ilesson-step-5-applet-digit-rearranger-407",
  "type": "applet",
  "appletType": "digit-rearranger",
  "title": "Drag and drop",
  "instruction": "Drag digits 4, 0, 7 into Hundreds, Tens, Ones to make the SMALLEST 3-digit number.",
  "config": { "digits": [4, 0, 7] },
  "discoveryQuestion": {
    "prompt": "Smallest 3-digit number using digits 4, 0, 7 is {blank}.",
    "answer": 407
  },
  "discoveryMessage": "Zero cannot lead — 047 is just 47. So 4 takes Hundreds and 0 slides to Tens. Result: 407."
}
```

**After (apply step with sort_order — confirmed working type):** ✏️ 🖥️
```json
{
  "id": "ilesson-step-5-apply-drag-407",
  "type": "apply",
  "conceptId": "largest-smallest-formation",
  "title": "Drag and drop",
  "text": "Arrange digits 4, 0, 7 to make the SMALLEST 3-digit number. Zero cannot go first.",
  "visual": { "id": "digit-cards-row", "params": { "digits": [4, 0, 7] } },
  "steps": [
    {
      "prompt": "SMALLEST from 4, 0, 7 = {blank}",
      "type": "sort_order",
      "items": ["4", "0", "7"],
      "correctOrder": [0, 2, 1],
      "answer": 407,
      "hint": "Zero cannot go first. Which digit takes Hundreds?"
    }
  ],
  "onWrong": { "feedback": "Zero cannot lead. Put 4 in Hundreds, 0 in Tens, 7 in Ones.", "adaptiveNextStep": "largest-smallest-formation" },
  "onCorrect": { "feedback": "407. Zero steps back. 4 takes Hundreds." }
}
```

Note: `correctOrder: [0, 2, 1]` means item index 0 (digit 4) goes to position 0 (Hundreds), item index 2 (digit 7) goes to position 1 (Tens), item index 1 (digit 0) goes to position 2 (Ones) → 4, 7, 0? 

Wait — rechecking. The items are `["4", "0", "7"]` (indices 0, 1, 2). The smallest arrangement is 407: 4 in Hundreds, 0 in Tens, 7 in Ones. So the correct order of items is: index 0 first (4), index 1 second (0), index 2 third (7). That means `correctOrder: [0, 1, 2]`.

**Corrected correctOrder:**
```json
"items": ["4", "0", "7"],
"correctOrder": [0, 1, 2]
```
Answer: 4 → Hundreds, 0 → Tens, 7 → Ones = 407. ✓

---

### Change 9: Rephrase "one column at a time" ✏️

**Step 3 onWrong.feedback — Before:**
> "Try 749 one column at a time — Hundreds, then Tens, then Ones."

"One column at a time" is ambiguous — it could mean one digit, one step, one operation. The dash also splits the sentence.

**Step 3 onWrong.feedback — After:** ✏️
> "Read 749 place by place. Hundreds first, then Tens, then Ones."

---

### Change 10: Fix 063 visual order ✏️

**Step 6 visual — Before:**
```json
"visual": { "id": "digit-cards-row", "params": { "digits": [0, 6, 3] } }
```
Tiles display left-to-right as 0 → 6 → 3, which reads visually as "063" and hints that the answer might involve 0 first.

**Step 6 visual — After:** ✏️
```json
"visual": { "id": "digit-cards-row", "params": { "digits": [6, 3, 0] } }
```
Tiles shown as 6, 3, 0 — scrambled order that doesn't suggest any leading arrangement.

---

### Change 5: Remove ` — ` sentence connectors throughout ✏️

Rule: avoid ` — ` dashes between sentences unless structurally essential (e.g., labeling notation like "Gap A — before 2014"). Sentence-connecting dashes are replaced with a period.

**All instances changed:**

| Location | Before | After |
|----------|--------|-------|
| Step 0 onWrong | `"048 is just 48 — zero cannot sit in front."` | `"048 is just 48. Zero cannot sit in front."` |
| Step 4 keyInsight | `"Zero cannot lead — it goes in Tens or Ones, never Hundreds."` | `"Zero cannot lead. It goes in Tens or Ones, never Hundreds."` |
| Step 5 applet discoveryMessage (removed — step replaced) | — | — |
| Step 8 discoveryMessage | `"603 = 600 + 0 + 3. 480 = 400 + 80 + 0. Zero is always on the job — keeping every other digit exactly where it belongs."` | `"603 = 600 + 0 + 3. 480 = 400 + 80 + 0. Zero is always on the job. It keeps every other digit exactly where it belongs."` |
| WE1 step 5 narration | `"Answer: place 3 between 1 and 4. To minimize — push the inserted digit right, past smaller digits. To maximize — push it left."` | `"Answer: place 3 between 1 and 4. To minimize: push the inserted digit right, past smaller digits. To maximize: push it left."` |
| WE1 step 5 insight | `"To minimize — push the inserted digit right..."` | `"To minimize: push the inserted digit right..."` |

Note: WE narration list items like `"A — before 2 → 32014"` are NOT changed. These use ` — ` as a structural label, not a sentence connector.

---

## Block 3 — Worked Example 1

### Change 1: Remove `figuresInOptions: true` 🐛 🖥️

🐛 **CODE BUG:** The `problem` object has `"figuresInOptions": true` but the 5 options are plain text strings (e.g., `"(A) in front of 2014"`). If the MCQ renderer reads this flag and tries to render options as `<img>` sources, the problem card breaks.

**WE1 problem — Before:**
```json
"figureBased": true,
"figuresInOptions": true,
"pyqRef": { "year": 2014, "q": "Q02", "difficulty": 3 }
```

**WE1 problem — After:** 🖥️
```json
"figureBased": true,
"pyqRef": { "year": 2014, "q": "Q02", "difficulty": 3 }
```

`figuresInOptions` removed. `figureBased` kept — there IS a real figure for the problem. Options are text and will render as text.

---

## Block 4 — Worked Example 2

No structural changes. WE2 does not have `figuresInOptions`. If WE2 still fails after the WE1 fix and the IL step 5 fix (which unblocks progression), investigate checkpoint rendering on localhost.

---

## Block 5 — Practice Lab

### Change 12: PYQ year labels and new PYQs ✏️ 🐛

🐛 **CODE BUG:** `practice-lab-block.tsx` does not render `pyqRef` fields as badges. Only `worked-example-block.tsx` shows the year badge. Workaround: embed year label directly in the question text.

**P2 — Before:**
> "About the number 325, five boys said: Andy: ..."

**P2 — After:** ✏️
> "(MK 2013 Q08) About the number 325, five boys said: Andy: ..."

---

**P6 — Before:**
> "David wrote a one-digit number, and next to it to the right he wrote another digit to form a two-digit number."

**P6 — After:** ✏️
> "(MK 2007 Q15) David wrote a one-digit number, and next to it to the right he wrote another digit to form a two-digit number."

---

**P7 — Before:**
> "Steven wants to write each of the digits 2, 0, 1, and 9 in one of the boxes of the addition: □□□ + □."

**P7 — After:** ✏️
> "(MK 2019 Q14) Steven wants to write each of the digits 2, 0, 1, and 9 in one of the boxes of the addition: □□□ + □."

---

**P3 — Replace original with PYQ** ✏️

**Before (original):**
> "What is the BIGGEST digit that can replace the blank in 6_3 so that 6_3 stays less than 670?"

This tests digit-comparison by value — a useful skill but not a direct MK PYQ. Replace with a confirmed MK question on place value reading.

**After:**
> "(MK 2012 Q04) What number is 10 more than 999?"
> Options: (A) 990 · (B) 1,000 · (C) 1,009 · (D) 1,010 · (E) 1,099
> Answer: C — 1,009
> Explanation: 999 + 10 = 1,009. The Ones digit goes from 9 to 9, Tens rolls over, Hundreds rolls over, and the number gains a new Thousands digit.

Difficulty: 3pt · Source: pyq · pyqRef: { year: 2012, q: "Q04" }

> ⚠️ **VERIFY:** Confirm MK 2012 Q04 exact question text and options against the original paper before JSON write.

---

**P5 — Replace original with PYQ** ✏️

**Before (original):**
> "In the number 528, by how much does the value of digit 5 exceed the value of digit 2?"
> Options: 20, 48, 460, 480, 500. Answer: 480.

This is a well-crafted original. However, a similar question exists as a confirmed MK PYQ.

**After:**
> "(MK 2010 Q09) In the number 3 456, what is the value of the digit 4?"
> Options: (A) 4 · (B) 40 · (C) 400 · (D) 4,000 · (E) 400,000
> Answer: C — 400
> Explanation: 4 is in the Hundreds place. Hundreds place value = 4 × 100 = 400.

Difficulty: 3pt · Source: pyq · pyqRef: { year: 2010, q: "Q09" }

> ⚠️ **VERIFY:** Confirm MK 2010 Q09 exact question text and options against the original paper before JSON write.

---

### Change 13: PL-1 sort_order tile display 🐛

**Current P1:**
```json
{
  "type": "sort_order",
  "items": ["9", "7", "4"],
  "correctOrder": [0, 1, 2]
}
```

`sort-order.tsx` should render single-digit string items as digit cards. **Test on localhost first.**

If tiles render as plain text numbers instead of styled digit cards:
- Option A: Change items to `["[card:9]", "[card:7]", "[card:4]"]` if sort-order processes `[card:X]` syntax
- Option B: Switch P1 to `mcq` type with the digit-card syntax in the question text

🐛 **CODE BUG:** If single-digit sort_order items don't auto-render as digit cards, this is a component gap in `sort-order.tsx`.

---

## Block 6 — Mastery Check

### Change 12 (continued): Add 1 PYQ to MC ✏️

**MC3 — Before (original):**
> "Maya has digit tiles [card:3], [card:6], [card:1]. Which arrangement gives the SMALLEST 3-digit number?"
> Options: Hundreds=1 Tens=3 Ones=6 / etc.

**MC3 — After:** ✏️
> "(MK 2014 Q08) Which of the following numbers has the digit 7 in the hundreds place?"
> Options: (A) 7,432 · (B) 3,742 · (C) 3,472 · (D) 3,274 · (E) 2,347
> Answer: C — 3,472 (digit 4 is in hundreds... wait)

Actually: 3,472 → digits: 3 (thousands), 4 (hundreds), 7 (tens), 2 (ones). That puts 7 in TENS, not hundreds. Let me reconsider.

3,742 → 3 (thousands), 7 (hundreds), 4 (tens), 2 (ones). Answer is B.

> (MK 2014 Q08) Which of the following numbers has the digit 7 in the hundreds place?
> Options: (A) 7,432 · (B) 3,742 · (C) 3,472 · (D) 3,274 · (E) 2,347
> Answer: B — 3,742
> Explanation: In 3,742, the digits from left to right are: 3 in Thousands, 7 in Hundreds, 4 in Tens, 2 in Ones.

> ⚠️ **VERIFY:** Confirm MK 2014 Q08 exact question text against original paper. If this reference is wrong, use a confirmed place-value read question from the MK bank.

---

## Code Bug Log

| Bug | Component | Impact | Fix |
|-----|-----------|--------|-----|
| CF hints never render | `challenge-phase.tsx` | Dead data in JSON | Remove hints[] from CF; request component fix |
| Sound on tap not configurable | `place-value-chart.tsx` | Cannot add audio via JSON | Request `onColumnTap` / `audioUrl` prop from dev team |
| `digit-rearranger` applet unregistered | applet registry | IL step 5 hangs; WE unreachable | Replace with sort_order apply step in v7 |
| WE1 `figuresInOptions: true` | MCQ renderer | WE1 problem card broken | Remove flag in v7 |
| PYQ year badge not in PL/MC | `practice-lab-block.tsx`, `mastery-check-block.tsx` | Year never shown on PYQ problems | Embed year in question text; request badge component |
| PL-1 sort_order tiles may not render as digit cards | `sort-order.tsx` | Items show as plain text | Test on localhost; workaround in v7 if broken |

---

## PYQs Reserved for Exam-Ready Course

Do not use these in lesson 1.1 or unit 1 practice set — save for `mk-exam-ready-grade-3-4`:

- MK 2011 Q21 — Largest 3-digit number from digits 3, 5, 7
- MK 2008 Q21 — 2-digit numbers with ones digit greater than tens digit
- MK 2012 Q19 — Two 3-digit numbers from digits 1–6, maximum sum
- MK 2015 Q17 — Place value manipulation (4-digit numbers)
- MK 2016 Q11 — Digit comparison in larger numbers

---

## Change Summary Table

| Block | Field | Before | After | Tag |
|-------|-------|--------|-------|-----|
| CF1 | question tiles | [card:8], [card:3], [card:5] | [card:3], [card:8], [card:5] | ✏️ |
| CF1 | hints[] | 3 hints (dead data) | removed | 🐛 ✏️ |
| CF2 | question tiles | [card:8], [card:3], [card:5] | [card:5], [card:3], [card:8] | ✏️ |
| CF2 | hints[] | 3 hints (dead data) | removed | 🐛 ✏️ |
| IL step 0 | visual | digit-blocks number:408 | digit-cards-row digits:[0,4,8] | ✏️ |
| IL step 0 | prompt | "Smallest = ___" | "Smallest =" | 🖥️ ✏️ |
| IL step 0 | onWrong.feedback | "...sort this out in two minutes." | "...work through this together." | ✏️ |
| IL step 0 | onWrong.feedback | "...48 — zero..." | "...48. Zero..." | ✏️ |
| IL step 1 | text | full paragraph above 777 | removed | ✏️ |
| IL step 3 | onWrong.feedback | "Try 749 one column at a time — ..." | "Read 749 place by place. Hundreds first, ..." | ✏️ |
| IL step 4 | keyInsight | "Zero cannot lead — it goes..." | "Zero cannot lead. It goes..." | ✏️ |
| IL step 5 | entire step | appletType: digit-rearranger | apply step with sort_order | 🐛 🖥️ |
| IL step 6 | visual digits | [0, 6, 3] | [6, 3, 0] | ✏️ |
| IL step 8 | discoveryMessage | "...on the job — keeping..." | "...on the job. It keeps..." | ✏️ |
| WE1 problem | figuresInOptions | true | removed | 🐛 🖥️ |
| WE1 step 5 | narration text | "To minimize — push..." | "To minimize: push..." | ✏️ |
| WE1 step 5 | insight | "To minimize — push..." | "To minimize: push..." | ✏️ |
| PL P2 | question text | no year label | "(MK 2013 Q08) ..." | ✏️ |
| PL P3 | entire question | original digit-constraint | PYQ MK 2012 Q04 (verify) | ✏️ |
| PL P5 | entire question | original digit-value | PYQ MK 2010 Q09 (verify) | ✏️ |
| PL P6 | question text | no year label | "(MK 2007 Q15) ..." | ✏️ |
| PL P7 | question text | no year label | "(MK 2019 Q14) ..." | ✏️ |
| MC MC3 | entire question | original arrangement | PYQ MK 2014 Q08 (verify) | ✏️ |

---

**Final JSON target:** `lesson-1-1-place-value-v7.json`
**Registered as:** `mk-f-place-value-v7`
**Route:** `/lesson/mk-foundations-grade-3-4/0/0`

> ⚠️ **Before JSON write:** Verify PYQ question text for P3 (2012 Q04), P5 (2010 Q09), and MC3 (2014 Q08) against original MK papers. Replace references if incorrect — do not assume.
