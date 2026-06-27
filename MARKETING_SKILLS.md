# Marketing Skills — Installation Reference

> Generated: 2026-06-27

## Location

All skills are installed at:

```
/Users/juan/.claude/skills/
```

Each skill is its own subdirectory containing a `SKILL.md` file (and a `scripts/`
folder where the skill ships Python tooling). Claude Code auto-discovers them on
launch; invoke any with `/<skill-name>`.

```
~/.claude/skills/
├── brand-strategist/
│   ├── SKILL.md
│   └── scripts/
│       ├── brand_architecture_analyzer.py
│       ├── brand_health_dashboard.py
│       └── positioning_map_generator.py
├── brand-guidelines/
│   ├── SKILL.md
│   └── scripts/
│       ├── brand_audit_scorer.py
│       ├── color_accessibility_checker.py
│       └── messaging_consistency_checker.py
└── ... (36 more)
```

## Source

Cloned from `https://github.com/Krypton-Kr36/Claude-Skills-Borghei.git`
(the `marketing/` directory). The cloned repo at `/tmp/borghei` was removed after install.

A separate **brand-building-skills** plugin (28 namespaced skills, e.g.
`brand-building-skills:brand-strategy`) was also installed via `/plugin` and is
distinct from these file-based skills.

## Installed Marketing Skills (38)

| Skill | Purpose |
|-------|---------|
| ab-test-setup | Sample size, experiment design, significance testing |
| ad-creative | Ad copy/creative across Google, Meta, LinkedIn, X, TikTok |
| ai-seo | Generative engine optimization (GEO) for AI search |
| analytics-tracking | GA4, GTM, event taxonomy, conversion tracking |
| app-store-optimization | ASO keyword research & metadata |
| brand-guidelines | Brand identity systems, audits, governance |
| brand-strategist | Positioning, architecture, messaging, brand health |
| campaign-analytics | Multi-touch attribution, funnel, ROI |
| cold-email | B2B cold outreach sequences |
| content-creator | SEO content with brand voice |
| content-humanizer | De-AI-ify robotic content |
| content-production | End-to-end content pipeline |
| content-strategy | Pillars, clusters, audits, editorial planning |
| copy-editing | Seven Sweeps editorial framework |
| copywriting | Persuasive page/landing/CTA copy |
| email-sequence | Lifecycle/drip email automation |
| email-template-builder | React Email / MJML template systems |
| growth-marketer | Experimentation, AARRR funnel, viral loops |
| landing-page-generator | High-converting landing pages |
| launch-strategy | Product/feature launches, Product Hunt |
| marketing-analyst | Attribution, MMM, ROI, reporting |
| marketing-context | Foundational ICP/positioning context doc |
| marketing-demand-acquisition | Multi-channel demand gen |
| marketing-ideas | 139+ proven marketing tactics |
| marketing-ops | MarTech, automation, skill routing |
| marketing-psychology | 70+ behavioral mental models |
| marketing-strategy-pmm | Positioning, GTM, competitive intel |
| paid-ads | PPC across Google, Meta, LinkedIn, X, TikTok |
| programmatic-seo | Template-based page generation at scale |
| schema-markup | JSON-LD structured data |
| seo-audit | 85-point technical SEO audit |
| seo-specialist | Technical SEO, keywords, link building |
| site-architecture | IA, URL hierarchy, internal linking |
| social-content | Platform-specific social posts |
| social-media-analyzer | Engagement rate, ROI, benchmarking |
| social-media-manager | B2B SaaS social strategy |
| video-content-strategist | YouTube strategy, video SEO |
| x-twitter-growth | Twitter/X growth & threads |

## Verification / Test Results

### brand-strategist — PASS
- Skill loads from `~/.claude/skills/brand-strategist`.
- `positioning_map_generator.py --demo` → ASCII map, quadrant analysis, white-space opportunities. (exit 0)
- Ran on real "Lumen" smart-lighting data → correctly identified Lumen as most differentiated. (exit 0)
- Scripts present: `brand_architecture_analyzer.py`, `brand_health_dashboard.py`, `positioning_map_generator.py`.
- Note: SKILL.md references a `references/` folder not shipped upstream — cosmetic gap, core workflow unaffected.

### brand-guidelines — PASS
- Skill loads from `~/.claude/skills/brand-guidelines`.
- `color_accessibility_checker.py` → pass case `#2563EB`/white = 5.17:1 (AA); fail case `#CCCCCC`/white = 1.61:1 flagged + suggested fix `#767676`. (exit 0)
- `messaging_consistency_checker.py` → scored jargon text 80/100, caught leverage/paradigm/disrupt/game-changer. (exit 0)
- `brand_audit_scorer.py` → 3-channel weighted audit, flagged social_media critical (2.9, high-visibility). (exit 0)

## Usage

- Invoke a skill: `/<skill-name>` (e.g. `/copywriting`, `/seo-audit`).
- Run a bundled script directly, e.g.:
  ```bash
  python3 ~/.claude/skills/brand-strategist/scripts/positioning_map_generator.py competitors.json
  python3 ~/.claude/skills/brand-guidelines/scripts/color_accessibility_checker.py --fg "#2563EB" --bg "#FFFFFF"
  ```
- List skills in-session: `/skills`
