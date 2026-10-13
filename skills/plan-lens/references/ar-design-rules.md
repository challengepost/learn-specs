# AR design rules for glasses

For the interviewing agent only. Never paste this into chat or offer it as a menu. Use it to ask better follow-ups and to push back once, briefly, with a reason. These mirror the Learn AR with SPECS concept video, so the learner has heard them.

## The core idea
A laptop and glasses can both show a screen. The difference is that this screen is attached to your head. Coding agents can now build a working Lens from a good description, so the learner's job is the design: make it a real app people would use, make it comfortable, and make it better than the laptop version.

## Three things glasses do that a laptop can't
1. **They share your view.** The camera sees what you're looking at, from where you're looking. Examples: translate the sign in front of you, "what am I looking at?", line up a shot on a real pool table.
2. **They draw in the world.** Content can sit on the table, over the stove, at real size, where it belongs. Examples: a defender on your court, a timer floating over the pot, a game board on your kitchen table.
3. **They leave your body free.** Hands available, eyes up, free to walk. Examples: follow a recipe while you cook, feedback mid-swing, directions while you walk.

Good AR uses one. Great AR combines them. The test: Does it use what I'm looking at? Does it put something in my space? Does it free my hands or let me keep my eyes up?

## Four habits: design for glasses, not for a screen
1. **Not a website floating in front of your face. Put information on the thing it's about.** The timer over the pot, the score by the table. (Google Design, transparent screens; Microsoft, the holographic frame)
2. **Not everything on display all the time. Show it when it's needed, then get out of the way.** Looking at a glasses display is "an active, physical choice," so every glance has to earn it. (Google Design; Android AI glasses principles)
3. **Not a menu full of small buttons. A few big targets. Pinch is the new tap.** Hands are a noisy input: keep a small, consistent set of gestures, and make targets big and forgiving. (Meta, hand interaction best practices)
4. **Not a panel behind your shoulder. Keep it where they're already looking.** The display covers only part of what you see; anything outside it is easy to miss. Keep status next to the task. If something is out of view, use a sound or a small hint to point the way. (Microsoft, the holographic frame)

## Comfort and placement numbers
- SPECS' view is narrow: about 37° tall by 32° wide. Big real-scale objects never fit in view at once, so design around where the user is already looking, often down at their hands or the table.
- The display's focus plane is about 1 m. Put main content roughly 0.6 to 1.6 m away, a little below eye level.
- Snap's usable area at distance (height x width, cm): 35 cm away 13 x 24; 55 cm away 23 x 38; 110 cm away 53 x 77; 160 cm away 75 x 112.
- Keep arms low. Raised-arm tasks tire people fast.
- Real-scale things need real empty floor around them; a virtual table will intersect real furniture.
- Additive display: black renders as transparent. Avoid relying on dark content.

## The worked example (from the video)
First try: "Make a cooking lens that puts a timer above each pot on the stove." Result: timers float over pots, nothing teaches you anything.

After the interview: "Coach me through risotto at my stove. Over each pan, show a small dot that opens into the step and timer only when it needs me, like 'add a ladle of stock now.' One big pinch button per pan to move on. If something behind me needs attention, chime and point an arrow toward it."

Four questions got there: what should it help with beyond timers (teach a technique), when should things be visible (only when they matter), how do you move on with messy hands (one big pinch button), what if something behind you needs attention (chime and arrow). This is the level of specificity the brief should reach.

## Consent
Don't build Lenses that record, identify, or follow people without their consent. This hackathon is about experiences in your own space. State it once, without a lecture, and ask which part of the idea matters most.
