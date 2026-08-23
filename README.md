## AI engineering · agent systems · Hebrew/RTL tooling

I build agent systems that have to be *right*, not just fluent — and I'm drawn to the part
most demos skip: what the thing actually costs, what it silently breaks, and how you would
know either way.

### What I work on

**Agent & skill engineering.** Multi-agent workflows, skill and prompt design, and the
measurement layer around them — cost per trigger, context a model can never reach, and
honest labels on every number.

**Biomedical evidence tagging.** Volunteer AI research advisor to a rare-disease research
effort (CCHS / *PHOX2B*): controlled-vocabulary tagging, ontology anchoring to MeSH/MONDO,
and grounding-enforced extraction built on one rule — *the LLM extracts, deterministic code
decides.* Same corpus, same tags, byte-identical output across runs and across models.

**Hebrew / RTL document pipelines.** Bidi-correct PDF, DOCX and PPTX generation. A narrow
niche that is genuinely hard and very often done badly.

### Selected work

**[talkbrief](https://github.com/yosishe/talkbrief)** — turns a YouTube talk into a
grounded, slide-by-slide brief. Deterministic slide extraction, transcript alignment,
Claude-written notes — and then every quote is **mechanically verified** against the
transcript before you see it (a real-model run came back 351/354 grounded, and the 3
misses are flagged in amber, never dropped). Bidi-correct Hebrew/RTL output, offline-first,
no API key — it rides the Claude Code CLI. MIT.

**[token-efficient-skill-optimizer](https://github.com/yosishe/token-efficient-skill-optimizer)**
— audits AI skills, system prompts, and agent instruction sets for what they actually cost
per trigger, under a hard constraint: no task-success loss, no safety weakening.

The design choice I care about most is that it can tell you *not* to optimize. Several rules
exist only to stop an edit — keep the repetition that looks redundant but is load-bearing,
keep the verbose instruction carrying a safety obligation. "Already efficient" is a
successful outcome, and the pilot that came back at −0.7% was published at −0.7%.

Every number carries an enforced label — `[measured]`, `[estimated]`, `[projected]` — and a
`[measured]` claim with no pointer to its data file fails the build, including in the
project's own reports. 27 rules over 42 sources, each citation machine-checked against its
primary page. MIT.

### Background

Computer Science graduate · data science certificate · based in Israel · Hebrew and English.
[LinkedIn](https://www.linkedin.com/in/yossi--shemer)

Most of what I build is applied and client- or research-facing, so a fair amount of it lives
outside this profile. Happy to walk through any of it.
