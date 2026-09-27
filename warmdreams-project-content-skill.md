---
name: warmdreams-project-content
description: Generate SEO-optimized portfolio project content for WarmDreams Windows & Doors website. Use this skill whenever you need to create project page content (title, meta tags, hero intro, overview, challenge/solution sections) from a brief project summary. The skill generates 2-3 content variations for local SEO, allowing you to pick the best fit for your CMS. Speeds up daily project publishing with consistent, location-optimized copy.
---

# WarmDreams Project Content Generator

Generate complete, SEO-optimized portfolio content for residential windows and doors projects.

## What This Skill Does

Takes a brief project paragraph and generates all the content needed for a WarmDreams project portfolio page:

- **Project Title** — Features the project location with SEO optimization for local search
- **Hero Intro Text** — Compelling one-liner for the hero banner
- **Meta Title** — SEO-optimized page title (includes location)
- **Meta Description** — Compelling summary under 160 characters
- **Project Overview** — 1-2 paragraphs explaining what was completed
- **Challenge Section** — 30-50 words describing client problems/issues (balanced width columns)
- **Solution Section** — 30-50 words detailing how WarmDreams solved it (must closely match challenge section length)

## Input Format

Provide a brief project summary paragraph containing:

- **Project location** (city/neighborhood name)
- **Property type** (e.g., single-family home, townhouse, etc.)
- **Products/services** (doors, windows, specific styles or features installed)
- **Client challenge or problem** (what prompted the project)
- **Outcome or unique aspect** (energy efficiency, aesthetic transformation, etc.)

**Example input:**
> "Recently completed a comprehensive window replacement project at a 1970s ranch home in Arlington Heights. The homeowners struggled with drafty, single-pane windows that drove up heating costs in winter. We installed energy-efficient double-hung vinyl windows throughout the home with a modern satin nickel finish. The transformation was dramatic—the home now stays warmer in winter and cooler in summer, and the homeowners report noticing a real difference in their utility bills."

## Output Format

All content is provided in clean, copy-paste-ready markdown format. You get **2–3 variations** of all content sections, allowing you to choose the version that best fits your brand voice and CMS.

Each variation set includes:
```
## Variation 1

**Project Title:**
[Location-optimized title]

**Hero Intro Text:**
[One-liner for hero banner]

**Meta Title:**
[SEO-optimized page title under 60 chars]

**Meta Description:**
[Compelling summary under 160 chars]

**Project Overview:**
[1-2 paragraphs]

**Challenge Section:**
[30-50 words on client problems]

**Solution Section:**
[30-50 words on how WarmDreams solved it — within 8 words of the Challenge]
```

Then Variation 2, Variation 3, etc.

## SEO Principles Applied

- **Location naturally integrated** into all primary content (title, intro, overview)
- **Local search optimization** — city name featured prominently without awkward keyword stuffing
- **Meta title and description** optimized for click-through from search results
- **Balance in Challenge/Solution** — sections are similar word counts to work well in side-by-side column layouts

## Best Practices for Selection

1. **Project Title** — Should be short enough for large hero font; avoid overly long titles
2. **Hero Intro** — Aim for brevity; evokes the transformation at a glance
3. **Meta Description** — Pick the version that makes you want to click from search results
4. **Challenge & Solution** — Prefer versions where both sections feel balanced in depth and detail

## Instructions for Use

**Step 1:** Prepare your brief project paragraph (or just talk through the project informally)

**Step 2:** Provide it to Claude with this skill active

**Step 3:** Review the 2-3 variations generated

**Step 4:** Pick your preferred version from each section, or ask Claude to blend/refine specific sections

**Step 5:** Copy the markdown into your CMS or content editor

---

## Content Guidelines

### Tone

- Professional yet approachable (for homeowners, not industry jargon-heavy)
- Benefit-focused (emphasize outcomes: comfort, energy savings, aesthetics, durability)
- Solution-oriented (show how WarmDreams solved the problem)

### Word Targets

- **Project Title:** 4–8 words including location
- **Hero Intro:** 10–15 words
- **Overview:** 150–250 words (1–2 paragraphs)
- **Challenge Section:** 30–50 words
- **Solution Section:** 30–50 words (keep within 8 words of the Challenge)

**Column balance rule:** The Challenge and Solution render side by side. After drafting, count both. If they differ by more than ~8 words, tighten the longer one rather than padding the shorter one.

**Writing at this length:** 30–50 words is two to three sentences. There is room for exactly one idea per section, and the two sections must mirror each other — whatever problem the Challenge names, the Solution answers directly. Pick the single most important pain point; do not try to list several. Cut scene-setting, cut transitional phrases, cut the closing summary sentence. Lead with the concrete noun, not a wind-up ("Original single-pane windows leaked heat all winter" — not "The homeowners were facing a common problem in older homes").

**Load-bearing Overview:** Because the Challenge is too short to carry context, the Overview must establish the property, the scope of work, and the outcome. Write the Overview first, then let the Challenge open directly on the problem.

### SEO Keywords to Favor

- Window replacement / Door installation [City Name]
- Energy-efficient windows / Doors
- [Property type] windows [City]
- Custom window installation
- Professional window/door contractor [City]

*Note: Keywords are naturally woven in, not forced.*

---

## How to Trigger This Skill

Use this skill when you:

- Have a completed WarmDreams project and need portfolio content
- Want to batch-generate content for multiple projects
- Need consistent, local-SEO-optimized phrasing across your portfolio
- Are publishing projects daily and need speed + quality

The skill works best with even brief project info — a paragraph or conversation about the work, the client situation, and the outcome.
