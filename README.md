# Unstuck

**Know what to say.** An AI skill for every message you're stuck on: a Hinge match going quiet, "I can't do this relationship anymore", a coffee chat that didn't turn into a referral, a professor who said no, a manager asking where your work is, a client who hasn't paid.

Works with Claude, ChatGPT, Gemini, Codex, Cursor, Copilot, and any agent that reads the open `SKILL.md` format.

## What it does

Paste the message (or describe the situation) and Unstuck:

1. **Decodes it:** what they said, what they most likely mean, and what they're feeling
2. **Switches perspective:** how your reply will land on *their* end, and what they're worried about
3. **Names your goal:** get the outcome, keep the relationship, or keep your self-respect, and shows the trade-off
4. **Gives 2–3 reply options:** real strategies, not one message in three tones, each with "gets you / risks", plus a pick
5. **Sounds like you:** platform-native (Hinge ≠ email ≠ Slack) and matched to your texting style
6. **Tells you when to send:** now, after a break, or as a call instead. Includes what *not* to do and what to say if they reply X.

```
**Reading it:** A decision, not an opening to negotiate. She's been thinking about it for a while and is bracing for a bad reaction.
**From their side:** A calm reply will be a relief. Pleading makes her more sure.
**Your goal here:** Self-respect and ending on a good note.

**Option A — Gracious and honest** (recommended)
> that's really hard to read but I appreciate you telling me straight. I've genuinely enjoyed being with you. I'm not going to try to change your mind, take care of yourself ok?
Gets you: you leave with your head up · Risks: no closure on why

**Before you send:** wait 30–60 min if you're upset. Don't ask "is there someone else."
```

## Covers

| Area | Examples |
|---|---|
| Dating and texting | Openers, dry convos, asking out, ghosting, slow replies |
| Relationships | Breakups, fights, apologies, exes, ending things kindly |
| Friends and family | Saying no, boundaries, guilt, conflict |
| LinkedIn and networking | Cold outreach, coffee chat follow-ups, no referral, post comments |
| Job search | Recruiters, rejections, ghosting after interviews, offers, negotiation |
| School | Extensions (and when they're denied), grades, rec letters, group projects |
| Work | "You're late on this", pushback, mistakes, asking for things |
| Clients | Scope creep, late payments, bad news, angry clients |

## How it's different

Most communication skills and AI wingman apps are either **workplace-only** or **dating-only**, give **one draft**, and stop there. Unstuck:

- covers **every relationship** in one skill
- takes the **other person's perspective** before drafting
- gives **options with trade-offs** instead of one "perfect" message
- includes **timing, channel advice, and "if they reply…" follow-ups**
- is built on real frameworks: DBT (DEAR MAN, GIVE, FAST), Nonviolent Communication, BLUF, SBI, and Gottman's repair work (used behind the scenes, never as jargon in your messages)
- has **guardrails**: no manipulation, no pressuring someone who said no, and safety first when a message involves self-harm, threats or abuse

## Install

### Any coding agent (one command)

Claude Code, Codex, Cursor, Gemini CLI, GitHub Copilot, OpenCode, Cline, Windsurf, and more:

```
npx skills add jayeed17/unstuck
```

### Claude Code (plugin)

```
/plugin marketplace add jayeed17/unstuck
/plugin install unstuck@unstuck
```

### ChatGPT (Custom GPT or Project)

ChatGPT → **Explore GPTs** → **Create** → **Configure** → paste [`prompts/instructions.md`](prompts/instructions.md) into **Instructions** (it fits the 8,000-character limit) → Save. Or paste it into a ChatGPT **Project**'s instructions.

### Gemini (Gem)

Gemini → **Gems** → **New Gem** → paste [`prompts/instructions.md`](prompts/instructions.md) → Save.

### Claude app (claude.ai / desktop)

Upload `skills/unstuck` as a zip in the app's Skills settings, or paste [`prompts/instructions.md`](prompts/instructions.md) into a Project's instructions.

### Anything else

Paste [`prompts/instructions.md`](prompts/instructions.md) into the system prompt or custom instructions of any AI tool.

## Usage

Just talk to it:

- "she said 'I don't think I can do this relationship anymore' — what do I say"
- "coffee chat went well but no referral, app closes friday"
- "professor said no extension, how do I reply without being weird"
- "manager on slack: where is the deck?? it was due yesterday"
- "hinge match only replies 'haha'"
- "review my draft before I send it: …"
- "just write it" (skips the analysis)

Paste screenshots or the exact message for the best read.

## Repo layout

```
skills/unstuck/
  SKILL.md                    # core workflow (open Agent Skills format)
  references/
    contexts.md               # playbooks: dating, relationships, LinkedIn, school, work, clients…
    channels.md               # platform norms + timing
    frameworks.md             # DBT, NVC, BLUF, SBI, Gottman, apology structure
    examples.md               # worked examples
    guardrails.md             # ethics, safety, limits
prompts/instructions.md       # single-file version for ChatGPT, Gemini, etc.
evals/scenarios.md            # test prompts with pass/fail criteria
AGENTS.md                     # pointer for agents that read AGENTS.md
.claude-plugin/               # Claude Code plugin + marketplace manifest
```

## Contributing

Found a situation it handles badly? Open an issue with the (anonymized) message and what went wrong, or add a scenario to `evals/scenarios.md`.

## Disclaimer

Unstuck is communication coaching, not therapy, legal or HR advice. If you or someone you're talking to is in crisis, contact local emergency services or a crisis line (in the US, call or text 988).

## License

MIT © Zayeed Bin Kabir
