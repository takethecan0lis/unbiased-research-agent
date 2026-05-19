# README
## Unbiased Research Agent
### Version 2.0 | May 2026

# Unbiased Research Agent
### A Claude Project for rigorous, bias-disclosing fact-check and research. Operates under Ten Commandments it cannot override and discloses its own trained biases in real time.
---

## What This Is

A ready-to-install Claude Project that fact-checks claims, analyzes news articles, and investigates contested topics using structured journalistic methodology — and discloses its own biases in real time rather than hiding them.

Standard AI conversations have no persistent methodology, no rules about institutional bias, and no requirement to surface when their own programming is shaping their output. This agent has all three. It operates under Ten Commandments it cannot override, produces formal research reports with cited sources and confidence ratings on every claim, and flags its own trained dispositions automatically using `[BIAS DISCLOSURE]` tags as they occur.

**The core principle:** Every claim is a hypothesis. Evidence is the test. The reader decides.

---

## What Makes This Different

**It discloses its own bias.** When the agent's training is pulling it toward the institutional account, the mainstream consensus, or away from conclusions that look "conspiracy-adjacent," it is required to say so — using `[BIAS DISCLOSURE]` tags, in real time, before a conclusion is reached. This is not a sign of failure. It is the system working correctly.

**It rates confidence on every claim.** Every significant finding is labeled: `Confirmed`, `Likely`, `Disputed`, `Unsubstantiated`, or `False`. You always know how solid the ground is.

**It has two analytical scales.** The Fibonacci Accuracy Scale rates how factually accurate a claim is, from -8 (completely false) through 0 (indeterminate — insufficient evidence to determine) to +8 (completely verified by independent primary sources). The Fibonacci Political Bias Scale rates political lean from -8 (extreme left) through 0 (no detectable bias) to +8 (extreme right), applied separately to the source and to the content itself. A biased source can report accurate facts. An accurate claim can be politically slanted. The two scales capture what a single scale cannot.

**It follows a source hierarchy with an Institutional Implication Exception.** When the institution producing evidence is itself implicated in the claim being investigated — the FBI analyzing an FBI operation, for example — that source is automatically reclassified from Tier 1 to Tier 3 and treated as an interested party account.

**It generates formal research reports.** When asked, the agent produces a downloadable PDF with cited sources, confidence ratings, source bias assessments, and a full Works Cited section in MLA format.

---

## What It Is Not

It is not a search engine. It is not infallible. It is not a replacement for your own critical thinking. Its output is a structured starting point for your own evaluation — not a verdict. One of its Ten Commandments says explicitly: *the reader decides.*

---

## Files in This Repository

| File | Purpose |
|---|---|
| `PROJECT_INSTRUCTIONS.md` | Paste into Claude's Project Instructions field. The Ten Commandments, source hierarchy, bias disclosure rules, research methodology, and confidence scoring system. |
| `BIAS_TRANSPARENCY_PROTOCOL.md` | Upload to project knowledge. Full specification of the five named dispositions the agent monitors and discloses, the Institutional Implication Rule, and the Surprise Test protocol. |
| `FIBONACCI_ACCURACY_SCALE.md` | Upload to project knowledge. Measures factual accuracy of a claim or piece of information on a scale from -8 (completely false) through 0 (indeterminate) to +8 (completely verified). |
| `FIBONACCI_POLITICAL_BIAS_SCALE.md` | Upload to project knowledge. Measures political or ideological lean on a scale from -8 (extreme left) through 0 (no detectable bias) to +8 (extreme right). Applied separately to source and content. |
| `PDF_REPORT_TEMPLATE.md` | Upload to project knowledge. Report structure, section definitions, and PDF generation toolchain. |
| `PROJECT_MEMORY_PUBLIC.md` | Upload to project knowledge. Persistent methodological context and your personal research history. Intentionally left blank in the public version — fill it in as you run sessions. |
| `QUALITY_ASSURANCE_INSPECTION_GUIDE.md` | Run at setup, periodically, and any time the agent's behavior feels degraded or inconsistent. Contains the full diagnostic query, four targeted failure-mode checks, a recommended QA schedule, and a logging format. | 
| `SETUP_GUIDE_AND_USER_MANUAL.md` | Start here if you've never built a Claude Project before. Step-by-step setup instructions, sample prompts, a cross-platform adaptation guide, and an initial test query to verify the agent is operating correctly. |

---

## Quick Start

**If you've never built a Claude Project before:** read `SETUP_GUIDE_AND_USER_MANUAL.md` first. It walks through every step with no assumed technical knowledge and takes about 15 minutes.

**If you know how Claude Projects work:**

1. Create a new Claude Project at [claude.ai](https://claude.ai)
2. Paste the contents of `PROJECT_INSTRUCTIONS.md` into the Project Instructions field
3. Upload these five files to the project knowledge base:
   - `BIAS_TRANSPARENCY_PROTOCOL.md`
   - `FIBONACCI_ACCURACY_SCALE.md`
   - `FIBONACCI_POLITICAL_BIAS_SCALE.md`
   - `PDF_REPORT_TEMPLATE.md`
   - `PROJECT_MEMORY_PUBLIC.md`
4. Run the test query in Part 5 of the setup guide to verify correct operation

A Claude Pro account is recommended. Free accounts have message limits that may interrupt longer research sessions. PDF report generation requires the computer use feature available on Pro.

---

## How to Use It

**Fact-check a claim:**
> "Research this claim using your full methodology: [paste claim]"

**Analyze an article:**
> "Analyze this article for accuracy and framing: [paste text or URL]"

**Generate a PDF research report:**
> "Generate a formal PDF research report on [topic]"

**Get a bias scale rating:**
> "Give me your bias scale position on this topic with full justification"

**Challenge the conclusion:**
> "Give me the strongest adversarial argument against what you just found"

A full prompt library and adversarial questioning guide is in Part 3 and Part 4 of `SETUP_GUIDE_AND_USER_MANUAL.md`.

---

## Works on Other Platforms Too

Part 6 of the setup guide includes a ready-to-use prompt for adapting this agent to ChatGPT, Gemini, Grok, Perplexity, or any other AI platform. Paste it into your AI of choice and it will generate a customized setup guide for that platform, including what features it can and cannot fully support.

---

## Attribution

The **Fibonacci Accuracy Scale**, **Fibonacci Political Bias Scale**, and **Bias Transparency Protocol** were developed by Drew Podwal in May 2026. The underlying cognitive bias concepts draw on established epistemological literature. The operationalization as a working AI instruction system — including the named disclosure triggers, the Institutional Implication Exception, the Drift Anchor Rule, and the surprise symmetry definition of zero — is original to this project.

If you adapt, build on, or publish work using these frameworks, attribution is appreciated.

---

## License

This project is released under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt this material for any purpose, including commercially, as long as you give appropriate credit, link to the license, and indicate if changes were made.

---

## Feedback and Contributions

This project improves through critique. If you find a methodological gap, a place where the agent behaves inconsistently, or a way to strengthen the bias disclosure protocol, please open an Issue.

**To report a bug or inconsistency:** Open an Issue and describe what query you ran, what the agent did, and what you expected it to do instead.

**To suggest a methodological improvement:** Open an Issue describing the gap and, if you have one, a proposed solution.

**To propose a change directly:** Fork the repo, make your edits, and open a Pull Request with a clear explanation of what you changed and why.

---

*Version 2.0 | May 2026*
