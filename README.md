# SaaSoned 🧂

> **SaaS** + sea**soned** — seasoned skills for builders, served with flavor.

A [Claude Code](https://claude.com/claude-code) plugin marketplace. The name is a pun: *seasoned* as in **well-flavored** and *seasoned* as in **experienced** — these are battle-tested skills from real building, not theory.

The first plugin is **`saasoned`**, a growth & go-to-market toolkit.

---

## Install

```bash
# 1. Add the marketplace (once)
/plugin marketplace add williancesar/saasoned

# 2. Install the plugin
/plugin install saasoned@saasoned
```

That's it. Restart isn't needed — the skills become available immediately.

## What you get

A hub-and-spoke set of seven growth skills. Start at the hub — it routes you to the right one:

| Skill | What it owns |
|-------|--------------|
| `saasoned:growth-foundations` | **Hub / router.** Worldview, shared vocabulary, and dispatch to the right skill below. |
| `saasoned:growth-traction-channels` | Pick the ONE distribution channel that moves the needle (Traction's 19 channels + Bullseye). |
| `saasoned:growth-positioning` | What is this, for whom, in what context (Obviously Awesome + Crossing the Chasm). |
| `saasoned:growth-habit-loops` | Retention via habit formation (Hooked's Hook Model + Fogg) with a mandatory ethics gate. |
| `saasoned:growth-customer-discovery` | Learn the truth from customers and build with an audience (The Mom Test + Embedded Entrepreneur). |
| `saasoned:growth-network-effects` | Cold-start and network/marketplace growth (The Cold Start Problem). |
| `saasoned:growth-experiments` | Turn any framework into a cheap, measurable test with a pre-stated kill condition. |

Claude invokes these automatically when relevant. You can also call one explicitly, e.g. *"use saasoned:growth-positioning to sharpen my pitch."*

### Grounded in

Zero to One · Traction · Hooked · The Mom Test · Crossing the Chasm · Obviously Awesome · The Embedded Entrepreneur · The Cold Start Problem.

## How it's structured

This repo is both the **marketplace** (catalog) and the **plugin** (content):

```
saasoned/
├── .claude-plugin/marketplace.json   # the catalog
└── plugins/
    └── saasoned/
        ├── .claude-plugin/plugin.json
        └── skills/                   # the seven skills, each with references/
```

More plugins may be added to this marketplace over time.

## Contributing

Issues and PRs welcome. Each skill lives in `plugins/saasoned/skills/<name>/SKILL.md` with supporting material under `references/`.

## License

MIT © Willian Cesar
