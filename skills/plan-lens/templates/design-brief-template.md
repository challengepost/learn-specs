---
status: draft
---

# Design brief: <Lens name>

<!-- Filled in by plan-lens from the learner's interview. Use the learner's words. Mark any value they didn't choose as (default). -->

## The one spatial moment
<One or two sentences: what the user is doing and what they see when the Lens is at its best.>

## Why it belongs on glasses
- Uses: <shares your view / draws in the world / leaves your body free; one or more>
- Why it's better than the phone or laptop version: <...>

## Product or overlay
- Type: <product: the virtual thing is the experience | overlay: it responds to something real>
- What the real version would sense: <... or "nothing">
- Stand-in for the preview: <how the Lens fakes recognition, e.g. a "Found it" button or a hard-coded answer; or "none needed">

## Where things live
- Where the user is looking during the main task: <...>
- <Element>: <where it sits, what it's anchored to, distance and height, size in cm>
- <Element>: <...>

## Hands and input
- <Action>: <pinch / grab / drag / throw / button / slider, on what>
- Targets are big and highlight when aimed at.
- Voice (if any) and the button that does the same job: <...>

## When things show
- <Element>: shows when <...>, hides when <...>
- If something needs attention out of view: <sound / small arrow / none>

## Done criteria
Each one can be checked in Lens Studio's preview.
1. <...>
2. <...>
3. <...>

## Out of scope
- <What this version won't do.>

## Risks and open questions
- <Choices the learner kept despite a concern, and anything only real glasses could answer. Or "none".>

## Build notes for CLAD
- Build for SPECS so it runs and can be demonstrated in Lens Studio's preview. No SPECS device is available.
- Use Spectacles Interaction Kit (SIK) and UI Kit for all interactions, so they work with the mouse in Interactive Preview and with LEAF.
- Build any stand-in exactly as described above, and keep it obvious in the scene.
- Use real-world scale in centimeters. Keep content inside the user's view during the main task.
- The display is additive: black renders as transparent. Don't rely on black or very dark content to be seen; keep text light and readable from where the user stands.
- Get the basic flow working first, then add detail.
- Write LEAF scenarios for each done criterion, run them in preview, and report which pass. Say which criteria have no test.
- Don't record, identify, or follow people.

## After the build: judge it
This part is for you, after CLAD finishes.

1. **Does it work?** Ask your agent which LEAF tests passed and which done criteria have no test.
2. **Walk around it.** Open the preview in Interactive Preview. Use WASD to move, Q and E to go down and up, and right-drag (or hold Shift) to look around. Clicking acts as a pinch. Stand where a user would and look at the task.
3. **Ask the three questions.**
   - Does it use what I'm looking at?
   - Does it put something in my space, where it belongs?
   - Does it free my hands or let me keep my eyes up?
   - Would it be just as good on a phone? If so, what would make it need the glasses?
4. **Check comfort.**
   - Everything I need is in view while I do the task. Nothing sits at the edges, behind me, or stuck to my face.
   - Every control is within reach of someone standing there.
   - Text reads easily from where I stand. No dark UI disappearing.
   - Things show when needed and get out of the way.
5. **Label what you know.** Write "logic proven" next to anything the tests and preview show working, and "feel unproven" next to anything only real glasses could tell you (comfort over time, real hand tracking, real recognition).
6. **Fix with design notes, not code.** Tell your agent what to change in design terms, for example: "Move the step card 15 cm lower and next to the pan. Make the Next button twice as big. Re-run the tests." If a fix takes under a minute, like nudging a panel, do it yourself in the scene.
7. **Submit.** Record a video under 3 minutes of your Lens in the preview, public on YouTube. Make your repo public with your Lens Studio project and this `devpost/` folder. Details are on the hackathon site: https://learn-specs.devpost.com/resources
