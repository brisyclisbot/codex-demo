# Can you make 24? Original Codex Prompt

This file preserves the original prompt used to create the `can-you-make-24.html` app in this demo repo.

Target output:
- `can-you-make-24.html`

Original prompt:

```text
Build a single-page web application as one self-contained HTML file (HTML, CSS, and JavaScript all in the same file).

The page is NOT the main homepage of the site. I already have another index.html page that links to this SPA and other SPA pages. So this app should include a clear backlink near the top that goes to:

index.html

The app name should be:

Can you make 24?

The intended audience is casual Facebook viewers, so the design should feel:
- playful
- colorful
- rounded
- mobile-first
- clean enough not to look messy

Make it visually appealing on phones first, but also good on desktop.

Core game rules
- The game uses exactly 4 digits.
- Digits must be from 1 to 9 only.
- 0 is not allowed.
- Repeated digits are allowed.
- The goal is to make exactly 24.
- Allowed operations are addition, subtraction, multiplication, and division.
- Parentheses are allowed.
- Each of the 4 digits must be used exactly once.
- Show standard math symbols to users: +, −, ×, ÷
- Internally you can use normal JavaScript operators as needed.

The page should be a combined single page, not tabs. It should include:
1. A top area with the title, short instructions, and the backlink to index.html
2. A Play section
3. A Solver section

PLAY SECTION
This section should generate 4 digits for the player to solve.

Important:
- Generated puzzles must always be solvable.
- Do not generate unsolvable puzzles in play mode.

The player should NOT type raw text with the keyboard to answer. Instead, the app should use a guided expression builder.

Guided expression builder requirements
- Show the 4 digits as large tappable number cards.
- If digits repeat, each repeated digit must still appear as its own separate card.
- Show operator buttons: +, −, ×, ÷
- Show parentheses buttons: ( and )
- Show an expression display area so the user can see what they have built.
- Include buttons for:
  - Undo
  - Clear
  - Check
  - New Puzzle
  - Show Solution

Guided input behavior
- At the start, only a number card or ( should be allowed.
- After a number, only an operator or ) should be allowed.
- After an operator, only a number or ( should be allowed.
- A number card becomes disabled once it has been used.
- Undo should correctly restore the previous state, including re-enabling a number card if appropriate.
- ) should only be usable when there is an unmatched (.
- The app should guide the user enough to prevent obvious invalid input sequences, but it does not need to be overly complicated.

Validation behavior for Check
When the user presses Check, validate that:
- the expression is mathematically valid
- all 4 digits were used exactly once
- only the allowed operators were used
- the final result is exactly 24
- division by zero is handled safely as invalid

Use friendly validation messages for casual users, for example:
- You still need to use all 4 digits.
- This expression is incomplete.
- That equals 18, not 24.
- Nice work — you made 24!

SHOW SOLUTION behavior
- In play mode, Show Solution should reveal one valid solution for the current puzzle.
- It is fine to show just one solution in play mode.

SOLVER SECTION
This section should let users test their own 4 digits.

Requirements
- Use 4 separate input boxes.
- Each input box should accept exactly one digit from 1 to 9.
- 0 should not be accepted.
- Include a Solve button.
- When the user enters 4 digits and presses Solve, the app should determine whether a valid way to make 24 exists.
- If solutions exist, show up to 10 distinct solutions.
- If no solution exists, clearly show: No solution
- Display solutions nicely using the symbols × and ÷ instead of * and /
- Make the solver results area clean and readable, and fine on mobile.

Implementation expectations
- No backend.
- No frameworks required.
- No build tools.
- Just one self-contained HTML file that can be dropped into a static site or GitHub Pages project.
- Write clean, readable JavaScript.
- Keep the code understandable and reasonably organized.
- Include comments where useful.
- Make sure the page is responsive and touch-friendly.

Important implementation notes
- The Play section must only generate puzzles that have at least one solution.
- The Solver section must be able to detect both solvable and unsolvable 4-digit sets.
- Distinct solutions should be deduplicated reasonably well so the solver does not show obvious duplicates repeatedly.
- Use exact arithmetic carefully enough to avoid obvious floating-point mistakes where possible, especially for division-heavy expressions.
- The UI should feel polished for a casual audience, not like a developer demo.

Please output the final answer as the full complete HTML file only, with no extra explanation before or after it.
```
