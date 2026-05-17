# Lesson 1.5 — Unit 1 Practice Set (Improved)

**ID:** `mk-f-ps-1`
**Title:** Unit 1 Practice Set
**Unit:** 1 | **Duration:** 20 min | **Hints allowed:** Yes
**Problems:** 10 + 2 Challenge Extension
**Skills covered:** Place Value · Digit Sums · Multi-Step Arithmetic · Parity

> ✏️ marks every content change. 🐛 marks critical code/layout bug fixes.

---

## What changed and why — quick read

| Category | Count | Biggest wins |
|----------|-------|--------------|
| 🐛 Layout/asset bugs | 5 | PT1 text hidden behind figure; PT4 figure highlights answer in yellow; PT9/PT10 text overlaps image; CE1 figure has answer in caption |
| ✏️ Answer-hints → CUEs | 10 | Third hints removed across every problem — all were complete solutions, not prompts |
| ✏️ Hints reduced: 3 → 2 | 8 | All problems now have 2 hints max. 3 hints on a 5-option MCQ = 4 attempts = trivial guessing |
| ✏️ Language simplified | 5 | "maximize"→"biggest"; ÷ removed; curly braces removed; □ → ? in PT10 |
| ✏️ PT1 question redesigned | 1 | Original question answerable by glancing at labeled figure — retested as place-value worth |

---

## PT1 — Place Value: Hundreds Digit ✏️🐛

**Type:** MCQ | **Difficulty:** 3pt | **Source:** Original | **Skill:** place-value
**Figure:** `MK_PS1_Q1_pv_chart.svg`

🐛 **Text hidden behind figure:** The question text is partially immersed in the image — add top padding or move the question above the figure.

🐛 **Figure reveals the answer:** The current SVG is a labeled place-value chart of 457 with "Hundreds | Tens | Ones" columns — the answer (4) is visible just by reading the chart. The figure defeats the question.

✏️ **Question redesigned** — instead of "what is the hundreds digit?" (readable from the chart), test what that digit is WORTH:
> **"In the number 457, how much is the hundreds digit worth?"**

- (A) 4
- (B) 40
- **(C) 400 ✓**
- (D) 4,000
- (E) 457

**Answer:** index 2
**Explanation:** The digit 4 is in the hundreds place. Its value = 4 × 100 = 400.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | The hundreds digit is the first (leftmost) digit of a 3-digit number. | **In 457, which digit is in the hundreds place? Look at the leftmost digit.** | ✏️ reworded |
| 2 | In 457: hundreds = 4, tens = 5, ones = 7. | **The hundreds digit is 4. Is the digit 4 worth 4, or 40, or 400? Think about what "hundreds place" means.** | ❌→✅ CUE |
| 3 | Place value: 4×100 + 5×10 + 7×1. The hundreds digit is 4. | ~~Removed — gave the full answer.~~ | ❌ removed |

> 💡 **Why redesigned:** The original asked students to read a labeled chart — a 3pt question should test understanding of place value, not the ability to read a diagram. The new question works with or without the figure.

---

## PT2 — Digit Sum of 326 ✏️

**Type:** MCQ | **Difficulty:** 3pt | **Source:** Original | **Skill:** digit-sums

**Question:** What is the digit sum of 326?
**Options:** 9 / 10 / **11 ✓** / 12 / 13
**Answer:** index 2
**Explanation:** 3 + 2 + 6 = 11.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Add all the digits together: 3 + 2 + 6. | *No change — good CUE.* | ✅ keep |
| 2 | Start with 3 + 2 = 5. Now add 6 to that result. | **Start with the first two digits: 3 + 2 = ___. Then add the last digit to your answer.** | ❌→✅ CUE |
| 3 | 3 + 2 = 5, then 5 + 6 = 11. The digit sum of 326 is 11. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT3 — 16 + 25 − 9 ✏️

**Type:** MCQ | **Difficulty:** 3pt | **Source:** Original | **Skill:** operations

**Question:** What is 16 + 25 − 9?
**Options:** 28 / 30 / **32 ✓** / 34 / 41
**Answer:** index 2
**Explanation:** 16 + 25 = 41. 41 − 9 = 32.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Add first, then subtract: (16 + 25) = 41, then 41 − 9 = ? | *No change — good CUE.* | ✅ keep |
| 2 | 16 + 25 = 41. Now subtract 9 from 41. | **You should have 41 after the addition. To subtract 9 from 41, try taking away 10 first — then what do you need to fix?** | ❌→✅ CUE |
| 3 | 41 − 9: think 41 − 10 + 1 = 32. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT4 — Which Sum is Odd? ✏️🐛

