# AI SEO / GEO Skill for Claude Code

> Get your content **retrieved and cited as a source inside AI answers** — ChatGPT, Perplexity, Google AI Overviews, Gemini, Copilot, and Claude. Traditional SEO gets a page ranked. GEO gets a passage *cited*.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-6f42c1.svg)](https://code.claude.com/docs/en/skills)
[![Made by Eduk8agentic](https://img.shields.io/badge/by-Zara%20Hunter%20·%20Eduk8agentic-0a7.svg)](https://github.com/zarahunter)
[![MENA / Arabic ready](https://img.shields.io/badge/MENA%20%2F%20Arabic-ready-success.svg)](#-mena--arabic-playbook)

A production-grade [Claude Code](https://code.claude.com) skill that teaches Claude how to make any page **discoverable, extractable, and citable** by AI answer engines — with a dedicated **MENA / Arabic** playbook most GEO guidance ignores.

Built and maintained by **[Zara Hunter](https://github.com/zarahunter) — [Eduk8agentic](https://github.com/arabicaiagents)**, teaching agentic AI and Arabic AI agents.

---

## Why this exists

AI assistants increasingly answer questions *without* sending a click to your site. Ranking #1 on Google no longer guarantees you are mentioned when someone asks ChatGPT or Perplexity. This skill optimizes for the new unit of visibility: **the cited passage**.

It is opinionated and honest:

- It leads with what **suppresses** citation (promotional tone, keyword stuffing) — often higher leverage than any tactic you can add.
- It treats every citation statistic as **perishable** and tells Claude to verify before quoting.
- It never lets Claude **fabricate** an AI answer it could not observe.
- It distinguishes **fast** wins (retrieval) from **slow** wins (the model's parametric memory of your brand).

---

## Quick start

### Option A — Install as a plugin (recommended)

In Claude Code:

```
/plugin marketplace add zarahunter/seo-geo-skills
/plugin install ai-seo@eduk8agentic
```

Then just ask naturally — the skill auto-activates on AI-SEO / GEO tasks. Or invoke it explicitly with `/ai-seo`.

### Option B — Manual install

```bash
git clone https://github.com/zarahunter/seo-geo-skills.git
cp -R seo-geo-skills/plugins/ai-seo/skills/ai-seo ~/.claude/skills/ai-seo
```

Restart Claude Code (or run `/reload-plugins`). The skill now lives at `~/.claude/skills/ai-seo/`.

### Try it

```
"Audit why ChatGPT cites my competitor for 'best CRM for agencies' but never us."
"Rewrite this page so Perplexity will quote it."
"Why doesn't AI mention my Arabic content, and how do I fix it?"
```

---

## What's inside

The skill routes Claude through six tasks and seven reference files.

| Task | What Claude does |
| --- | --- |
| **Audit** | Find where competitors are cited and you are not — and *exactly why*, via a passage-diff method |
| **Optimize a page** | Front-load the answer, convert prose to extractable blocks, raise citability, strip own-goals |
| **Create AI-first content** | Comparison, roundup, guide, product, and how-to formats built to be quoted |
| **Monitor** | Non-deterministic testing, citation velocity, a no-tool DIY protocol |
| **Entity presence** | Consistent-facts baseline, Wikidata/Wikipedia, third-party source map (parametric memory) |
| **MENA / Arabic** | Dialect testing, multilingual entity work, Arabic citation density, regional source priority |

Reference library: `content-patterns` · `platform-factors` · `measurement` · `entity-presence` · `hard-cases` · `mena-arabic` · `research-stats` · plus a full **worked example** (audit → before/after rewrite) for calibration.

---

## 🌍 MENA / Arabic playbook

Most GEO advice is English-only. This skill ships a dedicated Arabic / MENA reference because **LLMs handle Arabic less comprehensively than English — which means less competition for Arabic AI citations.** That gap is an opening. It covers Modern Standard Arabic and dialect query testing (Gulf, Egyptian), transliterated and mixed-language prompts, multilingual entity consistency (Arabic Wikipedia/Wikidata), Arabic citation density, and a MENA source-priority table.

---

## Repository layout

```
seo-geo-skills/
├── .claude-plugin/
│   └── marketplace.json          # makes this repo a Claude Code marketplace
├── plugins/
│   └── ai-seo/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           └── ai-seo/
│               ├── SKILL.md       # the skill entry point
│               └── references/    # the reference library
├── README.md
├── LICENSE                        # MIT
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
└── CHANGELOG.md
```

---

## Contributing

Issues and pull requests are welcome — corrections, new verticals, fresh citation research (dated, please), and additional language playbooks especially. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Released under the **[MIT License](LICENSE)** — use, adapt, and build on it freely, including commercially. Copyright stays with Zara Hunter (Eduk8agentic).

Credit isn't required under MIT, but it's appreciated and helps others find the original: a mention of **Zara Hunter (Eduk8agentic)** and a link back to this repo.

## About the author

**Zara Hunter** builds and teaches **agentic AI and Arabic AI agents** under **Eduk8agentic**. If this skill helps you, a ⭐ on the repo and a share with your network is the best support — and the most honest way to help others discover it.

- GitHub: [@zarahunter](https://github.com/zarahunter)
- Eduk8agentic / Arabic AI Agents: [@arabicaiagents](https://github.com/arabicaiagents)

<sub>Educational resource. AI citation behavior changes fast; figures in the references are dated and marked perishable — verify before relying on them.</sub>
