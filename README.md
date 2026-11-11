# Content Directors research

This is the research behind the Content Directors skill. It gives each director a real point of view to argue from, so the debate over your content idea sounds like a sharp person in the room and not a generic AI.

## What is in here
- `SKILL.md`: the /content-directors command, a version that reads the research first.
- `research/`: one file per seat.
  - **Value Lens**: how Alex Hormozi judges offers and value.
  - **Hook Lens**: how Sabri Suby judges hooks and direct response.
  - **Distribution**: how Gary Vaynerchuk thinks about attention, volume and platform-native content.
  - **Remarkable**: how Seth Godin thinks about what is worth remarking on, permission and the smallest audience that matters.
  - **Founder-time**: how Dan Martell thinks about your hours, leverage and systems.
  - **Champion, Executioner, Chair**: the three role seats with no person behind them. These hold how each argues, the six-point score (hook, value, proof, next step, effort, fit) and the KEEP, RESHAPE or REJECT rule.

Each file covers who the person is and why they hold the seat, their core ideas in their own terms, the questions they ask and the red flags they spot, how they talk, what they would say about common content mistakes, and where to read or watch more.

These are simulations built from public work. They are not the real people, and none of them has seen or approved your content. Never say or imply they did. Items marked **(verify)** are ones the author was less sure of, so check them before relying on them.

## How Claude uses it
Before each director answers, Claude reads that seat's file in `research/`. The director then asks that person's questions, watches for their red flags and speaks in their style. The three extra seats (Distribution, Remarkable, Founder-time) sit in when your idea needs them, or when you ask for the full board.

## Install
Ask Claude to do this for you, or do it yourself:

1. Put this folder at `~/content-directors` (clone it there, or download it and move it).
2. Copy `SKILL.md` to `~/.claude/skills/content-directors/SKILL.md`.
3. Restart Claude Code or Cowork, then type `/content-directors`.

The skill reads `research/<seat>.md` before each director answers. Your own `about-me.md` and `rulings/` folder live in the same place and stay on your computer, since they are ignored by git.

## Make it yours
Add or edit any file in `research/`. Swap a seat's person for someone you trust more, add a book you love, or add what you have learned from your own results. Claude reads whatever is there.
