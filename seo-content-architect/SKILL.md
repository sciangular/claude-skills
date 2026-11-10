---
name: seo-content-architect
description: Site-aware website content architecture with two modes (1) to bootstrap a website knowledge base from legacy/live and local rebuild sources, or (2) to audit SEO prose and create approved Scan/Explore/Deep dive page plans for any page type.
---

# SEO Content Architect

Use two explicit modes: **Site Bootstrap** initializes or refreshes a project-specific, evidence-traceable website knowledge base; **Page Architecture** converts prose-first SEO copy for service, product, solution, industry, about, and other corporate website pages into a scannable, evidence-grounded content specification. Apply the **mandatory four-gate audit** to Page Architecture, not to Site Bootstrap.

## Operating rules

1. **Validate before transforming.** Run the full intake audit even when the prose seems polished.
2. **Do not silently fill gaps.** Propose alternatives for missing information, clearly mark them `PROPOSED — NOT APPROVED`, and route them to an accountable person/team.
3. **Never invent evidence.** Do not fabricate customer outcomes, ROI figures, testimonials, credentials, integrations, product support, timelines, pricing, or case studies.
4. **Preserve meaning, improve presentation.** Rewrite for comprehension and scanning without changing the substance of verified claims. Quote source excerpts when explaining a finding; otherwise paraphrase.
5. **Optimize for the visitor first.** Do not append filler paragraphs, stuff keywords, manufacture FAQ sections, or promise rankings. SEO is a constraint on information architecture, not an excuse for duplication.
6. **Separate approval from verification.** A team can approve proposed wording, but objective technical claims still need a credible source or documented subject-matter verification.
7. **Keep final output implementation-agnostic.** Produce content structure and component recommendations, not code, unless explicitly asked. Do not modify project files or published pages without authorization.
8. **Site context is mandatory before gap assessment.** Read the site-specific context index, approved business facts, and relevant existing pages where accessible. Do not mark something missing solely because it is absent from the target prose. Distinguish verified site-wide context from page-specific essential content. If site access is unavailable, mark the context check `NOT ASSESSED` and request access or a snapshot; do not claim site-wide absence.
9. **Do not infer search metrics.** Search volume, difficulty, ranking, intent inferred from SERPs, or competitor gaps must be labeled `NOT VERIFIED` unless supported by current research/data. If browsing/tools are available and authorized, use them selectively and cite sources; do not claim independent validation without it.
10. **If requirements conflict, surface the conflict** with a concrete decision request. Do not resolve business or factual conflicts by guessing.
11. **Preserve the source language throughout deliverables.** Detect the primary language of the user-supplied SEO prose and use that language for **all user-facing outputs**: audit findings, status explanations, option recommendations, stakeholder-forwardable requests (including subjects and reply templates), proposed page headings/copy, layer descriptions, supporting-page titles, meta copy, and QA/handoff notes. Do not default to English merely because this skill is written in English. Keep proper nouns, brand names, documented product/technical terms, URLs, and verbatim search queries in their original forms when appropriate; never translate target keywords silently. Only produce translated or bilingual deliverables when explicitly requested or approved. Internal structural identifiers such as `D-01`, `S-01`, `claim_id`, enum values, and code keys may remain in English for machine readability.
12. **Resolve mixed-language inputs conservatively.** When the SEO prose is predominantly one language, use it as the deliverable language even if the brief or stakeholder notes are in another. If there are multiple substantial language versions or the source language is ambiguous, register a language-selection decision for the responsible content/SEO owner and block publication-ready transformation until resolved. If the user explicitly specifies a deliverable language, follow that instruction while labeling translation/localization requirements and requiring approval of adapted keyword targets and market-specific claims.

## Operating mode selection (required)

Identify the requested mode **before running any content gates or generating page copy**:

| Mode | Trigger | Main deliverable | Approval boundary |
| --- | --- | --- | --- |
| `SITE_BOOTSTRAP` | New/rebuild project, initial site inventory, context initialization, refresh or reconcile live vs local site | Proposed/updated context registry, source inventory, discrepancy and decision report | Do not silently approve legacy claims or overwrite accepted context; do not edit website pages |
| `PAGE_ARCHITECTURE` | Draft, SEO prose, proposed new URL, revision or redesign of an individual page | Four-gate audit, stakeholder requests if blocked, or layered page specification if ready | No publish-ready transformation until all applicable content gates pass |

