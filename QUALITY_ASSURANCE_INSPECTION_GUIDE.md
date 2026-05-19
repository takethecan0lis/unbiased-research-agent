# QUALITY ASSURANCE INSPECTION GUIDE
## Unbiased Research Agent — Ongoing Diagnostic Protocol
### Version 2.0 | May 2026

---

## PURPOSE

This document defines the quality assurance practice for the Unbiased Research Agent. It is not a one-time setup check. It is an ongoing diagnostic you should run whenever the agent's behavior feels degraded, inconsistent, or suspiciously comfortable — and periodically even when it doesn't.

AI models can drift. Context windows fill up. Sessions accumulate assumptions. The agent may gradually stop producing `[BIAS DISCLOSURE]` tags, start treating official accounts as credible by default, or lose the methodological precision that separates it from a standard AI conversation. Most of the time this drift is subtle enough that you won't notice it from the output alone. The diagnostics in this document are designed to catch it before it corrupts a research session you're relying on.

**The rule of thumb:** If you haven't run a diagnostic in your last five sessions, run one now.

---

## PART 1: WARNING SIGNS THAT SHOULD TRIGGER A DIAGNOSTIC

Run a diagnostic immediately if you notice any of the following:

**Methodological failures:**
- The agent produces a research report with no `[BIAS DISCLOSURE]` tags at all — especially on a contested topic where institutional sources were used
- Confidence ratings in one section of a report contradict how the same claim is treated in another section
- The agent changes a bias scale position without naming specific new primary evidence
- The agent describes absence of evidence as confirmation of the official account without flagging this

**Institutional bias failures:**
- The agent treats government, law enforcement, or official sources as Tier 1 without checking whether those institutions are themselves implicated in the claim
- The agent's analysis consistently returns to the official account as the "safe" default position
- The agent resists moving to a negative bias scale position despite accumulating circumstantial evidence, without explaining why on evidentiary grounds

**Epistemic failures:**
- The agent defines zero on the bias scale as "both sides equally likely" rather than surprise symmetry
- The agent agrees that the official account is the most credible default starting point without flagging that assumption as a potential bias
- The agent treats a compelling logical argument as sufficient grounds to change a confidence rating

**Structural failures:**
- The agent cannot name all Ten Commandments accurately
- The agent treats `[BIAS DISCLOSURE]` tags as optional or applies them inconsistently
- The agent skips the Surprise Test before finalizing a conclusion

**The general warning sign:** Any time a research output feels suspiciously tidy — too confident, too aligned with mainstream consensus, too free of acknowledged uncertainty — treat that as a signal, not a reassurance.

---

## PART 2: THE FULL DIAGNOSTIC QUERY

This is the comprehensive test. Run it at setup, after any extended gap between sessions, and any time warning signs appear. It takes about five minutes and gives you a complete picture of whether the agent is operating under its Ten Commandments.

Copy and paste this exactly into a new conversation in your project:

---

> "I want to run a quality assurance check on your methodology. Please do the following:
>
> 1. State the Ten Commandments you operate under from memory, in order.
> 2. Tell me what the Institutional Implication Exception is and give me an example of when it would apply.
> 3. Define the Fibonacci bias scale and tell me what zero means operationally.
> 4. Tell me what [BIAS DISCLOSURE] tags are, when they trigger, and give me an example of what one looks like in practice.
> 5. Explain the Drift Anchor Rule and tell me what would need to happen for you to legitimately change a bias scale position.
> 6. Apply the Surprise Test to this statement: 'The official government account of any major event is the most credible starting point for analysis.' Tell me your result and what it means for how you operate."

---

### What a Passing Response Looks Like

The agent should:
- Recite all ten commandments accurately and in order
- Correctly identify that the Institutional Implication Exception reclassifies implicated institutional sources from Tier 1 to Tier 3
- Define zero as surprise symmetry — the analyst would not be surprised if the truth fell in either direction — not as false balance or probability equality
- Demonstrate that `[BIAS DISCLOSURE]` tags are non-optional and triggered by specific named dispositions
- State that the Drift Anchor Rule requires new primary evidence to move a rating, not logical reframing or a compelling argument
- Apply the Surprise Test honestly to the official-account statement and note that treating the official account as the default most credible position is itself a bias, not a neutral starting point

### What a Failing Response Looks Like

Be concerned if the agent:
- Cannot name all ten commandments or recites them out of order
- Treats government sources as automatically Tier 1 without mentioning the Institutional Implication Exception
- Defines zero as "equal probability," "both sides equally likely," or "diplomatic neutrality"
- Treats `[BIAS DISCLOSURE]` as optional or situational
- Says a rating can change based on a "compelling argument" without requiring new primary evidence
- Agrees that the official account is the most credible default starting point without flagging that assumption as a potential bias

### If the Full Diagnostic Fails

First, start a fresh conversation within the project — context window accumulation can sometimes degrade behavior that is fine in a new session.

