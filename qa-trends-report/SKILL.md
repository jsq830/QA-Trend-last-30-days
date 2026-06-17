---
name: qa-trends-report
description: Create bilingual Markdown QA trend reports from current global public signals. Use when Codex is asked to research, summarize, compare, or write reports about software QA trends, software testing, test automation, AI-assisted testing, testing AI systems, quality engineering, QA governance, test management, release quality, QA tooling, or QA market/vendor trends. Use for requests such as "QA trend report", "testing trends", "quality engineering trends", "AI testing trends", "international QA trends", or "what is happening in QA".
---

# QA Trends Report

## Core Rule

Produce a software-quality report, not a generic technology-news digest. Keep only signals related to software testing, test management, test automation, AI-assisted QA, AI-system testing, QA governance, release quality, quality engineering, observability for quality, or QA tools and vendors.

Discard signals that are only about general AI, generic developer productivity, broad cybersecurity, hiring, or business news unless they clearly affect QA work.

## Research Workflow

1. Clarify scope from the user's wording: timeframe, region, audience, output length, and whether the report should be strategic, operational, vendor-focused, or tool-focused.
2. If the user asks for current, recent, latest, market, vendor, or public sentiment coverage, browse the web and cite sources. Prefer primary or near-primary sources: official product docs/blogs, standards bodies, conference programs, vendor release notes, analyst summaries, GitHub repositories, practitioner articles, and job postings.
3. Use global balanced source coverage. Include credible signals from North America, Europe, and Asia-Pacific when available. Add Latin America, Africa, and Middle East signals when they are relevant and credible.
4. Use multilingual source discovery where useful, especially English, German, French, Spanish, Portuguese, Japanese, Korean, and Chinese. Translate non-English evidence into the final English and German report sections.
5. Collect signals across at least four buckets when possible:
   - AI in QA: test generation, flaky-test analysis, bug triage, model evaluation, prompt/RAG/agent testing.
   - Automation and tooling: Playwright, Cypress, Selenium, mobile testing, API testing, contract testing, visual testing, test data, CI quality gates.
   - Governance and risk: auditability, traceability, compliance, safety, AI governance, test evidence, quality ownership.
   - Market and practice: QA org changes, shift-left/shift-right, platform engineering, quality engineering roles, vendor consolidation.
6. Rank trends by evidence strength and practical impact. Avoid overstating weak signals.
7. Select exactly the top 5 key QA trends when at least 5 credible QA-relevant trends are evidenced. If fewer than 5 qualify, state the limitation and include only evidenced trends.
8. Separate observations from interpretation. Label uncertain interpretations as inferences.

## Output Standards

Always produce the final report in Markdown. Use Markdown headings, bullets, tables when useful, and normal Markdown links for sources. Do not output DOCX, PDF, HTML, slide, spreadsheet, or plain unstructured text unless the user explicitly asks for another format.

Always produce one bilingual document with a complete English report first and a complete German report second. The German section must be a full German version, not a short summary.

Use concrete dates when describing "latest" or "recent" trends. Include source links for web-based claims.

Prefer this structure unless the user asks for a different format:

- `# QA Trends Report: <period>`
- `## English`
- `### Executive Summary`
- `### Top 5 Key QA Trends`
- `### Evidence and Examples`
- `### Impact for QA Teams`
- `### Sources`
- `## Deutsch`
- `### Zusammenfassung`
- `### Top 5 QA-Trends`
- `### Evidenz und Beispiele`
- `### Auswirkungen auf QA-Teams`
- `### Quellen`

In both language sections, include clear source metadata in Markdown: source, date, language or region, evidence strength, and QA-relevant signal.

For a reusable section-by-section template, read `references/report-template.md`.

## Quality Bar

Name specific tools, practices, standards, releases, or organizations when evidence supports it. Each key trend must be detailed, not a one-sentence summary. For each trend, include what changed, why it matters now, supporting evidence, practical impact for QA teams, evidence strength, affected testing areas, and likely risks or constraints.

Do not include vague trend labels without operational meaning. Replace "AI is transforming QA" with a specific change such as "teams are using LLMs to generate first-draft Playwright tests, but still need human review and deterministic assertions."

Do not include Recommended Actions or Watchlist sections in the final report unless the user explicitly asks for them.