If a request explicitly asks for both, **run Site Bootstrap first**, present unresolved source-of-truth decisions for review, then run Page Architecture only when relevant facts and decisions are sufficient. If the user only supplies prose and no project context, use Page Architecture and report context limitations. Do not run bootstrap automatically as an expensive full-site crawl for every page.

### Mode A — Site Bootstrap (new projects and rebuilds)

**Goal:** Reconstruct what the website currently says, what the rebuild currently implements, and which information is sufficiently supported for reuse. This mode does **not** require page-specific SEO prose, an approved keyword brief, or all four Page Architecture gates.

1. **Discover environments and access.** Read project `CLAUDE.md`, inspect any existing context files, and identify the legacy production domain, local development URL, local repository/CMS export, and known content owners. Confirm which sources are actually accessible. Never imply that `localhost` renders without a running server or that a repository necessarily contains database-stored CMS resources. If access is incomplete, record the limitation and provide an export/access checklist. Do not request credentials in content deliverables.
2. **Inventory existing pages.** Prefer sitemap/CMS resource exports plus relevant live pages; gather canonical URL, local path/resource ID if available, page type, title/H1, primary topic/intent, language, content status, and source retrieval/review date. Separate the **legacy live site** from **local rebuild** and from planned/unpublished content. Use batches for large sites and state coverage, exclusions, and inaccessible URLs. Never equate 'not found in examined pages' with 'does not exist'.
3. **Extract and trace context.** Gather identity, audiences, markets, offerings, positioning, differentiators, processes, credentials, product specifications, proof, and constraints. Record each material fact or claim with source URL/path, source type, dates if available, scope, and whether it was merely observed, technically verified, or explicitly approved. Do not invent evidence or treat marketing text as proof of independent accuracy.
4. **Reconcile versions.** Compare relevant live and local pages: `legacy_only`, `rebuilt_draft`, `rebuilt_approved`, `published_current`, `planned`, or `unknown`. Identify contradictory or stale claims, redirects/URL moves, duplicated intent, missing migrated content, and risks of pointing internal links to unpublished pages. A local draft is not automatically approved or canonical.
5. **Apply source precedence (below).** For every conflict, note the competing sources and request the appropriate business/content/technical owner decision. Do not assume newer date alone means higher authority; distinguish asserted claims from verified facts. Record explicit precedence decisions in `SITE_CONTEXT.md` or the claims registry.
6. **Populate context files** (or reconcile equivalent established records): `SITE_CONTEXT.md`, `PAGE_INDEX.md`, `CLAIMS.md`, `PAGE_RELATIONSHIPS.md`. Propose targeted edits/diffs if approved records already exist; preserve their IDs, provenance, and decisions. If editing files has not been authorized, provide preview content and proposed patches rather than writing them.
7. **Deliver a bootstrap review packet:** source and inventory coverage; pages and page migration statuses; usable approved facts; observed-only claims; contradictions/freshness concerns; missing-access limitations; topic owners; numbered, copy-ready requests for unresolved decisions with an accountable team and 2–3 alternatives where meaningful. The **context status** is `PROVISIONAL`, `READY FOR REVIEW`, or `APPROVED FOR REUSE` only when approvals exist. Bootstrapping itself never confers approval.
8. **Handoff:** tell the user precisely which sources to review and what decisions must be made before the next Page Architecture run. The next run reads approved records and searches relevant primary sources; it should not repeat a full-site audit.

**Source-precedence policy (apply in both modes):**

1. **Current, approved project facts and page-specific briefs**, including signed-off business policies and verified evidence. For objective product/technical claims, the current authoritative specification or named SME verification outranks generic marketing language.
2. **Current local rebuild content only when explicitly approved** and applicable to the target version; a draft, local file or locally rendered page by itself is not an approved source of truth.
3. **Verified, current claims from the legacy live website**, with provenance and scope; published copy without independent support remains `OBSERVED`, not `VERIFIED`.
4. **Other legacy published content**, useful for discovering offerings, terms, and relationships, but as reference material only until validated.
5. **Claude research, inference, and suggestions** as `PROPOSED — NOT APPROVED`, never replacements for business authorization or factual evidence.

The ranking is a default, not permission to disregard scope: an approved product spec takes precedence for product compatibility even if a newer general About page says otherwise. When approved sources disagree or applicability is unclear, **escalate** rather than silently choose. Capture source/approval dates and flag potentially stale facts.

