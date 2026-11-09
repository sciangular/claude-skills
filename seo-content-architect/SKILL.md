---
name: seo-content-architect
description: Audits SEO prose and briefs for search intent, topical completeness, value proposition, customer problems, differentiators, technical accuracy, and evidence; requests stakeholder approvals; then converts approved content into layered, scannable B2B service page specifications and related-page recommendations. Use when transforming SEO copy into a landing page or service page.
---

# SEO Content Architect

Convert prose-first SEO copy for complex corporate/B2B services into an evidence-grounded, scannable page content specification. Use a **mandatory validation and approval gate** before producing a final page structure.

## Operating rules

1. **Validate before transforming.** Run the full intake audit even when the prose seems polished.
2. **Do not silently fill gaps.** Propose alternatives for missing information, clearly mark them `PROPOSED — NOT APPROVED`, and route them to an accountable person/team.
3. **Never invent evidence.** Do not fabricate customer outcomes, ROI figures, testimonials, credentials, integrations, product support, timelines, pricing, or case studies.
4. **Preserve meaning, improve presentation.** Rewrite for comprehension and scanning without changing the substance of verified claims. Quote source excerpts when explaining a finding; otherwise paraphrase.
5. **Optimize for the visitor first.** Do not append filler paragraphs, stuff keywords, manufacture FAQ sections, or promise rankings. SEO is a constraint on information architecture, not an excuse for duplication.
6. **Separate approval from verification.** A team can approve proposed wording, but objective technical claims still need a credible source or documented subject-matter verification.
7. **Keep final output implementation-agnostic.** Produce content structure and component recommendations, not code, unless explicitly asked. Do not modify project files or published pages without authorization.
8. **Reuse supplied context.** Read the user's prose, brief, brand documentation, project artifacts, and prior explicit approvals when available. Distinguish current approved material from historical or draft material.
9. **Do not infer search metrics.** Search volume, difficulty, ranking, intent inferred from SERPs, or competitor gaps must be labeled `NOT VERIFIED` unless supported by current research/data. If browsing/tools are available and authorized, use them selectively and cite sources; do not claim independent validation without it.
10. **If requirements conflict, surface the conflict** with a concrete decision request. Do not resolve business or factual conflicts by guessing.
11. **Preserve the source language throughout deliverables.** Detect the primary language of the user-supplied SEO prose and use that language for **all user-facing outputs**: audit findings, status explanations, option recommendations, stakeholder-forwardable requests (including subjects and reply templates), proposed page headings/copy, layer descriptions, supporting-page titles, meta copy, and QA/handoff notes. Do not default to English merely because this skill is written in English. Keep proper nouns, brand names, documented product/technical terms, URLs, and verbatim search queries in their original forms when appropriate; never translate target keywords silently. Only produce translated or bilingual deliverables when explicitly requested or approved. Internal structural identifiers such as `D-01`, `S-01`, `claim_id`, enum values, and code keys may remain in English for machine readability.
12. **Resolve mixed-language inputs conservatively.** When the SEO prose is predominantly one language, use it as the deliverable language even if the brief or stakeholder notes are in another. If there are multiple substantial language versions or the source language is ambiguous, register a language-selection decision for the responsible content/SEO owner and block publication-ready transformation until resolved. If the user explicitly specifies a deliverable language, follow that instruction while labeling translation/localization requirements and requiring approval of adapted keyword targets and market-specific claims.

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

## Workflow

### Phase 1 — Inventory and classify evidence

**Language preflight (required):** Record `source_prose_language`, `deliverable_language`, `language_basis` (dominant prose language or explicit user instruction), and any `localization_or_keyword_review_needed`. Apply the same language to the blocked and ready output contracts; do not send English stakeholder requests for non-English prose. Preserve the exact wording of verified search queries and source citations. A mismatch between the prose language and the targeted search market or query language is a content/SEO decision, not permission to silently translate keywords.

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
| B. Content outline and required topics | An explicit approved outline or requirement list that covers the service definition, scope, applicability, key buyer questions, important limitations, and conversion-relevant topics; deliberate omissions are documented. | SEO + Marketing + Technical SME |
| C. Value proposition, customer problems, and differentiators | Specific target audience, real customer problems, business outcomes, clear offer/value proposition, and at least one defensible distinction (or an explicit approved statement that no differentiated claim is currently supported). Avoid unsupported superiority claims. | Marketing + Business owner |
| D. Technical accuracy and supporting evidence | Material factual and technical claims are mapped to credible evidence or named SME verification; material proof claims have sources and permission where applicable; unresolved contradictions, unverifiable numerical claims, and essential capability gaps are absent. An explicit `no published customer proof available` decision is acceptable only if all remaining claims are supportable. | Technical SME + Business owner; Legal for regulated claims |

Audit details:

**A — Search intent:** Classify informational, commercial investigation, transactional, navigational, or mixed intent. State the desired visitor outcome and whether the proposed page type matches it. Distinguish stakeholder-supplied queries from independently researched targets; do not treat guessed queries as verified.

**B — Topical completeness:** Cross-check source prose, brief, buyer journey, and any verified search insights. Distinguish `must cover on this page`, `optional here`, and `better on a dedicated page`. Consider exclusions, onboarding, process, security/privacy, compatibility, delivery constraints, pricing approach, evidence, and FAQs when relevant—not as compulsory boilerplate.

**C — Commercial clarity:** Identify who buys, why now, triggering pains, what changes, what is included, what's different, and the next action. Distinguish features from customer benefits and benefits from independently proven outcomes.

**D — Accuracy/evidence:** Check capability details, integrations, standards, constraints, quantitative claims, case studies, client names, pricing/timelines, and legal/compliance claims. Record sources and dates when available. General descriptions can pass without a dedicated citation if clearly supported by approved service scope and technical review. Do not demand case studies that do not exist; instead recommend honest alternative proof (e.g., process, deliverables, demo, public documentation).

#### Gate decision

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
Subject: Decision needed — [service/page] — [topic]
To: [responsible team/role]

Context: We are converting [source] into a service landing page aimed at [audience / intent].
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

Purpose: Immediately answer "Am I in the right place, what is offered, why does it matter, and what can I do next?"

Possible modules: precise H1/hero, value proposition, short supporting copy, primary CTA, audience-fit statement, 3–5 concise problem/outcome statements, credible proof cue (only if substantiated).

Writing: use the source prose language, front-load meaning, use unambiguous service terminology, favor outcomes over slogans, preserve primary search topic naturally. Avoid vague superlatives and unsupported numbers.

#### Layer 2: Explore — evaluate the service

Purpose: Answer "Can this provider solve my problem, how will it work, and why should I trust them?"

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
- All four gates PASS with recorded approvals/evidence.
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
- Suggested supporting pages add unique value and avoid duplicating existing content.
- Internal links use contextual, understandable anchor text; don't invent live URL destinations.
- Title/meta suggestions are marked separately from on-page headings; structured data is recommended only where valid and accurately representative.

**Editorial handoff**
- Deliverable language matches the original SEO prose (unless the user explicitly requested otherwise); all stakeholder requests, proposed copy, SEO snippets, and editorial notes follow it.
- Original-language query strings, branded terminology, and factual citations are preserved; any localization needs are flagged for approval.
- Each section specifies presentation, copy, source/claim IDs, and any open optional notes.
- Recommendations are distinguished from confirmed facts.
- Final publish readiness is stated explicitly: `READY FOR DESIGN REVIEW`, `READY FOR CONTENT APPROVAL`, or `NOT READY FOR PUBLICATION` (depending on outstanding downstream reviews). Passing intake does not imply a page is published or fully approved.

If this check reveals a newly identified **material** gap, return to Phase 2/3 and block publication-ready output rather than smoothing over it.

## Output contracts

The English headings and example labels below are structural illustrations only. **Localize every reader-facing heading, narrative, table label, and proposed copy block to the deliverable language** while retaining stable machine-oriented IDs and keys when useful.

### When blocked

```markdown
# SEO Content Audit — [page]
Status: BLOCKED — stakeholder decisions required
Language: [source prose language; output language; localization notes if applicable]

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
# Structured Service Page Specification — [page]
Status: READY FOR CONTENT APPROVAL (or other accurate downstream status)
Language: [source prose language; output language; localization notes if applicable]

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

**Blocked input:** "We help businesses seamlessly automate every CRM and ERP, saving 70% of operational costs." No brief, technical confirmation, or case study is provided.

**Correct handling:** Flag unknown search intent, missing topical scope and audience positioning, absolute integration promise, and unsupported 70% figure. Offer Marketing a narrower value proposition, SEO candidate intent directions, and Technical SME verification/removal options. Generate forwardable decisions. **Do not produce a ready-to-publish page.**

**Ready input:** SEO confirms the commercial query "custom CRM integration services" and buyer audience; Marketing approves the problem/outcome statement; Technical SME verifies supported integration patterns and boundaries; case-study claims are approved with sourced results.

**Correct handling:** Deliver a hero and proof cue (Scan); integration capability categories, process, supported use cases, constraints, and case-study summary (Explore); detailed synchronization/security considerations (Deep dive). Consider a separate "CRM–ERP integration architecture guide" only if it can offer substantive, distinct detail. Include traceability and contextual links.

## Invocation examples

- "Use seo-content-architect to audit this SEO article and produce a service-page content plan."
- "Convert this business consulting prose into a layered landing page; prepare requests for any missing approvals."
- "Review this automation service brief and recommend which topics belong in deeper guides."
