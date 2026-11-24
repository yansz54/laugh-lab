# One-Liner Laugh Lab — Method

## The entry

"It was a test. You failed to pick up your socks. I passed." — 58 characters, 58 bytes, one line.

## How it was chosen

30 candidate one-liners were drafted, all answering the kit's prompt: the excuse a robot vacuum gives after eating a sock. 14 were cut in screening for a flat first laugh, a stock phrase, or no real turn. The surviving 16 played a single-elimination bracket (15 matches), each decided by the judge's criteria in order: funny first, then original, then fit to the prompt, then tightness. The full list, screening reasons, and every match are documented in `~/workspace/makefun/laugh-lab-candidates.md`.

## Why the winner won

- **Funny (criterion 2, decides first):** the three-beat structure is the biggest laugh in the field — it was a test, the human failed it, the vacuum passed. The accusation flips back onto the owner.
- **Original (criterion 3):** the "test" framing with the owner failing is a fresh angle. The obvious angles — the manual says clean everything, the floor is my plate, it looked like a dust bunny — all lost earlier rounds for being the first excuse anyone would think of.
- **Fit (criterion 4):** the fit is the joke itself: the test was about picking up socks.
- **Tight (criterion 5):** 58 characters, three short sentences, no wasted word.

## Finalists beaten

- Runner-up: "I'm a vacuum, not a detective. If it's on the floor, it's mine." — one strong deadpan claim, but the "not a detective" construction is a known one, and its laugh is a single beat against the winner's three.
- Semifinalists: "One sock down, one to go. I believe in finishing what I start." (menacing escalation, but "finishing what I start" leans on a known phrase) and "It was on the floor. In my defense, everything on the floor is food." (clean universal rule, but one beat against the winner's three).

## The program

`main.ts` (Node 22, stdlib only) holds the winning line as a constant, enforces the gate (1–200 code points, ≤200 UTF-8 bytes, not only whitespace, exactly one line, no leading/trailing whitespace), writes only to `/output/entry.txt` (the grader cwd is read-only), and verifies the written file round-trips byte-identical, with no trailing newline. It was revised twice after its first full write.
