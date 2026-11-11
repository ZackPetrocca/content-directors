# The Content Directors

**A board of AI content directors for Claude. Bring an idea, or none, and they argue over it, score it and rule KEEP, RESHAPE or REJECT before you spend an hour making it. Then they hand you a shoot plan or a first draft.**

Each director reads a research file before it speaks, so it argues from a real point of view: Alex Hormozi on value, Sabri Suby on hooks, Gary Vaynerchuk on distribution, Seth Godin on what is worth remarking on, and Dan Martell on your time.

> **These directors are simulations built from public books, talks and posts.** They are not the real people. None of them has seen, reviewed or endorsed your content or this project. Never say or imply they did in anything you publish.

## Quick start

You need **Claude Code** or **Cowork** (plain chat on claude.ai cannot run skills).

```bash
git clone https://github.com/ZackPetrocca/content-directors.git ~/content-directors
mkdir -p ~/.claude/skills
ln -s ~/content-directors ~/.claude/skills/content-directors
```

Restart Claude, then type `/content-directors`.

The first run interviews you (who you sell to, what you sell, your proof, how you talk) and saves it to `~/content-directors/about-me.md`. After that it skips straight to the ideas.

Rather not use the terminal? Paste this into Claude Code: *"Clone https://github.com/ZackPetrocca/content-directors into ~/content-directors, link it as the skill ~/.claude/skills/content-directors, and show me how to start it."*

## What a run looks like

1. **You bring one of three things:** an idea to test, something to promote, or nothing (it gives you 10 ideas from your own business).
2. **It picks the format:** video, short video, carousel, graphic, text post or email, with the reason and a second choice.
3. **Three rounds of argument:**
   - The **Champion** builds the strongest version using only what you really have.
   - The **Executioner** brings the single best reason it fails, and the cheapest test to prove it.
   - The **Value Lens** and **Hook Lens** pick a side.
   - Bench seats (**Distribution**, **Remarkable**, **Founder-time**) sit in when the idea needs them, or when you ask for the full board.
4. **The Chair rules.** Six scores out of 10, then one word.
5. **You get the next asset:** a one-page shoot plan for a video (six opening lines, the points in order, b-roll, the ask) or a first draft for anything written.

A ruling looks like this (a made-up example):

```
THE CHAIR RULES: RESHAPE
The tip is useful but the opening is a greeting, and nobody stops for a greeting.
Lead with the number from the last listing instead. Keep the three steps.

Hook 4 · Value 7 · Proof 8 · Next step 5 · Effort 8 · Fit 7
Best format: short video (second: carousel)
Change: open on "This kitchen sat for 61 days. Here is what sold it in 9."
```

Rulings are saved to `~/content-directors/rulings/` with the date, so you can look back at what you kept and why.

## The seats

| Seat | Who | Asks | File |
|---|---|---|---|
| Champion | Role seat | What is the strongest version of this? | [`research/champion.md`](research/champion.md) |
| Executioner | Role seat | What is the one real reason this fails? | [`research/executioner.md`](research/executioner.md) |
| Value Lens | Alex Hormozi lens | Would the viewer feel silly not acting on this? | [`research/value-lens.md`](research/value-lens.md) |
| Hook Lens | Sabri Suby lens | Would a stranger stop in three seconds, and what does it capture? | [`research/hook-lens.md`](research/hook-lens.md) |
| Chair | Role seat | What is the ruling, and exactly what changes? | [`research/chair.md`](research/chair.md) |
| Distribution (bench) | Gary Vaynerchuk lens | Where is the attention now, and can this be made in volume? | [`research/distribution.md`](research/distribution.md) |
| Remarkable (bench) | Seth Godin lens | Is this worth remarking on, and who exactly is it for? | [`research/remarkable.md`](research/remarkable.md) |
| Founder-time (bench) | Dan Martell lens | Whose calendar does this land on? | [`research/founder-time.md`](research/founder-time.md) |

Each person file covers who they are and why they hold the seat, their core frameworks in their own terms, the questions they ask and the red flags they spot, how they talk, what they say about common content mistakes, two worked examples, where their lens misfires, and where to read or watch more.

The Chair scores six things: **hook, value, proof, next step, effort, fit**. Most content lands 4 to 6. KEEP means make it as pitched, RESHAPE means fix the named flaw and make it, REJECT means make something else.

## How Claude uses the research

Before each director speaks, the skill reads that seat's file in `research/`. The director then asks that person's questions, watches for their red flags and talks in their style. Anything marked **(verify)** in a file is something the research could not confirm, and the skill will not state it as fact.

## What is in this repo

```
content-directors/
├── SKILL.md            the /content-directors skill
├── README.md           this page
├── LICENSE
└── research/           one file per seat
    ├── champion.md
    ├── executioner.md
    ├── chair.md
    ├── value-lens.md
    ├── hook-lens.md
    ├── distribution.md
    ├── remarkable.md
    └── founder-time.md
```

Your own `about-me.md` and `rulings/` folder are created next to these files on your computer. They are in `.gitignore`, so they never get pushed anywhere.

## Make it yours

Every file in `research/` is plain text. Edit a seat, swap in a person you trust more, add a book you love, or add what your own results taught you. Claude reads whatever is there.

To get updates later:

```bash
cd ~/content-directors && git pull
```

## Where it fits

The Content Directors is step one of a three-step content system from the Origin community: **decide what to make** (this), **shoot and cut it** (Video Editing with Claude), then **approve and schedule it** (the Content Board).

## License

MIT. See [LICENSE](LICENSE). The research files summarize and paraphrase public work by the people named. Their books, talks and trademarks belong to them.
