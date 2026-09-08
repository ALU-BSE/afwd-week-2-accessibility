# Activity 1 — Fix the Broken Form

**25 minutes of work · 7 minutes of share-back · groups of 3–4**
Evidences learning outcomes 1 and 2.

`starter-files/starter-form.html` is a course registration form. It looks finished
and is broken underneath. Eight defects, one per category listed below. Find them,
repair them in the markup, and prove each repair.

## The rule

You may not fix anything you cannot first demonstrate is broken.

Show the failure, then show the fix, then show the failure is gone. A repair with
no before-state is not assessed, however correct the code is.

## Verify every fix two ways

**By keyboard.** Tab through the form. Can you reach everything? Can you see where
you are at every stop? Does the order match the visual layout?

**By screen reader.** VoiceOver (Cmd + F5) or NVDA. Is every field announced with a
name that means something? "Edit text, blank" means the field has no accessible
name, whatever is printed next to it on screen.

## Where to look

Eight categories, one defect in each. The categories are the hint; the locations
are not.

1. Labels and how they are associated
2. Input types
3. Button semantics
4. Grouping of related controls
5. Error messages and how they are announced
6. Tab order
7. Focus visibility
8. Anything that exists only as placeholder text

Two of the eight are the failures you hit in the cold open. Naming those two is
part of the exercise.

## Record every defect

Use the defect log (`print/worksheets.pdf`, page 1). For each one:

| What was wrong | Line | Your fix | How you verified it |
|---|---|---|---|

"How you verified it" is the column that carries the marks. "Looks right now" is
not a verification. "Reader announced 'Phone number, edit text' instead of 'edit
text, blank'" is.

## Share-back

Two minutes per group. Name the defect you argued about most, rather than reciting
all eight. Disagreement usually sits on the fake button and on whether a visible
heading counts as a label, and both arguments are worth the room's time.

## Marking

Ten marks, collected on the log.

| Criterion | Marks |
|---|---|
| Defects found and correctly categorised (1 mark per 2 defects) | 4 |
| Repairs are correct and use native HTML wherever it will do the job | 3 |
| Every repair carries a verification that names the observed before and after | 3 |

Marks are lost for repairs that add ARIA where a native element would have worked,
and for any entry where the verification column repeats the fix instead of
describing an observation.