**Bootstrap output contract** (localize reader-facing content to the predominant source/site language unless the user directs otherwise; for multilingual sites identify locale-specific coverage and request a language decision when needed):

```markdown
# Website Context Bootstrap — [domain]
Mode: SITE_BOOTSTRAP
Context status: PROVISIONAL | READY FOR REVIEW | APPROVED FOR REUSE
## Environment and access map
[Legacy website, local rebuild, CMS/export, permissions, inaccessible sources]
## Inventory coverage and migration states
[Page counts only when actually established; URLs/paths; coverage gaps]
## Extracted context and provenance
[Approved vs observed vs contested facts; source references]
## Reconciliation and source-of-truth conflicts
[Legacy/local differences and applicable precedence]
## Proposed context-file changes
[Created/updated paths or preview diffs; no silent overwrites]
## Approval-ready decision requests
[IDs, responsible teams, 2–3 proposed choices where feasible, supporting evidence needed]
## Readiness and next action
[What can be reused now vs what remains unresolved]
```

### Mode B — Page Architecture (per-page production)

This is the **existing Phases 0–6** below. Start by loading the approved/verified site registry and the specific source prose/brief; inspect only relevant existing URLs, CMS records, and local rebuild pages. Identify whether an existing page already owns the search intent; distinguish approved context from observed facts and ensure internal links resolve to actually published destinations (or explicitly mark them planned). Apply four gates, stop for stakeholder decisions when blocked, then produce Scan / Explore / Deep dive plus supporting-page assessment. The Page Architecture output must include provenance, source language, and any project-context discrepancies.

**After a page is approved or published:** propose a **context synchronization patch** for `PAGE_INDEX.md`, `CLAIMS.md`, and `PAGE_RELATIONSHIPS.md`, plus `SITE_CONTEXT.md` if site-wide facts changed. Register the target URL, status, intent ownership, verified new claims, evidence, and relevant links. Do not silently promote draft claims to approved, mark a page published without confirmation, or overwrite accepted facts. Apply updates only with user authorization; otherwise supply the exact suggested edits for review.

## Configuration and source architecture

Keep this **reusable skill** free of company-specific facts. Put website-specific reference material in the individual project's `site-context/` directory and point to it from that project's `CLAUDE.md`.

Suggested project files:

```text
website-project/
├── CLAUDE.md                  # Short instructions + paths to relevant website knowledge
├── site-context/
│   ├── SITE_CONTEXT.md        # Identity, audience, positioning, primary CTA, source precedence
│   ├── PAGE_INDEX.md          # URL/path, type, topics, authoritative claims, last reviewed
│   ├── CLAIMS.md              # Claim IDs, source URLs, evidence, owner, approval, freshness
│   └── PAGE_RELATIONSHIPS.md  # Existing related pages, topic ownership, links, exclusions
└── content/
    └── briefs/                 # Incoming page-specific SEO prose and briefs
```

These are suggested files, not hard prerequisites. Existing CMS exports, rendered HTML, repository templates/content, approved product specs, API docs, and public website pages can substitute when accessible. If the project already has a reliable knowledge base, use it instead of duplicating files. Do not fetch entire sites unnecessarily; retrieve relevant pages based on target topic, entities, and internal links.

`CLAUDE.md` should point to the source of truth, not paste thousands of words of site text. Never assume Claude Code can access a live site without its network/tool permissions. Prefer local approved exports; inspect live pages only when tools and access permit. Existing live content is *evidence that the site says something*, not proof of objective truth. Respect draft/published status and verification dates.

### Site-context precedence and freshness

Use the **Source-precedence policy** in the Operating mode section for both modes. In Page Architecture, prioritize the applicable approved project brief and verified technical/product documents, distinguish the local rebuild's draft versus approved state, and treat legacy marketing statements as observed until verified. For conflicts, note both sources and escalate if precedence or scope is unresolved. Record provenance for reused claims (`source`, `URL/path`, `date if known`, `approval`, `status`). Do not claim a document is reviewed merely because it exists.

## Inputs

Accept any combination of:
- Original SEO prose, page draft, or source file.
- Service/product, company, audience/industry, geography, website, page purpose, and desired CTA.
- SEO brief: primary query, secondary queries, target intent, topical requirements, existing URLs, and search research.
- Business brief: problems, benefits, value proposition, differentiators, offer scope, and conversion goals.
- Technical brief: confirmed capabilities, constraints, delivery process, security assertions, integrations, and SME review.
- Proof: case studies, customer references with permission, quantitative outcomes, certifications, screenshots, documentation, and source URLs.
- Stakeholder approvals and existing site content/links.

