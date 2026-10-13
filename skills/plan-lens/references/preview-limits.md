# What Lens Studio's preview can do

For the interviewing agent only. Never paste this into chat or offer it as a menu.

Everyone builds and demos in Lens Studio's preview: a simulated room on a laptop, walked with keyboard and mouse. Assume nobody has SPECS glasses. The demo video is a recording of the preview. So every done criterion must be something a person can check in the preview.

Based on Devpost's own CLAD builds in Lens Studio 5.24 (preview only) and Snap's docs. When in doubt, choose the version the preview can clearly show.

## Works well in the preview
- Walking around the Lens (WASD, Q/E, mouse look) and judging placement and readability.
- Objects placed in the room at real scale, anchored in front of the user at start, on the floor, or on a virtual table the Lens provides.
- SIK and UI Kit interactions driven by the mouse: pinch to press buttons, sliders, toggles, panels that follow or face the user, grab, drag, throw. Mouse = one hand doing a pinch.
- Spatial sound, simple physics, animation, text, 3D models (CLAD can generate models and sounds).
- The additive look (black shows as transparent) is simulated.
- LEAF tests can press buttons and simulate pinches and grabs on SIK interactables, so done criteria built on these can be tested automatically.

## Needs a stand-in
| The idea needs | Stand-in in the preview |
|---|---|
| Recognizing a real thing (sign, ball, text, object, food) | A button that says "found it," a pinch to mark where it is, or a hard-coded result. Build what happens next for real. |
| A real surface (your table, your wall) | A virtual table, wall or floor at real size. |
| A real place or route (walking directions) | A virtual path or markers in the room; a button to advance. |
| AI answers | May work in the editor, but plan a hard-coded answer as a fallback so the demo never depends on it. |
| Voice commands | May not work in the preview. Pair every voice action with a button. |
| Data from outside (weather, scores) | Hard-coded sample data. |

A 3D model of a real object does not stand in for recognizing it. The glasses don't recognize things from models.

## Can't be shown in the preview (keep out of done criteria)
- Two-hand gestures and custom gestures (swings, strokes, hand speed, hand poses, raw finger joints). The mouse only drives standard SIK interactions. These can be built and tested by CLAD with LEAF, but the learner can't try them or show them convincingly. If the learner insists, it's a Risk, and a standard interaction should carry the demo.
- Live camera vision on real frames (SnapML, reading the real world).
- Remembering things between sessions, or spatial anchors that persist.
- Two people sharing one Lens (Connected Lenses). Needs two devices and two people to demo.
- Feel: comfort over time, real hand-tracking dropouts, latency. Label these "feel unproven."

## Sizing the idea
One spatial moment, done well, is a full project. One standard interaction plus good placement and timing is plenty. If an idea needs several items from the stand-in table, or anything from the can't-show list, help the learner pick the one moment they most want in their video.

## Out of scope entirely
Recording, identifying, or following people who haven't agreed to it; face recognition; always-on capture of surroundings. Demo videos show the learner's own space.
