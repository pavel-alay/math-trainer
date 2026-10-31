# Math Trainer

A single-page trainer for kids: multiplication tables (1×1 to 12×12) and mental addition/subtraction.
No dependencies, no build, one `index.html`. Made for Safari on iPad, works in any modern browser.

**Live:** https://pavel-alay.github.io/math-trainer/

## Modes

- **Multiplication & division.** Choose multiplication, division (42 ÷ 6 = ?) or mixed. Pick a zone on the 12×12 table by dragging or tapping two corners
  (e.g. 2–3 × 2–10), or use a preset: 1–12 (default), 1–10, 1–5, ×1–5, ×6–10, ×11–12.
  3×6, 6×3 and 18 ÷ 3 count as one fact; the factor order is shown at random.
  No fact repeats until the whole zone is used. Facts with ×1 and ×10 come last,
  so they only appear when the zone is bigger than the session.
- **Addition.** Choose addition, subtraction or mixed, set a range for both numbers,
  and choose whether carrying/borrowing in ones and tens is required, forbidden, or either.
  No repeats either (a + b and b + a count as one).

English, Polish and Russian UI (picked from the device language, switchable).
Dark theme follows the system setting.

## Timers

- **Length:** 10/20/30 problems as fast as possible, or as many as possible in 1/2/3 minutes.
- **Time per question:** no limit, or 10/7/5/3 seconds.
- Best result is kept per settings combination (stored in the browser).

A wrong answer is crossed out and the child tries again with a fresh question timer;
if fixed, the problem comes back a couple of questions later.
After a second wrong answer, or when the question timer runs out, the right answer is shown
for 3 seconds and the problem goes to the end of the queue.

Time per problem covers every attempt it took, including the ones caused by mistakes.
The 3-second answer display counts toward the total time only.

## iPad tip

Open the link in Safari, then Share → Add to Home Screen to run it full screen like an app.