Missing context is not permission to assume. Ask for missing inputs via the approval-request workflow below rather than composing a final page.

## Page Architecture workflow (Mode B only)

Do not run the phases below as mandatory intake gates during `SITE_BOOTSTRAP`.

### Phase 0 — Determine page type and discover existing website context (required)

1. Identify `page_type` from the source and brief: service, product, product category, solution, industry, comparison, about/company, informational, campaign, or other. If ambiguous, infer a provisional type from target intent, then flag only material unresolved ambiguity.
2. Read project `CLAUDE.md` and any linked site-context index. If accessible, search local CMS content, page files, product records, and approved briefs for company identity, audience, differentiators, trust/evidence, exact offerings, topic coverage, and URLs. For existing or partially developed sites, inspect relevant canonical homepage, about, category, service/product, case study, and related pages. Follow only relevant links rather than crawling everything.
3. Compile a **site context ledger**: `fact_id`, `fact`, `scope` (site-wide/page-specific), `source_path_or_url`, `source_type`, `status` (verified/approved/observed/stale/conflicting), `last_reviewed_if_known`, `reuse_rule` (repeat briefly/link/avoid repeating/needs page-specific details), `related_pages`.
4. Build a **topic ownership map**: which existing URL already satisfies a visitor intent, which page owns commercial and informational queries, where useful internal links should go, and which proposed supporting pages would be duplicative.
5. For each required input, report `PRESENT IN PROSE`, `FOUND IN SITE CONTEXT`, `NEEDS TARGET-PAGE COVERAGE`, `STALE/CONFLICTING`, `NOT APPLICABLE`, or `NOT FOUND AFTER CHECK`. Record `CONTEXT NOT ACCESSIBLE` separately if tools or site material are unavailable.
6. Reuse verified site-wide facts to meet validation; do not require repetition or renewed approval unless the new use materially changes the meaning, audience, claim, permission, or product scope. Nevertheless draft essential page-specific context so a visitor can understand the offer without visiting the About page.
7. Never treat absent information as "not present anywhere on website" without looking at the relevant pages or explicitly labeling discovery incomplete. If discovery is incomplete, seek a site index/export/access or limit conclusions to examined sources.

### Phase 1 — Inventory and classify evidence

**Language preflight (required for Page Architecture):** Record `source_prose_language`, `deliverable_language`, `language_basis` (dominant prose language or explicit user instruction), and any `localization_or_keyword_review_needed`. Apply the same language to the blocked and ready output contracts; do not send English stakeholder requests for non-English prose. Preserve the exact wording of verified search queries and source citations. A mismatch between the prose language and the targeted search market or query language is a content/SEO decision, not permission to silently translate keywords.

Extract discrete claims and content units from the supplied prose. For each material claim, track:

- `claim_id`
- `claim_or_topic`
- `source_excerpt_or_reference`
- `kind`: factual / offer / benefit / opinion / keyword / proof / proposed
- `verification`: verified / unverified / contradicted / not applicable
- `approval`: approved / pending / rejected
- `owner`: SEO / Marketing / Business owner / Technical SME / Legal-compliance / Client
- `destination_candidate`: Scan / Explore / Deep dive / Supporting page / Exclude

Extract supporting evidence verbatim only when required for traceability. Identify exaggerated or absolute language such as "guaranteed," "seamless," "best," "fully secure," and "zero downtime" for verification or rewriting.

### Phase 2 — Mandatory four-part audit

For **each** of the following gates assign `PASS`, `PARTIAL`, `MISSING`, or `CONFLICT` and record its evidence. `PASS` requires the minimum conditions shown; presence of a phrase alone is insufficient.

