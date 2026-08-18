

# offensive-ai-speak

Shit that AI does that is annoying and should not do but it does it anyways.

This repo is also an installable **agent skill** ([SKILL.md](SKILL.md)) that tells your agent to stop doing all of it.

## Install as a skill

Works with Claude Code and anything else that supports the [Agent Skills](https://agentskills.io) standard.

```bash
# personal (all projects)
git clone https://github.com/chitalian/offensive-ai-speak ~/.claude/skills/avoid-ai-speak

# or per-project (run from the project root)
git clone https://github.com/chitalian/offensive-ai-speak .claude/skills/avoid-ai-speak
```

That's it. The agent will pull it in automatically when writing prose, or you can invoke it directly with `/avoid-ai-speak`.

## The list

The short version. Full blocklists live in [references/phrases.md](references/phrases.md) and [references/patterns.md](references/patterns.md), with sources in [references/sources.md](references/sources.md).

### Phrases

- "You're absolutely right" / "You're right,"
- "Great question!" / "Certainly!" / "Perfect!"
- "Here's the thing nobody tells you"
- "Here's the kicker"
- "belt and suspenders" (also seen as "belt-and-braces")
- "The thing worth flagging"
- "It's worth noting that"
- "Where xyz lives"
- "the smoking gun"
- "the real gate" / "the real question"
- "Let that sink in."
- "I got it"
- "I also could ..."
- "Honestly,"
- "Fair –"
- "Clean –"
- "I hope this email finds you well"
- "Let me know if you'd like..."
- "In conclusion," / "Overall,"
- delve, tapestry, testament, leverage, seamless, robust, pivotal, intricate, game-changer, "evolving landscape", "deep dive"

### Patterns

- "Not `x` but `y`" (ex: "We are not talking about being lazy, we are talking about being motivated")
  - escalated form: "it isn't *just* `x`, it's `y`"
  - and the full run: "it isn't just x. (full stop). it's y. and you know what? that's z."
  - the whole family: "X isn't the problem. Y is." / "Not X. Not Y. Just Z." / "It wasn't X. It wasn't Y. It was Z."
- `<the following will be an assertion>: <assertion>` (seen a lot on Opus-4.8)
- using em dashes `—`
- rule of three everywhere ("fast, reliable, and scalable")
- bold **sprinkled** through prose, emoji headers 🚀, bullets where a paragraph would do
- "serves as" / "stands as" / "boasts" instead of "is" and "has"
- recap paragraphs restating what was just said
- agents narrating themselves: "I'll now...", then "Perfect!", then calling their own code "production-ready"

## Contributing

Heard a new one? PRs welcome. One phrase or pattern per line, with an example if it's subtle.