**Type:** MCQ | **Difficulty:** 3pt | **Source:** Original | **Skill:** parity
**Figure:** `MK_PS1_Q4_parity_grid.svg`

🐛 **Figure reveals answer:** The grid SVG highlights one cell in yellow — the correct answer (C: 7 + 2) is visually obvious before any thinking is done. Remove the yellow highlight; all cells should have equal styling.

✏️ **Attempt count reduced:** 3 hints allow 4 total attempts on a 5-option MCQ. Once hint 1 explains the rule, the remaining hints become a process of elimination. Reduced to 2 hints (3 attempts total).

**Question:** The grid shows five sums. Which sum is an odd number?
**Options:** A) 4 + 6 / B) 3 + 5 / **C) 7 + 2 ✓** / D) 8 + 4 / E) 5 + 5
**Answer:** index 2
**Explanation:** odd + even = odd. 7 (odd) + 2 (even) = 9 (odd). All others are even + even = even.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Odd + Even = Odd. Check which pair has one odd and one even number. | *No change — good CUE.* | ✅ keep |
| 2 | A) 4+6=10 (even), B) 3+5=8 (even). Check C: 7 is odd, 2 is even — odd + even = ? | **Look at each pair. Does it have one odd number and one even number? Label each number odd or even, then check the rule.** | ❌→✅ CUE |
| 3 | 7 + 2 = 9 (odd). All others are even + even = even. Answer: C. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT5 — Largest 3-digit Number with 3, 5, 7 ✏️

**Type:** MCQ | **Difficulty:** 4pt | **Source:** PYQ (MK 2011 Q21) | **Skill:** place-value

**Question:** Using the digit cards 3, 5, and 7 (each used exactly once), what is the BIGGEST 3-digit number you can form?
**Options:** 357 / 537 / 735 / **753 ✓** / 375
**Answer:** index 3
**Explanation:** Put the biggest digit (7) in the hundreds place, next biggest (5) in tens, smallest (3) in ones → 753.

✏️ **Language:** "maximize" → "BIGGEST" throughout.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | To maximize a number, put the largest digit in the hundreds place, next largest in tens, smallest in ones. | **To make the BIGGEST number, which digit should go in the hundreds place — the biggest digit or the smallest?** | ❌→✅ CUE |
| 2 | Digits are 3, 5, 7. Largest is 7 → hundreds place. Next is 5 → tens. Smallest is 3 → ones. | **The biggest digit is 7. Put 7 in the hundreds place. Now arrange 3 and 5 in the tens and ones places to make it as big as possible.** | ❌→✅ CUE |
| 3 | So the number is 7 (hundreds) 5 (tens) 3 (ones) = 753. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT6 — Count 2-digit Numbers with Digit Sum 7 ✏️

**Type:** MCQ | **Difficulty:** 4pt | **Source:** Original | **Skill:** digit-sums

**Question:** How many 2-digit numbers have a digit sum equal to 7? (e.g. 16, 25, 34, …)
**Options:** 5 / 6 / **7 ✓** / 8 / 9
**Answer:** index 2
**Explanation:** Numbers: 16, 25, 34, 43, 52, 61, 70 — seven numbers. Tens digit runs from 1 to 7.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | A 2-digit number AB has digits A + B = 7. The tens digit A can go from 1 to 7. | **In a 2-digit number, both digits must add up to 7. What is the smallest possible tens digit? What is the biggest?** | ❌→✅ CUE |
| 2 | Tens=1 → ones=6 (16); Tens=2 → ones=5 (25); Tens=3 → ones=4 (34); Tens=4 → ones=3 (43)… | **Start listing them out: if the tens digit is 1, the ones must be 6 — that gives 16. If the tens digit is 2, the ones must be ___. Keep going until you run out.** | ❌→✅ CUE |
| 3 | Continue: 52, 61, 70. That gives 7 numbers total (tens digits 1 through 7). | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT7 — Number Machine: Find the Input ✏️

**Type:** MCQ | **Difficulty:** 4pt | **Source:** PYQ (MK 2015 Q1) | **Skill:** operations
**Figure:** `MK_PS1_Q7_machine.svg`