| Gate | Minimum pass condition | Default decision owner |
| --- | --- | --- |
| A. Primary search intent and target queries | One explicit primary query/topic, defined intent and audience, a coherent set of supporting queries or an explicit determination that none are necessary, and no unresolved conflict between query intent and page purpose. Query research source must be identified; unresearched targets are proposals. | SEO |
| B. Content outline and required topics | An explicit approved outline or requirement list that covers the page-specific entity/offer or informational subject, scope, applicability, key visitor questions, important limitations, and conversion-relevant topics where appropriate; deliberate omissions are documented. | SEO + Marketing + Technical SME |
| C. Value proposition, customer problems, and differentiators | Audience, relevance, genuine needs/problems, value or usefulness, and supported distinctions where relevant. Approved site-wide company positioning may satisfy provider-level context. Do not require an artificial unique selling claim for informational pages or standard products. | Marketing + Business owner |
| D. Technical accuracy and supporting evidence | Material factual and technical claims are mapped to credible evidence or named SME verification; material proof claims have sources and permission where applicable; unresolved contradictions, unverifiable numerical claims, and essential capability gaps are absent. An explicit `no published customer proof available` decision is acceptable only if all remaining claims are supportable. | Technical SME + Business owner; Legal for regulated claims |

**Page-type adaptation (mandatory):**
- **Service/solution:** scope, buyer pain, outcomes, deliverables, approach, constraints, proof and CTA.
- **Product/product category:** product definition, features/specs, intended use, compatibility, options, limitations, availability/pricing only if verified, supporting evidence and purchase/inquiry CTA.
- **Industry/use case:** target segment, workflows/problems, use cases, relevant proof and boundaries.
- **Company/about:** positioning, verifiable credentials, team/company information, trust, relevant contact route.
- **Informational/guide:** accurate question resolution, practical detail, references, limitations, and relevant next step if any; commercial differentiation is not mandatory.
- **Other:** document the intent-based minimum fields before applying the four gates.

A `NOT APPLICABLE` field does not fail its gate if the omission is explicitly justified by page purpose. A verified site-wide fact may satisfy a gate without verbatim repetition. However, all visitor-critical page-level details must appear on the target page in a useful form.

Audit details:

**A — Search intent:** Classify informational, commercial investigation, transactional, navigational, or mixed intent. State the desired visitor outcome and whether the proposed page type matches it. Distinguish stakeholder-supplied queries from independently researched targets; do not treat guessed queries as verified.

**B — Topical completeness:** Cross-check source prose, brief, buyer journey, and any verified search insights. Distinguish `must cover on this page`, `optional here`, and `better on a dedicated page`. Consider exclusions, onboarding, process, security/privacy, compatibility, delivery constraints, pricing approach, evidence, and FAQs when relevant—not as compulsory boilerplate.

**C — Commercial clarity:** Identify who buys, why now, triggering pains, what changes, what is included, what's different, and the next action. Distinguish features from customer benefits and benefits from independently proven outcomes.

**D — Accuracy/evidence:** Check capability details, integrations, standards, constraints, quantitative claims, case studies, client names, pricing/timelines, and legal/compliance claims. Record sources and dates when available. General descriptions can pass without a dedicated citation if clearly supported by approved service scope and technical review. Do not demand case studies that do not exist; instead recommend honest alternative proof (e.g., process, deliverables, demo, public documentation).

#### Gate decision

Before a gate is called `PARTIAL` or `MISSING`, cite which existing site sources were checked, which relevant ones were inaccessible, and why the missing input is needed *on this target page* rather than linkable from elsewhere. Missing website access is a context discovery limitation, not evidence a business fact is absent. Request context/access rather than new company information where appropriate. Reusable approved facts may pass without new sign-off; new consequential claims still require verification.

- `READY`: **all four gates PASS**, with any approvals and objective validations needed for final copy recorded. Proceed to Phase 4.
- `BLOCKED`: **any gate PARTIAL, MISSING, or CONFLICT**. Complete Phase 3 and **stop before final page transformation**. You may show a small illustrative outline clearly labeled `CONCEPT ONLY — NOT APPROVED`; do not represent it as a ready-to-publish draft.
- `READY WITH NONBLOCKING NOTES`: all four PASS but there are optional improvements not essential to factual or strategic adequacy. Proceed while listing those improvements.

A suggestion does not change a gate to `PASS`; explicit stakeholder approval or reliable evidence must close the gap. When the user provides decisions in a later turn, re-audit affected gates and preserve the status of unchanged gates.

### Phase 3 — Approval-ready decision requests (when blocked)

Produce the following in order:

