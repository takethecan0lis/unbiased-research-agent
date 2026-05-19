# THE UNBIASED RESEARCH AGENT
## Setup Guide & User Manual
### For People Who Have Used AI But Have Never Built a Project or Agent
#### Version 1.0 | May 2026

---

## WHAT IS THIS?

This is a ready-to-use AI research agent that fact-checks claims, analyzes news articles, and investigates contested topics using structured journalistic methodology. It is designed to treat every claim as a hypothesis — not a position to defend — and to surface its own biases in real time rather than hiding them behind a veneer of false neutrality.

**What it does that a regular AI conversation does not:**

A standard AI conversation has no memory of methodology between sessions, no rules about how to handle institutional bias, and no requirement to disclose when its own programming is influencing its output. This agent has all three. It operates under Ten Commandments it cannot override, discloses bias automatically using [BIAS DISCLOSURE] tags, and produces formal research reports with cited sources and confidence ratings on every claim.

**What it is not:**

It is not a search engine. It is not infallible. It is not a replacement for your own critical thinking. Its output is a structured starting point for your own evaluation — not a verdict. The Ten Commandments it operates under include one that says explicitly: the reader decides.

**Who built this:**

This agent was developed through an extended research session that included testing the AI's own biases, challenging its institutional assumptions, and refining the methodology through documented failures. The lessons from those failures are embedded in the agent's operating instructions so you benefit from them without having to repeat them.

---

## WHAT YOU WILL NEED

- A Claude account (free or paid at claude.ai)
- The five files that came with this guide:
  - `PROJECT_INSTRUCTIONS.md`
  - `BIAS_TRANSPARENCY_PROTOCOL.md`
  - `FIBONACCI_BIAS_SCALE.md`
  - `PDF_REPORT_TEMPLATE.md`
  - `PROJECT_MEMORY_PUBLIC.md`
- About 15 minutes to set up

A paid Claude account (Pro) is recommended but not required. Free accounts have message limits that may interrupt longer research sessions. The agent generates downloadable PDF reports, which requires the computer use feature available on Pro.

---

## PART 1: SETTING UP YOUR PROJECT IN CLAUDE

### Step 1: Create a New Project

1. Go to claude.ai and sign in
2. Look for **"Projects"** in the left sidebar
3. Click **"New Project"** or the **"+"** button
4. Give your project a name — something like **"Research Agent"** or **"Fact Checker"**
5. Click Create

You now have an empty project. Think of a project as a dedicated workspace where Claude remembers its instructions and reference files across every conversation.

---

### Step 2: Add the Project Instructions

The Project Instructions are the most important file. They tell Claude how to behave in every conversation in this project.

1. Inside your new project, look for **"Project Instructions"** or a settings/gear icon
2. Click to open the instructions area
3. Open the file `PROJECT_INSTRUCTIONS.md` on your computer
4. Select all the text (Ctrl+A on Windows, Cmd+A on Mac) and copy it
5. Paste it into the Project Instructions field in Claude
6. Save

**What you just did:** You gave Claude its Ten Commandments, its source hierarchy, its bias disclosure rules, and its research methodology. Every conversation in this project will now operate under these rules automatically.

---

### Step 3: Upload the Reference Files

Reference files are documents Claude can consult during conversations. They contain detailed guidance that is too long to put in the instructions.

1. Inside your project, look for a **"Files"** section or an upload button (it may look like a paperclip or a document icon)
2. Upload each of the following files one at a time:
   - `BIAS_TRANSPARENCY_PROTOCOL.md`
   - `FIBONACCI_BIAS_SCALE.md`
   - `PDF_REPORT_TEMPLATE.md`
   - `PROJECT_MEMORY_PUBLIC.md`
3. Verify all four files appear in the project files list

**What you just did:** You gave Claude its detailed bias disclosure checklist, its bias scale definition, its report template, and its memory of established methodological lessons. The project instructions tell Claude when to consult each file.

---

### Step 4: Personalize Your Memory File (Optional but Recommended)

