# SEO + GEO Skills for Claude Code

> Two skills that fully optimize a page: **rank it** in classic search *and* get it **cited** inside AI answers — ChatGPT, Perplexity, Google AI Overviews, Gemini, Copilot, and Claude. Traditional SEO gets a page ranked. GEO gets a passage *cited*. This does both.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Claude Code Skill](https://img.shields.io/badge/Claude%20Code-Skill-6f42c1.svg)](https://code.claude.com/docs/en/skills)
[![Made by Eduk8agentic](https://img.shields.io/badge/by-Zara%20Hunter%20·%20Eduk8agentic-0a7.svg)](https://www.eduk8agentic.com/)
[![MENA / Arabic ready](https://img.shields.io/badge/MENA%20%2F%20Arabic-ready-success.svg)](#-mena--arabic-playbook)

Two production-grade [Claude Code](https://code.claude.com) skills that work together to fully optimize a page: **`on-page-seo`** makes it *rank* in classic Google / Bing search, and **`ai-seo` (GEO)** makes it *retrieved and cited* by AI answer engines — with a dedicated **MENA / Arabic** playbook most GEO guidance ignores.

Built and maintained by **[Zara Hunter](https://github.com/zarahunter) — [Eduk8agentic](https://www.eduk8agentic.com/)**, teaching agentic AI and Arabic AI agents.

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
/plugin install seo-geo@eduk8agentic
```

Then just ask naturally — the right skill auto-activates on SEO or GEO tasks. You can also invoke them explicitly with `/seo-geo:on-page-seo` or `/seo-geo:ai-seo`.

### Option B — Manual install

```bash
git clone https://github.com/zarahunter/seo-geo-skills.git
cp -R seo-geo-skills/plugins/seo-geo/skills/* ~/.claude/skills/
```

Restart Claude Code (or run `/reload-plugins`). Both skills now live under `~/.claude/skills/`.

### Try it

```
"Audit why ChatGPT cites my competitor for 'best CRM for agencies' but never us."
"Rewrite this page so Perplexity will quote it."
"Why doesn't AI mention my Arabic content, and how do I fix it?"
```

---

## What's inside

Two skills, designed to run as one optimization pass.

### `on-page-seo` — rank in classic search

Search-intent matching, primary/supporting keyword selection and placement, title tags, meta descriptions, URL slugs, heading hierarchy, internal linking, and alt text — plus an on-page checklist and copy-paste templates. Names the hand-offs for technical SEO, schema, and backlinks.

### `ai-seo` (GEO) — get cited by AI answers

Six tasks and a full reference library:

| Task | What Claude does |
| --- | --- |
| **Audit** | Find where competitors are cited and you are not — and *exactly why*, via a passage-diff method |
| **Optimize a page** | Front-load the answer, convert prose to extractable blocks, raise citability, strip own-goals |
| **Create AI-first content** | Comparison, roundup, guide, product, and how-to formats built to be quoted |
| **Monitor** | Non-deterministic testing, citation velocity, a no-tool DIY protocol |
| **Entity presence** | Consistent-facts baseline, Wikidata/Wikipedia, third-party source map (parametric memory) |
| **MENA / Arabic** | Dialect testing, multilingual entity work, Arabic citation density, regional source priority |

Reference library: `content-patterns` · `platform-factors` · `measurement` · `entity-presence` · `hard-cases` · `mena-arabic` · `research-stats` · plus a full **worked example** (audit → before/after rewrite).

### The two-pass method

Ask for full optimization and Claude runs the **SEO pass** (intent, keywords, title/meta, headings, links) → then the **GEO pass** (extractable, citable, promo-tone stripped). Where they conflict, the GEO "write naturally" rule wins on the body copy.

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
│   └── seo-geo/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           ├── on-page-seo/       # rank in classic search
│           │   ├── SKILL.md
│           │   └── references/
│           └── ai-seo/            # get cited by AI answers
│               ├── SKILL.md
│               └── references/
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

- Website: [eduk8agentic.com](https://www.eduk8agentic.com/)
- GitHub: [@zarahunter](https://github.com/zarahunter)
- LinkedIn: [Zara Hunter](https://www.linkedin.com/in/zarahunter/)
- Community: [Arabic AI Agents Academy](https://www.skool.com/arabic-ai-agents-academy) (Skool)
- Arabic AI Agents on GitHub: [@arabicaiagents](https://github.com/arabicaiagents)

<sub>Educational resource. AI citation behavior changes fast; figures in the references are dated and marked perishable — verify before relying on them.</sub>