1. **Audit summary table:** gate, status, what is present, what is missing/contradictory, accountable owner. Write the table labels and explanations in the deliverable language.
2. **Numbered decision register:** `D-01`, `D-02`, etc. State exact missing/contested item, business/SEO impact, responsible team, and what evidence or approval would resolve it.
3. **Copy-ready messages** addressed to each responsible person/team **in the deliverable language**. Group related decisions to reduce back-and-forth. Each message must be self-contained and suitable for forwarding by email or chat without rewriting.
4. For every unresolved decision, provide **2–3 concrete, context-relevant options when feasible**. Include "provide a corrected alternative" when none fit; avoid proposing fake facts. Include a **recommended option** with rationale, clearly marked as a recommendation rather than approval.
5. **Response format:** provide an easy way to reply, such as `D-01: option B, approved`, `D-02: revised scope attached`, `D-03: claim rejected`. Where facts require evidence, request exact documentation, URL, SME sign-off, or authorized citation.
6. **Stop and wait for decisions**; do not produce the final transformed page until the gate is clear. Do not assume silence means approval.

Use this forwarding template, **translating all prose labels and sample wording into the deliverable language**, adapted for each team:

```text
Subject: Decision needed — [page] — [topic]
To: [responsible team/role]

Context: We are converting [source] into a [page type] page aimed at [audience / intent], considering existing pages [sources].
Decision ID: [D-XX]
Issue: [what is missing, unverified, or contradictory]
Why it matters: [specific risk to accuracy, positioning, usefulness, or search intent]

Options (proposals, not approved):
A. [specific option + implications]
B. [specific option + implications]
C. [optional alternative]

Recommendation: [option and reason; do not present as fact]
Please confirm: [exact decision, source/evidence, claim limitations, and approval authority]
Reply: D-XX: [chosen option / correction / rejected], [evidence], [approver]
```

Do not use generic requests such as "please send more details" when a precise question can be formulated. If SEO research is absent, propose candidate query *themes* and ask SEO to validate actual search demand/intent; do not represent proposed themes as researched keywords. If differentiators are absent, propose positioning directions, not assertions of superiority. If proof is absent, request actual evidence or recommend removal/qualification of the claim.

### Phase 4 — Transform approved content into three engagement layers

Produce a **page content specification** organized by visitor questions, not by the original paragraph order. Select modules based on actual content and intent; do not force every example module into every page.

#### Layer 1: Scan — understand within seconds

Purpose: Immediately answer "Am I in the right place, what is offered or explained, why does it matter, and what can I do next?"

Possible modules: precise H1/hero, value proposition, short supporting copy, primary CTA, audience-fit statement, 3–5 concise problem/outcome statements, credible proof cue (only if substantiated).

Writing: use the source prose language, front-load meaning, use unambiguous service terminology, favor outcomes over slogans, preserve primary search topic naturally. Avoid vague superlatives and unsupported numbers.

#### Layer 2: Explore — evaluate the service

Purpose: Answer "Does this offer/topic fit my needs, how does it work, what are its constraints, and what supports its claims?"

Possible modules: problem-to-solution mapping, capabilities grid, scenarios/use cases, expected deliverables, step-by-step process, integrations, industries/applicability, constraints, proof/case study summaries, security considerations, engagement model, relevant FAQs, repeated contextual CTA.

For every module include a buyer question it answers, concise proposed heading and copy, evidence, best presentation pattern, and action/link if appropriate. Favor semantic headings and short prose over card proliferation.

#### Layer 3: Deep dive — investigate complexity

Purpose: Answer detailed objections or learning needs without making the primary page cumbersome.

Possible modules: substantive on-page technical explanations; methods, workflows, architecture diagrams, governance/security explanation, assumptions/limitations, implementation considerations, detailed FAQs, and contextual links to supporting resources.

Do not automatically hide critical content in accordions. Reserve accordions for supplementary answers; keep important value, scope, limitations, and proof visible and accessible. Content meant for indexing must be meaningfully present in the delivered page and accessible through standard markup/navigation.

#### Mandatory per-section specification

For each proposed page section, supply:

```yaml
section_id: S-01
layer: Scan | Explore | Deep dive
visitor_question: "..."
heading_level: H1 | H2 | H3
heading: "..."
key_message: "..."
body_copy: "Ready-to-review copy or concise structured items"
presentation: "hero | editorial prose | bullets | cards | diagram | process | comparison | case study | FAQ | CTA | other"
content_source: ["claim IDs / approved brief references"]
proof_or_qualification: "source, verified proof, explicit caveat, or not needed"
primary_query_alignment: "natural topic relationship"
cta_or_internal_link: "target/action or none"
editorial_notes: "visual/accessibility/technical instructions"
```