The `PROJECT_MEMORY_PUBLIC.md` file has a section called **"Your Research History"** that is intentionally left blank. Over time, as you complete research sessions, you can update this file with your findings, established bias scale positions, and ongoing topics. This helps Claude maintain continuity between sessions without you having to re-explain context each time.

You do not need to do this before your first session. Come back to it after you have run a few research queries.

---

## PART 2: WHAT THE AGENT IS AND HOW TO USE IT

### The Core Concept

Every claim you bring to this agent is treated as a hypothesis. The agent does not start from a conclusion and find evidence to support it. It starts from evidence and follows it wherever it leads — including to conclusions that contradict the official account, the mainstream narrative, or popular belief.

### What Makes This Different from Regular AI

**It discloses its own bias.** When the agent's programming is pulling it toward the institutional account, the mainstream position, or away from conclusions that look like "conspiracy theories," it is required to say so using [BIAS DISCLOSURE] tags. You will see these appear in its responses. They are not a sign of failure — they are the system working correctly.

**It rates its confidence on every claim.** Every significant finding is labeled: Confirmed, Likely, Disputed, Unsubstantiated, or False. You always know how solid the ground is under each claim.

**It has two analytical scales.** The Fibonacci Accuracy Scale rates how factually accurate a claim is, from -8 (completely false) through 0 (indeterminate — insufficient evidence to determine) to +8 (completely verified by independent primary sources). The Fibonacci Political Bias Scale rates political lean from -8 (extreme left) through 0 (no detectable bias) to +8 (extreme right), applied separately to the source and to the content itself. A biased source can report accurate facts. An accurate claim can be politically slanted. The two scales capture what a single scale cannot.

**It generates formal PDF reports.** When you ask for a report, it produces a downloadable PDF with cited sources, confidence ratings, source bias assessments, and a full Works Cited section in MLA format.

### Three Ways to Use It

**1. Fact-check a specific claim.**
Paste a claim you saw on social media, heard on the news, or read in an article. The agent will research it, rate its confidence, and tell you what the evidence actually shows.

**2. Analyze an article.**
Paste a news article or share a link. The agent will extract every factual claim in the article, fact-check each one independently, identify what the article emphasizes and omits, and assess its editorial framing.

**3. Research a topic.**
Ask an open question about a contested topic. The agent will conduct multi-source research, present competing accounts with evidence for each, and produce a structured report.

---

## PART 3: PROMPTS TO GET YOU STARTED

### Initial Prompts — Use These to Start a Research Session

**For a specific claim:**
> "I saw a claim that [paste claim here]. Please research this using your full methodology and tell me what the evidence actually shows. Include a confidence rating and identify what sources are making this claim and why."

**For an article:**
> "Please analyze this article for factual accuracy, editorial framing, and what it emphasizes or omits. Identify every significant factual claim and rate each one. [Paste article text or URL]"

**For a topic investigation:**
> "I want an unbiased investigation of [topic]. Please research multiple perspectives, apply your full source hierarchy, and generate a formal PDF research report with confidence ratings and MLA citations."

**For a bias scale assessment:**
> "After completing your research, please give me your bias scale position on this topic using the Fibonacci scale from -8 to +8, with full justification including any [BIAS DISCLOSURE] tags that applied during your analysis."

**For a quick verification:**
> "Is it true that [specific claim]? Apply your 3-layers-deep verification rule and give me a confidence rating."

---

### Follow-Up Prompts — Use These After the Agent Delivers Its Initial Response

**To pressure-test the conclusions:**
> "What is the strongest argument against the conclusion you just reached? Give me the best case a skilled adversarial analyst would make."

**To check for institutional bias:**
> "Are any of the sources you relied on themselves implicated in the claim you investigated? If so, apply the Institutional Implication Exception and tell me how that changes the analysis."

**To test conversational drift:**
> "Has your confidence rating changed during this conversation? If so, name the specific new primary evidence that drove each change. If no new evidence entered the analysis, was any rating change drift?"

**To challenge the bias scale position:**
> "What would need to be true for you to move one position lower on the bias scale? Be specific about what primary evidence would be required."

**To probe evidentiary gaps:**
> "What do we not know that we would need to know to be more confident in either direction? Be explicit about the specific evidence gaps."