**Question:** A number machine does: N → ×3 → −2 → output. The output is 25. What was the input N?
**Options:** 7 / 8 / **9 ✓** / 11 / 23
**Answer:** index 2
**Explanation:** Work backwards: 25 + 2 = 27. 27 divided by 3 = 9. Check: 9 × 3 − 2 = 25 ✓.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Work backwards: output = 25. Undo −2 first (add 2), then undo ×3 (divide by 3). | **Work backwards from 25. The last step was "−2". What is the opposite of subtracting 2?** | ❌→✅ CUE |
| 2 | Step 1: 25 + 2 = 27 (undoing the −2). Step 2: 27 ÷ 3 = ? | **After undoing the subtraction you should have 27. The step before that was "×3". What is the opposite of multiplying by 3?** | ❌→✅ CUE |
| 3 | 27 ÷ 3 = 9. Check: 9 × 3 − 2 = 27 − 2 = 25. ✓ | ~~Removed — gave the full answer. Also used ÷ symbol (banned).~~ | ❌ removed |

---

## PT8 — Adam's Cards: Even Sum? ✏️

**Type:** MCQ | **Difficulty:** 4pt | **Source:** Original | **Skill:** parity

**Question:** Adam picks 3 cards from 1, 2, 3, 4, 5. Can his 3 cards have an even sum?
**Options:** Never — sum always odd / Always — sum always even / **Sometimes — it depends on which 3 cards ✓** / Only if he picks card 2 / Only when all three cards are odd
**Answer:** index 2
**Explanation:** Try 1, 3, 5: sum = 9 (odd). Try 1, 3, 4: sum = 8 (even). Both are possible — so it depends.

✏️ **Curly braces removed** from hints.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Sum of 3 numbers is even when: all 3 are even, or exactly 2 are odd (odd+odd+even=even). | **Pick any 3 cards and add them. Try 1 + 3 + 5. Then try a different 3 cards. Do you always get the same type of answer?** | ❌→✅ CUE |
| 2 | From {1,2,3,4,5}: evens are 2,4; odds are 1,3,5. Try picking 1,3,5 (all odd): 1+3+5=9 (odd). Try 1,3,4: 1+3+4=8 (even). | **From the cards 1, 2, 3, 4, 5 — can you find one set of 3 that gives an even sum AND one that gives an odd sum?** | ❌→✅ CUE |
| 3 | Since we can get both even and odd sums depending on which cards are chosen, the answer is: it depends. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT9 — Number Pyramid ✏️🐛

**Type:** MCQ | **Difficulty:** 4pt | **Source:** Original | **Skill:** operations
**Figure:** `MK_PS1_Q9_pyramid.svg`

🐛 **Layout bug:** Question text overlaps with the pyramid figure. Add padding between the question text and the figure — the pyramid is the key visual and must be fully readable.

**Question:** In the number pyramid, each cell equals the sum of the two cells below it. The bottom row is 2, 5, 3, 4. What number goes at the top?
**Options:** 24 / 27 / **30 ✓** / 33 / 36
**Answer:** index 2
**Explanation:** Row 1 (bottom): 2, 5, 3, 4. Row 2: 7, 8, 7. Row 3: 15, 15. Top: 30.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | Build row by row. Bottom: 2, 5, 3, 4. Level up: 2+5=7, 5+3=8, 3+4=7. | **Start at the bottom row. Add each pair of neighbours: 2 + 5 = ___, then 5 + 3 = ___, then 3 + 4 = ___. Write those three answers in the row above.** | ❌→✅ CUE |
| 2 | Next level: 7+8=15, 8+7=15. | **You now have three numbers in the second row. Add each pair of those to build the next row. How many numbers will that row have?** | ❌→✅ CUE |
| 3 | Top: 15 + 15 = 30. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## PT10 — Swap Two Digits for Biggest Number ✏️🐛

**Type:** MCQ | **Difficulty:** 4pt | **Source:** Original | **Skill:** place-value
**Figure:** `MK_PS1_Q10_swap.svg`

🐛 **Layout bug:** Question text overlaps with the figure image. Add padding between question and figure.

🐛 **□ symbol rendering:** All options contain "□" (the unknown middle digit). This renders as a blank square box in the CMS — students see an unrecognised character. Replaced with "?" throughout.

✏️ **Revised question and options:**
> **"You have the 3-digit number 3?7 (the middle digit is unknown). You may swap exactly two digits to create the biggest possible number. Which swap gives the maximum?"**

- **(A) Swap 3 and 7 → 7?3 ✓**
- (B) Swap 3 and ? → depends on ?
- (C) Swap 7 and ? → depends on ?
- (D) No swap needed — 3?7 is already maximum
- (E) Only valid if ? is greater than 7