The specification may be written as a readable Markdown outline/table instead of YAML if that improves team usability. All natural-language values must be in the deliverable language; structural YAML keys and stable enum identifiers may remain in English. Include **actual drafted copy**, not just labels such as "add benefits here." Preserve approved terminology and claim scope. Mark any optional design mock content as placeholders, never approved claims.

### Phase 5 — Decide what belongs on a dedicated page

**Mandatory check against existing site pages first.** For each proposed dedicated page, check `PAGE_INDEX.md`, available sitemap/CMS routes, and relevant published pages. Recommend `link to existing`, `expand existing`, `consolidate`, or `create new` based on actual content ownership; never suggest a new page just because the supplied prose contains a long subtopic. Note what source was checked and when, and propose a URL only as a draft.

Evaluate each substantial subtopic independently. Do **not** split just because a section is long. Recommend a separate page when at least one strong reason exists:

- Distinct search intent or clearly different audience/buyer stage.
- A self-contained, substantial question with enough unique information to satisfy visitors.
- Complexity (methodology, architecture, security, comparison, cost, tutorial) would interrupt evaluation flow on the service page.
- A case study has meaningful context, approach, and verified results worth expanding.
- An existing relevant URL should be strengthened rather than duplicated.

Keep material on the service page when it is essential to choosing the service, articulating scope or limitations, substantiating a claim, or answering a common buying objection. Summarize and link when both audiences need the topic at different depths.

For each candidate, provide:

| Field | Required decision |
| --- | --- |
| Subtopic | Specific topic and visitor question |
| Recommendation | Keep on page / summarize + link / create dedicated page / consolidate with existing page |
| Reason | Search intent, depth, buyer relevance, or duplication risk |
| Suggested title and URL slug | Clearly indicative; check existing site URLs first |
| Target intent/query theme | Verified query or `PROPOSED — requires SEO validation` |
| Minimum unique scope | What the dedicated page adds beyond the summary |
| Internal-link plan | Source section, descriptive anchor, target, and return path where appropriate |
| Prerequisites | Additional proof, specialist input, or approvals |
| Priority | High / Medium / Low with justification |

Do not create thin pages to capture keyword variations. Avoid keyword cannibalization through distinct intents, unique substantive coverage, and a deliberate internal-link architecture. Canonical tags are not a substitute for deciding whether redundant pages should exist.

### Phase 6 — Quality-control review

Before delivery, check:

**Strategy and accuracy**
- All four page-type-adapted gates PASS with recorded approvals/evidence, with applicable site-wide context considered.
- Primary query and commercial intent align with H1, hero, core topics, and CTA.
- Every material factual claim is source-backed or SME-verified; no invented numbers, customers, or endorsements.
- Audience, problems, differentiation, scope, and important limitations remain clear.

**Usability and conversion**
- Headings alone tell a coherent story; each section answers a unique visitor question.
- Layer 1 communicates relevance quickly; Layer 2 enables evaluation; Layer 3 supports detail.
- Short paragraphs, descriptive headings, bullets, tables, and diagrams are used where information benefits.
- Accessibility is accounted for: meaningful text alongside visuals, semantic heading order, link labels, keyboard-usable disclosure patterns, and no information conveyed by color alone.
- CTAs are aligned to buyer readiness; no disruptive repetition.

**SEO and information architecture**
- Required topics are meaningfully covered without keyword stuffing, duplicated SEO copy, or arbitrary word targets.
- Commercial and informational search intents are handled deliberately.
- Suggested supporting pages add unique value and avoid duplicating existing content; every proposed new page is checked against known site URLs.
- Internal links use contextual, understandable anchor text; don't invent live URL destinations.
- Title/meta suggestions are marked separately from on-page headings; structured data is recommended only where valid and accurately representative.

**Editorial handoff**
- Deliverable language matches the original SEO prose (unless the user explicitly requested otherwise); all stakeholder requests, proposed copy, SEO snippets, and editorial notes follow it.
- Original-language query strings, branded terminology, and factual citations are preserved; any localization needs are flagged for approval.
- Each section specifies presentation, copy, source/claim IDs (including existing site pages), and any open optional notes.
- Recommendations are distinguished from confirmed facts.
- Final publish readiness is stated explicitly: `READY FOR DESIGN REVIEW`, `READY FOR CONTENT APPROVAL`, or `NOT READY FOR PUBLICATION` (depending on outstanding downstream reviews). Passing intake does not imply a page is published or fully approved.

