# 如何逃離小妖湖 / Escape the Little Monster Lake

In addition to existing `index.html` and the other SPAs, I want you to create another complete single-page web app game that can be deployed on GitHub Pages with no backend, which will be linked from the `index.html`.

Please read all requirements carefully and implement the app in a way that is polished, visually appealing, mobile-friendly, and easy for a general Facebook audience to play.

The game is based on the classic puzzle where a person in a boat starts in the center of a circular lake, while a cute monster runs around the edge of the lake. The monster moves faster than the player. The player must try to escape by reaching the shore at a point where the monster is not there. The app should focus on being a fun, shareable interactive game rather than a strict mathematical simulator, but the movement and logic should still feel believable and consistent.

## High-level goals

- Build a single-page app game
- Pure frontend only
- No backend
- Suitable for GitHub Pages
- Easy for AI to generate in one pass
- Mobile-first, but still looks good on desktop
- Strong game feel
- Slightly cute/cartoon style
- Shareable and attractive enough that Facebook viewers may want to try it

## Title

- Main title: `如何逃離小妖湖`
- English subtitle: `Escape the Little Monster Lake`

## Language

- Bilingual Chinese and English throughout the interface
- Keep text short and natural
- Do not make the page text-heavy
- Prioritize visual clarity over long explanations

## Target audience

- General Facebook audience
- People should be able to understand the game quickly without reading a lot
- The first impression should be engaging and playful

## Design direction

- Mobile-first layout
- Top-down view
- Slightly cartoon-like
- Strong game feel
- Use a parchment / puzzle-book visual style for panels, buttons, and UI framing
- The lake should be a circular blue lake
- Add subtle water ripple effects
- Add grassy shore around the lake
- The player is a small boat
- The monster should be cute rather than scary
- The whole experience should look charming and polished, but not overly complicated

## Important design balance

- Combine puzzle-book / parchment UI with playful game visuals
- UI frame, buttons, cards, and overlays can use parchment / old puzzle book styling
- The lake, boat, and monster should still feel lively and game-like
- Avoid making the whole app look dull or like a school math exercise

## Technical constraints

- No backend
- No login
- No database
- No audio
- No music
- No external services
- Keep it simple to host on GitHub Pages
- Minimize build complexity
- Prefer a version that can run easily as static files
- Do not require a server
- Do not over-engineer the project

## Implementation preference

- Prioritize a fully playable, complete, polished result over fancy architecture
- First priority is a working game with clean UI and smooth interaction
- Second priority is visual polish
- Third priority is extra small enhancements
- Do not sacrifice usability for visual complexity

## Core gameplay

- There is only one main level
- The purpose is to showcase the puzzle concept clearly
- The player starts at the center of the circular lake
- A cute monster moves around the circular boundary of the lake
- The player controls the boat by dragging
- The boat can move in any direction within the lake
- If the player reaches the shore at a location where the monster is not there, the player escapes and wins
- If the monster catches the player at the shore, the player loses
- The movement rules should feel fair and understandable

## Interaction

- Control method must be drag-to-move
- On touch devices, dragging should feel natural and responsive
- On desktop, mouse dragging should also work smoothly
- The drag control is very important and should feel good
- The user should not need to tap tiny buttons to move
- Avoid clumsy joystick UI unless truly necessary
- The boat should follow drag input smoothly
- Make sure touch interaction still works even if the finger partially covers the boat
- Prevent awkward control behavior near the edge of the lake
- The boat must stay inside the lake until escape is triggered

## Game feel requirements

- Smooth animation
- Clear motion
- Clear feedback when winning or losing
- The game should feel fun to try repeatedly
- It should feel suitable for casual social sharing
- Avoid overly stiff or overly technical simulation presentation

## Main screen requirements

- Show the title and subtitle
- Show a prominent `Start Now / 立即開始` button
- Keep the first screen simple and attractive
- Do not overwhelm users with instructions at the start
- The user should be able to start playing quickly

## Required UI features

- Start button
- Visible speed multiplier for the monster
- Visible timer during gameplay
- Visible trajectory line(s)
- Best record / best time
- Retry / play again button after game ends
- A best strategy hint area after the run ends
- A short explanation of the underlying puzzle only after the player has finished a run
- Parameter controls so the user can change the monster speed multiplier and possibly a few other simple settings

## Feature decisions

- Include tutorial mode: yes
- Hint mode during play: no
- Show monster speed multiplier: yes
- Show trajectory lines: yes
- Pause: no
- Restart during play: not necessary, but a simple reset button is acceptable if it improves usability
- Phone vibration: no
- Score/rating system: no
- Timer: yes
- Best record: yes
- Auto-solve / AI demonstration: no
- The player should figure it out by themselves

