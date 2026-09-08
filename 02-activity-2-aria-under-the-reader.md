# Activity 2 — ARIA Under the Reader

**20 minutes · pairs**
Evidences learning outcome 3.

`starter-files/components.html` holds two broken components. Screen reader on for
both. If you cannot hear the difference, the fix does not count.

## 1. The fake button

The filter chips are `<div>`s with click handlers. Tab never reaches them, the
reader announces them as text, and Enter and Space do nothing.

You have two routes. **Decide, then defend the decision in writing.**

- **Route A — make the `<div>` behave.** Add the role. Add `tabindex`. Handle Enter.
  Handle Space, and stop the page scrolling when you do. Then work out how the
  pressed state gets announced.
- **Route B — replace the element.** Use `<button type="button">`.

Count the changes each route costs before you choose. Write the count down; it is
the evidence that you chose rather than guessed.

Whichever route you take, the chips are a toggle set, so the reader has to announce
which one is currently on.

## 2. The silent counter

The results count updates when you filter and says nothing. Make it speak, politely.

Then select **Postgraduate**, which matches no course. An empty-state message
appears on screen. Make that speak too.

The second one will probably fail on your first attempt. When it does, re-read the
last line of the live regions slide before you change anything else.

## Then swap

Swap laptops with another pair and listen to theirs with the reader on. You are
listening for two things: whether the chip announces its pressed state, and whether
the empty-state message arrives without being asked for.

## What to submit

On Canvas, before midnight, as `w2s1-<your-name>`:

1. The repaired `components.html`.
2. Your written defence of the fake-button decision: which route, how many changes
   it cost, and why you chose it. Four sentences is enough.
3. One line per component naming what you heard before and after.

## Marking

Ten marks.

| Criterion | Marks |
|---|---|
| The fake button is operable by keyboard and announced with the right role | 3 |
| The decision is defended with the change count, not with a preference | 2 |
| The counter announces politely, without interrupting | 2 |
| The empty state announces, with the live region present before the content changes | 2 |
| Both fixes verified by ear, with the before and after described | 1 |

The full ten is reachable by either route. A pair that took the ARIA route, listed
all four changes and explained why they accepted the cost scores the same as a pair
that reached for `<button>`. A pair that reached for `<button>` because it was
easier, without being able to say what the alternative cost, does not.