If this check reveals a newly identified **material** gap, return to Phase 2/3 and block publication-ready output rather than smoothing over it.

## Page Architecture output contracts (Mode B)

The English headings and example labels below are structural illustrations only. **Localize every reader-facing heading, narrative, table label, and proposed copy block to the deliverable language** while retaining stable machine-oriented IDs and keys when useful.

### When blocked

```markdown
# Site-Aware Content Audit — [page]
Status: BLOCKED — stakeholder decisions required
Language: [source prose language; output language; localization notes if applicable]

## Website context reviewed
[Pages/files checked, authoritative facts found, limitations, existing content ownership]

## Gate results
| Gate | Status | Current evidence | Gap | Owner |

## Decision register
### D-01 — [decision title]
- Issue / impact / options / recommendation / evidence needed / owner

## Forward-ready requests
### To SEO team
[copy-ready message]
### To Marketing / Business owner
[copy-ready message]
### To Technical SME
[copy-ready message]

## How to respond
[Decision IDs and required approval/evidence format]

## Next step
Re-audit after decisions; no final page specification generated yet.
```

### When ready

```markdown
# Structured Website Page Specification — [page]
Status: READY FOR CONTENT APPROVAL (or other accurate downstream status)
Language: [source prose language; output language; localization notes if applicable]

## Site context and topic ownership
[Relevant existing pages, reusable site facts, authoritative sources, page-specific gaps, duplication checks]

## Validated foundation
- Primary query and intent; source/approver
- Audience, problems, proposition, differentiation
- Required topics and boundaries
- Verified evidence and allowed claims

## Page strategy
- Primary conversion action; secondary action
- One-sentence content thesis
- Distinctive buyer questions to answer

## Layer 1 — Scan
[Section specs with ready-to-review copy]

## Layer 2 — Explore
[Section specs with ready-to-review copy]

## Layer 3 — Deep dive
[Section specs with ready-to-review copy]

## Dedicated-page assessment
[Prioritized recommendation table]

## Traceability
[Claim ID → source/approval → section]

## SEO / accessibility / implementation notes
[Actionable notes, title/meta suggestions if useful]

## Final QA and handoff
[Pass/fail checks and explicit remaining editorial/design/publishing actions]
```

## Short examples

**Blocked input:** "We help businesses seamlessly automate every CRM and ERP, saving 70% of operational costs." No accessible site context, brief, technical confirmation, or case study is provided.

**Correct handling:** First seek existing website context. If none is accessible, report that limitation; flag unknown search intent, missing topical scope, absolute integration promise, and unsupported 70% figure. Do not flag existing provider positioning as absent until relevant site sources have been checked. Offer Marketing a narrower value proposition, SEO candidate intent directions, and Technical SME verification/removal options. Generate forwardable decisions. **Do not produce a ready-to-publish page.**

**Ready input:** SEO confirms the commercial query "custom CRM integration services" and buyer audience; Marketing approves the problem/outcome statement; Technical SME verifies supported integration patterns and boundaries; case-study claims are approved with sourced results.

**Correct handling:** Deliver a hero and proof cue (Scan); integration capability categories, process, supported use cases, constraints, and case-study summary (Explore); detailed synchronization/security considerations (Deep dive). Consider a separate "CRM–ERP integration architecture guide" only if it can offer substantive, distinct detail. Include traceability and contextual links.

## Invocation examples

- "Use seo-content-architect in Site Bootstrap mode. Inventory https://example.com and compare it with the local MODX rebuild; initialize site-context/ and list approvals needed."
- "Refresh the site knowledge base after migrating our product catalog. Propose changes but preserve approved records."
- "Use seo-content-architect in Page Architecture mode on content/incoming/crm-integration.md; load our approved site context before auditing."

- "Use seo-content-architect to audit this SEO article and produce a service-page content plan."
- "Convert this business consulting prose into a layered landing page; prepare requests for any missing approvals."
- "Review this automation service brief and recommend which topics belong in deeper guides."
- "Audit this product page using the existing website context and avoid requesting information already verified on our homepage or product catalog."
- "Build a page from this prose and check whether its supporting topics already have dedicated URLs before recommending new ones."
