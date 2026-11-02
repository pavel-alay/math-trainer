# Math Trainer

A single-page trainer for kids: multiplication tables (1×1 to 12×12) and mental addition/subtraction.
No dependencies, no build, one `index.html`. Made for Safari on iPad, works in any modern browser.

**Live:** https://pavel-alay.github.io/math-trainer/

## Modes

- **Multiplication & division.** Choose multiplication, division (42 ÷ 6 = ?) or mixed. Pick a zone on the table by dragging or tapping two corners
  (e.g. 2–3 × 2–10), or use a preset: 1–5, 1–10 (default), 1–12, 1–15. The table is 10×10;
  it grows to 12×12 or 15×15 only with the 1–12 or 1–15 preset.
  3×6, 6×3 and 18 ÷ 3 count as one fact; the factor order is shown at random.
  No fact repeats until the whole zone is used. Facts with ×1 and ×10 come last,
  so they only appear when the zone is bigger than the session.
- **Addition.** Choose addition, subtraction or mixed, set a range for both numbers,
  and choose whether carrying/borrowing in ones and tens is required, forbidden, or either.
  No repeats either (a + b and b + a count as one).

English, Polish and Russian UI (picked from the device language, switchable).
Dark theme follows the system setting.

## Timers

- **Length:** 10/20/30/40 problems as fast as possible, or as many as possible in 1/2/3 minutes.
- **Time per question:** no limit, or 10/7/5/3 seconds.
- Best result is kept per settings combination (stored in the browser).

A wrong answer is crossed out and the child tries again with a fresh question timer;
if fixed, the problem still goes to the end of the queue and comes back after all new ones.
After a second wrong answer, or when the question timer runs out, the right answer is shown
in green for 3 seconds and the problem goes to the end of the queue. It keeps coming back,
marked "Repeat N", until it is solved, and every mistake doubles its question time limit.
The Skip key (left of 0) shows the answer right away, the same way: it counts as a mistake
and the problem comes back later.

Time per problem covers every attempt it took, including the ones caused by mistakes.
The 3-second answer display counts toward the total time only.

## Weak spots

Every run remembers weak facts (in the browser) and brings them back in the next runs.
A mistake marks a fact for 3 clean answers; a slow answer (over 1.5× the run's median and over 2 s)
for 1. Each quick, clean answer takes one off. 6×8, 8×6, 48 ÷ 6 and 48 ÷ 8 are one fact;
after a mistake it comes back in both orders. Weak facts fill every second slot
until used up, up to 40% of a counted run (or one per 10 s of a timed one), and only
if they fit the current settings. The setup screen lists the facts waiting for practice.

The setup table marks weak facts with a dot (orange: slow, red: mistakes). After a
multiplication run the results show the table (10×10, or 12×12 / 15×15 once such facts
have come up) coloured from red (mistakes) through
yellow (slow) to green (known); a known fact gets greener with each quick, clean answer in a row,
up to 5. Grey cells have not come up yet. Only the lower half is shown: 6×8 and 8×6 are one fact,
so the mirrored half would count every mistake twice. Column numbers sit on the steps
right above each column.
The results screen may scroll; Menu and Again stay pinned to the bottom.

## Stats

The results screen has a summary for parents, for the current mode (multiplication and
addition are counted apart): last run, today, all time. The Stats tab at the top of the menu
shows the same summary for both modes and the coloured table. Rows: solved, share of answers
without a mistake, average time per problem, practice time. Kept per day in the browser.
The share without mistakes (green at 100%, red at 50%) and the time per problem
(green at 2 s, red at 8 s) are coloured on the same red-to-green scale as the table.

## iPad tip

Open the link in Safari, then Share → Add to Home Screen to run it full screen like an app.