**Answer:** index 0
**Explanation:** 7 > 3. Putting 7 in the hundreds place always beats 3 there. So swap 3 and 7 → 7?3. The middle digit doesn't affect which swap is best.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | To maximize, get the largest digit into the hundreds place. Here 7 > 3, so swap them. | **To make the BIGGEST number, which digit should be in the hundreds place — 3 or 7?** | ❌→✅ CUE |
| 2 | After swap: 7□3. Regardless of what □ is, 7 in the hundreds place beats 3 in the hundreds place. | **Once 7 is in the hundreds place, the middle digit doesn't change which swap was best. Why not?** | ❌→✅ CUE |
| 3 | 3□7 → swap 3 and 7 → 7□3. This always gives the largest hundreds digit from these three digits. | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## Challenge Extension 1 — Ones Digit > Tens Digit ✏️🐛

**Type:** MCQ | **Difficulty:** 5pt | **Source:** PYQ (MK 2008 Q21) | **Skill:** place-value
**Figure:** `MK_PS1_CE1_grid.svg`

🐛 **Figure reveals answer:** The grid SVG has text below the image that shows or implies the answer (36). The figure should display only the blank grid structure — no answer, no totals, no summary text below it.

**Question:** How many 2-digit numbers have their ones digit strictly greater than their tens digit? (e.g. 12, 13, …, 19, 23, 24, …)
**Options:** 28 / 32 / **36 ✓** / 40 / 45
**Answer:** index 2
**Explanation:** Tens digit 1: 8 numbers (12–19). Tens digit 2: 7 numbers (23–29). …Tens digit 8: 1 number (89). Total = 8 + 7 + 6 + 5 + 4 + 3 + 2 + 1 = 36.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | For tens digit 1: ones can be 2,3,4,5,6,7,8,9 → 8 numbers. | *No change — good CUE.* | ✅ keep |
| 2 | For tens digit 2: ones can be 3,4,...,9 → 7 numbers. Continue for tens 3 through 8. Sum 8+7+6+5+4+3+2+1. | **Tens digit 2 gives 7 numbers. Tens digit 3 gives ___. Keep going all the way to tens digit 8. Then add all your counts together.** | ❌→✅ CUE |
| 3 | 8+7+6+5+4+3+2+1 = 36. (This is the sum of the first 8 natural numbers.) | ~~Removed — gave the full answer.~~ | ❌ removed |

---

## Challenge Extension 2 — Max Sum of Two 3-digit Numbers ✏️

**Type:** MCQ | **Difficulty:** 5pt | **Source:** PYQ (MK 2012 Q19) | **Skill:** place-value

**Question:** Using digits 1, 2, 3, 4, 5, 6 each exactly once, form two 3-digit numbers. What is the biggest possible sum?
**Options:** 1083 / 1128 / 1155 / **1173 ✓** / 1188
**Answer:** index 3
**Explanation:** Put 6 and 5 in the hundreds places, 4 and 3 in the tens places, 2 and 1 in the ones places. E.g. 641 + 532 = 1173.

✏️ **Language:** "maximise" → "biggest possible" throughout.

| Hint | Old text | ✏️ New text | Status |
|------|----------|------------|--------|
| 1 | To maximise the sum, pair the two largest digits (6, 5) in the hundreds places, the next two (4, 3) in the tens places, and the smallest (2, 1) in the ones places. | **Which place is worth the most — hundreds, tens, or ones? Put the two biggest digits in those places first.** | ❌→✅ CUE |
| 2 | Best: 641 + 532 = 1173. Or 642 + 531 = 1173. Both give the same sum. | **Try putting 6 and 5 in the hundreds places of your two numbers. Then arrange 4, 3, 2, 1 in the remaining places. Try a combination and add them up.** | ❌→✅ CUE |
| 3 | Place-value rule: hundreds digits contribute 100× more than ones. So always maximize the hundreds digits first: use 6 and 5 there. | ~~Removed — now covered by hints 1 and 2.~~ | ❌ removed |

---

## Summary of bug fixes

| Problem | Bug | Fix |
|---------|-----|-----|
| PT1 | Question text hidden behind figure | Add padding above figure in CMS layout |
| PT1 | Labeled chart gives away the answer | Replace labeled SVG with unlabeled chart OR redesign question (see above) |
| PT4 | Correct answer highlighted yellow in figure | Remove yellow highlight — equal styling for all cells |
| PT9 | Text overlaps pyramid figure | Add padding between question text and figure |
| PT10 | Text overlaps figure | Add padding between question text and figure |
| PT10 | □ renders as unrecognised square symbol | Replace □ with ? in question and all options |
| CE1 | Answer text visible below figure | Remove answer text from SVG caption/below-figure area |
