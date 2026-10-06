# Halden Tint

A passion-project landing page for a fictional window-tint and paint-protection studio. The whole page behaves like one continuous film: scroll and the car moves, the heat drains out, and a shade slider runs over real sunlight footage from Kuala Lumpur.

> Halden Tint is a made-up business. The email and phone number in the footer are placeholders, and the booking form is front-end only (it validates input and shows a thank-you message; nothing is sent or stored).

## Stack
- Plain HTML, CSS and JavaScript in a single `index.html`
- GSAP + ScrollTrigger (cdnjs) for scroll-driven motion
- Phosphor Icons (unpkg, pinned to 2.1.2), Geist / Geist Mono (Google Fonts)
- Brand logos from Simple Icons, placeholder photos from picsum.photos
- Short looping videos in `media/` used as scroll/hover backdrops

## How it was made
Built end to end with AI tools, as an experiment in how far a solo designer can get with a small credit budget.

1. **Design and code.** Claude Code wrote the page using the `design-taste-frontend` skill, which pushes away from generic template layouts toward a deliberate design direction.
2. **Video footage.** The clips in `media/` (`hero`, `heat`, `craft`, `kl-window`) were generated with **Higgsfield**, then trimmed and compressed to web-friendly H.264 mp4s with a poster `.jpg` for each.
3. **Launch video.** The share video was produced with the `brag` skill, which uses Hyperframes (`hyperframes-*` skills) to turn the site's code into a short composition. It is not included in this repo.

### Higgsfield prompt iterations
<!-- TODO(author): paste your real prompts below. Left blank on purpose rather than guessed. -->

| Clip | Iteration | Prompt | What changed / why |
|------|-----------|--------|--------------------|
| hero | v1 | _add prompt_ | _what looked wrong_ |
| hero | v2 | _add prompt_ | _what improved_ |
| kl-window | v1 | _add prompt_ | |
| kl-window | v2 | _add prompt_ | |

### Skills used
| Skill | Source | Used for |
|-------|--------|----------|
| `design-taste-frontend` | Leonxlnx/taste-skill | Anti-template layout and visual direction |
| `brag` | latent-spaces/brag | Turning the site into a launch video |
| `hyperframes-core`, `-animation`, `-creative`, `-audio`, `-keyframes`, `-cli` | heygen-com/hyperframes | Composition, motion and rendering for the launch video |

## Limitations
Not polished on purpose: video generation credits ran out, so some clips are single takes and a few details (placeholder photos, front-end-only form) were left as is.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` in this folder.