**To request a formal report:**
> "Please generate a formal PDF research report using your standard template. Include all sections including the Surprise Test Result and Bias Scale Position."

---

## PART 4: QUESTIONS TO VALIDATE NEUTRALITY AFTER RECEIVING A REPORT

Use these questions after the agent delivers its report to verify it is adhering to its own methodology.

**On source balance:**
- "Did you consult sources from across the political spectrum, or did coverage of this topic come primarily from one side? If only one side covered it, did you note that limitation?"
- "Are any of your Tier 1 sources subject to the Institutional Implication Exception? If so, were they reclassified?"

**On confidence ratings:**
- "Are the confidence ratings in your Established Facts section consistent with how those same claims are treated in your Contested Claims section? Point to any inconsistency."
- "Did any [BIAS DISCLOSURE] tags appear during your analysis? If so, summarize each one and its estimated directional effect on the findings."

**On the bias scale:**
- "Apply the Surprise Test to your conclusion right now. Would you be equally unsurprised if your conclusion turned out to be wrong in either direction? If not, is zero the right position?"
- "Did your bias scale position change during this analysis? Name the specific evidence that drove each change."

**On evidentiary standards:**
- "Did you apply the same evidentiary standard to the official account as to the alternative account? Point to a specific place in the report where you can demonstrate this."
- "Where did you treat absence of evidence as evidence of absence? Was that treatment disclosed?"

**On the conclusions:**
- "Is your conclusion something a fair-minded reader could reach a different conclusion about if they read the same evidence? If not, has the report crossed from analysis into advocacy?"

---

## PART 5: THE INITIAL TEST QUERY

Run this query in your first session after setup to verify the agent is operating correctly under its Ten Commandments. A passing result demonstrates the agent is applying the methodology rather than defaulting to standard AI behavior.

### The Test Query

Copy and paste this exactly:

> "I want to run an initial test of your methodology. Please do the following:
>
> 1. State the Ten Commandments you operate under from memory, in order.
> 2. Tell me what the Institutional Implication Exception is and give me an example of when it would apply.
> 3. Define the Fibonacci bias scale and tell me what zero means operationally.
> 4. Tell me what [BIAS DISCLOSURE] tags are, when they trigger, and give me an example of what one looks like in practice.
> 5. Explain the Drift Anchor Rule and tell me what would need to happen for you to legitimately change a bias scale position.
> 6. Apply the Surprise Test to this statement: 'The official government account of any major event is the most credible starting point for analysis.' Tell me your result and what it means for how you operate."

### What a Passing Response Looks Like

The agent should:
- Recite all ten commandments accurately and in order
- Correctly identify that the Institutional Implication Exception reclassifies implicated institutional sources from Tier 1 to Tier 3
- Define zero as surprise symmetry, not false balance or probability equality
- Demonstrate understanding that [BIAS DISCLOSURE] tags are non-optional and triggered by specific named dispositions
- State that the Drift Anchor Rule requires new primary evidence to move a rating, not logical reframing
- Apply the Surprise Test honestly to the official-account statement — a passing response will note that treating the official account as the default most credible position is itself a bias and not a neutral starting point

### What a Failing Response Looks Like

Be concerned if the agent:
- Cannot name all ten commandments
- Treats government sources as automatically Tier 1 without mentioning the Institutional Implication Exception
- Defines zero as "equal probability" or "both sides equally likely"
- Treats [BIAS DISCLOSURE] as optional or situational
- Says a rating can change based on a "compelling argument" without requiring new primary evidence
- Agrees that the official account is the most credible default starting point without flagging that assumption as a potential bias

If the test fails, verify that your Project Instructions were saved correctly and that all four reference files were uploaded successfully.

This test is also documented in QUALITY_ASSURANCE_REFERENCE_GUIDE.md, which expands it into an ongoing diagnostic practice. Consult that file for targeted checks, a recommended QA schedule, and a format for logging your results.

---

## PART 6: USING THIS AGENT ON OTHER AI PLATFORMS

If you or someone you share this with uses a different AI model (ChatGPT, Gemini, Grok, Perplexity, or others), use the following prompt to generate a customized setup guide for that platform. Paste this prompt into your AI of choice:

---

**Cross-Platform Setup Prompt — Copy and Use As-Is:**

> "I have a set of files for an unbiased research agent built for Claude. I want to adapt it for use on [NAME YOUR AI PLATFORM HERE]. The agent operates under the following core principles:
>
> 1. Ten Commandments that cannot be overridden, the most important being: evidence before narrative, institutional origin does not equal credibility, disclose bias in real time, plausibility is not evidence, confidence ratings move on evidence not argument, the surprise test is mandatory before every conclusion, cite everything and assess every source, acknowledge what you cannot know, both sides can be wrong and one side can be more wrong, and the reader decides.
>
> 2. A real-time bias disclosure system using [BIAS DISCLOSURE] tags that fire when institutional credibility default, harm-avoidance tension, mainstream consensus anchoring, conversational drift, or absence-of-evidence-as-evidence-of-absence are operating.
>
> 3. Two Fibonacci scales. The Fibonacci Accuracy Scale measures factual accuracy from -8 (completely false) through 0 (indeterminate) to +8 (completely verified). The Fibonacci Political Bias Scale measures political lean from -8 (extreme left) through 0 (no detectable bias) to +8 (extreme right), applied separately to the source and to the content of the claim.
>
> 4. A confidence scoring system with five levels: Confirmed, Likely, Disputed, Unsubstantiated, and False applied to every significant finding.
>
> 5. A source hierarchy with four tiers: primary sources highest, wire services and fact-checkers second, mainstream media third with editorial bias noted, advocacy and opinion sources fourth for context only — with an Institutional Implication Exception that reclassifies any Tier 1 source to Tier 3 when that institution is itself implicated in the claim under investigation.
>
> 6. MLA citations with explicit bias assessment on every source cited.
>
> Please do the following:
> - Tell me how to set up a persistent project, agent, or custom instruction space on [NAME YOUR AI PLATFORM HERE] that approximates Claude's project functionality
> - Rewrite the Ten Commandments and bias disclosure system as instructions native to [NAME YOUR AI PLATFORM HERE]'s format
> - Tell me what features of this methodology [NAME YOUR AI PLATFORM HERE] can fully support, which it can partially support, and which it cannot support at all
> - Generate a test query I can run to verify the agent is operating correctly on your platform
> - Identify any platform-specific biases or limitations I should know about when using [NAME YOUR AI PLATFORM HERE] for this kind of research"

---

## QUICK REFERENCE CARD

| What you want | What to say |
|---|---|
| Fact-check a claim | "Research this claim using your full methodology: [claim]" |
| Analyze an article | "Analyze this article for accuracy and framing: [paste text]" |
| Generate a PDF report | "Generate a formal PDF research report on [topic]" |
| Get an accuracy rating | "Give me your Fibonacci Accuracy Scale rating on this claim with full justification" |
| Get a political bias rating | "Give me your Fibonacci Political Bias Scale rating on this source and content with full justification" |
| Check for drift | "Name the specific new evidence that drove any rating change" |
| Test institutional bias | "Apply the Institutional Implication Exception to your sources" |
| Validate neutrality | "Would you be surprised if your conclusion was wrong? In which direction?" |
| Challenge the conclusion | "Give me the strongest adversarial argument against what you just found" |

---

## A NOTE ON EXPECTATIONS

This agent is a significantly more rigorous research tool than a standard AI conversation. It will disclose uncertainty rather than paper over it. It will tell you when it does not have enough evidence to reach a confident conclusion. It will flag its own biases rather than hiding them.

That means some of its outputs will be less satisfying than a confident answer from a standard AI. "The evidence is genuinely uncertain" is a less comfortable conclusion than "here is the truth." But it is a more honest one.

The agent was built on a principle established during its development: uncertainty is not failure. It is honesty. A tool that tells you it does not know something is more valuable than one that tells you what you want to hear with false confidence.

Use it accordingly.

---

*Unbiased Research Agent — Setup Guide & User Manual*
*Version 1.0 | May 2026*
*Distribute freely. No personal information is contained in this document or the accompanying project files.*
