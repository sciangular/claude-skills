---
name: warmdreams-project-content
description: Generate structured, SEO-optimized portfolio project content for WarmDreams Windows & Doors from a brief project summary. Use this skill for individual or batch project-page generation, including project title, hero intro, meta title, meta description, overview, challenge, and solution. Generate 3 meaningfully distinct variations, optimize naturally for local search, preserve supplied project facts, avoid unsupported claims, and minimize factual repetition across and within sections.
---

# WarmDreams Project Content Generator

Generate complete, SEO-optimized portfolio content for residential windows and doors installation projects.

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

All content is provided in clean, copy-paste-ready markdown format. You get **3 meaningfully distinct variations** of all content sections, allowing you to choose the version that best fits your brand voice and CMS. Each variation must remain factually consistent with the same project but should differ in framing, emphasis, rhythm, and sentence construction. Do not create variations by merely swapping synonyms or lightly paraphrasing the same copy.

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

- **Location used strategically** — include the city prominently where it benefits local relevance, especially in the Project Title, Meta Title, and Overview. Do not force the city name into every section or repeat it when context is already clear.
- **Local search optimization** — city name and relevant service terms are used naturally without awkward keyword stuffing
- **Meta title and description** optimized for click-through from search results
- **Balance in Challenge/Solution** — sections are similar word counts to work well in side-by-side column layouts

## Best Practices for Selection

1. **Project Title** — Should be short enough for large hero font; avoid overly long titles
2. **Hero Intro** — Aim for brevity; evokes the transformation at a glance
3. **Meta Description** — Pick the version that makes you want to click from search results
4. **Challenge & Solution** — Prefer versions where both sections feel balanced in depth and detail
5. **Avoid factual repetition across sections** — Do not repeat the same project facts, product details, homeowner problems, benefits, or outcomes in the Hero Intro, Overview, Challenge, and Solution unless repetition is necessary for clarity. Treat each section as having a distinct purpose and distribute available facts across them.
6. **Prefer genuinely different variations** — Across Variations 1–3, vary emphasis, structure, and supporting details rather than producing near-duplicate paraphrases.

## Instructions for Use

**Step 1:** Prepare your brief project paragraph (or just talk through the project informally)

**Step 2:** Provide it to Claude with this skill active

**Step 3:** Review the 3 variations generated

**Step 4:** Pick your preferred version from each section, or ask Claude to blend/refine specific sections

**Step 5:** Copy the markdown into your CMS or content editor

---

## Content Guidelines

### Tone

- Professional yet approachable (for homeowners, not industry jargon-heavy)
- Benefit-focused (emphasize outcomes: comfort, energy savings, aesthetics, durability)
- Solution-oriented (show how WarmDreams solved the problem)

### Factual Grounding and Information Distribution

**Factual grounding:** Use only project facts provided in the input or established WarmDreams business information explicitly available to the skill. Do not invent product specifications, quantified savings, homeowner feedback, installation conditions, project duration, warranties, or performance outcomes. Reasonable descriptive wording is allowed, but factual claims must remain supported by the source information.

**Fact distribution rule:** Before drafting, identify the available project facts and assign them to sections. Avoid restating the same fact in several sections using slightly different wording. Each section should contribute new information or serve a distinct communication purpose instead of retelling the entire project in progressively shorter forms.

Use the sections this way:

- **Hero Intro** — Summarize the transformation or core value at a glance; avoid detailed facts that belong in the Overview.
- **Project Overview** — Carry the broad project narrative: property context, scope of work, notable product or design details, and outcome.
- **Challenge** — Isolate the single most important client problem or project constraint.
- **Solution** — Explain the intervention that directly addresses the Challenge; maintain logical correspondence without repeating the Challenge in different words.
- **Meta Title / Description** — Summarize for search intent and click-through; some overlap with page content is acceptable because these are search-result elements, but avoid unnecessary repetition within the visible page copy.

**Variation diversity rule:** Preserve factual accuracy across all 3 variations, but vary what is foregrounded, how the story is structured, and the sentence patterns used. When the input contains enough distinct facts, distribute different supporting details across variations. Do not manufacture new facts merely to make variations different.

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
