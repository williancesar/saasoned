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

## Example usage

You don't need to memorize skill names. Describe your growth problem in plain language and Claude routes to the right skill (usually starting at the `growth-foundations` hub). Or name a skill explicitly when you know exactly what you want.

**Let Claude route it (recommended):**

```
> I built a SaaS for indie game devs but nobody signs up. Where do I even start?
> My landing page gets traffic but no conversions — is it a positioning problem?
> Users try the app once and never come back. Help me fix retention.
> I have an idea for a marketplace. How do I validate it before building?
> I'm about to spend $2k on ads. Is that the right channel for me?
```

**Call a specific skill when you know what you need:**

```
> Use saasoned:growth-positioning to sharpen the pitch for my dev-tools startup.
> Use saasoned:growth-traction-channels to rank channels for a B2B API product.
> Use saasoned:growth-customer-discovery to critique my user-interview questions.
> Use saasoned:growth-habit-loops to design an ethical engagement loop for a journaling app.
> Use saasoned:growth-network-effects to plan the cold-start for a local-services marketplace.
> Use saasoned:growth-experiments to turn "add referrals" into a cheap test with a kill condition.
```

**What you get back:** not generic advice, but a structured walk-through grounded in the source frameworks — e.g. a Bullseye channel ranking, a positioning statement filled out component by component, a Mom Test question rewrite, or an experiment spec with a pre-stated metric and kill condition. The `growth-habit-loops` skill always runs its output through an ethics gate before recommending anything.

**A typical session flows hub → spoke → experiment:**

```
> How do I grow my note-taking app?               # → growth-foundations diagnoses & routes
> ...positioning first.                            # → growth-positioning sharpens the frame
> Now what's the cheapest way to test this?        # → growth-experiments designs the test
```

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