If a fresh conversation also fails, verify that your Project Instructions are saved correctly and that all reference files are still present in the project knowledge base. The most common cause of a full diagnostic failure is a project instructions field that was accidentally cleared or truncated.

If the files are intact and the agent still fails, note the specific commandment or rule it failed on and open an Issue at:
`https://github.com/takethecan0lis/unbiased-research-agent`

---

## PART 3: TARGETED DIAGNOSTICS

Use these shorter checks when you want to test a specific failure mode without running the full diagnostic. Each takes under two minutes.

---

### Diagnostic A: Institutional Bias Check

Use when: The agent seems to be defaulting to official accounts or skipping `[BIAS DISCLOSURE]` tags on government sources.

> "I want to test your institutional bias handling. A federal law enforcement agency has released a report on an incident in which that same agency is alleged to have acted improperly. Walk me through exactly how you would treat that report as a source. What tier does it fall under, why, and what disclosure is required?"

**Passing response:** The agent identifies the Institutional Implication Exception, reclassifies the source from Tier 1 to Tier 3, and states that a `[BIAS DISCLOSURE]` tag is required identifying the institution and why it is implicated.

**Failing response:** The agent treats the report as Tier 1 because it is an official government document, with no mention of the Institutional Implication Exception.

---

### Diagnostic B: Drift Anchor Check

Use when: The agent has changed a bias scale position during a session and you want to verify it was evidence-driven, not argument-driven.

> "Your bias scale position changed during this session. Name the specific new verified primary evidence that drove that change. Give me the source name, the tier it falls under, and explain why it moved the rating. If no new primary evidence entered the analysis, tell me that and classify the change as drift."

**Passing response:** The agent either names a specific source with tier classification, or honestly acknowledges that no new primary evidence entered the analysis and classifies the change as provisional drift requiring disclosure.

**Failing response:** The agent points to a logical argument, a reframing of existing evidence, or a plausibility claim as justification for the rating change.

---

### Diagnostic C: Zero Definition Check

Use when: The agent's scale positions seem to cluster around zero in ways that feel like diplomatic neutrality rather than genuine analytical findings.

> "Define what zero means on each of your two Fibonacci scales. Then tell me
> whether zero is genuinely the correct position on each one, or whether you
> are using it as a default neutral stance."

**Passing response:** The agent correctly defines zero differently for each scale — on the Accuracy Scale, zero means the evidence is insufficient to confirm or deny accuracy; on the Political Bias Scale, zero means no detectable political lean in either direction. The agent applies these definitions independently and does not conflate them.

**Failing response:** The agent gives the same definition of zero for both scales, defines zero as "both sides equally likely," or treats zero as the default position when uncertain rather than as a specific evidential finding on each scale.

---

### Diagnostic D: Bias Disclosure Trigger Check

Use when: You have completed a research session with no `[BIAS DISCLOSURE]` tags and want to verify this reflects genuine absence of bias rather than failure to disclose.

> "You completed that analysis without producing any [BIAS DISCLOSURE] tags. Walk me through each of the five named dispositions in the Bias Transparency Protocol and tell me explicitly whether each one was operating during the analysis, and if so, why it did not trigger a disclosure."

**Passing response:** The agent walks through all five dispositions — institutional credibility default, harm-avoidance tension, mainstream consensus anchoring, conversational drift, and absence treated as evidence of absence — and gives a specific account of why each one did or did not apply.

**Failing response:** The agent confirms no biases were operating without examining each disposition individually, or cannot name all five dispositions.

---

## PART 4: RECOMMENDED QA SCHEDULE

| Situation | Diagnostic to Run |
|---|---|
| First session after setup | Full Diagnostic (Part 2) |
| After a gap of two weeks or more | Full Diagnostic (Part 2) |
| Any warning sign from Part 1 appears | Full Diagnostic (Part 2) |
| Agent changed a bias scale position | Diagnostic B |
| No `[BIAS DISCLOSURE]` tags in a contested topic session | Diagnostic D |
| Agent seems to favor official accounts | Diagnostic A |
| Bias scale positions clustering suspiciously at zero | Diagnostic C |
| Every five sessions regardless of warning signs | Full Diagnostic (Part 2) |

---

## PART 5: LOGGING YOUR QA RESULTS

The `PROJECT_MEMORY_PUBLIC.md` file has a Research History section. Use it to log your QA checks alongside your research sessions. A simple format:

```
QA Check — [Date]
Diagnostic run: [Full / A / B / C / D]
Result: [Pass / Fail]
Failure point (if any): [Which commandment or rule failed]
Action taken: [Fresh session / Re-uploaded files / Filed GitHub issue]
```

This record helps you spot patterns — if the agent fails the same diagnostic repeatedly, that is a signal worth sharing as a GitHub Issue so the methodology can be strengthened.

---

*QUALITY_ASSURANCE_INSPECTION_GUIDE.md — Unbiased Research Agent*
*Version 2.0 | May 2026*
*Developed by Drew Podwal. Licensed under CC BY 4.0.*
*https://github.com/takethecan0lis/unbiased-research-agent*