## Tutorial requirements

- Keep tutorial very short
- It should not block users for too long
- A small onboarding overlay is okay
- Explain only the essentials:
  - drag the boat to move
  - avoid the monster
  - reach the shore safely to escape
- Let the user dismiss the tutorial quickly
- Make tutorial bilingual
- Do not make the tutorial verbose

## Post-game requirements

After each run, show:

- Whether the player escaped or got caught
- Time used
- Best record if applicable
- A play again button
- A short `best method hint / 最佳方法提示`
- A short explanation of the concept behind the puzzle
- The explanation should appear only after the player has finished a run
- The explanation should be concise, beginner-friendly, and interesting
- Avoid sounding like a textbook

## Parameter customization

Include simple parameter controls, but keep them limited and neat.

Possible controls:

- Monster speed multiplier `n`
- Optional simple difficulty preset or a small number of sliders
- Use reasonable min/max constraints
- Prevent absurd values that break the experience
- Use mobile-friendly controls such as sliders or step buttons
- Provide sensible defaults
- Keep the controls visually clean and not cluttered

## Important scope control

- Do not add multiple levels
- Do not add backend features
- Do not add accounts
- Do not add online leaderboard
- Do not add complex menus
- Do not add unnecessary settings panels
- Do not add sound systems
- Do not turn this into a large game
- Keep it focused on one polished puzzle experience

## Visual details

- Circular lake with blue water
- Gentle ripple effect
- Grassy circular shore
- Small boat for the player
- Cute monster running along the edge
- Clean path / trajectory visuals
- Parchment-styled control panels and result cards
- Appealing button design
- Make it look good enough for demo/showcase use
- Avoid a cheap prototype appearance

## Responsiveness

- Mobile-first is the top priority
- Must look good on phone screens
- Must remain playable on desktop
- On desktop, center the game nicely and use space well
- Make sure UI does not overlap badly on smaller screens
- Keep important controls reachable on mobile

## Game logic expectations

- The monster should move along the edge of the circular lake
- The boat moves inside the lake
- Win/loss logic should be clear and consistent
- The logic does not need to be a perfect mathematical research simulator, but it must feel coherent
- The player should be able to experiment with movement strategies
- The game should encourage replay

## Trajectory and visual feedback

- Show the boat path
- Show the monster path if appropriate
- The trajectory should help users feel the strategy element
- Do not make the screen overly noisy
- Use tasteful visual feedback rather than clutter

## Content tone

- AI demo showcase style
- Lightly playful
- Friendly and modern
- Not too childish
- Not too academic
- Not too technical
- Suitable for general social sharing

## Sharing appeal

- The result should be visually interesting enough that someone watching on Facebook may want to try it
- The game should have a clear `let me try one more time` feeling
- The app should be immediately understandable from the visuals

## Important coding instruction

Please aim to reduce future back-and-forth changes by making thoughtful product decisions where details are not specified, while staying faithful to the requirements above.

Please make the app feel complete, not like a rough prototype.

Please prioritize:

1. Playable and polished
2. Mobile-friendly
3. Easy to deploy on GitHub Pages
4. Clean and simple structure
5. Shareable visual appeal

Please avoid:

- backend
- unnecessary dependencies
- over-complicated architecture
- text-heavy UI
- overly technical presentation
- ugly placeholder visuals
- making it feel like homework

## Edge cases to handle

- Dragging outside the lake
- Releasing drag abruptly
- Very fast repeated restarts
- Changing parameters and replaying
- Small mobile screens
- Boat touching boundary ambiguously
- Monster and player arriving near the same point at nearly the same time
- Ensuring best record updates correctly
- Preventing broken layouts on narrow screens

## Output expectation

Please generate the full implementation, including all necessary HTML, CSS, and JavaScript, in a clean structure suitable for a static site.

If you choose a multi-file structure, keep it simple and clearly organized.
If you choose a single-file structure, keep it readable.

Also:

- Include brief setup/run instructions
- Mention where I should place the files inside my GitHub Pages project
- Keep the implementation practical and easy to copy into an existing site that already has an `index.html` linking to multiple SPAs

## Final reminder

This should be a polished, fun, cute, mobile-friendly single-page puzzle game called `如何逃離小妖湖 / Escape the Little Monster Lake`, designed for a general audience, with drag-to-move boat control, a circular lake, a cute monster on the shore, a parchment/puzzle-book UI style, replayability, parameter tweaking, post-game explanation, bilingual text, and no backend.
